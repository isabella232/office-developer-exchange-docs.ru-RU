---
title: PendingMailTips
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- PendingMailTips
api_type:
- schema
ms.assetid: 0cd70eea-8d36-4b1b-bf80-5edf359e7ba7
description: Элемент PendingMailTips указывает, что почтовые подсказки в этот элемент не удалось вычислить до истечения времени ожидания обработки на сервере.
ms.openlocfilehash: 73d597f6534ea29f7d26d6526c48631251521ae5
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834704"
---
# <a name="pendingmailtips"></a>PendingMailTips

Элемент **PendingMailTips** указывает, что почтовые подсказки в этот элемент не удалось вычислить до истечения времени ожидания обработки на сервере. 
  
```XML
<PendingMailTips>All | OutOfOfficeMessage | MailboxFullStatus | CustomMailTip | ExternalMemberCount | TotalMemberCount | MaxMessageSize | DeliveryRestriction | ModerateStatus | InvalidRecipient</PendingMailTips>
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
|[Почтовые подсказки](mailtips.md) <br/> |Представляет значения для различных типов почтовые подсказки.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

В следующей таблице приведены возможные значения для элемента **PendingMailTips** . 
  
|**Значение**|**Описание**|
|:-----|:-----|
|Все  <br/> |Представляет все доступные почтовые подсказки.  <br/> |
|OutOfOfficeMessage  <br/> |Представляет сообщение об отсутствии на работе Office (отсутствие на работе).  <br/> |
|MailboxFullStatus  <br/> |Представляет сведения о состоянии, полный почтовый ящик.  <br/> |
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
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

