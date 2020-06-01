---
title: IsHidden
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 2377b584-bd1e-49fc-b80a-a6634721a297
description: Элемент Hidden содержит логическое значение, которое указывает, следует ли скрыть или отобразить основной контакт в составе персонажа.
ms.openlocfilehash: a22628e9ab4a46de04fe395f2d6c1b70083a5c77
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44464240"
---
# <a name="ishidden"></a>IsHidden

Элемент **Hidden** содержит логическое значение, которое указывает, следует ли скрыть или отобразить основной контакт в составе персонажа. 
  
```XML
<IsHidden>true | false</IsHidden>
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
|[Атрибуты (Персонааттрибутионтипе)](attribution-personaattributiontype.md) <br/> |Указывает экземпляр в массиве атрибутов для элемента **персоны** .  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение **true** для элемента **Hidden** указывает на то, что основной контакт должен быть скрыт или отображаться в составе персонажа. Значение **false** указывает, что базовый контакт не должен быть скрытым или отображаться как часть персонажа. 
  
## <a name="remarks"></a>Примечания

Этот элемент появился в Exchange Server 2013.
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема типа  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> ||
   
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

