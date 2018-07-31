---
title: Контакты доступа роли представителя с помощью веб-служб Exchange в Exchange
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 3cd34c14-18b0-4fe2-a4c2-d884318c88fc
description: Узнайте, как получить доступ к роли представителя контактов с помощью управляемого интерфейса API веб-служб Exchange или веб-служб Exchange в Exchange.
ms.openlocfilehash: 47540082f7e60645cae60fe2347e50e17cd226dd
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/28/2018
ms.locfileid: "21353723"
---
# <a name="access-contacts-as-a-delegate-by-using-ews-in-exchange"></a>Контакты доступа роли представителя с помощью веб-служб Exchange в Exchange

Узнайте, как получить доступ к роли представителя контактов с помощью управляемого интерфейса API веб-служб Exchange или веб-служб Exchange в Exchange.
  
Можно использовать управляемый API EWS или веб-служб Exchange для предоставления пользователю доступа к владельца почтового ящика папки «Контакты». Делегат может затем создание контактов от имени владельца почтового ящика и извлечения, обновление и удаление контактов из папки Контакты владельца почтового ящика, в зависимости от их разрешения.
  
Роли представителя используйте ту же методов и операций для доступа владельца почтового ящика папки «Контакты», которая используется для доступа к папке контактов. Основное различие —, что вам следует использовать [явный доступ](delegate-access-and-ews-in-exchange.md#bk_explicit) для поиска или создание элемента контакта и затем после определения идентификатора элемента, можно использовать [неявный доступ](delegate-access-and-ews-in-exchange.md#bk_implicit) для получения, обновить или удалить элемент. 
  
**В таблице 1. Управляемый API EWS методы и операции веб-служб Exchange для доступа к контакту роли представителя**

|**Задача**|**Используйте этот метод управляемый API EWS...**|**Используйте эту операцию EWS...**|
|:-----|:-----|:-----|
|Создание контакта в качестве делегата  <br/> |[Item.Save](http://msdn.microsoft.com/en-us/library/dd635209%28v=exchg.80%29.aspx) , где параметр [FolderId](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx) предоставляет [явный доступ](delegate-access-and-ews-in-exchange.md#bk_explicitewsma) к папке Контакты владельца почтового ящика  <br/> |[CreateItem](http://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) , где элемент [почтового ящика](http://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) указывает [EmailAddress](http://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) владельца почтового ящика  <br/> |
|Создание нескольких контактов в качестве делегата  <br/> |[ExchangeService.CreateItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.createitems%28v=exchg.80%29.aspx) , где параметр **FolderId** предоставляет [явный доступ](delegate-access-and-ews-in-exchange.md#bk_explicitewsma) к папке Контакты владельца почтового ящика  <br/> |[CreateItem](http://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) , где элемент [почтового ящика](http://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) указывает [EmailAddress](http://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) владельца почтового ящика  <br/> |
|Разрешить контакт роли представителя  <br/> |[ExchangeService.ResolveName](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.resolvename%28v=exchg.80%29.aspx) , где параметр [FolderId](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx) предоставляет [явный доступ](delegate-access-and-ews-in-exchange.md#bk_explicitewsma) к папке Контакты владельца почтового ящика  <br/> |[ResolveNames](http://msdn.microsoft.com/library/6b4eb4b3-9ad6-4804-a09f-7e20cfea4dbb%28Office.15%29.aspx) , где элемент [почтового ящика](http://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) указывает [EmailAddress](http://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) владельца почтового ящика  <br/> |
|Поиск или найдите контакт роли представителя  <br/> |[ExchangeService.FindItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) , где параметр **FolderId** предоставляет [явный доступ](delegate-access-and-ews-in-exchange.md#bk_explicitewsma) к папке Контакты владельца почтового ящика  <br/> |[FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) , где элемент [почтового ящика](http://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) указывает [EmailAddress](http://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) владельца почтового ящика  <br/> |
|Получение контакт роли представителя  <br/> |[Contact.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.contact.bind%28v=exchg.80%29.aspx) <br/> |[GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) <br/> |
|Обновление контакт роли представителя  <br/> |[Contact.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.contact.bind%28v=exchg.80%29.aspx) , а затем [Contact.Update](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.update%28v=exchg.80%29.aspx) <br/> |[GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) , а затем [UpdateItem](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) <br/> |
|Удаление контакта в качестве делегата  <br/> |[Contact.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.contact.bind%28v=exchg.80%29.aspx) , а затем [Contact.Delete](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.delete%28v=exchg.80%29.aspx) <br/> |[GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) , а затем [DeleteItem](../web-service-reference/deleteitem-operation.md) <br/> |
   
> [!NOTE]
> В примерах кода в этой статье primary@contoso.com — это владелец почтового ящика. 

<a name="bk_prereq"> </a>

## <a name="prerequisite-tasks"></a>Обязательные задачи

Пользователь может получить доступ к папки контактов владельца почтового ящика для делегата, пользователь должен быть [добавлен в качестве делегата с разрешениями](how-to-add-and-remove-delegates-by-using-ews-in-exchange.md) для папки «Контакты» владельца почтового ящика. 

<a name="bk_createewsma"> </a>

## <a name="create-a-contact-as-a-delegate-by-using-the-ews-managed-api"></a>Создание контактов как делегат с помощью управляемого интерфейса API веб-служб Exchange

Управляемый API EWS позволяет использовать объект службы для пользователя делегат для создания контактов для владельца почтового ящика. В этом примере показано, как использовать метод [сохранения](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.save%28v=exchg.80%29.aspx) для создания собрания и отправки приглашений на собрание участникам. 
  
В этом примере предполагается, что эта **Служба** является допустимым объектом [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) делегата и делегата предоставлены необходимые разрешения для папки «Контакты» владельца почтового ящика. 
  
```cs
 public static void DelegateAccessCreateContact(ExchangeService service)
{
    // Create the contact.
    Contact contact = new Contact(service);
    // Specify the name and how the contact should be filed.
    contact.GivenName = "Brian";
    contact.MiddleName = "David";
    contact.Surname = "Johnson";
    contact.FileAsMapping = FileAsMapping.SurnameCommaGivenName;
    // Specify the company name.
    contact.CompanyName = "Contoso";
    // Specify the business, home, and car phone numbers.
    contact.PhoneNumbers[PhoneNumberKey.BusinessPhone] = "425-555-0110";
    contact.PhoneNumbers[PhoneNumberKey.HomePhone] = "425-555-0120";
    contact.PhoneNumbers[PhoneNumberKey.CarPhone] = "425-555-0130";
    // Specify two email addresses.
    contact.EmailAddresses[EmailAddressKey.EmailAddress1] = 
        new EmailAddress("brian_1@contoso.com");
    contact.EmailAddresses[EmailAddressKey.EmailAddress2] = 
        new EmailAddress("brian_2@contoso.com");
    // Save the contact in the mailbox owner's Contacts folder.
    // This method call results in a CreateItem call to EWS. 
    // The contact identifier contains the context for the mailbox owner's 
    // Contact folder. Any additional actions take on this contact will 
    // be performed in the mailbox owner's mailbox. 
    contact.Save(new FolderId(WellKnownFolderName.Contacts, 
        "primary@contoso.com"));
    // Verify that the contact was created.
    // This method call results in a GetItem call to EWS
    // to load the display name property on the contact. 
    contact.Load(new PropertySet (ContactSchema.DisplayName));
    Console.WriteLine("\nContact created: " + contact.DisplayName + "\n");
}
```

Обратите внимание, что при сохранении элемента вызова метода [Сохранить](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.save%28v=exchg.80%29.aspx) необходимо определить владельца почтового ящика папки «Контакты». Если владелец почтового ящика папки «Контакты» не указан, запрос на собрание получает сохранены делегата папки «Контакты» и не владельца почтового ящика папки «Контакты». В вызове метода **Сохранить** в двухстороннем может включать владельца почтового ящика папки «Контакты». Рекомендуется создать новый экземпляр объекта [FolderId](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx) с помощью [WellKnownFolderName](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.wellknownfoldername%28v=exchg.80%29.aspx) и SMTP-адреса владельца почтового ящика. 
  
```cs
contact.Save(new FolderId(WellKnownFolderName.Contacts, "primary@contoso.com"));
```

Тем не менее, можно также [привязать](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) к папке контактов во-первых и затем используйте идентификатор папки в вызове метода **сохранения** . Однако следует помнить, что при этом создается дополнительных вызовов веб-служб Exchange. 
  
```cs
    // Identify the mailbox owner's SMTP address 
    // and bind to their Contacts folder.
    Mailbox primary = new Mailbox("primary@contoso.com"); 
    Folder primaryContacts = Folder.Bind(service, new FolderId(WellKnownFolderName.Contacts, primary)); 
…
    // Save the contact to the mailbox owner's Contacts folder.
    meeting.Save(primaryContacts.Id);
```

<a name="bk_createews"> </a>

## <a name="create-a-contact-as-a-delegate-by-using-ews"></a>Создание контактов в качестве делегата с помощью веб-служб Exchange

Веб-служб Exchange позволяет использовать объект службы для пользователя делегат для создания элементов контактов для владельца почтового ящика. В этом примере показано, как использовать операции [CreateItem](http://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) для создания контакта. 
  
Это также XML-запрос, который отправляет управляемый API EWS при использовании метода **Сохранить** , чтобы [Создать контакт](#bk_createewsma).
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
  </soap:Header>
  <soap:Body>
    <m:CreateItem MessageDisposition="SaveOnly">
      <m:SavedItemFolderId>
        <t:DistinguishedFolderId Id="contacts">
          <t:Mailbox>
            <t:EmailAddress>primary@contoso.com</t:EmailAddress>
          </t:Mailbox>
        </t:DistinguishedFolderId>
      </m:SavedItemFolderId>
      <m:Items>
        <t:Contact>
          <t:FileAsMapping>LastCommaFirst</t:FileAsMapping>
          <t:GivenName>Brian</t:GivenName>
          <t:MiddleName>David</t:MiddleName>
          <t:CompanyName>Contoso</t:CompanyName>
          <t:EmailAddresses>
            <t:Entry Key="EmailAddress1">brian_1@contoso.com</t:Entry>
            <t:Entry Key="EmailAddress2">brian_2@contoso.com</t:Entry>
          </t:EmailAddresses>
          <t:PhoneNumbers>
            <t:Entry Key="BusinessPhone">425-555-0110</t:Entry>
            <t:Entry Key="HomePhone">425-555-0120</t:Entry>
            <t:Entry Key="CarPhone">425-555-0130</t:Entry>
          </t:PhoneNumbers>
          <t:Surname>Johnson</t:Surname>
        </t:Contact>
      </m:Items>
    </m:CreateItem>
  </soap:Body>
</soap:Envelope>
```

Сервер отвечает на запрос **CreateItem** [CreateItemResponse](http://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) сообщение, которое содержит значение элемента [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) **NoError**, это означает, что контакт был успешно создан. Ответ также содержит идентификатор только что созданный контакта.

<a name="bk_resolveewsma"> </a>

## <a name="resolve-a-contact-as-a-delegate-by-using-the-ews-managed-api"></a>Разрешить контакт роли представителя с помощью управляемого интерфейса API веб-служб Exchange

Поиск контакта на основе возможно неоднозначное имя или терминов, необходимо использовать один из методов [ExchangeService.ResolveName](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.resolvename%28v=exchg.80%29.aspx) , включает параметр [FolderId](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx) , таким образом, можно указать папку Контакты владельца почтового ящика. 
  
```cs
private static void DelegateAccessResolveContacts(ExchangeService service)
{
    // Create a list to store folders to search.
    List<FolderId> folders = new List<FolderId>();
   
    // Add the mailbox owner's folder to the list.
    folders.Add(new FolderId(WellKnownFolderName.Contacts, 
        "primary@contoso.com"));
    
    // Resolve the ambiguous name "Johnson".
    // This method call results in a ResolveNames call to EWS.
    NameResolutionCollection resolvedNames = service.ResolveName(
        "johnson", folders, ResolveNameSearchLocation.ContactsOnly, true);
    // Output the list of candidate email addresses and contact names.
    foreach (NameResolution nameRes in resolvedNames)
    {
        Console.WriteLine("Contact e-mail address: " + nameRes.Mailbox.Address);
        Console.WriteLine("Contact ID: " + nameRes.Mailbox.Id);
    }
}
```

После вызова метода **ResolveNames** возвращает ответ с кодом, можно [получить, обновить или удалить контакт](#bk_getewsma) с помощью идентификатора и [неявный доступ](delegate-access-and-ews-in-exchange.md#bk_implicit)&mdash;и необходимо указать SMTP-адреса владельца почтового ящика. 

<a name="bk_resolveews"> </a>

## <a name="resolve-a-contact-as-a-delegate-by-using-ews"></a>Разрешения роли представителя контакта с помощью веб-служб Exchange

Веб-служб Exchange позволяет использовать объект службы для пользователя делегат для разрешения имен частичное в папке контактов владельца почтового ящика. В этом примере показано, как использовать операцию [ResolveNames](http://msdn.microsoft.com/library/6b4eb4b3-9ad6-4804-a09f-7e20cfea4dbb%28Office.15%29.aspx) Поиск собраний в владельца почтового ящика папки «Контакты», содержащие слово «johnson». 
  
Это также запроса XML, управляемый API EWS отправляет при использовании **ResolveName** метод для [разрешения контакта](#bk_resolveewsma).
  
```xml
 <?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
  </soap:Header>
  <soap:Body>
    <m:ResolveNames ReturnFullContactData="true"
                    SearchScope="Contacts">
      <m:ParentFolderIds>
        <t:DistinguishedFolderId Id="contacts">
          <t:Mailbox>
            <t:EmailAddress>primary@contoso.com</t:EmailAddress>
          </t:Mailbox>
        </t:DistinguishedFolderId>
      </m:ParentFolderIds>
      <m:UnresolvedEntry>johnson</m:UnresolvedEntry>
    </m:ResolveNames>
  </soap:Body>
</soap:Envelope>
```

Сервер отвечает на запрос **ResolveNames** [ResolveNamesResponse](http://msdn.microsoft.com/library/5e7be1e2-44ea-403f-9135-2388d030078c%28Office.15%29.aspx) сообщение, которое содержит значение элемента [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) **NoError**, который указывает, что операция успешно завершена и найти только один результат, или **ErrorNameResolutionMultipleResults** Если найдено несколько результатов - являющийся, отображаемые в третьем примере кода на основании контакт, [Создание контактов роли представителя с помощью управляемого интерфейса API веб-служб Exchange](#bk_createewsma). Ответ также содержит [ItemId](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) каждого результата. 
  
Значение элемента **ItemId** был усечен для удобства чтения. 
  
```XML
 <?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="893"
                         MinorBuildNumber="17"
                         Version="V2_10"
                         xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body>
    <m:ResolveNamesResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
                            xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:ResolveNamesResponseMessage ResponseClass="Warning">
          <m:MessageText>Multiple results were found.</m:MessageText>
          <m:ResponseCode>ErrorNameResolutionMultipleResults</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
          <m:ResolutionSet TotalItemsInView="2"
                           IncludesLastItemInRange="true">
            <t:Resolution>
              <t:Mailbox>
                <t:Name>brian_1@contoso.com</t:Name>
                <t:EmailAddress>brian_1@contoso.com</t:EmailAddress>
                <t:RoutingType>SMTP</t:RoutingType>
                <t:MailboxType>Contact</t:MailboxType>
                <t:ItemId Id="iMihAAA="
                          ChangeKey="EQAAABYAAADOilbYa8KaT7ZgMoTz2P+hAAABiPQo" />
              </t:Mailbox>
            </t:Resolution>
            <t:Resolution>
              <t:Mailbox>
                <t:Name>brian_2@contoso.com</t:Name>
                <t:EmailAddress>brian_2@contoso.com</t:EmailAddress>
                <t:RoutingType>SMTP</t:RoutingType>
                <t:MailboxType>Contact</t:MailboxType>
                <t:ItemId Id="iMihAAA="
                          ChangeKey="EQAAABYAAADOilbYa8KaT7ZgMoTz2P+hAAABiPQo" />
              </t:Mailbox>
            </t:Resolution>
          </m:ResolutionSet>
        </m:ResolveNamesResponseMessage>
      </m:ResponseMessages>
    </m:ResolveNamesResponse>
  </s:Body>
</s:Envelope>
```

Теперь, когда у вас есть **идентификатор элемента** для контактов, которые соответствуют неоднозначное имя, можно [получить, обновить и удаление элементов контактов в качестве делегата с помощью веб-служб Exchange](#bk_getews) с помощью **ItemId** и [неявный доступ](delegate-access-and-ews-in-exchange.md#bk_implicit)&mdash;и необходимо указать SMTP-адреса владельца почтового ящика. 

<a name="bk_getewsma"> </a>

## <a name="get-update-or-delete-contact-items-as-a-delegate-by-using-the-ews-managed-api"></a>Получение, обновление и удаление элементов контактов роли представителя с помощью управляемого интерфейса API веб-служб Exchange

Можно использовать управляемый API EWS для получения, обновить или удалить контакт так же, как выполнять эти действия, если вы не используете делегированный доступ. Единственное отличие — объект службы для делегата. Идентификатор элемента, включенные в вызове метода **Привязка** уникальным образом определяет элемент в хранилище почтовых ящиков в папке контактов владельца почтового ящика. 
  
**В таблице 2. Управляемый API EWS методы работы с контактом роли представителя**

|**Задача**|**Метод управляемого API EWS**|**Пример кода**|
|:-----|:-----|:-----|
|Получение контакта.  <br/> |[Привязка](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.bind%28v=exchg.80%29.aspx) <br/> |[Получение элемента с помощью управляемого API EWS](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_getewsma) <br/> |
|Обновление контакта  <br/> |[Привязка](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.bind%28v=exchg.80%29.aspx) следуют [обновления](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.update%28v=exchg.80%29.aspx) <br/> |[Изменение элемента с помощью управляемого API EWS](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_updateewsma) <br/> |
|Удалить контакт  <br/> |[Привязка](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.bind%28v=exchg.80%29.aspx) , а затем [Удалить](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.delete%28v=exchg.80%29.aspx) <br/> |[Удаление элемента с помощью управляемого API EWS](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_deleteewsma) <br/> |

<a name="bk_getews"> </a>

## <a name="get-update-or-delete-contact-items-as-a-delegate-by-using-ews"></a>Получение, обновление и удаление элементов контактов роли представителя с помощью веб-служб Exchange

Чтобы получить, обновить или удалить контакт собранием или встречей так же, как выполнять эти действия, если вы не используете делегированный доступ, можно использовать веб-служб Exchange. Единственное отличие — объект службы для делегата. Идентификатор элемента, включенных в запрос [GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) уникальным образом определяет элемент в хранилище почтовых ящиков в папке контактов владельца почтового ящика. 
  
**В таблице 3. Операции EWS для работы с контактом роли представителя**

|**Задача**|**Операция служб EWS**|**Пример**|
|:-----|:-----|:-----|
|Получение контакта.  <br/> |[GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) <br/> |[Получение элемента с помощью веб-служб Exchange](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_getews) <br/> |
|Обновление контакта  <br/> |[GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) , а затем [UpdateItem](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) <br/> |[Изменение элемента с помощью веб-служб Exchange](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_updateews) <br/> |
|Удалить контакт  <br/> |[GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) , а затем [DeleteItem](../web-service-reference/deleteitem-operation.md) <br/> |[Удаление элемента с помощью веб-служб Exchange](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_deleteews) <br/> |
   
## <a name="see-also"></a>См. также

- [Передача прав доступа и EWS в Exchange](delegate-access-and-ews-in-exchange.md)
- [Добавление и удаление делегаты с помощью веб-служб Exchange в Exchange](how-to-add-and-remove-delegates-by-using-ews-in-exchange.md)
- [Настройка разрешений папки другого пользователя с помощью веб-служб Exchange в Exchange](how-to-set-folder-permissions-for-another-user-by-using-ews-in-exchange.md)
- [Пользователи и контакты в EWS для Exchange](people-and-contacts-in-ews-in-exchange.md)
- [Разрешения неоднозначных имен с помощью веб-служб Exchange в Exchange 2013](how-to-resolve-ambiguous-names-by-using-ews-in-exchange-2013.md)
    

