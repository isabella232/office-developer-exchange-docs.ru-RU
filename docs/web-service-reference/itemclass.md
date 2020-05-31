---
title: ItemClass
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ItemClass
api_type:
- schema
ms.assetid: 56020078-50b4-4880-894a-a9f234033cfb
description: Элемент ItemClass представляет класс сообщения элемента.
ms.openlocfilehash: 7f146a8472362b8f3cd4062a4af2ce452e204742
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834149"
---
# <a name="itemclass"></a>ItemClass

Элемент **ItemClass** представляет класс сообщения элемента. 
  
```XML
<ItemClass/>
```

 **итемкласстипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[акцептитем](acceptitem.md) <br/> |Представляет ответ на принять приглашение на собрание.  <br/> |
|[календаритем](calendaritem.md) <br/> |Представляет элемент календаря Exchange.  <br/> |
|[Контакт](contact.md) <br/> |Представляет элемент контакта Exchange.  <br/> |
|[Беседы (ConversationType)](conversation-conversationtype.md) <br/> |Представляет одну беседу.  <br/> |
|[деклинеитем](declineitem.md) <br/> |Представляет отклонить ответ на приглашения на собрание.  <br/> |
|[дистрибутионлист](distributionlist.md) <br/> |Представляет список рассылки.  <br/> |
|[глобалитемклассес](globalitemclasses.md) <br/> |Содержит список классов элементов, которые представляют все классы элементов для элементов беседы в почтовом ящике.  <br/> |
|[Элемент](item.md) <br/> |Представляет общий элемент Exchange.  <br/> |
|[митингканцеллатион](meetingcancellation.md) <br/> |Представляет отмену собрания в хранилище Exchange.  <br/> |
|[митингмессаже](meetingmessage.md) <br/> |Представляет собрание в хранилище Exchange.  <br/> |
|[Свойство meetingrequest](meetingrequest.md) <br/> |Представляет приглашение на собрание в хранилище Exchange.  <br/> |
|[митингреспонсе](meetingresponse.md) <br/> |Представляет ответ на приглашение на собрание в хранилище Exchange.  <br/> |
|[Message](message-ex15websvcsotherref.md) <br/> |Представляет сообщение электронной почты Exchange.  <br/> |
|[RemoveItem](removeitem.md) <br/> |Удаляет элемент из хранилища Exchange.  <br/> |
|[Задача](task.md) <br/> |Представляет задачу в хранилище Exchange.  <br/> |
|[тентативелякцептитем](tentativelyacceptitem.md) <br/> |Представляет под вопросом ответ на приглашения на собрание.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Может потребоваться текстовое значение, которое соответствует типу элемента. Например, при создании или обновлении сообщения объект IPM. Примечание или необходимо указать другой класс, который соответствует сообщению. Пустое значение не разрешено. Однако при создании или обновлении элемента допустимым является пустой тип.
  
Если для свойства **ItemClass** задано значение, которое не согласуется с типом элемента, возвращается ошибка. Например, **ItemClassу** сообщения невозможно задать значение **ItemClass** для задачи. 
  
## <a name="remarks"></a>Примечания

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |True  <br/> |
   
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

