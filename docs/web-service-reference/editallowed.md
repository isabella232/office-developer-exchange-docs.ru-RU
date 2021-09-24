---
title: EditAllowed
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: e63c4f7e-77c0-4826-b4e2-43b795d03914
description: Элемент EditAllowed указывает, можно ли изменить управление правами на информацию.
ms.openlocfilehash: 2bd88dd47eb3f1964eae678412a6748ee8d28ec8
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59540120"
---
# <a name="editallowed"></a>EditAllowed

Элемент **EditAllowed** указывает, можно ли изменить управление правами на информацию. 
  
```XML
<EditAllowed> true | false </EditAllowed>
```

 **Boolean**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[RightsManagementLicenseData](rightsmanagementlicensedata.md) <br/> |Указывает сведения о лицензии на управление правами.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Значение текста, **истинное** для **элемента EditAllowed,** указывает на то, что управление правами на информацию (IRM) может быть изменено. Значение false **указывает,** что IRM нельзя изменить. 
  
## <a name="remarks"></a>Заметки

Этот элемент появился в Exchange Server 2013.
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема типа  <br/> |
|Файл проверки  <br/> |types.xsd  <br/> |
|Может быть пустым  <br/> ||
   
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

