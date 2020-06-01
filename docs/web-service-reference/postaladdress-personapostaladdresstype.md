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
ms.openlocfilehash: 9e316e5e0135c2d18fab4067241988c65eceec66
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465389"
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

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

[Улица](street.md)  |  [City (город](city.md)  |  ) [State (состояние](state-ex15websvcsotherref.md)  |  ) [Country (страна](country.md)  |  ) [PostalCode](postalcode.md)  |  [PostOfficeBox](postofficebox.md)  |  [Тип (строка)](type-string.md)  |  [Широта](latitude.md)  |  [Долгота](longitude.md)  |  [Точность](accuracy.md)  |  [Высота](altitude.md)  |  [Алтитудеаккураци](altitudeaccuracy.md)  |  [Форматтедаддресс](formattedaddress.md)  |  [LocationUri](locationuri.md)  |  [Локатионсаурце](locationsource.md)
  
### <a name="parent-elements"></a>Родительские элементы

[EnhancedLocation](enhancedlocation.md)
  
## <a name="remarks"></a>Примечания

Этот элемент появился в Exchange Server 2013.
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> ||
   

