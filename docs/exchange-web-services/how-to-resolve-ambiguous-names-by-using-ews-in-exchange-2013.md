---
title: Устранение неоднозначности имен с помощью EWS в Exchange 2013
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.localizationpriority: medium
ms.assetid: 1ba21c54-ecd2-4a1e-80d4-0f4171dea84f
description: Узнайте, как использовать управляемый API EWS или EWS для решения неоднозначных имен, получив возможные совпадения с службами домена Active Directory (AD DS) или папкой контактов в почтовом ящике пользователя.
ms.openlocfilehash: 5946dad32639b454b3961eaa172b6069ce118b58
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59521125"
---
# <a name="resolve-ambiguous-names-by-using-ews-in-exchange-2013"></a>Устранение неоднозначности имен с помощью EWS в Exchange 2013

Узнайте, как использовать управляемый API EWS или EWS для решения неоднозначных имен, получив возможные совпадения с службами домена Active Directory (AD DS) или папкой контактов в почтовом ящике пользователя.
  
Пользователю в организации предоставляется рукописный список имен и адресов сотрудников, которые присутствовали на учебном занятии. Они хотят отправить сообщение электронной почты с некоторыми дополнительными сведениями для людей из списка, но они не могут читать электронный адрес каждого. Если вы хотите решить эту проблему для пользователей в приложении, EWS может помочь. Вы можете использовать метод управляемого API [ExchangeService.ResolveName](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.exchangeservice.resolvename%28v=exchg.80%29.aspx) EWS или операцию [ResolveNames](https://msdn.microsoft.com/library/c85207e1-1315-443b-94ec-2b58f405076b%28Office.15%29.aspx) EWS, чтобы вернуть список потенциальных совпадений для выбора текста, например в составе фамилии. Возвращаемые элементы могут быть общедоступными почтовыми ящиками пользователей, группами рассылки и контактами. 
  
Обратите внимание, Exchange сохраняет адреса электронной почты с помощью префиксированных типов маршрутиза, таких как smtp или sip, в многоценном массиве. Метод **ResolveName** и операция **ResolveNames** частично соответствуют каждому значению этого массива при добавлении типа маршрутов в начале неурегулированного имени, например "sip:User1". Если не указать тип маршрутизации, метод или операция по умолчанию будут smtp, соединить его с основным свойством адресов smtp, а не искать многоценный массив. Например, если вы ищете User1 и не включаете префикс sip, вы не получите sip:User1@Contoso.com в результате, даже если это допустимый почтовый ящик. 
  
В одном запросе можно указать только одно неоднозначное имя. Если у вас есть список неоднозначных имен для решения, вам потребуется цикл через список и вызвать метод или операцию для каждой записи. Кандидаты из папки Контакты пользователя будут иметь значение ID элемента non-null, которое затем можно использовать в вызове метода [Contact.Bind](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.contact.bind%28v=exchg.80%29.aspx) или запросе на операцию [GetItem](https://msdn.microsoft.com/library/769df8eb-9c72-48b5-a49f-82c6b86bc5fc%28Office.15%29.aspx) для получения дополнительных сведений. Если кандидат является группой рассылки, для получения списка участников можно использовать метод управляемого API EWS [ExpandGroup (ItemId)](https://msdn.microsoft.com/library/office/ee356407%28v=exchg.80%29.aspx) или операцию [ExpandDL](https://msdn.microsoft.com/library/affe84a5-ad98-4aba-83f4-8732938b763d%28Office.15%29.aspx) EWS. Если параметр  _returnContactDetails_ или атрибут **ReturnFullContactData** EWS задан для true, записи Active Directory, возвращенные с помощью метода **ResolveName** или **операции ResolveNames,** будут включать дополнительные свойства, описывая контакт. Параметр  _returnContactDetails_ или атрибут **ReturnFullContactData** не влияют на данные, возвращаемые для контактов и контактных групп. 
  
## <a name="resolve-ambiguous-names-by-using-ews-managed-api"></a>Устранение неоднозначных имен с помощью управляемого API EWS
<a name="bk_EWSMA"> </a>

Вы можете использовать метод [ResolveName](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.exchangeservice.resolvename%28v=exchg.80%29.aspx) для поиска кандидатов, которые совпадают с неоднозначным именем, которое вы передаете. Вы можете использовать перегрузки метода **ResolveName** для поиска кандидатов пятью различными способами. 
  
**Таблица 1. Перегруженные методы ResolveName**

|**Способ**|**Принцип работы**|
|:-----|:-----|
|[ResolveName (String)](https://msdn.microsoft.com/library/dd635548%28v=exchg.80%29.aspx) <br/> |Находит контакты в папке Контакты пользователя и Глобальном списке адресов (GAL) — в этом порядке. Переменная строки — это неоднозначное имя, которое вы пытаетесь разрешить.  <br/> |
|[ResolveName(String, ResolveNameSearchLocation, Boolean)](https://msdn.microsoft.com/library/dd634595%28v=exchg.80%29.aspx) <br/> |Находит контакты в папке Контакты по умолчанию и/или глобальном списке адресов (GAL). Значение строки — это неоднозначное имя, в расположении поиска указывается папка Контакты и/или GAL, а значение Boolean указывает, следует ли возвращать полную контактную информацию.  <br/> |
|[ResolveName(String, ResolveNameSearchLocation, Boolean, PropertySet)](https://msdn.microsoft.com/library/hh532803%28v=exchg.80%29.aspx) <br/> |Находит контакты в папке контактов по умолчанию и/или глобальном списке адресов (GAL). Этот метод позволяет настроить возвращаемые свойства.  <br/> |
|[ResolveName(String, IEnumerable, \<FolderId\> ResolveNameSearchLocation, Boolean)](https://msdn.microsoft.com/library/dd636014%28v=exchg.80%29.aspx) <br/> |Находит контакты в указанных папках контактов и/или глобальном списке адресов (GAL). С помощью этого метода можно передать коллекцию папок для поиска. Это позволяет искать в папках контактов, кроме папки Контактов по умолчанию.  <br/> |
|[ResolveName(String, IEnumerable, \<FolderId\> ResolveNameSearchLocation, Boolean, PropertySet)](https://msdn.microsoft.com/library/hh532581%28v=exchg.80%29.aspx) <br/> |Находит контакты в глобальном списке адресов (GAL) и/или в определенных папках контактов. Этот метод позволяет настроить возвращаемые свойства.  <br/> |
   
Начнем с простого примера. В следующем примере показано, как разрешить текстовую строку "dan" и вытеснить имя и адрес электронной почты каждого найденного кандидата. В этом примере предполагается, что **служба** является действительным объектом [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx), и что пользователь прошел проверку подлинности на сервере Exchange server. 
  
```cs
// Resolve the ambiguous name "dan".
   NameResolutionCollection resolvedNames = service.ResolveName("dan");
   // Output the list of candidates.
   foreach (NameResolution nameRes in resolvedNames)
   {
      Console.WriteLine("Contact name: " + nameRes.Mailbox.Name);
      Console.WriteLine("Contact e-mail address: " + nameRes.Mailbox.Address);
      Console.WriteLine("Mailbox type: " + nameRes.Mailbox.MailboxType);
   }

```

Ответ возвращает максимум 100 кандидатов, хотя потенциальных кандидатов может быть более 100. Чтобы определить, были ли возвращены только первые 100 кандидатов большего числа кандидатов, проверьте значение [IncludesAllResolutions](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.nameresolutioncollection.includesallresolutions%28v=exchg.80%29.aspx) в [объекте NameResolutionCollection.](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.nameresolutioncollection%28v=exchg.80%29.aspx) Если значение верно, возможные кандидаты больше не существуют; если значение ложное, метод возвращает только первые 100 из большего числа потенциальных кандидатов. 
  
Если вы работаете в крупной организации, вполне вероятно, что имя типа "dan" возвращает максимальное число 100 кандидатов. Чтобы уменьшить число возвращенных кандидатов, ограничь место поиска. В следующем примере используется переумерия [ResolveNameSearchLocation,](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.resolvenamesearchlocation%28v=exchg.80%29.aspx) чтобы указать, где искать для устранения неоднозначного имени. 
  
```cs
// Resolve the ambiguous name "dan".
// Only use the Contacts folder.
   NameResolutionCollection resolvedNames = service.ResolveName("dan", ResolveNameSearchLocation.ContactsOnly, false);
   // Output the list of candidates.   
   foreach (NameResolution nameRes in resolvedNames)
   {
      Console.WriteLine("Contact name: " + nameRes.Mailbox.Name);
      Console.WriteLine("Contact e-mail address: " + nameRes.Mailbox.Address);
      Console.WriteLine("Mailbox type: " + nameRes.Mailbox.MailboxType);
   }

```

Если контакты хранятся в папке, отличной от известной папки Contacts, используйте один из перегруженных методов, чтобы указать, где искать кандидатов. В следующем примере создается список папок для метода **ResolveName** на основе ИД папки. Папка **Была** сокращена для читаемости. 
  
```cs
// Create a list to store folders to search.
List<FolderId> folders = new List<FolderId>();
// Add a folder to the list based on the FolderId.
folders.Add(new FolderId("AABR8mboAAA="));
// Resolve the ambiguous name "dan".
// Only use the folders specified.
NameResolutionCollection resolvedNames = service.ResolveName("dan", folders, ResolveNameSearchLocation.ContactsOnly, false);
   foreach (NameResolution nameRes in resolvedNames)
   {
      Console.WriteLine("Contact name: " + nameRes.Mailbox.Name);
      Console.WriteLine("Contact e-mail address: " + nameRes.Mailbox.Address);
      Console.WriteLine("Mailbox type: " + nameRes.Mailbox.MailboxType);
   }

```

Если применить фильтры и не возвращать кандидатов, [в NameResolutionCollection](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.nameresolutioncollection%28v=exchg.80%29.aspx) будут содержаться нулевые записи. Вы можете проверить это, посмотрев свойство [Count](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.nameresolutioncollection.count%28v=exchg.80%29.aspx) коллекции. 
  
## <a name="resolve-ambiguous-names-by-using-ews"></a>Устранение неоднозначных имен с помощью EWS
<a name="bk_EWSMA"> </a>

Вы можете использовать операцию [ResolveNames](https://msdn.microsoft.com/library/c85207e1-1315-443b-94ec-2b58f405076b%28Office.15%29.aspx) EWS для определения возможных кандидатов на неоднозначное имя. Элемент [UnresolvedEntry содержит](https://msdn.microsoft.com/library/5ac6116a-3b24-40f8-a877-dbe9a6935919%28Office.15%29.aspx) неоднозначное имя, которое необходимо разрешить. В следующем примере показано, как разрешить имя Sadie. Это также XML-запрос, который используется управляемым API EWS при использовании метода [ResolveName,](#bk_EWSMA)за исключением того, что для допустимого вывода используется другое имя.
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <ResolveNames xmlns="https://schemas.microsoft.com/exchange/services/2006/messages"
                  xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
                  ReturnFullContactData="true">
      <UnresolvedEntry>Sadie</UnresolvedEntry>
    </ResolveNames>
  </soap:Body>
</soap:Envelope>
```

Ответ возвращает максимум 100 кандидатов, хотя может быть более 100 потенциальных кандидатов, чтобы определить, были ли возвращены только первые 100 кандидатов большего числа кандидатов, проверьте значение атрибута [IncludesLastItemInRange](https://msdn.microsoft.com/library/e7d6c7d3-548e-48b0-a313-bfef81e4832a%28Office.15%29.aspx) элемента [ResolutionSet.](https://msdn.microsoft.com/library/43d5b876-0e87-4414-9b1d-bff1c1ec825c%28Office.15%29.aspx) Если значение верно, возможные кандидаты больше не существуют; если значение ложное, операция возвращает только первые 100 из большего числа потенциальных кандидатов. 
  
В следующем примере показан XML-ответ при обнаружении одного кандидата. Помните, [что в ResolutionSet](https://msdn.microsoft.com/library/43d5b876-0e87-4414-9b1d-bff1c1ec825c%28Office.15%29.aspx) может содержаться до 100 кандидатов, каждый из которых представлен элементом [Resolution](https://msdn.microsoft.com/library/573bed4b-d7b1-4baf-b16f-0795cdebf1a7%28Office.15%29.aspx) и его детскими элементами. 
  
```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Body>
    <ResolveNamesResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                          xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                          xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:ResolveNamesResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:ResolutionSet TotalItemsInView="1" IncludesLastItemInRange="true">
            <t:Resolution>
              <t:Mailbox>
                <t:Name>Sadie Daniels</t:Name>
                <t:EmailAddress>Sadie@Contoso.com</t:EmailAddress>
                <t:RoutingType>SMTP</t:RoutingType>
                <t:MailboxType>Mailbox</t:MailboxType>
              </t:Mailbox>
              <t:Contact>
                <t:DisplayName>Sadie Daniels</t:DisplayName>
                <t:EmailAddresses>
                  <t:Entry Key="EmailAddress1">SMTP:Sadie@Contoso.com</t:Entry>
                </t:EmailAddresses>
                <t:ContactSource>ActiveDirectory</t:ContactSource>
              </t:Contact>
            </t:Resolution>
          </m:ResolutionSet>
        </m:ResolveNamesResponseMessage>
      </m:ResponseMessages>
    </ResolveNamesResponse>
  </soap:Body>
</soap:Envelope>
```

Вы не всегда будете подходить к кандидатам для вашего неоднозначного имени. В следующем примере показан XML-ответ, как ошибка, когда не найдены кандидаты.
  
```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Body>
    <ResolveNamesResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                          xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                          xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:ResolveNamesResponseMessage ResponseClass="Error">
          <m:MessageText>No results were found.</m:MessageText>
          <m:ResponseCode>ErrorNameResolutionNoResults</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
        </m:ResolveNamesResponseMessage>
      </m:ResponseMessages>
    </ResolveNamesResponse>
  </soap:Body>
</soap:Envelope>

```

## <a name="see-also"></a>См. также


- [Пользователи и контакты в EWS для Exchange](people-and-contacts-in-ews-in-exchange.md)
    
- [Как: развернуть группы рассылки с помощью EWS в Exchange 2013](how-to-expand-distribution-groups-by-using-ews-in-exchange-2013.md)
    

