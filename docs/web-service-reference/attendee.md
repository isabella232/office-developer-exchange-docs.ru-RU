---
title: Участник
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Attendee
api_type:
- schema
ms.assetid: 393c3d7e-7416-458a-b976-270b88eaaa03
description: Элемент Attendee представляет участников и ресурсы для собрания.
ms.openlocfilehash: d48dcee42292b045ffc7cdcc5fd02f70109b1853
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59531196"
---
# <a name="attendee"></a>Участник

Элемент **Attendee** представляет участников и ресурсы для собрания. 
  
```xml
<Attendee>
   <Mailbox/>
   <ResponseType/>
   <LastResponseTime/>
</Attendee>
```

 **AttendeeType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Mailbox](mailbox.md) <br/> |Определяет полностью разрешенный адрес электронной почты.  <br/> |
|[ResponseType](responsetype.md) <br/> |Представляет тип ответа получателя, который получается для собрания. Это свойство относится только к элементу календаря организатора собраний.  <br/> |
|[LastResponseTime](lastresponsetime.md) <br/> |Представляет дату и время последнего полученного ответа.  <br/> |
|[ProposedStart](proposedstart-attendeetype.md) <br/> |Представляет предлагаемое время начала собрания. <br/> |
|[ProposedEnd](proposedend-attendeetype.md) <br/> |Представляет предлагаемое время окончания собрания. <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[RequiredAttendees](requiredattendees.md) <br/> |Представляет участников, которые должны присутствовать на собрании.  <br/> |
|[OptionalAttendees](optionalattendees.md) <br/> |Представляет участников, которые не обязаны присутствовать на собрании.  <br/> |
|[Ресурсы](resources.md) <br/> |Представляет запланированный ресурс для собрания.  <br/> |
   
## <a name="remarks"></a>Заметки

Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

