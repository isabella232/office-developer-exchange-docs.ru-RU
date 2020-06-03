---
title: Электронная почта и веб-службах Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.assetid: 4d7bdb37-f7f1-409f-9749-f8bcde7dc52a
description: Узнайте, как работать с сообщениями электронной почты, в том числе создавать электронную почту и выполнять другие задачи, связанные с электронной почтой, с помощью управляемого API EWS или EWS в Exchange.
localization_priority: Priority
ms.openlocfilehash: 323d9d2cc40aa86044a439ad53e53a4808916783
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44455445"
---
# <a name="email-and-ews-in-exchange"></a>Электронная почта и веб-службах Exchange

Узнайте, как работать с сообщениями электронной почты, в том числе создавать электронную почту и выполнять другие задачи, связанные с электронной почтой, с помощью управляемого API EWS или EWS в Exchange.
  

  
В основном Exchange — это электронная почта. Но что создает электронную почту? Кроме того, сообщения электронной почты — это один из [строго типизированных элементов](folders-and-items-in-ews-in-exchange.md#bk_item) в Exchange, что означает, что они содержат определенный [набор свойств](email-properties-and-elements-in-ews-in-exchange.md), даже перед отправкой. Сообщения электронной почты представлены классом [EmailMessage](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx) в УПРАВЛЯЕМОМ API EWS и элементом [Message](https://msdn.microsoft.com/library/2400b33c-43b2-4fc2-b6fb-275a99e0e810%28Office.15%29.aspx) и его дочерними элементами в EWS. 
  
В управляемом API EWS объект **EmailMessage** является производным от объекта [Item](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item%28v=exchg.80%29.aspx) . Класс **EmailMessage** расширяет класс **Item** , предоставляя дополнительные свойства, такие как [EmailMessage. sender](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage.sender%28v=exchg.80%29.aspx) и [EmailMessage. Read](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.emailmessage.isread%28v=exchg.80%29.aspx), которые теперь часто используются практически всеми сценариями обмена сообщениями. При получении, обновлении или удалении сообщения электронной почты в большинстве случаев это можно сделать с помощью объекта **EmailMessage** или объекта базового **элемента** в зависимости от того, находятся ли свойства, с которыми ведется работа, в классе [емаилмессажесчема](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessageschema%28v=exchg.80%29.aspx) или [итемсчема](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.itemschema%28v=exchg.80%29.aspx) . Создание элемента отличается из-за того, что класс **элемента** не имеет конструктора, поэтому при создании электронного сообщения используется [конструктор EmailMessage](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.emailmessage.emailmessage%28v=exchg.80%29.aspx) для его создания и [EmailMessage. Save](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage.save%28v=exchg.80%29.aspx) или [EmailMessage. SendAndSaveCopy](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage.sendandsavecopy%28v=exchg.80%29.aspx) , а также для его сохранения или отправки. 
  
Аналогично, в EWS используйте операцию [CreateItem](https://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) с элементом [Message](https://msdn.microsoft.com/library/2400b33c-43b2-4fc2-b6fb-275a99e0e810%28Office.15%29.aspx) для создания сообщения электронной почты. Чтобы получать, обновлять или удалять сообщения электронной почты с помощью EWS, факт того, что изменяемый элемент является сообщением электронной почты, не имеет значения, Кроме того факта, что дополнительные свойства доступны в сообщениях электронной почты. Для сообщений электронной почты также используются те же операции, что и для других строго типизированных элементов. 
  
|**Задача**|**Метод управляемого API EWS**|**Операция EWS**|
|:-----|:-----|:-----|
|Create  <br/> |[EmailMessage. Save](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage.save%28v=exchg.80%29.aspx) <br/> |[CreateItem](https://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) <br/> |
|Получение  <br/> |[EmailMessage. Bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage.bind%28v=exchg.80%29.aspx) <br/> |[GetItem](https://msdn.microsoft.com/library/e8492e3b-1c8d-4b14-8070-9530f8306edd%28Office.15%29.aspx) <br/> |
|Update  <br/> |[Item.Update](https://msdn.microsoft.com/library/dd635915%28v=exchg.80%29.aspx) <br/> |[UpdateItem](https://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) <br/> |
|Удаление  <br/> |[Item.Delete](https://msdn.microsoft.com/library/dd635072%28v=exchg.80%29.aspx) <br/> |[DeleteItem](../web-service-reference/deleteitem-operation.md) <br/> |
   
Так как сообщения электронной почты — это просто [строго типизированные элементы](folders-and-items-in-ews-in-exchange.md#bk_item), в некоторых случаях вы работаете с ними так же, как и [с общими элементами](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md). 
  
## <a name="create-an-email-message-by-using-the-ews-managed-api"></a>Создание электронного сообщения с помощью управляемого API EWS
<a name="bk_createewsma"> </a>

Вы можете создать сообщение электронной почты с помощью метода [Save](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage.save%28v=exchg.80%29.aspx) управляемого API EWS, как показано в коде, приведенном в следующем примере. Обратите внимание, что в этом примере только сообщение сохраняется в папке "Черновики", поэтому сообщение не отправляется. Сведения о том, как отправить сообщение или создать и отправить сообщение, см [в статье отправка сообщений электронной почты с помощью EWS в Exchange](how-to-send-email-messages-by-using-ews-in-exchange.md).
  
В этом примере предполагается, что **служба** является действительным объектом [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx), и что пользователь прошел проверку подлинности на сервере Exchange server. 
  
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

## <a name="create-an-email-message-by-using-ews"></a>Создание электронного сообщения с помощью EWS
<a name="bk_createews"> </a>

Вы можете создать сообщение электронной почты с помощью операции [CreateItem](https://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) , как показано в следующем примере. Это также запрос XML, который отправляет управляемый API EWS при [создании сообщения электронной почты](#bk_createewsma). Обратите внимание, что в приведенном ниже примере только сообщение сохраняется в папке "Черновики", поэтому сообщение не отправляется. Сведения о том, как отправить сообщение или создать и отправить сообщение в одном сте, приведены в статье [Отправка сообщений электронной почты с помощью EWS в Exchange](how-to-send-email-messages-by-using-ews-in-exchange.md).
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
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

В ответ на запрос **CreateItem** сервер отправляет сообщение [CreateItemResponse](https://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx), включающее параметр [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) со значением **NoError**, которое указывает, что сообщение было успешно создано, и свойство [ItemId](https://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) созданного сообщения. 
  
## <a name="get-update-and-delete-an-email-message-by-using-the-ews-managed-api"></a>Получение, обновление и удаление сообщения электронной почты с помощью управляемого API EWS
<a name="bk_getewsma"> </a>

Вы можете использовать управляемый API EWS для получения, обновления или удаления сообщения электронной почты так же, как и при выполнении этих действий с любым универсальным элементом из хранилища Exchange. Для получения дополнительных сведений ознакомьтесь [со статьей работу с элементами почтовых ящиков Exchange с помощью EWS в Exchange](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md).
  
Если вы обновляете сообщение электронной почты, ознакомьтесь со статьей " [Свойства и элементы электронной почты" в EWS в Exchange](email-properties-and-elements-in-ews-in-exchange.md) , чтобы получить список доступных для записи свойств сообщения электронной почты. Чтобы отправить черновик сообщения после его обновления, ознакомьтесь с [разадресом Отправка черновика электронного сообщения с помощью управляемого API EWS](how-to-send-email-messages-by-using-ews-in-exchange.md#bk_senddraftewsma).
  
## <a name="get-update-and-delete-an-email-message-by-using-ews"></a>Получение, обновление и удаление сообщения электронной почты с помощью EWS
<a name="bk_getews"> </a>

С помощью EWS вы можете получать, обновлять и удалять сообщения электронной почты так же, как и при выполнении этих действий с любым универсальным элементом из хранилища Exchange. Для получения дополнительных сведений ознакомьтесь [со статьей работу с элементами почтовых ящиков Exchange с помощью EWS в Exchange](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md).
  
Если вы обновляете сообщение электронной почты, ознакомьтесь со статьей " [Свойства и элементы электронной почты" в EWS в Exchange](email-properties-and-elements-in-ews-in-exchange.md) , чтобы получить список доступных для записи свойств сообщения электронной почты. Чтобы отправить черновик сообщения после его обновления, ознакомьтесь со статьей [Отправка черновика электронного сообщения с помощью EWS](how-to-send-email-messages-by-using-ews-in-exchange.md#bk_senddraftews).
  
## <a name="in-this-section"></a>В этой статье
<a name="bk_inthissection"> </a>

- [Свойства и элементы электронной почты в EWS в Exchange](email-properties-and-elements-in-ews-in-exchange.md)
    
- [Отправка сообщений электронной почты с помощью EWS в Exchange](how-to-send-email-messages-by-using-ews-in-exchange.md)
    
- [Ответ на сообщения электронной почты с помощью EWS в Exchange](how-to-respond-to-email-messages-by-using-ews-in-exchange.md)
    
- [Перемещение и копирование сообщений электронной почты с помощью EWS в Exchange](how-to-move-and-copy-email-messages-by-using-ews-in-exchange.md)
    
- [Взаимодействие с беседами с помощью EWS в Exchange](how-to-work-with-conversations-by-using-ews-in-exchange.md)
    
- [Извлечение объекта из сообщения электронной почты с помощью EWS в Exchange](how-to-extract-an-entity-from-an-email-message-by-using-ews-in-exchange.md)
    
- [Обработка сообщений электронной почты в пакетах с помощью EWS в Exchange](how-to-process-email-messages-in-batches-by-using-ews-in-exchange.md)
    
## <a name="see-also"></a>См. также


- [Разработка клиентов веб-служб для Exchange](develop-web-service-clients-for-exchange.md)
    
- [Папки и элементы в веб-службах Exchange](folders-and-items-in-ews-in-exchange.md)
    

