---
title: EndTime
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- EndTime
api_type:
- schema
ms.assetid: 82e4ef4f-a557-4044-b9b7-d91622f4ac55
description: Элемент EndTime представляет конец интервала времени.
ms.openlocfilehash: 5a30b32ecfeafe582cd07dd662aacb0a960257c9
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462994"
---
# <a name="endtime"></a>EndTime

Элемент **EndTime** представляет конец интервала времени. 
  
```xml
<EndTime>dateTime</EndTime>
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
|[TimeWindow](timewindow.md) <br/> |Определяет интервал времени, запрошенный для сведений о доступности пользователя.<br/><br/> Ниже приведено выражение XPath для этого элемента:<br/><br/>  `/GetUserAvailabilityRequest/FreeBusyViewOptions/TimeWindow` <br/> |
|[детаиледсугжестионсвиндов](detailedsuggestionswindow.md) <br/> |Определяет интервал времени, на который запрашивается подробная информация о предложенном времени проведения собрания.<br/><br/> Ниже приведено выражение XPath для этого элемента:<br/><br/>  `/GetUserAvailabilityRequest/SuggestionViewOptions/DetailedSuggestionsWindow`.  <br/> |
|[Продолжительность (Усеруфсеттингс)](duration-useroofsettings.md) <br/> | Указывает срок, в течение которого состояние отсутствия на работе (отсутствие на работе) включается, если для элемента [уфстате](oofstate.md) задано значение " **запланировано**".  <br/><br/>  Ниже приведены возможные выражения XPath для этого элемента.<br/><br/>  `/SetUserOofSettingsRequest/UserOofSettings/Duration` <br/><br/>  `/GetUserOofSettingsResponse/OofSettings/Duration` <br/> |
|[Экземпляр](occurrence.md) <br/> |Представляет один измененный экземпляр повторяющегося элемента календаря.  <br/> |
|[календаревент](calendarevent.md) <br/> |Представляет уникальное вхождение элемента календаря. Используется для запросов о доступности. Элемент **EndTime** необходим в элементе **календаревент** . Элемент **EndTime** в элементе **календаревент** уникален для типа **календаревент** .<br/><br/> Ниже приведено выражение XPath для этого элемента:<br/><br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/CalendarEventArray/CalendarEvent[i]` <br/> |
   
## <a name="text-value"></a>Текстовое значение

Необходимо указать текстовое значение.
  
## <a name="remarks"></a>Примечания

Элемент [StartTime](starttime.md) представляет начало интервала времени. 
  
Время окончания представляет время клиента.
  
Схема включает множество элементов [EndTime](endtime.md) . 
  
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

