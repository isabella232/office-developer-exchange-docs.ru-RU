---
title: Почтовые подсказки
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
description: Элемент подсказки представляет значения для различных типов почтовые подсказки.
ms.openlocfilehash: 3a2e95225b09fd2d81db32f821ea3069ab7e7852
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19834311"
---
# <a name="mailtips"></a>Почтовые подсказки

Элемент **подсказки** представляет значения для различных типов почтовые подсказки. 
  
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

 **Почтовые подсказки**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[RecipientAddress](recipientaddress.md) <br/> |Представляет почтовый ящик получателя.  <br/> |
|[PendingMailTips](pendingmailtips.md) <br/> |Указывает, что почтовые подсказки в этот элемент не удалось вычислить до истечения времени ожидания обработки на сервере.  <br/> |
|[Нет на месте](outofoffice.md) <br/> |Представляет ответное сообщение и время для отправки сообщения ответа.  <br/> |
|[MailboxFull](mailboxfull.md) <br/> |Указывает, является ли полный почтовый ящик получателя.  <br/> |
|[CustomMailTip](custommailtip.md) <br/> |Представляет подсказку настроенного почтового сообщения.  <br/> |
|[TotalMemberCount](totalmembercount.md) <br/> |Представляет количество всех элементов в группе.  <br/> |
|[ExternalMemberCount](externalmembercount.md) <br/> |Представляет количество внешних элементов в группе.  <br/> |
|[MaxMessageSize](maxmessagesize.md) <br/> |Представляет максимальный размер сообщения, можно принять получателя.  <br/> |
|[DeliveryRestricted](deliveryrestricted.md) <br/> |Указывает ли ограничения на доставку будет препятствовать сообщения достигает получателя.  <br/> |
|[IsModerated](ismoderated.md) <br/> |Указывает, является ли управляемым почтовый ящик получателя.  <br/> |
|[InvalidRecipient (подсказки)](invalidrecipient-mailtips.md) <br/> |Указывает, является ли получатель является недопустимым.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[MailTipsResponseMessageType](mailtipsresponsemessagetype.md) <br/> |Представляет почтовые подсказки параметров.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Нет.
  
## <a name="remarks"></a>Замечания

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

