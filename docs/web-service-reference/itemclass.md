---
title: ItemClass
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- ItemClass
api_type:
- schema
ms.assetid: 56020078-50b4-4880-894a-a9f234033cfb
description: Элемент ItemClass представляет класс сообщений элемента.
ms.openlocfilehash: 612fe582a1136cdba519d5a5f153999770095463
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59540875"
---
# <a name="itemclass"></a>ItemClass

Элемент **ItemClass** представляет класс сообщений элемента. 
  
```XML
<ItemClass/>
```

 **ItemClassType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[AcceptItem](acceptitem.md) <br/> |Представляет ответ на принять приглашение на собрание.  <br/> |
|[CalendarItem](calendaritem.md) <br/> |Представляет элемент календаря Exchange.  <br/> |
|[Контакт](contact.md) <br/> |Представляет элемент контакта Exchange.  <br/> |
|[Беседы (ConversationType)](conversation-conversationtype.md) <br/> |Представляет одну беседу.  <br/> |
|[DeclineItem](declineitem.md) <br/> |Представляет отклонить ответ на приглашения на собрание.  <br/> |
|[DistributionList](distributionlist.md) <br/> |Представляет список рассылки.  <br/> |
|[GlobalItemClasses](globalitemclasses.md) <br/> |Содержит список классов элементов, которые представляют все классы элементов разговорных элементов в почтовом ящике.  <br/> |
|[Элемент](item.md) <br/> |Представляет общий элемент Exchange.  <br/> |
|[MeetingCancellation](meetingcancellation.md) <br/> |Представляет отмену собрания в хранилище Exchange.  <br/> |
|[MeetingMessage](meetingmessage.md) <br/> |Представляет собрание в хранилище Exchange.  <br/> |
|[MeetingRequest](meetingrequest.md) <br/> |Представляет приглашение на собрание в хранилище Exchange.  <br/> |
|[MeetingResponse](meetingresponse.md) <br/> |Представляет ответ на приглашение на собрание в хранилище Exchange.  <br/> |
|[Message](message-ex15websvcsotherref.md) <br/> |Представляет сообщение электронной почты Exchange.  <br/> |
|[RemoveItem](removeitem.md) <br/> |Удаляет элемент из хранилища Exchange.  <br/> |
|[Задача](task.md) <br/> |Представляет задачу в хранилище Exchange.  <br/> |
|[TentativelyAcceptItem](tentativelyacceptitem.md) <br/> |Представляет под вопросом ответ на приглашения на собрание.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Может потребоваться текстовое значение, соответствующее типу элемента. Например, если вы создаете или обновляете сообщение, IPM. Примечание или другой класс, соответствующий сообщению. Пустое значение не допускается. Но если вы создаете или обновляете элемент, пустой тип действителен.
  
Ошибка возвращается, если **itemClass** за установлено значение, не соответствующее типу элемента. Например, элемент **ItemClass** сообщения не может быть установлен в значении **ItemClass** для задачи. 
  
## <a name="remarks"></a>Заметки

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |True  <br/> |
   
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

