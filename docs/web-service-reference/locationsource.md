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
ms.openlocfilehash: 7f5cf5fcca0a72287593349fcf5090a74225d012
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834248"
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

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

[Value (персонапосталаддресстипе)](value-personapostaladdresstype.md) | [посталаддресс (персонапосталаддресстипе)](postaladdress-personapostaladdresstype.md)
  
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
  

