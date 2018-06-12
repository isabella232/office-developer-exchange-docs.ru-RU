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
description: Элемент Attendee представляет участников и ресурсы, необходимые для собрания.
ms.openlocfilehash: 60cb0839c2f6de69b833c11f4594d40c14cd8887
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761515"
---
# <a name="attendee"></a>Участник

Элемент **Attendee** представляет участников и ресурсы, необходимые для собрания. 
  
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
|[Mailbox](mailbox.md) <br/> |Определяет адрес электронной почты полностью разрешенной.  <br/> |
|[ResponseType](responsetype.md) <br/> |Представляет тип получателя ответа, полученные на собрание. Это свойство применяется только для элемента календаря Организатор собрания.  <br/> |
|[LastResponseTime](lastresponsetime.md) <br/> |Представляет дату и время последнего ответа, полученные.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[RequiredAttendees](requiredattendees.md) <br/> |Представляет участников, которые необходимы на участие в собрании.  <br/> |
|[OptionalAttendees](optionalattendees.md) <br/> |Представляет участников, которые не требуется на участие в собрании.  <br/> |
|[Ресурсы](resources.md) <br/> |Ресурс запланированного собрания.  <br/> |
   
## <a name="remarks"></a>Замечания

Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

