---
title: Участник
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Attendee
api_type:
- schema
ms.assetid: 393c3d7e-7416-458a-b976-270b88eaaa03
description: Элемент "участник" представляет участников и ресурсы собрания.
ms.openlocfilehash: f376e59b27017e0a9d27692cb1a4ae759cd1af0e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457650"
---
# <a name="attendee"></a>Участник

Элемент " **участник** " представляет участников и ресурсы собрания. 
  
```xml
<Attendee>
   <Mailbox/>
   <ResponseType/>
   <LastResponseTime/>
</Attendee>
```

 **AttendeeType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Mailbox](mailbox.md) <br/> |Определяет полностью разрешенный адрес электронной почты.  <br/> |
|[ResponseType](responsetype.md) <br/> |Представляет тип ответа получателя, полученный для собрания. Это свойство относится только к элементу календаря организатора собрания.  <br/> |
|[ластреспонсетиме](lastresponsetime.md) <br/> |Представляет дату и время последнего полученного ответа.  <br/> |
|[ProposedStart](proposedstart-attendeetype.md) <br/> |Представляет предполагаемое время начала собрания для участника. <br/> |
|[пропоседенд](proposedend-attendeetype.md) <br/> |Представляет предложенное конечное время участника собрания. <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[RequiredAttendees](requiredattendees.md) <br/> |Представляет участников, которые необходимы для участия в собрании.  <br/> |
|[OptionalAttendees](optionalattendees.md) <br/> |Представляет участников, которые не являются обязательными для участия в собрании.  <br/> |
|[Ресурсы](resources.md) <br/> |Представляет запланированный ресурс для собрания.  <br/> |
   
## <a name="remarks"></a>Примечания

Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

