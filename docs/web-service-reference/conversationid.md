---
title: ConversationId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ConversationId
api_type:
- schema
ms.assetid: d5f1ddb3-9af3-4677-a6ba-111b304a951e
description: Элемент ConversationId содержит идентификатор элемента или беседы.
ms.openlocfilehash: 4f12d70ae6b72773760a731f5778cf6743ce699f
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461473"
---
# <a name="conversationid"></a>ConversationId

Элемент **ConversationId** содержит идентификатор элемента или беседы. 
  
```XML
<ConversationId Id="" ChangeKey="" />
```

 **итемидтипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|**Id** <br/> |Определяет определенный элемент в хранилище Exchange.  <br/> |
|**чанжекэй** <br/> | Определяет определенную версию элемента. **Чанжекэй** является обязательным для следующих сценариев:  <br/><br/>-Для элемента [UpdateItem](updateitem.md) требуется **чанжекэй** , если для атрибута **Конфликтресолутион** задано значение автоматического разрешения. Параметр "Авторазрешение" является значением по умолчанию. Если атрибут **чанжекэй** не включен, ответ вернет значение [респонсекоде](responsecode.md) , равное **еррорчанжекэйрекуиред**.<br/><br/>- Для элементов [SendItem](senditem.md), [DeleteItem](deleteitem.md)и [DeleteFolder](deletefolder.md) требуется **чанжекэй** , чтобы проверить, будет ли Предпринятая операция действовать в последней версии элемента. Если атрибут **чанжекэй** не включен в идентификатор **ItemId** или **чанжекэй** пуст, то ответ вернет значение [респонсекоде](responsecode.md) , равное **еррорсталеобжект**.  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

Отсутствуют.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[календаритем](calendaritem.md) <br/> |Представляет элемент календаря Exchange.  <br/> |
|[Контакт](contact.md) <br/> |Представляет элемент контакта Exchange.  <br/> |
|[конверсатионактион](conversationaction.md) <br/> |Представляет одно действие, которое будет применено к одной беседе.  <br/> |
|[дистрибутионлист](distributionlist.md) <br/> |Представляет список рассылки.  <br/> |
|[Элемент](item.md) <br/> |Представляет элемент в хранилище Exchange.  <br/> |
|[митингканцеллатион](meetingcancellation.md) <br/> |Представляет отмену собрания в хранилище Exchange.  <br/> |
|[митингмессаже](meetingmessage.md) <br/> |Представляет собрание в хранилище Exchange.  <br/> |
|[Свойство meetingrequest](meetingrequest.md) <br/> |Представляет приглашение на собрание в хранилище Exchange.  <br/> |
|[митингреспонсе](meetingresponse.md) <br/> |Представляет ответ на приглашение на собрание в хранилище Exchange.  <br/> |
|[Message](message-ex15websvcsotherref.md) <br/> |Представляет сообщение электронной почты Exchange.  <br/> |
|[PostItem](postitem.md) <br/> |Представляет элемент POST в хранилище Exchange.  <br/> |
|[RemoveItem](removeitem.md) <br/> |Удаляет элемент из хранилища Exchange.  <br/> |
|[Задача](task.md) <br/> |Представляет задачу в хранилище Exchange.  <br/> |
|[Беседы (ConversationType)](conversation-conversationtype.md) <br/> |Представляет одну беседу.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Нет.
  
## <a name="remarks"></a>Примечания

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Операция FindConversation](findconversation-operation.md)
- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

