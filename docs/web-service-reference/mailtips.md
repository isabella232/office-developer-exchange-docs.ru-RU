---
title: Подсказки
manager: sethgros
ms.date: 09/17/2015
ms.audience: ITPro
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- MailTips
api_type:
- schema
ms.assetid: c1cba493-bccc-4b8e-be8e-bfa8a8b10882
description: Элемент MailTips представляет значения для различных типов советов почты.
ms.openlocfilehash: bf7ed542d51f2a8cb3172275be12cb72104bc5b2
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59511140"
---
# <a name="mailtips"></a>Подсказки

Элемент **MailTips** представляет значения для различных типов советов почты. 
  
```XML
<MailTips>
   <RecipientAddress/>
   <PendingMailTips/>
   <OutOfOffice/>
   <MailboxFull/>
   <CustomMailTip/>
   <TotalMemberCount/>
   <ExternalMemberCount/>
   <MaxMessageSize/>
   <DeliveryRestricted/>
   <IsModerated/>
   <InvalidRecipient/>
</MailTips>
```

 **Подсказки**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[RecipientAddress](recipientaddress.md) <br/> |Представляет почтовый ящик получателя.  <br/> |
|[PendingMailTips](pendingmailtips.md) <br/> |Указывает, что советы по почте в этом элементе не могли быть оценены до истечения срока обработки сервера.  <br/> |
|[OutOfOffice](outofoffice.md) <br/> |Представляет сообщение отклика и время для отправки сообщения ответа.  <br/> |
|[MailboxFull](mailboxfull.md) <br/> |Указывает, заполнен ли почтовый ящик получателя.  <br/> |
|[CustomMailTip](custommailtip.md) <br/> |Представляет настраиваемые сообщения отзывов почты.  <br/> |
|[TotalMemberCount](totalmembercount.md) <br/> |Представляет количество всех участников группы.  <br/> |
|[ExternalMemberCount](externalmembercount.md) <br/> |Представляет количество внешних участников в группе.  <br/> |
|[MaxMessageSize](maxmessagesize.md) <br/> |Представляет максимальный размер сообщения, который может принять получатель.  <br/> |
|[DeliveryRestricted](deliveryrestricted.md) <br/> |Указывает, будут ли ограничения на доставку препятствовать сообщению отправщика до адресата.  <br/> |
|[IsModerated](ismoderated.md) <br/> |Указывает, модерироваться ли почтовый ящик получателя.  <br/> |
|[InvalidRecipient (MailTips)](invalidrecipient-mailtips.md) <br/> |Указывает, является ли получатель недействительным.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[MailTipsResponseMessageType](mailtipsresponsemessagetype.md) <br/> |Представляет параметры советов почты.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Нет.
  
## <a name="remarks"></a>Заметки

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

