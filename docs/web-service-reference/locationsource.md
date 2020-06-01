---
title: локатионсаурце
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: fc4d77d5-6200-4cf3-848a-1088fec0e0d6
description: Элемент Локатионсаурце указывает сведения о происхождении связанного почтового адреса, например контакт или телефонной книги.
ms.openlocfilehash: ceba52c43d1c798bb8f5492b779c7c45d7d00b0b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44467104"
---
# <a name="locationsource"></a>локатионсаурце

Элемент **локатионсаурце** указывает сведения о происхождении связанного почтового адреса, например контакт или телефонной книги. 
  
```XML
<LocationSource> None | LocationServices | PhonebookServices | Device | Contact | Resource </LocationSource>
```

 **локатионсаурцетипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

Отсутствуют.
  
### <a name="parent-elements"></a>Родительские элементы

[Значение (персонапосталаддресстипе)](value-personapostaladdresstype.md)  |  [Посталаддресс (персонапосталаддресстипе)](postaladdress-personapostaladdresstype.md)
  
## <a name="text-value"></a>Текстовое значение

Текстовые значения для элемента **локатионсаурце** перечислены в следующей таблице. 
  
**Текстовые значения элементов Локатионсаурце**

|**Значение**|**Описание**|
|:-----|:-----|
|Нет  <br/> |Источник расположения отсутствует.  <br/> |
|локатионсервицес  <br/> |Сведения получены из служб расположения.  <br/> |
|фонебуксервицес  <br/> |Сведения получены из службы телефонной книги.  <br/> |
|Device  <br/> |Сведения получены с устройства.  <br/> |
|Контакт  <br/> |Сведения получены из контакта.  <br/> |
|Resource  <br/> |Сведения получены из ресурса.  <br/> |
   
## <a name="remarks"></a>Примечания

Этот элемент появился в Exchange Server 2013.
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  

