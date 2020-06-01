---
title: Владелец
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: ea0f0afc-32fe-46cb-8530-62a6ce9490f6
description: Элемент Owner указывает, является ли указанный пользователь электронной почты владельцем.
ms.openlocfilehash: 2dd085aba34052d95efd1e72edca7be4aba71155
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44466523"
---
# <a name="isowner"></a>Владелец

Элемент **owner** указывает, является ли указанный пользователь электронной почты владельцем. 
  
```XML
<IsOwner>true | false</IsOwner>
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
|[ригхтсманажементлиценседата](rightsmanagementlicensedata.md) <br/> |Указывает сведения о лицензии на управление правами.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение **true** для элемента **owner** указывает на то, что пользователь является владельцем прав, выданных для элемента. Значение **false** указывает, что пользователь не является владельцем прав, выданных для элемента. 
  
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

