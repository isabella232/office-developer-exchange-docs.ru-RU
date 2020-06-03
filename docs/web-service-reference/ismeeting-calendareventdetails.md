---
title: Проведенное собрание (Календаревентдетаилс)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsMeeting
api_type:
- schema
ms.assetid: dd6900e4-e4a3-471a-909d-7240ebec501b
description: Элемент "собрание" указывает, является ли событие календаря собранием или встречей.
ms.openlocfilehash: b75dfba203177d6451f3847bf8d1f68014612e1c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465998"
---
# <a name="ismeeting-calendareventdetails"></a>Проведенное собрание (Календаревентдетаилс)

Элемент " **собрание** " указывает, является ли событие календаря собранием или встречей. 
  
[жетусераваилабилитиреспонсе](getuseravailabilityresponse.md)
  
[фрибусиреспонсеаррай](freebusyresponsearray.md)
  
[фрибусиреспонсе](freebusyresponse.md)
  
[фрибусивиев](freebusyview.md)
  
[календаревентаррай](calendareventarray.md)
  
[календаревент](calendarevent.md)
  
[календаревентдетаилс](calendareventdetails.md)
  
[Проведенное собрание (Календаревентдетаилс)](ismeeting-calendareventdetails.md)
  
```xml
<IsMeeting>true or false</IsMeeting>
```

 **boolean**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

Отсутствуют.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[календаревентдетаилс](calendareventdetails.md) <br/> |Предоставляет дополнительные сведения о событии календаря.  <br/> Ниже приведено выражение XPath для этого элемента:  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/CalendarEventArray/CalendarEvent[i]/CalendarEventDetails` <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение является обязательным, если этот элемент возвращается в ответе. Этот элемент является обязательным, если используется элемент [календаревентдетаилс](calendareventdetails.md) . 
  
## <a name="remarks"></a>Примечания

Разница между собранием и встречей состоит в том, что собрание является элементом календаря, включающим участников; Встреча — это элемент календаря, не содержащий участников.
  
Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция GetUserAvailability](getuseravailability-operation.md)
  
[жетусераваилабилитиреспонсе](getuseravailabilityresponse.md)


[Getting User Availability](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

