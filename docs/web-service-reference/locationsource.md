---
title: LocationSource
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: fc4d77d5-6200-4cf3-848a-1088fec0e0d6
description: Элемент LocationSource указывает сведения о происхождении связанного почтового адреса, например контакта или телефонной книги.
ms.openlocfilehash: f3569494d3e662fbc46060944c8bd399b62d656b
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59543263"
---
# <a name="locationsource"></a>LocationSource

Элемент **LocationSource** указывает сведения о происхождении связанного почтового адреса, например контакта или телефонной книги. 
  
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

[Значение (PersonaPostalAddressType)](value-personapostaladdresstype.md)  |  [PostalAddress (PersonaPostalAddressType)](postaladdress-personapostaladdresstype.md)
  
## <a name="text-value"></a>Текстовое значение

Текстовые значения элемента **LocationSource** перечислены в следующей таблице: 
  
**Текстовые значения элемента LocationSource**

|**Значение**|**Описание**|
|:-----|:-----|
|Нет  <br/> |Источник расположения не существует.  <br/> |
|LocationServices  <br/> |Информация была получена из служб расположения.  <br/> |
|PhonebookServices  <br/> |Эта информация была получена из служб телефонной книги.  <br/> |
|Устройство  <br/> |Информация была получена с устройства.  <br/> |
|Контакт  <br/> |Информация была получена из контакта.  <br/> |
|Ресурс  <br/> |Сведения получены с ресурса.  <br/> |
   
## <a name="remarks"></a>Заметки

Этот элемент появился в Exchange Server 2013.
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  

