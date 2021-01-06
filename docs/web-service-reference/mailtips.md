---
title: Подсказки
manager: sethgros
ms.date: 09/17/2015
ms.audience: ITPro
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MailTips
api_type:
- schema
ms.assetid: c1cba493-bccc-4b8e-be8e-bfa8a8b10882
description: Элемент MailTips представляет значения для различных типов подсказок.
ms.openlocfilehash: 9bacdea7b4f3108f700ed102025445e01a73e69d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44447598"
---
# <a name="mailtips"></a>Подсказки

Элемент **MailTips** представляет значения для различных типов подсказок. 
  
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
|[PendingMailTips](pendingmailtips.md) <br/> |Указывает, что подсказки электронной почты в этом элементе не удалось оценить до истечения времени действия обработки сервера.  <br/> |
|[OutOfOffice](outofoffice.md) <br/> |Представляет ответное сообщение и продолжительность отправки сообщения.  <br/> |
|[MailboxFull](mailboxfull.md) <br/> |Указывает, заполнен ли почтовый ящик получателя.  <br/> |
|[CustomMailTip](custommailtip.md) <br/> |Представляет настроенное сообщение подсказки почты.  <br/> |
|[TotalMemberCount](totalmembercount.md) <br/> |Представляет количество всех членов группы.  <br/> |
|[ExternalMemberCount](externalmembercount.md) <br/> |Представляет количество внешних участников в группе.  <br/> |
|[MaxMessageSize](maxmessagesize.md) <br/> |Представляет максимальный размер сообщения, который может принять получатель.  <br/> |
|[DeliveryRestricted](deliveryrestricted.md) <br/> |Указывает, будут ли ограничения доставки препятствовать доставке сообщения отправи мне.  <br/> |
|[IsModerated](ismoderated.md) <br/> |Указывает, является ли почтовый ящик получателя модером.  <br/> |
|[InvalidRecipient (MailTips)](invalidrecipient-mailtips.md) <br/> |Указывает, является ли получатель недопустимым.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[MailTipsResponseMessageType](mailtipsresponsemessagetype.md) <br/> |Представляет параметры подсказок почты.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Нет.
  
## <a name="remarks"></a>Примечания

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

