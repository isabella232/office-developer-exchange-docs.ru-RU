---
title: MailTipsRequested
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MailTipsRequested
api_type:
- schema
ms.assetid: 8037bbe5-a37f-4f77-8209-27a94f9095ef
description: Элемент MailTipsRequested содержит типы, запрашивается из службы почтовые подсказки.
ms.openlocfilehash: fa2bef394ea8473aa65bdc2f1d39c0794186fdc6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834348"
---
# <a name="mailtipsrequested"></a>MailTipsRequested

Элемент **MailTipsRequested** содержит типы, запрашивается из службы почтовые подсказки. 
  
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
|[GetMailTips](getmailtips.md) <br/> |Содержит получателей и типы почтовые подсказки для извлечения.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

В следующей таблице приведены возможные значения для элемента **MailTipsRequested** . 
  
|**Значение**|**Описание**|
|:-----|:-----|
|Все  <br/> |Представляет все доступные почтовые подсказки.  <br/> |
|OutOfOfficeMessage  <br/> |Представляет сообщение об отсутствии на работе Office (отсутствие на работе).  <br/> |
|MailboxFullStatus  <br/> |Представляет состояние почтового ящика, заполнена.  <br/> |
|CustomMailTip  <br/> |Представляет подсказку настраиваемых почты.  <br/> |
|ExternalMemberCount  <br/> |Представляет количество внешних элементов.  <br/> |
|TotalMemberCount  <br/> |Представляет количество всех элементов.  <br/> |
|MaxMessageSize  <br/> |Представляет максимальный размер сообщения, можно принять получателя.  <br/> |
|DeliveryRestriction  <br/> |Указывает ли ограничения на доставку будет препятствовать сообщения достигает получателя.  <br/> |
|ModerationStatus  <br/> |Указывает, будет ли сообщения будут проверены модератором.  <br/> |
|InvalidRecipient  <br/> |Указывает, является ли получатель является недопустимым.  <br/> |
   
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

