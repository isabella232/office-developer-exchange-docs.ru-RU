---
title: Доступ к электронной почте в качестве делегата с помощью EWS в Exchange
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.localizationpriority: medium
ms.assetid: a8123604-c7c0-405d-a0ed-7a9b4a431bfd
description: Узнайте, как получить доступ к электронной почте в качестве делегата с помощью управляемого API или EWS EWS в Exchange.
ms.openlocfilehash: aa921bc36004b3a26caa514390e52249021b304f
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59521216"
---
# <a name="access-email-as-a-delegate-by-using-ews-in-exchange"></a>Доступ к электронной почте в качестве делегата с помощью EWS в Exchange

Узнайте, как получить доступ к электронной почте в качестве делегата с помощью управляемого API или EWS EWS в Exchange.
  
Вы можете использовать управляемый API или EWS EWS, чтобы предоставить делегату пользователя доступ к папке "Входящие" владельца почтового ящика. Затем делегат может создавать запросы на собрания от имени владельца почтовых ящиков, искать электронную почту и получать, обновлять и удалять электронную почту из папки "Входящие" владельца почтового ящика в зависимости от их разрешений.
  
В качестве делегата вы используете те же методы и операции для доступа к папке "Входящие" владельца почтовых ящиков, которые используются для доступа к папке "Входящие" без доступа делегата. Главное отличие состоит в том, что для поиска или создания элемента электронной почты необходимо использовать [](delegate-access-and-ews-in-exchange.md#bk_implicit) явный доступ, а после идентификации элемента можно использовать неявный доступ для получения, обновления или удаления элемента. [](delegate-access-and-ews-in-exchange.md#bk_explicit) 
  
**Таблица 1. Методы управляемого API EWS и операции EWS для доступа к электронной почте в качестве делегата**

|**Задача**|**Используйте этот метод управляемого API EWS...**|**Используйте эту операцию EWS...**|
|:-----|:-----|:-----|
|Создание и отправка электронной почты в качестве делегата  <br/> |[EmailMessage.Save,](https://msdn.microsoft.com/library/dd635209%28v=exchg.80%29.aspx) где параметр [FolderId](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx) предоставляет явный доступ к папке Черновики владельца почтовых ящиков [](delegate-access-and-ews-in-exchange.md#bk_explicitewsma)  <br/> [EmailMessage.SendAndSaveCopy,](https://msdn.microsoft.com/library/dd634248%28v=exchg.80%29.aspx) где параметр [](delegate-access-and-ews-in-exchange.md#bk_explicitewsma) [FolderId](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx) предоставляет явный доступ к папке отправленных элементов владельца почтового ящика  <br/> |[CreateItem,](https://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) где элемент [почтовых ящиков](https://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) указывает [emailAddress](https://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) владельца почтового ящика  <br/> [SendItem,](https://msdn.microsoft.com/library/a966da19-b05a-4504-ac98-91acc1667b9a%28Office.15%29.aspx) где элемент [почтового ящика](https://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) указывает [emailAddress](https://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) владельца почтового ящика  <br/> |
|Создание нескольких сообщений электронной почты в качестве делегата  <br/> |[ExchangeService.CreateItems,](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.createitems%28v=exchg.80%29.aspx) где параметр **FolderId** предоставляет явный доступ к папке "Входящие" владельца почтового ящика [](delegate-access-and-ews-in-exchange.md#bk_explicitewsma)  <br/> |[CreateItem,](https://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) где элемент [почтовых ящиков](https://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) указывает [emailAddress](https://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) владельца почтового ящика  <br/> |
|Поиск или поиск электронной почты в качестве делегата  <br/> |[ExchangeService.FindItems,](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) где параметр **FolderId** предоставляет явный доступ к папке "Входящие" владельца почтового ящика [](delegate-access-and-ews-in-exchange.md#bk_explicitewsma)  <br/> |[FindItem,](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) где элемент [почтовых ящиков](https://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) указывает [emailAddress](https://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) владельца почтового ящика  <br/> |
|Получить сообщение электронной почты в качестве делегата  <br/> |[EmailMessage.Bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage.bind%28v=exchg.80%29.aspx) <br/> |[GetItem](https://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) <br/> |
|Обновление электронной почты в качестве делегата  <br/> |[EmailMessage.Bind,](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage.bind%28v=exchg.80%29.aspx) а затем [EmailMessage.Update](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage.update%28v=exchg.80%29.aspx) <br/> |[GetItem](https://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) с последующим [обновлениемItem](https://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) <br/> |
|Удаление электронной почты в качестве делегата  <br/> |[EmailMessage.Bind,](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage.bind%28v=exchg.80%29.aspx) а затем [EmailMessage.Delete](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage.delete%28v=exchg.80%29.aspx) <br/> |[GetItem](https://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) следуют [DeleteItem](../web-service-reference/deleteitem-operation.md) <br/> |
   
При работе с электронными письмами в качестве делегата следует помнить о следующих вещах:
  
- Если делегату требуется работать только с запросами и ответами на собрания, делегату не требуется доступ к папке "Входящие". Дополнительные сведения см. в [предварительных задачах для доступа к календарям в качестве делегата.](how-to-access-a-calendar-as-a-delegate-by-using-ews-in-exchange.md#bk_prereq)
    
- Когда получатель получает сообщение, отправленное от имени владельца почтового ящика,  отправитель отображается как "Делегирование от имени владельца *почтового ящика".* 
    
> [!NOTE]
> В примерах кода в этой статье primary@contoso.com является владельцем почтового ящика. 
  
## <a name="prerequisite-tasks"></a>Обязательные задачи
<a name="bk_prereq"> </a>

Прежде чем пользователь сможет получить доступ к папке "Входящие" владельца [](how-to-add-and-remove-delegates-by-using-ews-in-exchange.md) почтового ящика в качестве делегата, его необходимо добавить в качестве делегата с разрешениями в папку "Входящие" владельца почтового ящика. 
  
## <a name="create-and-send-an-email-as-a-delegate-by-using-the-ews-managed-api"></a>Создание и отправка электронной почты в качестве делегата с помощью управляемого API EWS
<a name="bk_createewsma"> </a>

Управляемый API EWS позволяет использовать объект службы для пользователя-делегата для создания и отправки электронной почты от имени владельца почтового ящика. В этом примере [](https://msdn.microsoft.com/library/dd635209%28v=exchg.80%29.aspx) показано, как использовать метод Сохранить для сохранения сообщения в папке Черновики владельца почтовых ящиков, а затем метод [SendAndSaveCopy](https://msdn.microsoft.com/library/dd634248%28v=exchg.80%29.aspx) для отправки почты и сохранения сообщения в папке отправленных элементов владельца почтового ящика. 
  
В этом примере предполагается, что служба является допустимым объектом [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) для делегата и что делегату были предоставлены соответствующие разрешения для папки "Входящие", "Черновики" и "Отправленные элементы" владельца почтового ящика.  [](how-to-set-folder-permissions-for-another-user-by-using-ews-in-exchange.md)
  
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

## <a name="create-and-send-an-email-as-a-delegate-by-using-ews"></a>Создание и отправка электронной почты в качестве делегата с помощью EWS
<a name="bk_createews"> </a>

EWS позволяет использовать объект службы для пользователя-делегата для создания и отправки электронной почты от имени владельца почтового ящика. В этом примере показано, как использовать операцию [CreateItem](https://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) для создания электронной почты и операции [SendItem](https://msdn.microsoft.com/library/337b89ef-e1b7-45ed-92f3-8abe4200e4c7%28Office.15%29.aspx) для отправки времени и сохранения его в папке отправленных элементов владельца почтового ящика. 
  
Это также первый XML-запрос, который отправляет управляемый API EWS при использовании метода **Сохранить** для создания и [отправки электронной почты.](#bk_createewsma)
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
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

Сервер отвечает на запрос **CreateItem сообщением** [CreateItemResponse,](https://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) которое включает элемент [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) значения **NoError,** что указывает на успешное создание и успешное спасение электронной почты. В ответе также содержится ID элемента вновь созданной электронной почты.
  
Значение **ItemId** было сокращено для читаемости. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="893"
                         MinorBuildNumber="17"
                         Version="V2_10"
                         xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body>
    <m:CreateItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
                          xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
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

Далее используйте операцию **SendItem** для отправки сообщения от имени владельца почтового ящика и сохранения его в папке отправленных элементов владельца почтового ящика. 
  
Значение **ItemId** было сокращено для читаемости. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
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

Сервер отвечает на запрос **SendItem** [сообщением SendItemResponse,](https://msdn.microsoft.com/library/26ac41c7-57d9-473e-ab7a-bae93e1d2aba%28Office.15%29.aspx) которое включает в себя значение элемента [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) **NoError,** которое указывает на успешность отправки и сберегивания электронной почты в папку отправленных элементов владельца почтового ящика.
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="893"
                         MinorBuildNumber="17"
                         Version="V2_10"
                         xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body>
    <m:SendItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
                        xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:SendItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
        </m:SendItemResponseMessage>
      </m:ResponseMessages>
    </m:SendItemResponse>
  </s:Body>
</s:Envelope>
```

## <a name="search-for-an-email-as-a-delegate-by-using-the-ews-managed-api"></a>Поиск электронной почты в качестве делегата с помощью управляемого API EWS
<a name="bk_searchewsma"> </a>

Для поиска электронной почты необходимо использовать один из методов [ExchangeService.FindItems,](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) который включает параметр [FolderId,](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx) чтобы можно было указать папку "Входящие" владельца почтового ящика. 
  
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

После того как вызов **FindItems** возвращает ответ с помощью ID, вы можете получить, обновить или удалить эту электронную почту с помощью ID и неявного [доступа,](delegate-access-and-ews-in-exchange.md#bk_implicit) и вам не нужно указывать SMTP-адрес владельца почтового ящика. 
  
## <a name="search-for-an-email-as-a-delegate-by-using-ews"></a>Поиск электронной почты в качестве делегата с помощью EWS
<a name="bk_searchews"> </a>

EWS позволяет использовать объект службы для пользователя делегирования для поиска сообщений электронной почты, которые соответствуют набору критериев поиска. В этом примере показано, как использовать операцию [FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) для поиска сообщений в папке "Входящие" владельца, содержащие слово "футбол" в субъекте. 
  
Это также XML-запрос, который отправляет управляемый API EWS при поиске [электронной почты.](#bk_searchewsma)
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
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

Сервер отвечает на запрос **FindItem** [сообщением FindItemResponse,](https://msdn.microsoft.com/library/c8b316df-d4ab-49b8-96d4-8e9a016730ef%28Office.15%29.aspx) которое включает элемент [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) значения **NoError,** что указывает на успешное завершенное поиск. Ответ содержит элемент [Message](https://msdn.microsoft.com/library/2400b33c-43b2-4fc2-b6fb-275a99e0e810%28Office.15%29.aspx) для любых электронных писем, которые соответствуют критериям поиска. В этом случае найдено только одно сообщение электронной почты. 
  
Значение элемента [ItemId](https://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) было сокращено для читаемости. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="893"
                         MinorBuildNumber="17"
                         Version="V2_10"
                         xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body>
    <m:FindItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
                        xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
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

Теперь, когда у вас есть **ItemId** для электронной почты, которая соответствует вашим критериям, вы можете получить, обновить или удалить это письмо с помощью **ItemId** и неявного доступа [,](delegate-access-and-ews-in-exchange.md#bk_implicit) и вам не нужно указывать SMTP-адрес владельца почтового ящика. 
  
## <a name="get-update-or-delete-email-items-as-a-delegate-by-using-the-ews-managed-api"></a>Получить, обновить или удалить элементы электронной почты в качестве делегата с помощью управляемого API EWS
<a name="bk_geteswma"> </a>

Управляемый API EWS можно использовать для получения, обновления или удаления электронной почты таким же образом, как вы выполняете эти действия, если вы не используете доступ делегатов. Единственное отличие состоит в том, что объект **ExchangeService** является для пользователя делегирования. Идентификатор элемента, включенный в вызов метода **Bind,** однозначно идентифицирует элемент в магазине почтовых ящиков в папке "Входящие" владельца почтового ящика. 
  
**Таблица 2. Методы управляемого API EWS, работающие с электронной почтой в качестве делегата**

|**Задача**|**Метод управляемого API EWS**|**Пример кода**|
|:-----|:-----|:-----|
|Получить сообщение электронной почты  <br/> |[Bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage.bind%28v=exchg.80%29.aspx) <br/> |[Получение элемента с помощью управляемого API EWS](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_getewsma) <br/> |
|Обновление электронной почты  <br/> |[Привязка](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage.bind%28v=exchg.80%29.aspx) с последующим [обновлением](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage.update%28v=exchg.80%29.aspx) <br/> |[Изменение элемента с помощью управляемого API EWS](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_updateewsma) <br/> |
|Удаление электронной почты  <br/> |[Привязка](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage.bind%28v=exchg.80%29.aspx) с последующим [удалением](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage.delete%28v=exchg.80%29.aspx) <br/> |[Удаление элемента с помощью управляемого API EWS](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_deleteewsma) <br/> |
   
## <a name="get-update-or-delete-email-items-as-a-delegate-by-using-ews"></a>Получить, обновить или удалить элементы электронной почты в качестве делегата с помощью EWS
<a name="bk_getews"> </a>

Управляемый API EWS можно использовать для получения, обновления или удаления электронной почты таким же образом, как вы выполняете эти действия, если вы не используете доступ делегатов. Единственное отличие состоит в том, что объект службы для пользователя делегирования. Идентификатор элемента, включенный в запрос **GetItem,** однозначно идентифицирует элемент в магазине почтовых ящиков в папке "Входящие" владельца почтового ящика. 
  
**Таблица 3. Операции EWS для работы с электронной почтой в качестве делегата**

|**Задача**|**Операция служб EWS**|**Пример кода**|
|:-----|:-----|:-----|
|Получить сообщение электронной почты  <br/> |[GetItem](https://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) <br/> |[Получение элемента с помощью веб-служб Exchange](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_getews) <br/> |
|Обновление электронной почты  <br/> |[GetItem](https://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) с последующим [обновлениемItem](https://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) <br/> |[Изменение элемента с помощью веб-служб Exchange](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_updateews) <br/> |
|Удаление электронной почты  <br/> |[GetItem](https://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) следуют [DeleteItem](../web-service-reference/deleteitem-operation.md) <br/> |[Удаление элемента с помощью веб-служб Exchange](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_deleteews) <br/> |
   
## <a name="see-also"></a>См. также

- [Передача прав доступа и EWS в Exchange](delegate-access-and-ews-in-exchange.md)    
- [Добавление и удаление делегатов с помощью EWS в Exchange](how-to-add-and-remove-delegates-by-using-ews-in-exchange.md)    
- [Установите разрешения папок для другого пользователя с помощью EWS в Exchange](how-to-set-folder-permissions-for-another-user-by-using-ews-in-exchange.md)    
- [Календари и веб-службах Exchange](calendars-and-ews-in-exchange.md)
    

