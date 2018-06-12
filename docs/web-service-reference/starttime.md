---
title: Время начала
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- StartTime
api_type:
- schema
ms.assetid: 1fac7937-7a06-4d66-9d2a-14423bcb3b37
description: Элемент StartTime представляет Пуск промежуток времени.
ms.openlocfilehash: 4346797d755bb6e577e1cacb8bec656a7562bf1f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19835560"
---
# <a name="starttime"></a>Время начала

Элемент **StartTime** представляет Пуск промежуток времени. 
  
```xml
<StartTime/
```

**dateTime**

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Значение TimeWindow](timewindow.md) <br/> |Определяет период времени, запрос пользователя сведений о доступности.  <br/><br/> Ниже приведен выражение XPath для этого элемента.  <br/><br/>  `/GetUserAvailabilityRequest/FreeBusyViewOptions/TimeWindow` <br/> |
|[DetailedSuggestionsWindow](detailedsuggestionswindow.md) <br/> |Определяет период времени, который будет опрошен на наличие подробные сведения о времени предложенного собрания.  <br/><br/> Ниже приведен выражение XPath для этого элемента. <br/> <br/>  `/GetUserAvailabilityRequest/SuggestionViewOptions/DetailedSuggestionsWindow` <br/> |
|[Продолжительность (UserOofSettings)](duration-useroofsettings.md) <br/> | Указывает, во время выполнения, для которого включен состояние об отсутствии на работе Office (OOF), если элемент [OofState](oofstate.md) задано значение **расписанию**.  <br/><br/>  Ниже приведены возможные выражения XPath для этого элемента. <br/> <br/>  `/SetUserOofSettingsRequest/UserOofSettings/Duration` <br/><br/>  `/GetUserOofSettingsResponse/OofSettings/Duration` <br/> |
|[CalendarEvent](calendarevent.md) <br/> |Представляет вхождение элемента уникальный календаря. Используется для обеспечения доступности запросы. Элемент **StartTime** является обязательным в элементе **CalendarEvent** . **Время начала** элемент в элементе **CalendarEvent** является уникальным для типа **CalendarEvent** , несмотря на то, что он содержит те же значения аспекта, которые содержат элементы **StartTime** в тип **длительность** .  <br/><br/> Ниже приведен выражение XPath для этого элемента.  <br/> <br/> `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/CalendarEventArray/CalendarEvent[i]` <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение является обязательным.
  
## <a name="remarks"></a>Замечания

Элемент [EndTime](endtime.md) представляет конец периода времени. 
  
Схема включает в себя многие [StartTime](starttime.md) элементы. 
  
> [!NOTE]
> Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа. 
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Операция GetUserAvailability](getuseravailability-operation.md)
- [Getting User Availability](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

