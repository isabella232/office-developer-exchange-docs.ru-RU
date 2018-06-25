---
title: Разрешения неоднозначных имен с помощью веб-служб Exchange в Exchange 2013
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 1ba21c54-ecd2-4a1e-80d4-0f4171dea84f
description: Узнайте, как использовать управляемый API EWS или веб-служб Exchange для разрешения неоднозначных имен, получив возможные варианты из доменных служб Active Directory (AD DS) или папку контактов в почтовом ящике пользователя.
ms.openlocfilehash: 05a88043083a27d2e6d445cd71e5f3919c5a775d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761105"
---
# <a name="resolve-ambiguous-names-by-using-ews-in-exchange-2013"></a>Разрешения неоднозначных имен с помощью веб-служб Exchange в Exchange 2013

Узнайте, как использовать управляемый API EWS или веб-служб Exchange для разрешения неоднозначных имен, получив возможные варианты из доменных служб Active Directory (AD DS) или папку контактов в почтовом ящике пользователя.
  
Пользователь в вашей организации, получает рукописное список имен и адресов для сотрудников, которые посетившие обучения. Требуется отправить сообщение электронной почты с некоторые дополнительные сведения для пользователей в списке, но они не могут читать все адреса электронной почты. Если необходимо решить эту проблему для пользователей в приложении, может помочь веб-служб Exchange. Чтобы возвратить список возможных соответствий для выбора текста, такие как часть имени последнего можно использовать метод управляемый API EWS [ExchangeService.ResolveName](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.exchangeservice.resolvename%28v=exchg.80%29.aspx) или [ResolveNames](http://msdn.microsoft.com/library/c85207e1-1315-443b-94ec-2b58f405076b%28Office.15%29.aspx) операции веб-служб Exchange. Возвращаемых элементов может быть почтовые ящики пользователей общедоступных служб, группы рассылки и контакты. 
  
Обратите внимание на то, что Exchange сохраняет адреса электронной почты с с префиксами типов маршрутизации, например smtp или sip в массиве нескольких значений. Метод **ResolveName** и операции **ResolveNames** выполните частичное соответствие каждого значения этого массива при добавлении типа маршрутизации в начале неизвестное имя, например, «sip: User1». Если не указать тип маршрутизации, метод или операция будет по умолчанию установлено равным smtp, соответствует свойству основной адрес smtp и поиск нескольких значений массива. К примеру Если поиск User1 и не используйте код sip не появится sip:User1@Contoso.com в результате даже в том случае, если это допустимый почтового ящика. 
  
В одном запросе можно указать только одного неоднозначное имя. Если у вас есть список неоднозначные имена для решения, необходимо цикл по списку и вызовите метод или операции для каждой записи. Кандидатов из папки Контакты будут иметь значение идентификатора элемента ненулевое, которую можно использовать в вызове метода [Contact.Bind](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.contact.bind%28v=exchg.80%29.aspx) или запрос операции [GetItem](http://msdn.microsoft.com/library/769df8eb-9c72-48b5-a49f-82c6b86bc5fc%28Office.15%29.aspx) для получения дополнительных сведений. Если объект группы рассылки, можно использовать операцию EWS [ExpandDL](http://msdn.microsoft.com/library/affe84a5-ad98-4aba-83f4-8732938b763d%28Office.15%29.aspx) или метод [ExpandGroup(ItemId)](http://msdn.microsoft.com/en-us/library/office/ee356407%28v=exchg.80%29.aspx) управляемый API EWS для получения списка элементов. Если параметр _returnContactDetails_ или **ReturnFullContactData** EWS атрибута задано значение true, возвращаемых записей Active Directory с помощью метода **ResolveName** или **ResolveNames** операция будет включать дополнительные свойства описывающие контакт. Параметр _returnContactDetails_ или атрибут **ReturnFullContactData** не влияет на данные, возвращаемые для контактов и группы контактов. 
  
## <a name="resolve-ambiguous-names-by-using-ews-managed-api"></a>Разрешения неоднозначных имен с помощью управляемого интерфейса API веб-служб Exchange
<a name="bk_EWSMA"> </a>

Метод [ResolveName](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.exchangeservice.resolvename%28v=exchg.80%29.aspx) поиск кандидатов, которые соответствуют неоднозначное имя, передаваемого. Перегрузки метода **ResolveName** можно использовать для поиска кандидатов пять различными способами. 
  
**В таблице 1. Перегруженные методы ResolveName**

|**Способ**|**Как это работает**|
|:-----|:-----|
|[ResolveName(String)](http://msdn.microsoft.com/en-us/library/dd635548%28v=exchg.80%29.aspx) <br/> |Поиск контактов в папке контактов пользователя и глобальный список адресов (GAL) — в указанном порядке. Строковой переменной является неоднозначным имя, которое вы пытаетесь решить.  <br/> |
|[ResolveName (строка, ResolveNameSearchLocation, Boolean)](http://msdn.microsoft.com/en-us/library/dd634595%28v=exchg.80%29.aspx) <br/> |Поиск контактов в папке контактов по умолчанию и/или глобального списка адресов (GAL). Неоднозначное имя — это строковое значение, указывает расположение поиска папку Контакты и/или глобального списка адресов и логическое значение, которое указывает, нужно ли возвращать полное контактные данные.  <br/> |
|[ResolveName (строка, ResolveNameSearchLocation, Boolean, PropertySet)](http://msdn.microsoft.com/en-us/library/hh532803%28v=exchg.80%29.aspx) <br/> |Поиск контактов в папке контактов по умолчанию и/или глобального списка адресов (GAL). Этот метод позволяет задать свойства, которые возвращаются.  <br/> |
|[ResolveName (String, IEnumerable\<FolderId\>, ResolveNameSearchLocation, Boolean)](http://msdn.microsoft.com/en-us/library/dd636014%28v=exchg.80%29.aspx) <br/> |Поиск контактов в указанных папках контактов и/или глобального списка адресов (GAL). Этот метод можно использовать для передачи коллекции папок для поиска. Это позволяет искать в папки контактов, отличных от папки Контакты по умолчанию.  <br/> |
|[ResolveName (String, IEnumerable\<FolderId\>, ResolveNameSearchLocation, Boolean, PropertySet)](http://msdn.microsoft.com/en-us/library/hh532581%28v=exchg.80%29.aspx) <br/> |Находит контакты в глобальном списке адресов (GAL) и/или в указанных папках контактов. Этот метод позволяет задать свойства, которые возвращаются.  <br/> |
   
Начнем с простого примера. Приведенный ниже показано, как устранить текстовая строка «Дэн» и вывода имя и адрес электронной почты каждого кандидата найден. В этом примере предполагается, что эта **Служба** является допустимым объектом [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) и пользователь прошел проверку подлинности на сервере Exchange. 
  
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

Ответ возвращается не более 100 кандидатов, несмотря на то, что может быть больше 100 потенциальных кандидатов. Чтобы определить, возвращаются ли только первые 100 кандидатов большее число кандидатов, проверьте значение [IncludesAllResolutions](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.nameresolutioncollection.includesallresolutions%28v=exchg.80%29.aspx) в объекте [NameResolutionCollection](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.nameresolutioncollection%28v=exchg.80%29.aspx) . Если значение равно true, существует заканчивается возможных кандидатов; Если значение равно false, метод возвращается только первые 100 большего количества потенциальных кандидатов. 
  
При работе в крупной организации, скорее всего, что имя, например «Дэн» возвращает максимальное число 100 кандидатов. Чтобы уменьшить количество возвращаемых кандидатов, ограничение, где проводится поиск. В следующем примере используется перечисление [ResolveNameSearchLocation](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.resolvenamesearchlocation%28v=exchg.80%29.aspx) , чтобы указать, где поиска для разрешения неоднозначное имя. 
  
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

Если сохранить контакты в папке, отличной от известных контакты, используйте одну из перегруженных методов чтобы указать, где следует искать кандидатов. В следующем примере создается список папок для метода **ResolveName** на основании папки. **FolderId** был усечен для удобства чтения. 
  
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

Если нет кандидатов возвращаются и применение фильтров, [NameResolutionCollection](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.nameresolutioncollection%28v=exchg.80%29.aspx) будет содержать ноль записей. Вы можете проверить, посмотрев свойства [Count](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.nameresolutioncollection.count%28v=exchg.80%29.aspx) коллекции. 
  
## <a name="resolve-ambiguous-names-by-using-ews"></a>Разрешения неоднозначных имен с помощью веб-служб Exchange
<a name="bk_EWSMA"> </a>

Можно использовать операцию [ResolveNames](http://msdn.microsoft.com/library/c85207e1-1315-443b-94ec-2b58f405076b%28Office.15%29.aspx) веб-служб Exchange для определения возможных кандидатов для разрешения неоднозначных псевдонимов. Элемент [UnresolvedEntry](http://msdn.microsoft.com/library/5ac6116a-3b24-40f8-a877-dbe9a6935919%28Office.15%29.aspx) содержит неоднозначное имя, которое требуется разрешить. В следующем примере показано, как для разрешения имени Sadie. Это также запроса XML, управляемый API EWS при можно [использовать метод ResolveName](#bk_EWSMA), за исключением того, он использует имя допустимого вывода примеры.
  
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

Ответ возвращается не более 100 кандидатов, несмотря на то, что может быть больше 100 потенциальных кандидатов для определения, возвращаются ли только первые 100 кандидатов большее число кандидатов, проверьте значение [IncludesLastItemInRange](http://msdn.microsoft.com/library/e7d6c7d3-548e-48b0-a313-bfef81e4832a%28Office.15%29.aspx) атрибут [ResolutionSet](http://msdn.microsoft.com/library/43d5b876-0e87-4414-9b1d-bff1c1ec825c%28Office.15%29.aspx) элемента. Если значение равно true, существует заканчивается возможных кандидатов; Если значение равно false, операция возвращается только первые 100 большего количества потенциальных кандидатов. 
  
В следующем примере показано XML-ответ при обнаружении одного кандидата. Помните, что [ResolutionSet](http://msdn.microsoft.com/library/43d5b876-0e87-4414-9b1d-bff1c1ec825c%28Office.15%29.aspx) может содержать до 100 кандидатов, каждый из которых представлена элемент [решение](http://msdn.microsoft.com/library/573bed4b-d7b1-4baf-b16f-0795cdebf1a7%28Office.15%29.aspx) и его дочерние элементы. 
  
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

Не всегда вы собираетесь обеспечиваемые кандидатов для неоднозначное имя. В следующем примере показано XML-ответ, как ошибка, при обнаружении кандидатов.
  
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
    
- [Разверните узел группы рассылки с помощью веб-служб Exchange в Exchange 2013](how-to-expand-distribution-groups-by-using-ews-in-exchange-2013.md)
    

