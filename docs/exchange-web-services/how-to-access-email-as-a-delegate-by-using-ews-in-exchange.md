---
title: Доступ к электронной почте в качестве делегата с помощью веб-служб Exchange в Exchange
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: a8123604-c7c0-405d-a0ed-7a9b4a431bfd
description: Узнайте, как получить доступ к электронной почте роли представителя с помощью управляемого интерфейса API веб-служб Exchange или веб-служб Exchange в Exchange.
ms.openlocfilehash: 8331f337136426913347cf6941d64b4611922d74
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760972"
---
# <a name="access-email-as-a-delegate-by-using-ews-in-exchange"></a>Доступ к электронной почте в качестве делегата с помощью веб-служб Exchange в Exchange

Узнайте, как получить доступ к электронной почте роли представителя с помощью управляемого интерфейса API веб-служб Exchange или веб-служб Exchange в Exchange.
  
Можно использовать управляемый API EWS или делегирование EWS, чтобы предоставить пользователю доступ к папке "Входящие" владельца почтового ящика. Делегат можно затем Создание приглашений на собрания от имени владельца почтового ящика, поиск электронной почты и извлечь, обновление и удаление электронной почты из папки "Входящие" владельца почтового ящика, в зависимости от их разрешения.
  
Роли представителя используйте ту же методов и операций на доступ к папке "Входящие" владельца почтового ящика, которая используется для доступа к папке "Входящие" без делегированный доступ. Основное различие —, что вам следует использовать [явный доступ](delegate-access-and-ews-in-exchange.md#bk_explicit) для поиска или создать элемент электронной почты, и затем после определения идентификатора элемента, можно использовать [неявный доступ](delegate-access-and-ews-in-exchange.md#bk_implicit) для получения, обновить или удалить элемент. 
  
**В таблице 1. Управляемый API EWS методы и операции веб-служб Exchange для доступа к электронной почте в качестве делегата**

|**Если вы хотите...**|**Используйте этот метод управляемый API EWS...**|**Используйте эту операцию EWS...**|
|:-----|:-----|:-----|
|Создание и отправка сообщения электронной почты как делегат  <br/> |[EmailMessage.Save](http://msdn.microsoft.com/en-us/library/dd635209%28v=exchg.80%29.aspx) , где параметр [FolderId](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx) предоставляет [явный доступ](delegate-access-and-ews-in-exchange.md#bk_explicitewsma) к папке «Черновики» владельца почтового ящика  <br/> [EmailMessage.SendAndSaveCopy](http://msdn.microsoft.com/en-us/library/dd634248%28v=exchg.80%29.aspx) , где параметр [FolderId](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx) предоставляет [явный доступ](delegate-access-and-ews-in-exchange.md#bk_explicitewsma) к папке "Отправленные" владельца почтового ящика  <br/> |[CreateItem](http://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) , где элемент [почтового ящика](http://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) указывает [EmailAddress](http://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) владельца почтового ящика  <br/> [SendItem](http://msdn.microsoft.com/library/a966da19-b05a-4504-ac98-91acc1667b9a%28Office.15%29.aspx) , где элемент [почтового ящика](http://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) указывает [EmailAddress](http://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) владельца почтового ящика  <br/> |
|Создание нескольких сообщений электронной почты в качестве делегата  <br/> |[ExchangeService.CreateItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.createitems%28v=exchg.80%29.aspx) , где параметр **FolderId** предоставляет [явный доступ](delegate-access-and-ews-in-exchange.md#bk_explicitewsma) к папке "Входящие" владельца почтового ящика  <br/> |[CreateItem](http://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) , где элемент [почтового ящика](http://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) указывает [EmailAddress](http://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) владельца почтового ящика  <br/> |
|Поиск и искать сообщения электронной почты в качестве делегата  <br/> |[ExchangeService.FindItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) , где параметр **FolderId** предоставляет [явный доступ](delegate-access-and-ews-in-exchange.md#bk_explicitewsma) к папке "Входящие" владельца почтового ящика  <br/> |[FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) , где элемент [почтового ящика](http://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) указывает [EmailAddress](http://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) владельца почтового ящика  <br/> |
|Получите сообщение электронной почты как делегат  <br/> |[EmailMessage.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.bind%28v=exchg.80%29.aspx) <br/> |[GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) <br/> |
|Обновление сообщения электронной почты в качестве делегата  <br/> |[EmailMessage.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.bind%28v=exchg.80%29.aspx) , а затем [EmailMessage.Update](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.update%28v=exchg.80%29.aspx) <br/> |[GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) , а затем [UpdateItem](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) <br/> |
|Удаление сообщения электронной почты как делегат  <br/> |[EmailMessage.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.bind%28v=exchg.80%29.aspx) , а затем [EmailMessage.Delete](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.delete%28v=exchg.80%29.aspx) <br/> |[GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) , а затем [DeleteItem](http://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx) <br/> |
   
При работе с по электронной почте в качестве делегата, следует в виду следующее.
  
- Если делегат должен работать с приглашений на собрания и ответы, делегат необходим доступ к папке "Входящие". Для получения дополнительных сведений см [обязательные задачи для доступа к календарям в качестве делегата](how-to-access-a-calendar-as-a-delegate-by-using-ews-in-exchange.md#bk_prereq).
    
- Когда получатель получает сообщение, которое было отправлено от имени владельца почтового ящика, отправителя отображается как « *делегат* от имени *владельца почтового ящика* ». 
    
> [!NOTE]
> В примерах кода в этой статье primary@contoso.com — это владелец почтового ящика. 
  
## <a name="prerequisite-tasks"></a>Обязательные задачи
<a name="bk_prereq"> </a>

Пользователь может получить доступ к папки "Входящие" владельца почтового ящика роли представителя, пользователь должен быть [добавлен в качестве делегата с разрешениями](how-to-add-and-remove-delegates-by-using-ews-in-exchange.md) для папки "Входящие" владельца почтового ящика. 
  
## <a name="create-and-send-an-email-as-a-delegate-by-using-the-ews-managed-api"></a>Создание и отправка сообщения электронной почты как делегат с помощью управляемого интерфейса API веб-служб Exchange
<a name="bk_createewsma"> </a>

Управляемый API EWS позволяет использовать объект службы для пользователя делегат для создания и отправки электронной почты от имени владельца почтового ящика. В этом примере показано, как использовать метод [Save](http://msdn.microsoft.com/en-us/library/dd635209%28v=exchg.80%29.aspx) , чтобы сохранить сообщение в папке «Черновики» владельца почтового ящика, а затем метод [SendAndSaveCopy](http://msdn.microsoft.com/en-us/library/dd634248%28v=exchg.80%29.aspx) для отправки почты и сохранить сообщение в папке "Отправленные" владельца почтового ящика. 
  
В этом примере предполагается, что эта **Служба** является допустимым объектом [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) делегата и делегата имеет [соответствующие разрешения для папки «Входящие», «Черновики» и отправленные владельца почтового ящика](how-to-set-folder-permissions-for-another-user-by-using-ews-in-exchange.md).
  
```cs
public static void DelegateAccessCreateEmail(ExchangeService service)
{
    // Create an email message and provide it with connection 
    // configuration information by using an ExchangeService 
    // object named service.
    EmailMessage message = new EmailMessage(service);
    // Set properties on the email message.
    message.Subject = "Company Soccer Team";
    message.Body = "Are you interested in joining?";
    message.ToRecipients.Add("sadie@contoso.com");
    // Save the email to the mailbox owner's Drafts folder.
    // This method call results in a CreateItem call to EWS.
    // The FolderId parameter contains the context for the 
    // mailbox owner's Inbox folder. Any additional actions 
    // taken on this message will be performed in the mailbox 
    // owner's mailbox. 
    message.Save(new FolderId(WellKnownFolderName.Drafts, new Mailbox("primary@contoso.com")));
    // Send the email and save the message in the mailbox owner's 
    // Sent Items folder.
    // This method call results in a SendItem call to EWS.
    message.SendAndSaveCopy(new FolderId(WellKnownFolderName.SentItems, new Mailbox("primary@contoso.com")));
    Console.WriteLine("An email with the subject '" + message.Subject + "' has been sent to '" 
    + message.ToRecipients[0] + "' and saved in the Sent Items folder of the mailbox owner.");
}
```

## <a name="create-and-send-an-email-as-a-delegate-by-using-ews"></a>Создание и отправка сообщения электронной почты как делегат с помощью веб-служб Exchange
<a name="bk_createews"> </a>

Веб-служб Exchange позволяет использовать объект службы для пользователя делегат для создания и отправки электронной почты от имени владельца почтового ящика. В этом примере показано, как использовать операцию [CreateItem](http://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) для создания сообщения электронной почты и операции [SendItem](http://msdn.microsoft.com/library/337b89ef-e1b7-45ed-92f3-8abe4200e4c7%28Office.15%29.aspx) отправлять время и сохраните его в папке "Отправленные" владельца почтового ящика. 
  
Это первый запрос XML, который отправляет управляемый API EWS при использовании метода **Save** для [создания и отправки сообщения электронной почты](#bk_createewsma).
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version=" Exchange2007_SP1" />
  </soap:Header>
  <soap:Body>
    <m:CreateItem MessageDisposition="SaveOnly">
      <m:SavedItemFolderId>
        <t:DistinguishedFolderId Id="drafts">
          <t:Mailbox>
            <t:EmailAddress>primary@contoso.com</t:EmailAddress>
          </t:Mailbox>
        </t:DistinguishedFolderId>
      </m:SavedItemFolderId>
      <m:Items>
        <t:Message>
          <t:Subject>Company Soccer Team</t:Subject>
          <t:Body BodyType="HTML">Are you interested in joining?</t:Body>
          <t:ToRecipients>
            <t:Mailbox>
              <t:EmailAddress>sadie@contoso.com</t:EmailAddress>
            </t:Mailbox>
          </t:ToRecipients>
        </t:Message>
      </m:Items>
    </m:CreateItem>
  </soap:Body>
</soap:Envelope>
```

Сервер отвечает на запрос **CreateItem** [CreateItemResponse](http://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) сообщение, которое содержит значение элемента [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) **NoError**, это означает, что сообщение электронной почты был создан и успешно сохранен. Ответ также содержит идентификатор только что созданный сообщений электронной почты.
  
Значение **ItemId** был усечен для удобства чтения. 
  
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
    <m:CreateItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
                          xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:CreateItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items>
            <t:Message>
              <t:ItemId Id="iNRaAAA="
                        ChangeKey="CQAAABYAAADOilbYa8KaT7ZgMoTz2P+hAAABiQPU" />
            </t:Message>
          </m:Items>
        </m:CreateItemResponseMessage>
      </m:ResponseMessages>
    </m:CreateItemResponse>
  </s:Body>
</s:Envelope>
```

Затем используйте операции **SendItem** отправлять сообщения от имени владельца почтового ящика и сохраните его в папке "Отправленные" владельца почтового ящика. 
  
Значение **ItemId** был усечен для удобства чтения. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version=" Exchange2007_SP1" />
  </soap:Header>
  <soap:Body>
    <m:SendItem SaveItemToFolder="true">
      <m:ItemIds>
        <t:ItemId Id="iNRaAAA="
                  ChangeKey="CQAAABYAAADOilbYa8KaT7ZgMoTz2P+hAAABiQPU" />
      </m:ItemIds>
      <m:SavedItemFolderId>
        <t:DistinguishedFolderId Id="sentitems">
          <t:Mailbox>
            <t:EmailAddress>primary@contoso.com</t:EmailAddress>
          </t:Mailbox>
        </t:DistinguishedFolderId>
      </m:SavedItemFolderId>
    </m:SendItem>
  </soap:Body>
</soap:Envelope>
```

Сервер отвечает на запрос **SendItem** [SendItemResponse](http://msdn.microsoft.com/library/26ac41c7-57d9-473e-ab7a-bae93e1d2aba%28Office.15%29.aspx) сообщение, которое содержит значение элемента [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) **NoError**, который указывает, что сообщение электронной почты было отправлено и сохраняются в папке "Отправленные" владельца почтового ящика успешно.
  
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
    <m:SendItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
                        xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:SendItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
        </m:SendItemResponseMessage>
      </m:ResponseMessages>
    </m:SendItemResponse>
  </s:Body>
</s:Envelope>
```

## <a name="search-for-an-email-as-a-delegate-by-using-the-ews-managed-api"></a>Поиск сообщения электронной почты в качестве делегата с помощью управляемого интерфейса API веб-служб Exchange
<a name="bk_searchewsma"> </a>

Для поиска сообщения электронной почты, необходимо использовать один из методов [ExchangeService.FindItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) , включает параметр [FolderId](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx) , таким образом, можно указать папку "Входящие" владельца почтового ящика. 
  
```cs
static void DelegateAccessSearchEmailWithFilter(ExchangeService service)
{
    // Limit the result set to 10 items.
    ItemView view = new ItemView(10);
    // Define the search filter.
    SearchFilter.ContainsSubstring filter = new SearchFilter.ContainsSubstring(ItemSchema.Subject, 
        "soccer", ContainmentMode.Substring, ComparisonMode.IgnoreCase);
    view.PropertySet = new PropertySet(ItemSchema.Subject,
                                       ItemSchema.DateTimeReceived,
                                       EmailMessageSchema.IsRead);
    // Item searches do not support deep traversal.
    view.Traversal = ItemTraversal.Shallow;
    // Sorting.
    view.OrderBy.Add(ItemSchema.DateTimeReceived, SortDirection.Descending);
    try
    {
        // Call FindItems to find matching Inbox items. 
        // The parameters of FindItems must denote the mailbox owner,
        // mailbox, and Inbox folder.
        // This call results in a FindItem call to EWS.
        FindItemsResults<Item> results = service.FindItems(new 
            FolderId(WellKnownFolderName.Inbox, "primary@contoso.com"), 
            filter, view);
        foreach (Item item in results.Items)
        {
            Console.WriteLine("Subject: {0}", item.Subject);
            Console.WriteLine("Id: {0}", item.Id.ToString());
            if (item is EmailMessage)
            {
                EmailMessage message = item as EmailMessage;
                Console.WriteLine("Read: {0}", message.IsRead.ToString());
            }
        }
    }
    catch (Exception ex)
    {
        Console.WriteLine("Exception while enumerating results: {0}", ex.Message);
    }
}
```

После вызова **FindItems** возвращает ответ с Идентификатором, можно получить, update или delete, электронной почты с помощью идентификатора и [неявный доступ](delegate-access-and-ews-in-exchange.md#bk_implicit) - вам не нужно указать SMTP-адреса владельца почтового ящика. 
  
## <a name="search-for-an-email-as-a-delegate-by-using-ews"></a>Поиск сообщения электронной почты в качестве делегата с помощью веб-служб Exchange
<a name="bk_searchews"> </a>

Веб-служб Exchange позволяет использовать объект службы для пользователя делегат для поиска по электронной почте, которые соответствуют набору условий поиска. В этом примере показано, как использовать операцию [FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) для поиска сообщений в папке "Входящие" владельца почтового, содержащие слово «футбольных» в теме сообщения. 
  
Это также запроса XML, что управляемый API EWS отправляет при [поиска для сообщения электронной почты](#bk_searchewsma).
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version=" Exchange2007_SP1" />
  </soap:Header>
  <soap:Body>
    <m:FindItem Traversal="Shallow">
      <m:ItemShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="item:Subject" />
          <t:FieldURI FieldURI="item:DateTimeReceived" />
          <t:FieldURI FieldURI="message:IsRead" />
        </t:AdditionalProperties>
      </m:ItemShape>
      <m:IndexedPageItemView MaxEntriesReturned="10"
                             Offset="0"
                             BasePoint="Beginning" />
      <m:Restriction>
        <t:Contains ContainmentMode="Substring"
                    ContainmentComparison="IgnoreCase">
          <t:FieldURI FieldURI="item:Subject" />
          <t:Constant Value="soccer" />
        </t:Contains>
      </m:Restriction>
      <m:SortOrder>
        <t:FieldOrder Order="Descending">
          <t:FieldURI FieldURI="item:DateTimeReceived" />
        </t:FieldOrder>
      </m:SortOrder>
      <m:ParentFolderIds>
        <t:DistinguishedFolderId Id="inbox">
          <t:Mailbox>
            <t:EmailAddress>primary@contoso.com</t:EmailAddress>
          </t:Mailbox>
        </t:DistinguishedFolderId>
      </m:ParentFolderIds>
    </m:FindItem>
  </soap:Body>
</soap:Envelope>
```

Сервер отвечает на запрос **FindItem** [FindItemResponse](http://msdn.microsoft.com/library/c8b316df-d4ab-49b8-96d4-8e9a016730ef%28Office.15%29.aspx) сообщение, которое содержит значение элемента [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) **NoError**, который указывает, что поиск успешно завершена. Ответ содержит элемент [сообщения](http://msdn.microsoft.com/library/2400b33c-43b2-4fc2-b6fb-275a99e0e810%28Office.15%29.aspx) для любого по электронной почте, выполнены условия поиска. В этом случае найти только один электронной почты. 
  
Значение элемента [ItemId](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) был усечен для удобства чтения. 
  
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
    <m:FindItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
                        xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:FindItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:RootFolder IndexedPagingOffset="1"
                        TotalItemsInView="1"
                        IncludesLastItemInRange="true">
            <t:Items>
              <t:Message>
                <t:ItemId Id="iNwoAAA="
                          ChangeKey="CQAAABYAAADOilbYa8KaT7ZgMoTz2P+hAAABiQuu" />
                <t:Subject>Soccer team</t:Subject>
                <t:DateTimeReceived>2014-03-10T06:16:55Z</t:DateTimeReceived>
                <t:IsRead>false</t:IsRead>
              </t:Message>
            </t:Items>
          </m:RootFolder>
        </m:FindItemResponseMessage>
      </m:ResponseMessages>
    </m:FindItemResponse>
  </s:Body>
</s:Envelope>
```

Теперь, когда у вас есть **идентификатор элемента** для электронной почты, который соответствует условиям, можно получить, update или delete, электронной почты с помощью **ItemId** и [неявный доступ](delegate-access-and-ews-in-exchange.md#bk_implicit) - вам не нужно указать SMTP-адреса владельца почтового ящика. 
  
## <a name="get-update-or-delete-email-items-as-a-delegate-by-using-the-ews-managed-api"></a>Получение, обновление и удаление элементов электронной почты роли представителя с помощью управляемого интерфейса API веб-служб Exchange
<a name="bk_geteswma"> </a>

Можно использовать управляемый API EWS для получения, обновлять или удалять сообщения электронной почты так же, как выполнять эти действия, если вы не используете делегированный доступ. Единственное отличие — объект **ExchangeService** для делегата. Идентификатор элемента, включенные в вызове метода **Привязка** уникальным образом определяет элемент в хранилище почтовых ящиков, в папке "Входящие" владельца почтового ящика. 
  
**В таблице 2. Управляемый API EWS методы работы с электронной почты в качестве делегата**

|**Задача**|**Метод управляемого API EWS**|**Пример кода**|
|:-----|:-----|:-----|
|Получите сообщение электронной почты  <br/> |[Привязка](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.bind%28v=exchg.80%29.aspx) <br/> |[Получение элемента с помощью управляемого интерфейса API веб-служб Exchange](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_getewsma) <br/> |
|Обновление сообщения электронной почты  <br/> |[Привязка](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.bind%28v=exchg.80%29.aspx) следуют [обновления](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.update%28v=exchg.80%29.aspx) <br/> |[Обновление элемента с помощью управляемого интерфейса API веб-служб Exchange](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_updateewsma) <br/> |
|Удаление сообщения электронной почты  <br/> |[Привязка](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.bind%28v=exchg.80%29.aspx) , а затем [Удалить](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.delete%28v=exchg.80%29.aspx) <br/> |[Удаление элемента с помощью управляемого интерфейса API веб-служб Exchange](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_deleteewsma) <br/> |
   
## <a name="get-update-or-delete-email-items-as-a-delegate-by-using-ews"></a>Получение, обновление и удаление элементов электронной почты роли представителя с помощью веб-служб Exchange
<a name="bk_getews"> </a>

Можно использовать управляемый API EWS для получения, обновлять или удалять сообщения электронной почты так же, как выполнять эти действия, если вы не используете делегированный доступ. Единственное отличие — объект службы для делегата. Идентификатор элемента, включенных в запрос **GetItem** уникальным образом определяет элемент в хранилище почтовых ящиков, в папке "Входящие" владельца почтового ящика. 
  
**В таблице 3. Операции EWS для работы с электронной почты в качестве делегата**

|**Задача**|**Операция служб EWS**|**Пример кода**|
|:-----|:-----|:-----|
|Получите сообщение электронной почты  <br/> |[GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) <br/> |[Получение элемента с помощью веб-служб Exchange](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_getews) <br/> |
|Обновление сообщения электронной почты  <br/> |[GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) , а затем [UpdateItem](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) <br/> |[Обновление элемента с помощью веб-служб Exchange](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_updateews) <br/> |
|Удаление сообщения электронной почты  <br/> |[GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) , а затем [DeleteItem](http://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx) <br/> |[Удаление элемента с помощью веб-служб Exchange](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_deleteews) <br/> |
   
## <a name="see-also"></a>См. также

- [Передача прав доступа и EWS в Exchange](delegate-access-and-ews-in-exchange.md)    
- [Добавление и удаление делегаты с помощью веб-служб Exchange в Exchange](how-to-add-and-remove-delegates-by-using-ews-in-exchange.md)    
- [Настройка разрешений папки другого пользователя с помощью веб-служб Exchange в Exchange](how-to-set-folder-permissions-for-another-user-by-using-ews-in-exchange.md)    
- [Календари и веб-службах Exchange](calendars-and-ews-in-exchange.md)
    

