---
title: StartTime
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
description: Элемент StartTime представляет начало интервала времени.
ms.openlocfilehash: 16bee698b65dc512a709e2af9ddfe8629347fee3
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458567"
---
# <a name="starttime"></a>StartTime

Элемент **StartTime** представляет начало интервала времени. 
  
```xml
<StartTime/
```

**дата и время**

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

Отсутствуют.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[TimeWindow](timewindow.md) <br/> |Определяет интервал времени, запрошенный для сведений о доступности пользователя.  <br/><br/> Ниже приведено выражение XPath для этого элемента:  <br/><br/>  `/GetUserAvailabilityRequest/FreeBusyViewOptions/TimeWindow` <br/> |
|[детаиледсугжестионсвиндов](detailedsuggestionswindow.md) <br/> |Определяет интервал времени, на который запрашивается подробная информация о предложенном времени проведения собрания.  <br/><br/> Ниже приведено выражение XPath для этого элемента: <br/> <br/>  `/GetUserAvailabilityRequest/SuggestionViewOptions/DetailedSuggestionsWindow` <br/> |
|[Продолжительность (Усеруфсеттингс)](duration-useroofsettings.md) <br/> | Указывает срок, в течение которого состояние отсутствия на работе (отсутствие на работе) включается, если для элемента [уфстате](oofstate.md) задано значение " **запланировано**".  <br/><br/>  Ниже приведены возможные выражения XPath для этого элемента. <br/> <br/>  `/SetUserOofSettingsRequest/UserOofSettings/Duration` <br/><br/>  `/GetUserOofSettingsResponse/OofSettings/Duration` <br/> |
|[календаревент](calendarevent.md) <br/> |Представляет уникальное вхождение элемента календаря. Используется для запросов о доступности. Элемент **StartTime** необходим в элементе **календаревент** . Элемент **StartTime** в элементе **календаревент** уникален для типа **календаревент** , несмотря на то, что он содержит те же значения аспекта, что и элементы **StartTime** в типе **Duration** .  <br/><br/> Ниже приведено выражение XPath для этого элемента:  <br/> <br/> `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/CalendarEventArray/CalendarEvent[i]` <br/> |
   
## <a name="text-value"></a>Текстовое значение

Необходимо указать текстовое значение.
  
## <a name="remarks"></a>Примечания

Элемент [EndTime](endtime.md) представляет конец интервала времени. 
  
Схема включает множество элементов [StartTime](starttime.md) . 
  
> [!NOTE]
> Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа. 
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Операция GetUserAvailability](getuseravailability-operation.md)
- [Getting User Availability](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

