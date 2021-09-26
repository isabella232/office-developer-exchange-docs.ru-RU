---
title: SharingEffectiveRights (CalendarPermissionReadAccessType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- SharingEffectiveRights
api_type:
- schema
ms.assetid: b519f642-a9ef-4300-92e6-ed8202855fde
description: Элемент SharingEffectiveRights указывает разрешения, которые есть у пользователя для общих данных календаря.
ms.openlocfilehash: d1e669b70ad816cc24e34554a116159025e267e6
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59547073"
---
# <a name="sharingeffectiverights-calendarpermissionreadaccesstype"></a>SharingEffectiveRights (CalendarPermissionReadAccessType)

Элемент **SharingEffectiveRights** указывает разрешения, которые есть у пользователя для общих данных календаря. 
  
```XML
<SharingEffectiveRights>None | TimeOnly | TimeAndSubjectAndLocation | FullDetails</SharingEffectiveRights>
```

 **CalendarPermissionReadAccessType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[CalendarFolder](calendarfolder.md) <br/> |Представляет папку, которая в основном содержит элементы календаря.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

В следующей таблице перечислены возможные значения элемента **SharingEffectiveRights.** 
  
|**Значение**|**Описание**|
|:-----|:-----|
|Нет  <br/> |Указывает, что у пользователя нет разрешения на просмотр элементов в календаре.  <br/> |
|TimeOnly  <br/> |Указывает, что у пользователя есть разрешение на просмотр только свободного или занятого времени в календаре.  <br/> |
|TimeAndSubjectAndLocation  <br/> |Указывает, что у пользователя есть разрешение на просмотр свободного или занятого времени в календаре, а также субъекта и расположения встреч.  <br/> |
|FullDetails  <br/> |Указывает, что у пользователя есть разрешение на просмотр всех элементов в календаре, в том числе свободного/занятого времени и темы, расположения и сведений о встречах.  <br/> |
   
## <a name="remarks"></a>Заметки

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

