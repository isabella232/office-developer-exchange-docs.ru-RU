---
title: ConversationId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- ConversationId
api_type:
- schema
ms.assetid: d5f1ddb3-9af3-4677-a6ba-111b304a951e
description: Элемент ConversationId содержит идентификатор элемента или беседы.
ms.openlocfilehash: 345c7c692576abb8c1e1b9848b005ca3d0c0fa0f
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59547542"
---
# <a name="conversationid"></a>ConversationId

Элемент **ConversationId** содержит идентификатор элемента или беседы. 
  
```XML
<ConversationId Id="" ChangeKey="" />
```

 **ItemIdType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|**Id** <br/> |Определяет определенный элемент в Exchange магазине.  <br/> |
|**ChangeKey** <br/> | Определяет определенную версию элемента. **ChangeKey** требуется для следующих сценариев:  <br/><br/>- Элемент [UpdateItem требует](updateitem.md) **changeKey,** если атрибут **ConflictResolution** задан для autoResolve. AutoResolve — это значение по умолчанию. Если атрибут **ChangeKey** не включен, ответ возвращает значение [ResponseCode,](responsecode.md) равное **errorChangeKeyRequired.**<br/><br/>- [Элементы SendItem,](senditem.md) [DeleteItem](deleteitem.md)и [DeleteFolder](deletefolder.md) требуют **changeKey** для проверки того, будет ли попытка операции действовать в последней версии элемента. Если атрибут **ChangeKey** не включен в **ItemId** или если **changeKey** пуст, ответ возвращает значение [ResponseCode,](responsecode.md) равное **errorStaleObject.**  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[CalendarItem](calendaritem.md) <br/> |Представляет элемент календаря Exchange.  <br/> |
|[Контакт](contact.md) <br/> |Представляет элемент контакта Exchange.  <br/> |
|[ConversationAction](conversationaction.md) <br/> |Представляет одно действие, применяемую к одному разговору.  <br/> |
|[DistributionList](distributionlist.md) <br/> |Представляет список рассылки.  <br/> |
|[Элемент](item.md) <br/> |Представляет элемент в хранилище Exchange.  <br/> |
|[MeetingCancellation](meetingcancellation.md) <br/> |Представляет отмену собрания в хранилище Exchange.  <br/> |
|[MeetingMessage](meetingmessage.md) <br/> |Представляет собрание в хранилище Exchange.  <br/> |
|[MeetingRequest](meetingrequest.md) <br/> |Представляет приглашение на собрание в хранилище Exchange.  <br/> |
|[MeetingResponse](meetingresponse.md) <br/> |Представляет ответ на приглашение на собрание в хранилище Exchange.  <br/> |
|[Message](message-ex15websvcsotherref.md) <br/> |Представляет сообщение электронной почты Exchange.  <br/> |
|[PostItem](postitem.md) <br/> |Представляет элемент столба в Exchange магазине.  <br/> |
|[RemoveItem](removeitem.md) <br/> |Удаляет элемент из хранилища Exchange.  <br/> |
|[Задача](task.md) <br/> |Представляет задачу в хранилище Exchange.  <br/> |
|[Беседы (ConversationType)](conversation-conversationtype.md) <br/> |Представляет одну беседу.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Нет.
  
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

- [Операция FindConversation](findconversation-operation.md)
- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

