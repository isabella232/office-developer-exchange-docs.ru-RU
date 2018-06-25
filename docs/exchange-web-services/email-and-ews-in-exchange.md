---
title: Электронная почта и веб-службах Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 4d7bdb37-f7f1-409f-9749-f8bcde7dc52a
description: Узнайте, как для работы с сообщениями электронной почты, включая сообщения электронной почты и выполнять другие задачи, связанные с электронной почты с помощью управляемого интерфейса API веб-служб Exchange или веб-служб Exchange в Exchange.
ms.openlocfilehash: d222be7409a3c3f4613a2be39b83b977fabb09e8
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760944"
---
# <a name="email-and-ews-in-exchange"></a>Электронная почта и веб-службах Exchange

Узнайте, как для работы с сообщениями электронной почты, включая сообщения электронной почты и выполнять другие задачи, связанные с электронной почты с помощью управляемого интерфейса API веб-служб Exchange или веб-служб Exchange в Exchange.
  

  
По сути Exchange — по электронной почте. Но что делает сообщения электронной почты сообщения электронной почты? Сообщений электронной почты являются одним из [строго типизированных элементов](folders-and-items-in-ews-in-exchange.md#bk_item) в Exchange, что означает, что они содержат определенный [набор свойств](email-properties-and-elements-in-ews-in-exchange.md), даже до отдельными. Сообщения электронной почты, представленные классом [EmailMessage](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx) в управляемый API веб-служб Exchange и элементом [сообщение](http://msdn.microsoft.com/library/2400b33c-43b2-4fc2-b6fb-275a99e0e810%28Office.15%29.aspx) и его дочерние элементы в веб-служб Exchange. 
  
Управляемый API веб-служб Exchange, в объекте **EmailMessage** является производным от объекта [элемента](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item%28v=exchg.80%29.aspx) . Класс **EmailMessage** расширяет класс **элемента** , предоставляя дополнительные свойства, такие как [EmailMessage.Sender](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.sender%28v=exchg.80%29.aspx) и [EmailMessage.IsRead](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.emailmessage.isread%28v=exchg.80%29.aspx), которые теперь являются общими для почти все сценарии обмена сообщениями. При получении, обновить или удалить сообщение электронной почты в большинстве случаев, которые можно выполнить с помощью объекта **EmailMessage** или базового объекта **элемента** , в зависимости от того свойства, с которыми работает в [EmailMessageSchema](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessageschema%28v=exchg.80%29.aspx) или [ ItemSchema](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.itemschema%28v=exchg.80%29.aspx) класса. Создание элемента различных так как **класс** не имеет конструктора, поэтому при создании сообщения электронной почты используется [Конструктор EmailMessage](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.emailmessage.emailmessage%28v=exchg.80%29.aspx) для создания его и [EmailMessage.Save](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.save%28v=exchg.80%29.aspx) или [EmailMessage.SendAndSaveCopy ](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.sendandsavecopy%28v=exchg.80%29.aspx)методы сохраните его, или отправить его и сохраните его. 
  
Аналогично в веб-служб Exchange, используйте операцию [CreateItem](http://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) с элементом [сообщений](http://msdn.microsoft.com/library/2400b33c-43b2-4fc2-b6fb-275a99e0e810%28Office.15%29.aspx) для создания сообщения электронной почты. Чтобы получить, обновить или удалить по электронной почте с помощью веб-служб Exchange, факт, что элемент изменяемого сообщения электронной почты не имеет значения, помимо того, что дополнительные свойства доступны в сообщениях электронной почты. Такие же операции, которые используются для других строго типизированных элементов также используется для сообщений электронной почты. 
  
|**Задача**|**Метод управляемого API EWS**|**Операция служб EWS**|
|:-----|:-----|:-----|
|Создание  <br/> |[EmailMessage.Save](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.save%28v=exchg.80%29.aspx) <br/> |[CreateItem](http://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) <br/> |
|Получить  <br/> |[EmailMessage.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.bind%28v=exchg.80%29.aspx) <br/> |[GetItem](http://msdn.microsoft.com/library/e8492e3b-1c8d-4b14-8070-9530f8306edd%28Office.15%29.aspx) <br/> |
|Update  <br/> |[Item.Update](http://msdn.microsoft.com/en-us/library/dd635915%28v=exchg.80%29.aspx) <br/> |[UpdateItem](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) <br/> |
|Удаление  <br/> |[Item.Delete](http://msdn.microsoft.com/en-us/library/dd635072%28v=exchg.80%29.aspx) <br/> |[DeleteItem](http://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx) <br/> |
   
Поскольку сообщения электронной почты, просто [строго типизированных элементов](folders-and-items-in-ews-in-exchange.md#bk_item), в некоторых случаях работать с ними так же, как этот [универсальный элементов](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md). 
  
## <a name="create-an-email-message-by-using-the-ews-managed-api"></a>Создание сообщения электронной почты с помощью управляемого интерфейса API веб-служб Exchange
<a name="bk_createewsma"> </a>

Можно создать сообщение электронной почты с помощью метода управляемый API EWS [Сохранить](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.save%28v=exchg.80%29.aspx) , как показано в примере кода в следующем примере. Обратите внимание на то, что только сохраняются сообщения в папке "Черновики", не отправляет сообщение. Сведения о том, как отправить сообщение или создания и отправки сообщения в один шаг можно [отправлять сообщения электронной почты с помощью веб-служб Exchange в Exchange](how-to-send-email-messages-by-using-ews-in-exchange.md).
  
В этом примере предполагается, что эта **Служба** является допустимым объектом [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) и пользователь прошел проверку подлинности на сервере Exchange. 
  
```cs
// Create a new email message.
EmailMessage message = new EmailMessage(service);
// Set properties on the email message.
message.ToRecipients.Add("mack@contoso.com");
message.Subject = "Project priorities";
message.Body = "(1) Buy pizza, (2) Eat pizza";
// Save the email message to the Drafts folder (where it can be retrieved, updated, and sent at a later time).
// This method call results in a CreateItem call to EWS.
message.Save(WellKnownFolderName.Drafts);
Console.WriteLine("A draft email message with the subject '" + message.Subject + "' has been saved to the Drafts folder.");
```

## <a name="create-an-email-message-by-using-ews"></a>Создание сообщения электронной почты с помощью веб-служб Exchange
<a name="bk_createews"> </a>

Можно создать сообщение электронной почты с помощью операции EWS [CreateItem](http://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) , как показано в следующем примере. Это также запроса XML, что управляемый API EWS отправляет при [создавать сообщения электронной почты](#bk_createewsma). Обратите внимание на то, что следующий пример сохраняет только сообщения в папке "Черновики", не отправляет сообщение. Сведения о том, как отправить сообщение или создания и отправки сообщения в один шаг можно [отправлять сообщения электронной почты с помощью веб-служб Exchange в Exchange](how-to-send-email-messages-by-using-ews-in-exchange.md).
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2010_SP2" />
  </soap:Header>
  <soap:Body>
    <m:CreateItem MessageDisposition="SaveOnly">
      <m:SavedItemFolderId>
        <t:DistinguishedFolderId Id="drafts" />
      </m:SavedItemFolderId>
      <m:Items>
        <t:Message>
          <t:Subject>Project priorities</t:Subject>
          <t:Body BodyType="HTML">(1) Buy pizza, (2) Eat pizza</t:Body>
          <t:ToRecipients>
            <t:Mailbox>
              <t:EmailAddress>mack@contoso.com</t:EmailAddress>
            </t:Mailbox>
          </t:ToRecipients>
        </t:Message>
      </m:Items>
    </m:CreateItem>
  </soap:Body>
</soap:Envelope>

```

Сервер отвечает на запрос **CreateItem** [CreateItemResponse](http://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) сообщение, содержащее значение [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) **NoError**, это означает, что сообщение электронной почты был успешно создан, и [ItemId](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) из вновь сообщение о создании. 
  
## <a name="get-update-and-delete-an-email-message-by-using-the-ews-managed-api"></a>Получение, обновление и удаление сообщения электронной почты с помощью управляемого интерфейса API веб-служб Exchange
<a name="bk_getewsma"> </a>

Можно использовать управляемый API EWS для получения, обновлять или удалять сообщения электронной почты так же, как выполнять эти действия с любой универсальный элемент из хранилища Exchange. Для получения дополнительных сведений см [элементы почтовых ящиков Exchange с помощью веб-служб Exchange в Exchange](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md).
  
При обновлении сообщения электронной почты, см в список свойств сообщения электронной почты для записи [электронной почты свойства и элементы в веб-служб Exchange в Exchange](email-properties-and-elements-in-ews-in-exchange.md) . Чтобы отправить черновик сообщения после его обновления, обратитесь к разделу [отправлять черновики по электронной почте с помощью управляемого интерфейса API веб-служб Exchange](how-to-send-email-messages-by-using-ews-in-exchange.md#bk_senddraftewsma).
  
## <a name="get-update-and-delete-an-email-message-by-using-ews"></a>Получение, обновление и удаление сообщения электронной почты с помощью веб-служб Exchange
<a name="bk_getews"> </a>

Можно использовать веб-служб Exchange для получения, обновлять и удалять сообщения электронной почты так же, как выполнять эти действия с любой универсальный элемент из хранилища Exchange. Для получения дополнительных сведений см [элементы почтовых ящиков Exchange с помощью веб-служб Exchange в Exchange](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md).
  
При обновлении сообщения электронной почты, см в список свойств сообщения электронной почты для записи [электронной почты свойства и элементы в веб-служб Exchange в Exchange](email-properties-and-elements-in-ews-in-exchange.md) . Чтобы отправить черновик сообщения после его обновления, обратитесь к разделу [отправлять черновики по электронной почте с помощью веб-служб Exchange](how-to-send-email-messages-by-using-ews-in-exchange.md#bk_senddraftews).
  
## <a name="in-this-section"></a>В этом разделе
<a name="bk_inthissection"> </a>

- [Отправить по электронной почте свойства и элементы в веб-служб Exchange в Exchange](email-properties-and-elements-in-ews-in-exchange.md)
    
- [Отправлять сообщения электронной почты с помощью веб-служб Exchange в Exchange](how-to-send-email-messages-by-using-ews-in-exchange.md)
    
- [Ответ на сообщения электронной почты с помощью веб-служб Exchange в Exchange](how-to-respond-to-email-messages-by-using-ews-in-exchange.md)
    
- [Перемещение и копирование сообщений электронной почты с помощью веб-служб Exchange в Exchange](how-to-move-and-copy-email-messages-by-using-ews-in-exchange.md)
    
- [Работа с беседы с помощью веб-служб Exchange в Exchange](how-to-work-with-conversations-by-using-ews-in-exchange.md)
    
- [Извлечь сущности из сообщения электронной почты с помощью веб-служб Exchange в Exchange](how-to-extract-an-entity-from-an-email-message-by-using-ews-in-exchange.md)
    
- [Обрабатывать сообщения электронной почты в пакетах с помощью веб-служб Exchange в Exchange](how-to-process-email-messages-in-batches-by-using-ews-in-exchange.md)
    
## <a name="see-also"></a>См. также


- [Разработка клиентов веб-служб для Exchange](develop-web-service-clients-for-exchange.md)
    
- [Папки и элементы в веб-службах Exchange](folders-and-items-in-ews-in-exchange.md)
    

