---
title: Операция GetConversationItems
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 8ae00a99-b37b-4194-829c-fe300db6ab99
description: Сведения об операции GetConversationItems.
ms.openlocfilehash: 0de9a380aa2f9b25e9a7ef90ebe7a9f485ca60d0
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59513670"
---
# <a name="getconversationitems-operation"></a>Операция GetConversationItems

Сведения об операции **GetConversationItems.** 
  
Операция **GetConversationItems** получает один или несколько наборов элементов, организованных в узлах в беседе. 
  
Эта операция появилась в Exchange Server 2013.
  
## <a name="using-the-getconversationitems-operation"></a>Использование операции GetConversationItems

Вы можете использовать **операцию GetConversationItems** для получения элементов в беседах для основных и архивных почтовых ящиков. 
  
### <a name="getconversationitems-operation-soap-headers"></a>Заглавные заготки операции GetConversationItems

В **операции GetConversationItems** можно использовать заглавные таблицы SOAP, указанные в следующей таблице. 
  
|**Имя заголовка**|**Элемент**|**Описание**|
|:-----|:-----|:-----|
|**Олицетворение** <br/> |[ExchangeImpersonation](exchangeimpersonation.md) <br/> |Определяет пользователя, которого клиентская заявка выдвигает. Этот заглавный заглавник применим к запросу.  <br/> |
|**RequestVersion** <br/> |[RequestServerVersion](requestserverversion.md) <br/> |Определяет версию схемы для запроса на операцию. Минимальное значение для этого элемента **Exchange2013**. Этот заглавный заглавник применим к запросу.  <br/> |
|**ServerVersion** <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |Определяет версию сервера, отвечаемого на запрос. Этот заглавный заглавник применим к ответу.  <br/> |
   
## <a name="getconversationitems-operation-request-example-get-items-in-a-single-conversation"></a>Пример запроса на операцию GetConversationItems: получить элементы в одном разговоре

В следующем примере запроса на операцию **GetConversationItems** показано, как получить все элементы беседы в одном разговоре, за исключением элементов, расположенных в папках Удаленные элементы и черновики. Каждый элемент, возвращенный в ответе, будет содержать идентификатор элемента, субъект и время, когда элемент был получен в почтовом ящике. 
  
> [!NOTE]
> Для сохранения читаемости сокращены все идентификаторы элементов и ключи изменений в этой статье. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013" />
   </soap:Header>
   <soap:Body>
      <m:GetConversationItems>
         <m:ItemShape>
            <t:BaseShape>IdOnly</t:BaseShape>
            <t:AdditionalProperties>
               <t:FieldURI FieldURI="item:Subject" />
               <t:FieldURI FieldURI="item:DateTimeReceived" />
            </t:AdditionalProperties>
         </m:ItemShape>
         <m:FoldersToIgnore>
            <t:DistinguishedFolderId Id="deleteditems" />
            <t:DistinguishedFolderId Id="drafts" />
         </m:FoldersToIgnore>
         <m:SortOrder>TreeOrderDescending</m:SortOrder>
         <m:Conversations>
            <t:Conversation>
               <t:ConversationId Id="AAQkADEzOTExYjJkakJCs=" />
            </t:Conversation>
         </m:Conversations>
      </m:GetConversationItems>
   </soap:Body>
</soap:Envelope>
```

В этом примере **запроса GetConversationItems** не содержатся следующие параметры: 
  
- Элемент [MaxItemsToReturn,](maxitemstoreturn.md) который задает максимальное количество элементов, возвращаемого в ответ. 
    
- Элемент [MailboxScope,](mailboxscope.md) который задает область почтового ящика, указывает, должна ли выполняться операция **GetConversationItems** на основном почтовом ящике, архивном почтовом ящике или обоих почтовых ящиках. 
    
- Элемент [SyncState (base64Binary),](syncstate-base64binary.md) который задает состояние синхронизации для получения только новых или обновленных элементов беседы. Этот элемент заданной для каждого разговора. 
    
Тело SOAP запроса содержит следующие элементы:
  
- [GetConversationItems](getconversationitems.md)
    
- [ItemShape](itemshape.md)
    
- [BaseShape](baseshape.md)
    
- [AdditionalProperties](additionalproperties.md)
    
- [FieldURI](fielduri.md)
    
- [FoldersToIgnore](folderstoignore.md)
    
- [DistinguishedFolderId](distinguishedfolderid.md)
    
- [SortOrder (ConversationNodeSortOrder)](sortorder-conversationnodesortorder.md)
    
- [Беседы](conversations-ex15websvcsotherref.md)
    
- [Conversation (ConversationRequestType)](conversation-conversationrequesttype.md)
    
- [ConversationId](conversationid.md)
    
## <a name="successful-getconversationitems-operation-response"></a>Успешный ответ на операцию GetConversationItems

В следующем примере показан успешный ответ на запрос **операции GetConversationItems** для получения элементов в одном разговоре. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15"
                           MinorVersion="0"
                           MajorBuildNumber="545"
                           MinorBuildNumber="11"
                           Version="Exchange2013"
                           xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types"
                           xmlns="https://schemas.microsoft.com/exchange/services/2006/types"
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <m:GetConversationItemsResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
                                      xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
         <m:ResponseMessages>
            <m:GetConversationItemsResponseMessage ResponseClass="Success">
               <m:ResponseCode>NoError</m:ResponseCode>
               <m:Conversation>
                  <t:ConversationId Id="AAQkADEzOTExYjJkakJCs=" />
                  <t:SyncState>AQIAAABNVkUwAgIAAABhHqHUAwIAAABNVkUxBAIAAABhHqHfBAIAAABhHqHV</t:SyncState>
                  <t:ConversationNodes>
                     <t:ConversationNode>
                        <t:InternetMessageId>6a4838fa804045e09d40c1a39b9ea916@contoso.com</t:InternetMessageId>
                        <t:ParentInternetMessageId>15a56698d503438fbdaa18186d5b81b7@contoso.com</t:ParentInternetMessageId>
                        <t:Items>
                           <t:Message>
                              <t:ItemId Id="AAMkADEzOTQrAABhHqHfAAA=" ChangeKey="CQAAABYAAACYAABhPpaq" />
                              <t:Subject>RE: Daily issue scrub</t:Subject>
                              <t:DateTimeReceived>2012-10-30T18:42:27Z</t:DateTimeReceived>
                           </t:Message>
                        </t:Items>
                     </t:ConversationNode>
                     <t:ConversationNode>
                        <t:InternetMessageId>2695d2b837954d68846b0c30491f5af1@contoso.com</t:InternetMessageId>
                        <t:ParentInternetMessageId>15a56698d503438fbdaa18186d5b81b7@contoso.com</t:ParentInternetMessageId>
                        <t:Items>
                           <t:Message>
                              <t:ItemId Id="AAMkADEzOTExYjJkLTYxZDAt" ChangeKey="CQAAABQrAABhPpaP" />
                              <t:Subject>RE: Daily issue scrub</t:Subject>
                              <t:DateTimeReceived>2012-10-30T17:38:26Z</t:DateTimeReceived>
                           </t:Message>
                        </t:Items>
                     </t:ConversationNode>
                     <t:ConversationNode>
                        <t:InternetMessageId>15a56698d503438fbdaa18186d5b81b7@contoso.com</t:InternetMessageId>
                        <t:ParentInternetMessageId>d3113e59c89c4288ae13100d033f8dbc@contoso.com</t:ParentInternetMessageId>
                        <t:Items>
                           <t:Message>
                              <t:ItemId Id="AAMkADEzOTFNVkUxAAA=" ChangeKey="CQAAABY4QrAABhPvYK" />
                              <t:Subject>RE: Daily issue scrub</t:Subject>
                              <t:DateTimeReceived>2012-10-30T17:37:00Z</t:DateTimeReceived>
                           </t:Message>
                        </t:Items>
                     </t:ConversationNode>
                     <t:ConversationNode>
                        <t:InternetMessageId>d3113e59c89c4288ae13100d033f8dbc@contoso.com</t:InternetMessageId>
                        <t:ParentInternetMessageId>189b712056c2430dbce334b40496ad00@contoso.com</t:ParentInternetMessageId>
                        <t:Items>
                           <t:Message>
                              <t:ItemId Id="AAMkm4QrAABhHqHUAAA=" ChangeKey="CQAAABQrAABhPpaN" />
                              <t:Subject>RE: Daily issue scrub</t:Subject>
                              <t:DateTimeReceived>2012-10-30T17:37:05Z</t:DateTimeReceived>
                           </t:Message>
                        </t:Items>
                     </t:ConversationNode>
                     <t:ConversationNode>
                        <t:InternetMessageId>189b712056c2430dbce334b40496ad00@contoso.com</t:InternetMessageId>
                        <t:Items>
                           <t:Message>
                              <t:ItemId Id="AAMkArAABNVkUwAAA=" ChangeKey="CQAAABm4QrAABhPvYJ" />
                              <t:Subject>Daily issue scrub</t:Subject>
                              <t:DateTimeReceived>2012-10-30T17:36:00Z</t:DateTimeReceived>
                           </t:Message>
                        </t:Items>
                     </t:ConversationNode>
                  </t:ConversationNodes>
               </m:Conversation>
            </m:GetConversationItemsResponseMessage>
         </m:ResponseMessages>
      </m:GetConversationItemsResponse>
   </s:Body>
</s:Envelope>
```

Рекомендуется сохранить SyncState для последующих запросов на операции **GetConversationItems.** 
  
Тело SOAP ответа содержит следующие элементы:
  
- [GetConversationItemsResponse](getconversationitemsresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [GetConversationItemsResponseMessage](getconversationitemsresponsemessage.md)
    
- [ResponseCode](responsecode.md)
    
- [Conversation (ConversationResponseType)](conversation-conversationresponsetype.md)
    
- [ConversationId](conversationid.md)
    
- [SyncState (base64Binary)](syncstate-base64binary.md)
    
- [ConversationNodes](conversationnodes.md)
    
- [ConversationNode](conversationnode.md)
    
- [InternetMessageId](internetmessageid.md)
    
- [Items (NonEmptyArrayOfAllItemsType)](items-nonemptyarrayofallitemstype.md)
    
- [Сообщение](message-ex15websvcsotherref.md)
    
- [ItemId](itemid.md)
    
- [Тема](subject.md)
    
- [DateTimeReceived](datetimereceived.md)
    
## <a name="getconversationitems-operation-error-response"></a>Ответ на ошибку операции GetConversationItems

В следующем примере показан ответ на запрос операции **GetConversationItems** для получения элементов в беседе, которые либо больше не существуют в почтовом ящике, либо для которых все элементы беседы находятся в папках, которые игнорируются. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="556" MinorBuildNumber="8" Version="Exchange2013" xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" xmlns="https://schemas.microsoft.com/exchange/services/2006/types" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:GetConversationItemsResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:GetConversationItemsResponseMessage ResponseClass="Error">
          <m:MessageText>The specified object was not found in the store.</m:MessageText>
          <m:ResponseCode>ErrorItemNotFound</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
        </m:GetConversationItemsResponseMessage>
      </m:ResponseMessages>
    </m:GetConversationItemsResponse>
  </s:Body>
</s:Envelope>
```

## <a name="see-also"></a>См. также

- [Операции EWS в Exchange](ews-operations-in-exchange.md)
    
- [Операция ApplyConversationAction](applyconversationaction-operation.md)
    
- [Операция FindConversation](findconversation-operation.md)
    

