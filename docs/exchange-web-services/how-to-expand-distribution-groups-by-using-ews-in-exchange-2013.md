---
title: 'Как: развернуть группы рассылки с помощью EWS в Exchange 2013'
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
localization_priority: Normal
ms.assetid: 25ee84e7-63bc-4f51-9b7d-e7f46fd574d5
description: Узнайте, как развернуть группу рассылки с помощью управляемого API EWS или EWS в Exchange.
ms.openlocfilehash: 0f9186fb71b3005c71a70e89aafb674ae15e4814
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761000"
---
# <a name="expand-distribution-groups-by-using-ews-in-exchange-2013"></a>Как: развернуть группы рассылки с помощью EWS в Exchange 2013

Узнайте, как развернуть группу рассылки с помощью управляемого API EWS или EWS в Exchange.
  
Можно использовать метод управляемого API [ExchangeService. ExpandGroup](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.exchangeservice.expandgroup%28v=exchg.80%29.aspx) EWS или операцию [ExpandDL](http://msdn.microsoft.com/library/1f7837e7-9eff-4e10-9577-c40f7ed6af94%28Office.15%29.aspx) EWS для расширения группы рассылки, чтобы определить всех получателей. 
  
Так как метод [ExpandGroup](http://msdn.microsoft.com/en-us/library/office/ee344007%28v=exchg.80%29.aspx) перегружен, его можно вызывать несколькими способами: 
  
- [ExpandGroup (строка)](http://msdn.microsoft.com/en-us/library/office/ee343988%28v=exchg.80%29.aspx) — разворачивает группу, определенную по SMTP-адресу. 
    
- [ExpandGroup (EmailAddress)](http://msdn.microsoft.com/en-us/library/office/ee344007%28v=exchg.80%29.aspx) — разворачивает группу, определенную по адресу электронной почты. 
    
- [ExpandGroup (ItemId)](http://msdn.microsoft.com/en-us/library/office/ee356407%28v=exchg.80%29.aspx) — разворачивает группу, определяемую по идентификатору группы. 
    
- [Експанграуп (String, String)](http://msdn.microsoft.com/en-us/library/office/ee356468%28v=exchg.80%29.aspx) — разворачивает группу, ОПРЕДЕЛЯЕМую SMTP-адресом, и типом маршрутизации этого адреса. 
    
## <a name="expand-a-universal-distribution-group-or-security-group-by-using-ews-managed-api"></a>Расширение универсальной группы рассылки или группы безопасности с помощью управляемого API EWS
<a name="bk_ExpandDGEWSMA"> </a>

В приведенном ниже примере показано, как развернуть универсальную группу рассылки или группу безопасности с помощью адреса электронной почты, что является самым простым способом. В этом примере предполагается, что **служба** является действительным объектом [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx), и что пользователь прошел проверку подлинности на сервере Exchange server. 
  
```cs
// Return the expanded group.
   ExpandGroupResults myGroupMembers = service.ExpandGroup("employees@contoso.com");
// Display the group members.
   foreach (EmailAddress address in myGroupMembers.Members)
   {
      Console.WriteLine("Email Address: {0}", address);
   }

```

Это не очень много кода, но он также довольно простой и может не дать вам того, что вы ищете. Поэтому давайте попробуем сделать это. Группы рассылки также могут содержать другие группы рассылки. При простом расширении он выводит адрес электронной почты вложенных групп рассылки, но не разворачивает их. Добавляя еще несколько строк кода, вы можете рекурсивно развернуть группы для вывода каждого контакта.
  
```cs
private static void ExpandDistributionLists(ExchangeService service, string Mailbox)
{
   // Return the expanded group.
      ExpandGroupResults myGroupMembers = service.ExpandGroup(Mailbox);
   // Display the group members.
      foreach (EmailAddress address in myGroupMembers.Members)
      {
         // Check to see if the mailbox is a public group
         if (address.MailboxType == MailboxType.PublicGroup)
      {
         // Call the function again to expand the contained
         // distribution group.
         ExpandDistributionLists(service, address.Address);
      }
      else
      {
         // Output the address of the mailbox.
         Console.WriteLine("Email Address: {0}", address);
      }
   }
}

```

Теперь вы можете вызвать эту новую функцию в коде и развернуть все общедоступные группы рассылки, содержащиеся в первой из них.
  
```cs
ExpandDistributionLists(service, "employees@contoso.com");

```

## <a name="expand-a-contact-group-by-using-ews-managed-api"></a>Развертывание группы контактов с помощью управляемого API EWS
<a name="bk_ExpandDGEWSMA"> </a>

Так как у групп контактов нет соответствующего адреса электронной почты, необходимо развернуть группу на основе ItemId с помощью метода [ExpandGroup (ItemId)](http://msdn.microsoft.com/en-us/library/office/ee356407%28v=exchg.80%29.aspx) . Вы можете создать функцию, как показано в предыдущем примере, и изменить второй тип параметра из строки в идентификатор [ItemId](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.itemid%28v=exchg.80%29.aspx).
  
```cs
private static void ExpandContactGroup(ExchangeService service, ItemId groupID)
{
   // Return the expanded group.
      ExpandGroupResults myGroupMembers = service.ExpandGroup(groupID);
   // Display the group members.
      foreach (EmailAddress address in myGroupMembers.Members)
      {
         if (address.MailboxType == MailboxType.PublicGroup)
         {
            ExpandDistributionLists(service, address.Address);
         }
         else
         {
            Console.WriteLine("Email Address: {0}", address);
         }
      }
}
```

Теперь вы можете вызвать эту функцию, используя объект службы Exchange и идентификатор **ItemId** группы контактов. Обратите внимание, что идентификатор **ItemId** в примере сокращается для удобочитаемости. 
  
```cs
ExpandContactGroup(service, new ItemId("AAMkADBlY…");

```

## <a name="expand-a-universal-distribution-group-or-security-group-by-using-ews"></a>Расширение универсальной группы рассылки или группы безопасности с помощью EWS
<a name="bk_ExpandDGEWSMA"> </a>

В следующем примере показано сообщение XML-запроса, которое отправляется с клиента на сервер при использовании операции [ExpandDL](http://msdn.microsoft.com/library/1f7837e7-9eff-4e10-9577-c40f7ed6af94%28Office.15%29.aspx) . Это также запрос XML, который отправляет управляемый API EWS при использовании управляемого API EWS для [расширения универсальной группы рассылки](#bk_ExpandDGEWSMA). 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <ExpandDL xmlns="http://schemas.microsoft.com/exchange/services/2006/messages"
              xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <Mailbox>
        <t:EmailAddress>employees@contoso.com</t:EmailAddress>
      </Mailbox>
    </ExpandDL>
  </soap:Body>
</soap:Envelope>
```

В следующем примере показано ответное сообщение XML, которое отправляется с сервера клиенту. Обратите внимание, что возвращаются как почтовые ящики, так и универсальные группы рассылки.
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
<s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
     xmlns:xsd="http://www.w3.org/2001/XMLSchema">
<ExpandDLResponse xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
                      xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <ResponseMessages xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
    <ExpandDLResponseMessage ResponseClass="Success">
      <ResponseCode>NoError</ResponseCode>
      <DLExpansion IncludesLastItemInRange="true" TotalItemsInView="4">
        <Mailbox xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
          <Name>Sadie Daniels</Name>
          <EmailAddress>sadie@contoso.com</EmailAddress>
          <RoutingType>SMTP</RoutingType>
          <MailboxType>Mailbox</MailboxType>
        </Mailbox>
        <Mailbox xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
          <Name>Alfred Welker</Name>
          <EmailAddress>alfred@contoso.com</EmailAddress>
          <RoutingType>SMTP</RoutingType>
          <MailboxType>Mailbox</MailboxType>
        </Mailbox>
        <Mailbox xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
          <Name>Contoso Sales</Name>
          <EmailAddress>sales@contoso.com</EmailAddress>
          <RoutingType>SMTP</RoutingType>
          <MailboxType>PublicDL</MailboxType>
        </Mailbox>
        <Mailbox xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
          <Name>Contoso Support</Name>
          <EmailAddress>support@contoso.com</EmailAddress>
          <RoutingType>SMTP</RoutingType>
          <MailboxType>PublicDL</MailboxType>
        </Mailbox>
      </DLExpansion>
    </ExpandDLResponseMessage>
  </ResponseMessages>
</ExpandDLResponse>
</s:Body>
</s:Envelope>
```

В отличие от использования управляемого API EWS, при использовании EWS для расширения универсальной группы рассылки невозможно рекурсивно расширять возвращаемые группы рассылки. Вам потребуется отправить дополнительный запрос, чтобы развернуть каждую из групп рассылки, включенных в ответ.
  
## <a name="expand-a-contact-group-by-using-ews"></a>Развертывание группы контактов с помощью EWS
<a name="bk_ExpandDGEWSMA"> </a>

Запрос XML для расширения группы контактов аналогичен запросу для расширения группы рассылки. Вместо адреса электронной почты используется идентификатор [ItemId](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) группы контактов. Элемент **ItemId** в этом примере сокращается для удобочитаемости. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <ExpandDL xmlns="http://schemas.microsoft.com/exchange/services/2006/messages"
              xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <Mailbox>
         <ItemId xmlns="http://schemas.microsoft.com/exchange/services/2006/types" Id="AAMkADBlY…" />
      </Mailbox>
    </ExpandDL>
  </soap:Body>
</soap:Envelope>
```

Структура ответа XML на запрос на расширение группы контактов такая же, как и в ответ на запрос на расширение универсальной группы рассылки.
  
## <a name="see-also"></a>См. также


- [Группы рассылки и EWS в Exchange](distribution-groups-and-ews-in-exchange.md)
    
- [Как: создать группы контактов с помощью EWS в Exchange](how-to-create-contact-groups-by-using-ews-in-exchange.md)
    

