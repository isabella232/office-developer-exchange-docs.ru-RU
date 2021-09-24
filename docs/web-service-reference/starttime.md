---
title: StartTime
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- StartTime
api_type:
- schema
ms.assetid: 1fac7937-7a06-4d66-9d2a-14423bcb3b37
description: Элемент StartTime представляет начало периода времени.
ms.openlocfilehash: e6d9034fa1b01f0f0969837761f4da7c36cea752
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59531655"
---
# <a name="starttime"></a>StartTime

Элемент **StartTime** представляет начало периода времени. 
  
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
|[TimeWindow](timewindow.md) <br/> |Определяет период времени, запрашиваемой для сведений о доступности пользователей.  <br/><br/> Ниже приводится выражение XPath к этому элементу:  <br/><br/>  `/GetUserAvailabilityRequest/FreeBusyViewOptions/TimeWindow` <br/> |
|[DetailedSuggestionsWindow](detailedsuggestionswindow.md) <br/> |Определяет период времени, запрашиваемой для получения подробных сведений о рекомендуемом времени собраний.  <br/><br/> Ниже приводится выражение XPath к этому элементу: <br/> <br/>  `/GetUserAvailabilityRequest/SuggestionViewOptions/DetailedSuggestionsWindow` <br/> |
|[Duration (UserOofSettings)](duration-useroofsettings.md) <br/> | Указывает продолжительность включения состояния Out of Office (OOF), если элемент [OofState](oofstate.md) задан в **Scheduled**.  <br/><br/>  Возможные выражения XPath к этому элементу: <br/> <br/>  `/SetUserOofSettingsRequest/UserOofSettings/Duration` <br/><br/>  `/GetUserOofSettingsResponse/OofSettings/Duration` <br/> |
|[CalendarEvent](calendarevent.md) <br/> |Представляет уникальный случай элементов календаря. Это используется для запросов доступности. Элемент **StartTime** необходим в **элементе CalendarEvent.** Элемент **StartTime** в **элементе CalendarEvent** уникален для типа **CalendarEvent,** хотя он содержит те же аспектные значения, что и элементы **StartTime** в типе **Duration.**  <br/><br/> Ниже приводится выражение XPath к этому элементу:  <br/> <br/> `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/CalendarEventArray/CalendarEvent[i]` <br/> |
   
## <a name="text-value"></a>Текстовое значение

Требуется текстовое значение.
  
## <a name="remarks"></a>Заметки

Элемент [EndTime](endtime.md) представляет собой конец периода времени. 
  
Схема включает в себя множество [элементов StartTime.](starttime.md) 
  
> [!NOTE]
> Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа. 
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Операция GetUserAvailability](getuseravailability-operation.md)
- [Getting User Availability](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

