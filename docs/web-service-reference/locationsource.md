---
title: LocationSource
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: fc4d77d5-6200-4cf3-848a-1088fec0e0d6
description: Элемент LocationSource определяет информацию о происхождении связанный почтовый адрес, например, контакт или телефонной книги.
ms.openlocfilehash: 7f5cf5fcca0a72287593349fcf5090a74225d012
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834248"
---
# <a name="locationsource"></a>LocationSource

Элемент **LocationSource** определяет информацию о происхождении связанный почтовый адрес, например, контакт или телефонной книги. 
  
```XML
<LocationSource> None | LocationServices | PhonebookServices | Device | Contact | Resource </LocationSource>
```

 **LocationSourceType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

[Значение (PersonaPostalAddressType)](value-personapostaladdresstype.md) | [PostalAddress (PersonaPostalAddressType)](postaladdress-personapostaladdresstype.md)
  
## <a name="text-value"></a>Текстовое значение

Текстовые значения для элемента **LocationSource** перечислены в следующей таблице: 
  
**LocationSource элемент текстовые значения**

|**Значение**|**Описание**|
|:-----|:-----|
|Нет  <br/> |Не указан источник расположения.  <br/> |
|LocationServices  <br/> |Сведения о был получен из расположения служб.  <br/> |
|PhonebookServices  <br/> |Сведения о был получен из службы телефонной книги.  <br/> |
|Устройство  <br/> |Сведения о был получен из устройства.  <br/> |
|Контакт  <br/> |Сведения о был получен контакт.  <br/> |
|Resource  <br/> |Сведения о был получен из ресурса.  <br/> |
   
## <a name="remarks"></a>Замечания

Этот элемент появился в Exchange Server 2013.
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  

