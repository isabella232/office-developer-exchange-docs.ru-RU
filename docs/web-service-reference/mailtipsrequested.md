---
title: MailTipsRequested
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- MailTipsRequested
api_type:
- schema
ms.assetid: 8037bbe5-a37f-4f77-8209-27a94f9095ef
description: Элемент MailTipsRequested содержит типы советов почты, запрашиваемого в службе.
ms.openlocfilehash: 14a463d3b00a9f8b3e2aa2e822209ff87a221f9b
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59524856"
---
# <a name="mailtipsrequested"></a>MailTipsRequested

Элемент **MailTipsRequested содержит** типы советов почты, запрашиваемого в службе. 
  
```XML
<MailTipsRequested/>
```

 **MailTipTypes**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[GetMailTips](getmailtips.md) <br/> |Содержит получателей и типы советов по извлечению почты.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

В следующей таблице перечислены возможные значения элемента **MailTipsRequested.** 
  
|**Значение**|**Описание**|
|:-----|:-----|
|Все  <br/> |Представляет все доступные советы по почте.  <br/> |
|OutOfOfficeMessage  <br/> |Представляет сообщение Out of Office (OOF).  <br/> |
|MailboxFullStatus  <br/> |Представляет состояние для заполненного почтового ящика.  <br/> |
|CustomMailTip  <br/> |Представляет настраиваемый совет по почте.  <br/> |
|ExternalMemberCount  <br/> |Представляет количество внешних участников.  <br/> |
|TotalMemberCount  <br/> |Представляет количество всех участников.  <br/> |
|MaxMessageSize  <br/> |Представляет максимальный размер сообщения, который может принять получатель.  <br/> |
|DeliveryRestriction  <br/> |Указывает, будут ли ограничения на доставку препятствовать сообщению отправщика до адресата.  <br/> |
|ModerationStatus  <br/> |Указывает, будет ли сообщение отправитель просмотреть модератором.  <br/> |
|InvalidRecipient  <br/> |Указывает, является ли получатель недействительным.  <br/> |
   
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

