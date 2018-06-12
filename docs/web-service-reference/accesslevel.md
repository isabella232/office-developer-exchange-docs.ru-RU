---
title: AccessLevel
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 09475586-00fa-4e82-a915-5ca263ab4d1c
description: Элемент AccessLevel указывает уровень доступа к собранию по сети.
ms.openlocfilehash: 1bf0a191fad529b555117e4ff992c352615bc79b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762478"
---
# <a name="accesslevel"></a>AccessLevel

Элемент **AccessLevel** указывает уровень доступа к собранию по сети. 
  
```XML
<AccessLevel/>
```

 **OnlineMeetingSettingsType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[OnlineMeetingSettings](onlinemeetingsettings.md) <br/> |Задает параметры для собраний по сети.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

В следующей таблице перечислены значения для элемента **AccessLevel** . 
  
**AccessLevel элемент текстовые значения**

|**Значение**|**Описание**|
|:-----|:-----|
|Всем пользователям  <br/> |Уровень доступа ко всем open.  <br/> |
|Внутренний  <br/> |Уровень доступа только является внутренним.  <br/> |
|Приглашение  <br/> |Уровень доступа — только приглашенные участники.  <br/> |
|Заблокирован  <br/> |Уровень доступа к заблокированному компьютеру.  <br/> |
   
## <a name="remarks"></a>Замечания

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
Этот элемент появился в Exchange Server 2013.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема типа  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> ||
   
## <a name="see-also"></a>См. также

- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

