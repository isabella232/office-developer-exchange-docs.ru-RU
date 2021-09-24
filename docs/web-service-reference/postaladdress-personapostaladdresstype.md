---
title: PostalAddress (PersonaPostalAddressType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 075f7d65-9d05-47cb-af26-0dd6d5593439
description: Элемент PostalAddress указывает почтовый адрес для персоны.
ms.openlocfilehash: 4e95a94c5a7ce917a0a4b9abf7b7ef120301ae6c
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59523904"
---
# <a name="postaladdress-personapostaladdresstype"></a>PostalAddress (PersonaPostalAddressType)

Элемент **PostalAddress** указывает почтовый адрес для персоны. 
  
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

 **PersonaPostalAddressType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

[Street](street.md)  |  [Город](city.md)  |  [Состояние](state-ex15websvcsotherref.md)  |  [Страна](country.md)  |  [Почтовый индекс](postalcode.md)  |  [PostOfficeBox](postofficebox.md)  |  [Тип (строка)](type-string.md)  |  [Широта](latitude.md)  |  [Долгота](longitude.md)  |  [Точность](accuracy.md)  |  [Высота](altitude.md)  |  [AltitudeAccuracacacy](altitudeaccuracy.md)  |  [FormattedAddress](formattedaddress.md)  |  [LocationUri](locationuri.md)  |  [LocationSource](locationsource.md)
  
### <a name="parent-elements"></a>Родительские элементы

[EnhancedLocation](enhancedlocation.md)
  
## <a name="remarks"></a>Заметки

Этот элемент появился в Exchange Server 2013.
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> ||
   

