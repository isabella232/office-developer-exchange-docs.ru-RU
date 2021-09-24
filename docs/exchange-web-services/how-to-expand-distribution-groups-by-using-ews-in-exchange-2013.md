---
title: 'Как: развернуть группы рассылки с помощью EWS в Exchange 2013'
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
ms.localizationpriority: medium
ms.assetid: 25ee84e7-63bc-4f51-9b7d-e7f46fd574d5
description: Узнайте, как расширить группу рассылки с помощью управляемого API или EWS EWS в Exchange.
ms.openlocfilehash: 6aeebbd14604295bce46049f0e383663414c01a0
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59513187"
---
# <a name="expand-distribution-groups-by-using-ews-in-exchange-2013"></a>Как: развернуть группы рассылки с помощью EWS в Exchange 2013

Узнайте, как расширить группу рассылки с помощью управляемого API или EWS EWS в Exchange.
  
Вы можете использовать метод управляемого API [ExchangeService.ExpandGroup](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.exchangeservice.expandgroup%28v=exchg.80%29.aspx) EWS или операцию [ExpandDL](https://msdn.microsoft.com/library/1f7837e7-9eff-4e10-9577-c40f7ed6af94%28Office.15%29.aspx) EWS для расширения группы рассылки для идентификации всех получателей. 
  
Так как метод [ExpandGroup](https://msdn.microsoft.com/library/office/ee344007%28v=exchg.80%29.aspx) перегружен, его можно вызвать несколькими способами: 
  
- [ExpandGroup (String)](https://msdn.microsoft.com/library/office/ee343988%28v=exchg.80%29.aspx) — расширяет группу, идентифицированную по адресу SMTP. 
    
- [ExpandGroup (EmailAddress)](https://msdn.microsoft.com/library/office/ee344007%28v=exchg.80%29.aspx) — расширяет группу, идентифицированную по адресу электронной почты. 
    
- [ExpandGroup (ItemId)](https://msdn.microsoft.com/library/office/ee356407%28v=exchg.80%29.aspx) — расширяет группу, идентифицированную по групповому ID. 
    
- [ExpanGroup (String, String)](https://msdn.microsoft.com/library/office/ee356468%28v=exchg.80%29.aspx) — расширяет группу, идентифицированную по smTP-адресу и типу маршрутировки этого адреса. 
    
## <a name="expand-a-universal-distribution-group-or-security-group-by-using-ews-managed-api"></a>Расширение универсальной группы рассылки или группы безопасности с помощью управляемого API EWS
<a name="bk_ExpandDGEWSMA"> </a>

В следующем примере показано, как расширить универсальную группу рассылки или группу безопасности с помощью адреса электронной почты, что является простейшим подходом. В этом примере предполагается, что **служба** является действительным объектом [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx), и что пользователь прошел проверку подлинности на сервере Exchange server. 
  
```cs
// Return the expanded group.
   ExpandGroupResults myGroupMembers = service.ExpandGroup("employees@contoso.com");
// Display the group members.
   foreach (EmailAddress address in myGroupMembers.Members)
   {
      Console.WriteLine("Email Address: {0}", address);
   }

```

Это не так много кода, но он также довольно простой и может не дать вам то, что вы ищете. Итак, давайте рассмотрим этот шаг дальше. Группы рассылки также могут содержать другие группы рассылки. Простое расширение будет выводить адрес электронной почты содержащихся групп рассылки, но не расширять их. Добавив еще несколько строк кода, можно повторно расширить группы для вывода каждого контакта.
  
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

Теперь вы можете вызвать эту новую функцию в коде и расширить все общедоступные группы рассылки, содержащиеся в первой.
  
```cs
ExpandDistributionLists(service, "employees@contoso.com");

```

## <a name="expand-a-contact-group-by-using-ews-managed-api"></a>Расширение контактной группы с помощью управляемого API EWS
<a name="bk_ExpandDGEWSMA"> </a>

Так как в контактных группах нет связанного адреса электронной почты, необходимо расширить группу на основе ItemId с помощью метода [ExpandGroup (ItemId).](https://msdn.microsoft.com/library/office/ee356407%28v=exchg.80%29.aspx) Можно создать функцию, как показано в предыдущем примере, и изменить второй тип параметра из строки в [ItemId.](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.itemid%28v=exchg.80%29.aspx)
  
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

Теперь эту функцию можно вызвать с помощью объекта Exchange и **ItemId** контактной группы. Обратите внимание, **что ItemId** в примере сокращается для читаемости. 
  
```cs
ExpandContactGroup(service, new ItemId("AAMkADBlY…");

```

## <a name="expand-a-universal-distribution-group-or-security-group-by-using-ews"></a>Расширение универсальной группы рассылки или группы безопасности с помощью EWS
<a name="bk_ExpandDGEWSMA"> </a>

В следующем примере показано сообщение XML-запроса, которое отправляется от клиента на сервер при использовании операции [ExpandDL.](https://msdn.microsoft.com/library/1f7837e7-9eff-4e10-9577-c40f7ed6af94%28Office.15%29.aspx) Это также XML-запрос, который отправляет управляемый API EWS при использовании API управляемых EWS для расширения [универсальной группы рассылки.](#bk_ExpandDGEWSMA) 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <ExpandDL xmlns="https://schemas.microsoft.com/exchange/services/2006/messages"
              xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <Mailbox>
        <t:EmailAddress>employees@contoso.com</t:EmailAddress>
      </Mailbox>
    </ExpandDL>
  </soap:Body>
</soap:Envelope>
```

В следующем примере показано сообщение ответа XML, которое отправляется с сервера клиенту. Обратите внимание, что возвращаются как почтовые ящики, так и универсальные группы рассылки.
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
<s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
     xmlns:xsd="http://www.w3.org/2001/XMLSchema">
<ExpandDLResponse xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
                      xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <ResponseMessages xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
    <ExpandDLResponseMessage ResponseClass="Success">
      <ResponseCode>NoError</ResponseCode>
      <DLExpansion IncludesLastItemInRange="true" TotalItemsInView="4">
        <Mailbox xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
          <Name>Sadie Daniels</Name>
          <EmailAddress>sadie@contoso.com</EmailAddress>
          <RoutingType>SMTP</RoutingType>
          <MailboxType>Mailbox</MailboxType>
        </Mailbox>
        <Mailbox xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
          <Name>Alfred Welker</Name>
          <EmailAddress>alfred@contoso.com</EmailAddress>
          <RoutingType>SMTP</RoutingType>
          <MailboxType>Mailbox</MailboxType>
        </Mailbox>
        <Mailbox xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
          <Name>Contoso Sales</Name>
          <EmailAddress>sales@contoso.com</EmailAddress>
          <RoutingType>SMTP</RoutingType>
          <MailboxType>PublicDL</MailboxType>
        </Mailbox>
        <Mailbox xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
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

В отличие от использования управляемого API EWS при использовании EWS для расширения универсальной группы рассылки нельзя повторно расширить возвращаемую группу рассылки. Для расширения каждой из групп рассылки, включенных в ответ, необходимо отправить дополнительный запрос.
  
## <a name="expand-a-contact-group-by-using-ews"></a>Расширение контактной группы с помощью EWS
<a name="bk_ExpandDGEWSMA"> </a>

Запрос XML для расширения контактной группы похож на запрос на расширение группы рассылки. Вместо адреса электронной почты используется [ItemId](https://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) контактной группы. **ItemId** в этом примере сокращается для читаемости. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <ExpandDL xmlns="https://schemas.microsoft.com/exchange/services/2006/messages"
              xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <Mailbox>
         <ItemId xmlns="https://schemas.microsoft.com/exchange/services/2006/types" Id="AAMkADBlY…" />
      </Mailbox>
    </ExpandDL>
  </soap:Body>
</soap:Envelope>
```

Структура ответа XML на запрос о расширении контактной группы такая же, как и ответ на запрос о расширении универсальной группы рассылки.
  
## <a name="see-also"></a>См. также


- [Группы рассылки и EWS в Exchange](distribution-groups-and-ews-in-exchange.md)
    
- [Как: создать группы контактов с помощью EWS в Exchange](how-to-create-contact-groups-by-using-ews-in-exchange.md)
    

