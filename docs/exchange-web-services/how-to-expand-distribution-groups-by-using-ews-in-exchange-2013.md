---
title: Разверните узел группы рассылки с помощью веб-служб Exchange в Exchange 2013
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
localization_priority: Normal
ms.assetid: 25ee84e7-63bc-4f51-9b7d-e7f46fd574d5
description: Узнайте, как с помощью управляемого интерфейса API веб-служб Exchange или веб-служб Exchange в Exchange разверните группу рассылки.
ms.openlocfilehash: 0f9186fb71b3005c71a70e89aafb674ae15e4814
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761000"
---
# <a name="expand-distribution-groups-by-using-ews-in-exchange-2013"></a>Разверните узел группы рассылки с помощью веб-служб Exchange в Exchange 2013

Узнайте, как с помощью управляемого интерфейса API веб-служб Exchange или веб-служб Exchange в Exchange разверните группу рассылки.
  
Можно использовать метод управляемый API EWS [ExchangeService.ExpandGroup](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.exchangeservice.expandgroup%28v=exchg.80%29.aspx) или операция [ExpandDL](http://msdn.microsoft.com/library/1f7837e7-9eff-4e10-9577-c40f7ed6af94%28Office.15%29.aspx) веб-служб Exchange разверните группу рассылки для идентификации всех получателей. 
  
Так как метод [ExpandGroup](http://msdn.microsoft.com/en-us/library/office/ee344007%28v=exchg.80%29.aspx) перегружен, его можно вызвать несколькими способами: 
  
- [ExpandGroup(String)](http://msdn.microsoft.com/en-us/library/office/ee343988%28v=exchg.80%29.aspx) - расширяет группу, определенную SMTP-адрес. 
    
- [ExpandGroup(EmailAddress)](http://msdn.microsoft.com/en-us/library/office/ee344007%28v=exchg.80%29.aspx) - расширяет группу, определенную с адресом электронной почты. 
    
- [ExpandGroup(ItemId)](http://msdn.microsoft.com/en-us/library/office/ee356407%28v=exchg.80%29.aspx) - расширяет группу, определенную группу ID. 
    
- [ExpanGroup (строка, строка)](http://msdn.microsoft.com/en-us/library/office/ee356468%28v=exchg.80%29.aspx) - расширяет группу, определенную SMTP-адреса и типа маршрутизации этот адрес. 
    
## <a name="expand-a-universal-distribution-group-or-security-group-by-using-ews-managed-api"></a>Разверните узел универсальная группа рассылки или группу безопасности с помощью управляемого интерфейса API веб-служб Exchange
<a name="bk_ExpandDGEWSMA"> </a>

Следующий пример демонстрирует разверните универсальная группа рассылки или группу безопасности, используя адрес электронной почты, которая наиболее простой способ. В этом примере предполагается, что эта **Служба** является допустимым объектом [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) и пользователь прошел проверку подлинности на сервере Exchange. 
  
```cs
// Return the expanded group.
   ExpandGroupResults myGroupMembers = service.ExpandGroup("employees@contoso.com");
// Display the group members.
   foreach (EmailAddress address in myGroupMembers.Members)
   {
      Console.WriteLine("Email Address: {0}", address);
   }

```

Который не является большой объем кода, но они также довольно просто и может не предоставить требуется найти. Давайте сделать его шаг дальнейшей. Группы рассылки также может содержать другие группы рассылки. Просто он был развернут вывода адрес электронной почты группы рассылки автономные но не раскрывать их. Путем добавления еще на несколько строк кода, можно рекурсивно развернуть группы выводить все контакты.
  
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

И теперь можно вызвать этой новой функции вашего кода и развернуть все группы рассылки общедоступных, содержащихся в первый.
  
```cs
ExpandDistributionLists(service, "employees@contoso.com");

```

## <a name="expand-a-contact-group-by-using-ews-managed-api"></a>Разверните группу контактов с помощью управляемого интерфейса API веб-служб Exchange
<a name="bk_ExpandDGEWSMA"> </a>

Так как группы контактов отсутствует адрес связанной электронной почты, вам нужно разверните группу на основании ItemId с помощью метода [ExpandGroup(ItemId)](http://msdn.microsoft.com/en-us/library/office/ee356407%28v=exchg.80%29.aspx) . Создание функции, как показано в предыдущем примере и измените второй тип параметра из строки на [идентификатор элемента](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.itemid%28v=exchg.80%29.aspx).
  
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

Теперь можно вызвать эту функцию с помощью объекта службы Exchange и **ItemId** группы контактов. Обратите внимание на то, что **идентификатор элемента** в примере — это сокращение для удобства чтения. 
  
```cs
ExpandContactGroup(service, new ItemId("AAMkADBlY…");

```

## <a name="expand-a-universal-distribution-group-or-security-group-by-using-ews"></a>Разверните узел универсальная группа рассылки или группу безопасности с помощью веб-служб Exchange
<a name="bk_ExpandDGEWSMA"> </a>

В следующем примере показано сообщение запроса XML, передаче от клиента к серверу при использовании операции [ExpandDL](http://msdn.microsoft.com/library/1f7837e7-9eff-4e10-9577-c40f7ed6af94%28Office.15%29.aspx) . Это также XML-запрос, который отправляет управляемый API веб-служб Exchange, когда использовать управляемый API веб-служб Exchange разверните [Универсальная группа рассылки](#bk_ExpandDGEWSMA). 
  
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

В следующем примере показано XML ответное сообщение, которое отправляется с сервера. Обратите внимание на то, что возвращаются почтовых ящиков и универсальные группы рассылки.
  
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

В отличие от при использовании управляемый API веб-служб Exchange при использовании веб-служб Exchange разверните универсальная группа рассылки, вы не можете рекурсивно расширять группы рассылки, которые возвращаются. Необходимо будет отправить дополнительного запроса развернуть каждый из группы рассылки, включенных в ответ.
  
## <a name="expand-a-contact-group-by-using-ews"></a>Разверните группу контактов с помощью веб-служб Exchange
<a name="bk_ExpandDGEWSMA"> </a>

В запросе XML, чтобы развернуть группу контактов похож на запрос, чтобы развернуть группу рассылки. Вместо адреса электронной почты используйте [ItemId](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) группы контактов. **Идентификатор элемента** в этом примере сокращение для удобства чтения. 
  
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

Структура XML-ответ на запрос, чтобы развернуть группу контактов — это то же, что ответ на запрос, чтобы развернуть универсальная группа рассылки.
  
## <a name="see-also"></a>См. также


- [Группы рассылки и EWS в Exchange](distribution-groups-and-ews-in-exchange.md)
    
- [Создание группы контактов с помощью веб-служб Exchange в Exchange](how-to-create-contact-groups-by-using-ews-in-exchange.md)
    

