---
title: HasPicture
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- HasPicture
api_type:
- schema
ms.assetid: 922a43fe-01bd-49f2-9261-e00e4699b8da
description: Элемент HasPicture указывает, есть ли у контактного элемента вложение файла, которое представляет изображение контакта.
ms.openlocfilehash: c00a51b5f43d951beb7325dbb6e10ae70ec94d04
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59519529"
---
# <a name="haspicture"></a>HasPicture

Элемент **HasPicture** указывает, есть ли у контактного элемента вложение файла, которое представляет изображение контакта. 
  
[Contact](contact.md)
  
[HasPicture](haspicture.md)
  
```xml
<HasPicture>true or false</HasPicture>
```

 **boolean**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Contact](contact.md) <br/> |Представляет элемент контакта в Exchange магазине.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение элемента **HasPicture** может быть верным **или** **ложным.** Значение по умолчанию — **false**.
  
## <a name="remarks"></a>Заметки

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

