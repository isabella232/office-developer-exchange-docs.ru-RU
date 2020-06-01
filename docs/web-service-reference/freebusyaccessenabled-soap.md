---
title: Фрибусякцессенаблед (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 8d2d3276-b180-424e-a707-7256d14a1776
description: Элемент Фрибусякцессенаблед представляет флаг Фрибусякцессенаблед (). Элемент Фрибусякцессенаблед предназначен только для внутреннего использования. Этот элемент не используется клиентами.
ms.openlocfilehash: c148d8fa1301339f8579884dc02b6c9e452f3035
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44461298"
---
# <a name="freebusyaccessenabled-soap"></a>Фрибусякцессенаблед (SOAP)

Элемент **фрибусякцессенаблед** представляет флаг **фрибусякцессенаблед ()** . Элемент **фрибусякцессенаблед** предназначен только для внутреннего использования. Этот элемент не используется клиентами. 
  
```XML
<FreeBusyAccessEnabled>true | false</FreeBusyAccessEnabled>
```

 **Boolean**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

Отсутствуют.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Организатионрелатионшипсеттингс (SOAP)](organizationrelationshipsettings-soap.md) <br/> |Представляет список отношений Организации для одной организации.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение **true** для элемента **фрибусякцессенаблед** указывает, что отношение общего доступа должно использоваться для получения сведений о занятости от пользователей в Организации. Значение **false** указывает, что отношение совместного доступа должно подавляться. 
  
## <a name="remarks"></a>Примечания

Используйте этот элемент, чтобы разрешить или запретить отправку сведений о доступности с сервера. 
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Имя схемы  <br/> |Схема автообнаружения  <br/> |
|Файл проверки  <br/> |Messages. xsd  <br/> |
|Может быть пустым  <br/> |True  <br/> |
   
## <a name="see-also"></a>См. также



[Операция Жеторганизатионрелатионшипсеттингс (SOAP)](getorganizationrelationshipsettings-operation-soap.md)

