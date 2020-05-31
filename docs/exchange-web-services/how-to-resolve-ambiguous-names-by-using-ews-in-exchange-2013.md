---
title: Устранение неоднозначности имен с помощью EWS в Exchange 2013
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 1ba21c54-ecd2-4a1e-80d4-0f4171dea84f
description: Узнайте, как использовать управляемый API EWS или EWS для разрешения неоднозначных имен, получая возможные совпадения из доменных служб Active Directory (AD DS) или из папки "Контакты" в почтовом ящике пользователя.
ms.openlocfilehash: 05a88043083a27d2e6d445cd71e5f3919c5a775d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761105"
---
# <a name="resolve-ambiguous-names-by-using-ews-in-exchange-2013"></a>Устранение неоднозначности имен с помощью EWS в Exchange 2013

Узнайте, как использовать управляемый API EWS или EWS для разрешения неоднозначных имен, получая возможные совпадения из доменных служб Active Directory (AD DS) или из папки "Контакты" в почтовом ящике пользователя.
  
Пользователю в вашей организации предоставляется письменный список имен и адресов для сотрудников, которые проводят обучающий сеанс. Они хотят отправить сообщение электронной почты с дополнительными сведениями о пользователях в списке, но не могут прочитать адрес электронной почты. Если вы хотите решить эту проблему для пользователей в вашем приложении, EWS поможет. Можно использовать метод управляемого API [ExchangeService. ресолвенаме](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.exchangeservice.resolvename%28v=exchg.80%29.aspx) EWS или [ResolveNames](http://msdn.microsoft.com/library/c85207e1-1315-443b-94ec-2b58f405076b%28Office.15%29.aspx) EWS для возврата списка потенциальных совпадений для выделенного текста, например части фамилии. Возвращаемые элементы могут быть общедоступными почтовыми ящиками пользователей, группами рассылки и контактами. 
  
Обратите внимание, что Exchange сохраняет адреса электронной почты с предфиксированными типами маршрутизации, такими как SMTP или SIP, в массиве с несколькими значениями. Метод **ресолвенаме** и операция **ResolveNames** выполняют частичное соответствие с каждым значением этого массива при добавлении типа маршрутизации в начале неизвестного имени, например "SIP: Пользователь1". Если не указать тип маршрутизации, метод или операция по умолчанию будут использовать SMTP, сопоставлять их с основным свойством SMTP-адреса, а не выполнять поиск по многозначному массиву. Например, если вы ищете Пользователь1 и не включили префикс SIP, вы не будете получать sip:User1@Contoso.com в результате, даже если это действительный почтовый ящик. 
  
В одном запросе можно указать только одно неоднозначное имя. Если у вас есть список неоднозначных имен для разрешения, вам потребуется перебрать список и вызвать метод или операцию для каждой записи. Для кандидатов из папки контактов пользователя будет задано значение идентификатора элемента, отличное от NULL, которое затем можно использовать в запросе метода [Contact. Bind](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.contact.bind%28v=exchg.80%29.aspx) или операции [GetItem](http://msdn.microsoft.com/library/769df8eb-9c72-48b5-a49f-82c6b86bc5fc%28Office.15%29.aspx) для получения дополнительных сведений. Если кандидат является группой рассылки, для получения списка элементов можно использовать метод управляемого API [ExpandGroup (ItemId)](http://msdn.microsoft.com/en-us/library/office/ee356407%28v=exchg.80%29.aspx) EWS или [ExpandDL](http://msdn.microsoft.com/library/affe84a5-ad98-4aba-83f4-8732938b763d%28Office.15%29.aspx) EWS. Если для параметра _ретурнконтактдетаилс_ или атрибута **ретурнфуллконтактдата** EWS задано значение true, записи Active Directory, возвращаемые с помощью метода **ресолвенаме** или операции **ResolveNames** , будут включать дополнительные свойства, описывающие контакт. Параметр _ретурнконтактдетаилс_ или атрибут **ретурнфуллконтактдата** не влияет на данные, возвращаемые для контактов и групп контактов. 
  
## <a name="resolve-ambiguous-names-by-using-ews-managed-api"></a>Разрешение неоднозначных имен с помощью управляемого API EWS
<a name="bk_EWSMA"> </a>

Метод [ресолвенаме](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.exchangeservice.resolvename%28v=exchg.80%29.aspx) можно использовать для поиска кандидатов, которые соответствуют неоднозначному имени, которое вы передавали. С помощью перегрузок метода **ресолвенаме** можно выполнять поиск кандидатов пять различными способами. 
  
**Таблица 1. Перегруженные методы Ресолвенаме**

|**Метод**|**Принцип работы**|
|:-----|:-----|
|[Ресолвенаме (строка)](http://msdn.microsoft.com/en-us/library/dd635548%28v=exchg.80%29.aspx) <br/> |Поиск контактов в папке "Контакты" пользователя и глобальном списке адресов (GAL) в указанном порядке. Строковая переменная — это неоднозначное имя, которое вы пытаетесь разрешить.  <br/> |
|[Ресолвенаме (String, Ресолвенамесеарчлокатион, Boolean)](http://msdn.microsoft.com/en-us/library/dd634595%28v=exchg.80%29.aspx) <br/> |Поиск контактов в папке "Контакты" по умолчанию и/или глобальном списке адресов (GAL). Строковое значение — это неоднозначное имя, место поиска указывает папку контактов и/или глобальный список адресов, а логическое значение указывает, следует ли возвратить полные контактные данные.  <br/> |
|[Ресолвенаме (String, Ресолвенамесеарчлокатион, Boolean, свойство)](http://msdn.microsoft.com/en-us/library/hh532803%28v=exchg.80%29.aspx) <br/> |Поиск контактов в папке "Контакты" по умолчанию и/или глобальном списке адресов (GAL). Этот метод позволяет задать возвращаемые свойства.  <br/> |
|[Ресолвенаме (String, IEnumerable\<FolderId\>, ресолвенамесеарчлокатион, Boolean)](http://msdn.microsoft.com/en-us/library/dd636014%28v=exchg.80%29.aspx) <br/> |Поиск контактов в указанных папках контактов и/или глобальном списке адресов (GAL). Этот метод можно использовать для передачи коллекции папок для поиска. Это позволяет искать в папках контактов, отличных от папки контактов по умолчанию.  <br/> |
|[Ресолвенаме (String, IEnumerable\<FolderId\>, Ресолвенамесеарчлокатион, Boolean, свойство)](http://msdn.microsoft.com/en-us/library/hh532581%28v=exchg.80%29.aspx) <br/> |Поиск контактов в глобальном списке адресов (GAL) и/или в определенных папках контактов. Этот метод позволяет задать возвращаемые свойства.  <br/> |
   
Начнем с простого примера. В приведенном ниже примере показано, как разрешить текстовую строку "" "") и вывести имя и адрес электронной почты каждого найденного кандидата. В этом примере предполагается, что **служба** является действительным объектом [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx), и что пользователь прошел проверку подлинности на сервере Exchange server. 
  
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

Ответ возвращает максимум 100 кандидатов, хотя может быть более 100 потенциальных кандидатов. Чтобы определить, были ли возвращены только первые 100 кандидатов большего числа кандидатов, проверьте значение параметра [инклудесаллресолутионс](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.nameresolutioncollection.includesallresolutions%28v=exchg.80%29.aspx) в объекте [намересолутионколлектион](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.nameresolutioncollection%28v=exchg.80%29.aspx) . Если задано значение true, возможны невероятные варианты. Если значение равно false, метод возвращает только первые 100 с большим количеством потенциальных кандидатов. 
  
Если вы работаете в крупной организации, вероятно, что имя, например "" "" "" ", будет возвращать максимальное число кандидатов 100. Чтобы уменьшить количество возвращаемых кандидатов, Ограничьте поиск. В следующем примере показано, как использовать перечисление [ресолвенамесеарчлокатион](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.resolvenamesearchlocation%28v=exchg.80%29.aspx) , чтобы указать, где искать для устранения неоднозначного имени. 
  
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

Если вы храните контакты в папке, отличной от общеизвестных контактов, используйте один из перегруженных методов, чтобы указать, где искать кандидатов. В следующем примере создается список папок для метода **ресолвенаме** на основе идентификатора папки. **FolderId** был сокращен для удобочитаемости. 
  
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

Если вы применяете фильтры и не возвращаете кандидатов, [намересолутионколлектион](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.nameresolutioncollection%28v=exchg.80%29.aspx) будет содержать нулевые записи. Это можно проверить, просмотрев свойство [Count](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.nameresolutioncollection.count%28v=exchg.80%29.aspx) коллекции. 
  
## <a name="resolve-ambiguous-names-by-using-ews"></a>Разрешение неоднозначных имен с помощью EWS
<a name="bk_EWSMA"> </a>

Вы можете использовать операцию [ResolveNames](http://msdn.microsoft.com/library/c85207e1-1315-443b-94ec-2b58f405076b%28Office.15%29.aspx) EWS для определения возможных кандидатов на неоднозначное имя. Элемент [унресолведентри](http://msdn.microsoft.com/library/5ac6116a-3b24-40f8-a877-dbe9a6935919%28Office.15%29.aspx) содержит неоднозначное имя, которое требуется разрешить. В приведенном ниже примере показано, как разрешить имя Ольга. Это также запрос XML, который использует управляемый API EWS при [использовании метода ресолвенаме](#bk_EWSMA), за исключением того, что для допустимых выходных примеров используется другое имя.
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <ResolveNames xmlns="http://schemas.microsoft.com/exchange/services/2006/messages"
                  xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
                  ReturnFullContactData="true">
      <UnresolvedEntry>Sadie</UnresolvedEntry>
    </ResolveNames>
  </soap:Body>
</soap:Envelope>
```

Ответ возвращает максимум 100 кандидатов, 100 хотя для определения того, были ли возвращены только первые 100 кандидатов с большим количеством кандидатов, следует проверить значение атрибута [инклудесластитеминранже](http://msdn.microsoft.com/library/e7d6c7d3-548e-48b0-a313-bfef81e4832a%28Office.15%29.aspx) элемента [Resolution](http://msdn.microsoft.com/library/43d5b876-0e87-4414-9b1d-bff1c1ec825c%28Office.15%29.aspx) . Если задано значение true, возможны невероятные варианты. Если значение равно false, операция возвращает только первые 100 с большим количеством потенциальных кандидатов. 
  
В следующем примере показан ответ XML при обнаружении одного кандидата. Помните [, что дочерний элемент может](http://msdn.microsoft.com/library/43d5b876-0e87-4414-9b1d-bff1c1ec825c%28Office.15%29.aspx) содержать до 100 кандидатов, каждый из которых представлен элементом [разрешения](http://msdn.microsoft.com/library/573bed4b-d7b1-4baf-b16f-0795cdebf1a7%28Office.15%29.aspx) и его дочерними элементами. 
  
```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Body>
    <ResolveNamesResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                          xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                          xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

Вы не всегда собираетесь с кандидатами на неоднозначное имя. В следующем примере показан ответ XML в виде ошибки, если кандидатов не найдено.
  
```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Body>
    <ResolveNamesResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                          xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                          xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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
    

