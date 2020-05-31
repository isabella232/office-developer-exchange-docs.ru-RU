---
title: Значение (Персонапосталаддресстипе)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: be838fc2-cfcb-4856-b095-a8e5366bb6c6
description: Элемент value указывает сведения, связанные с почтовым адресом.
ms.openlocfilehash: 048d3a49552f1a9e89744e4cd16ec1745417e923
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19840462"
---
# <a name="value-personapostaladdresstype"></a>Значение (Персонапосталаддресстипе)

Элемент **value** указывает сведения, связанные с почтовым адресом. 
  
```XML
<Value>
   <Street/>
   <City/>
   <State/>
   <Country/>
   <PostalCode/>
   <PostOfficeBox/>
   <Type/>
   <Latitude/>
   <Longitude/>
   <Accuracy/>
   <Altitude/>
   <AltitudeAccuracy/>
   <FormattedAddress/>
   <LocationUri/>
   <LocationSource/>
</Value>
```

**персонапосталаддресстипе**

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

[Street](street.md)[State](state-ex15websvcsotherref.md)[PostalCode](postalcode.md) | [Altitude](altitude.md) | [LocationSource](locationsource.md) [PostOfficeBox](postofficebox.md) | [Latitude](latitude.md) | [LocationUri](locationuri.md)[FormattedAddress](formattedaddress.md)[Country](country.md) | [City](city.md) |  |  | [AltitudeAccuracy](altitudeaccuracy.md)[Accuracy](accuracy.md)[Longitude](longitude.md)[Type (string)](type-string.md)Город проживания |  | страна с | адресом PostOfficeBox тип (String) Широта/Долгота точность точность высота алтитудеаккураци форматтедаддресс LocationUri локатионсаурце |  |  | 
  
### <a name="parent-elements"></a>Родительские элементы

[посталаддрессаттрибутедвалуе](postaladdressattributedvalue.md)
  
## <a name="remarks"></a>Примечания

Этот элемент появился в Exchange Server 2013.
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> ||
   

