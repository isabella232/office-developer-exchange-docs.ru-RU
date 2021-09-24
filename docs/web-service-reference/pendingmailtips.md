---
title: PendingMailTips
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- PendingMailTips
api_type:
- schema
ms.assetid: 0cd70eea-8d36-4b1b-bf80-5edf359e7ba7
description: Элемент PendingMailTips указывает, что советы почты в этом элементе не могли быть оценены до истечения срока ожидания обработки сервера.
ms.openlocfilehash: cadf1839acaeb7c25d1bbf42af5fc866f6c7a4cd
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59521762"
---
# <a name="pendingmailtips"></a>PendingMailTips

Элемент **PendingMailTips** указывает, что советы почты в этом элементе не могли быть оценены до истечения срока ожидания обработки сервера. 
  
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
|[Подсказки](mailtips.md) <br/> |Представляет значения для различных типов советов почты.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

В следующей таблице перечислены возможные значения элемента **PendingMailTips.** 
  
|**Значение**|**Описание**|
|:-----|:-----|
|Все  <br/> |Представляет все доступные советы по почте.  <br/> |
|OutOfOfficeMessage  <br/> |Представляет сообщение Out of Office (OOF).  <br/> |
|MailboxFullStatus  <br/> |Представляет состояние полного почтового ящика.  <br/> |
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
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

