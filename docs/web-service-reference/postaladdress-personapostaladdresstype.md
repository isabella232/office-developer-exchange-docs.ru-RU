---
title: Посталаддресс (Персонапосталаддресстипе)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 075f7d65-9d05-47cb-af26-0dd6d5593439
description: Элемент Посталаддресс указывает почтовый адрес пользователя.
ms.openlocfilehash: fb418154867aebb4d284e75be579003c0ddc88f6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834855"
---
# <a name="postaladdress-personapostaladdresstype"></a>Посталаддресс (Персонапосталаддресстипе)

Элемент **посталаддресс** указывает почтовый адрес пользователя. 
  
```XML
<PostalAddress>
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
</PostalAddress>
```

 **персонапосталаддресстипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

[Street](street.md)[State](state-ex15websvcsotherref.md)[PostalCode](postalcode.md) | [Altitude](altitude.md) | [LocationSource](locationsource.md) [PostOfficeBox](postofficebox.md) | [Latitude](latitude.md) | [LocationUri](locationuri.md)[FormattedAddress](formattedaddress.md)[Country](country.md) | [City](city.md) |  |  | [AltitudeAccuracy](altitudeaccuracy.md)[Accuracy](accuracy.md)[Longitude](longitude.md)[Type (string)](type-string.md)Город проживания |  | страна с | адресом PostOfficeBox тип (String) Широта/Долгота точность точность высота алтитудеаккураци форматтедаддресс LocationUri локатионсаурце |  |  | 
  
### <a name="parent-elements"></a>Родительские элементы

[EnhancedLocation](enhancedlocation.md)
  
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
   

