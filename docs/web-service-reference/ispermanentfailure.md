---
title: IsPermanentFailure
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 18dc3a97-cc0a-4092-934e-a6e86f52e668
description: Элемент IsPermanentFailure указывает, была ли предыдущая попытка индексировать элемент неудачной.
ms.openlocfilehash: e5ed20de3c3de9c39d1487e3177c1b6ec358d990
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59532722"
---
# <a name="ispermanentfailure"></a>IsPermanentFailure

Элемент **IsPermanentFailure** указывает, была ли предыдущая попытка индексировать элемент неудачной. 
  
```XML
<IsPermanentFailure>true | false</IsPermanentFailure>
```

 **Boolean**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

[NonIndexableItemDetail](nonindexableitemdetail.md)
  
## <a name="text-value"></a>Текстовое значение

Значение текста, **истинное** для **элемента IsPermanentFailure,** указывает на то, что предыдущая попытка индексировать элемент почтового ящика была неудачной. Значение false **указывает,** что предыдущая попытка индексировать элемент почтового ящика была успешной. 
  
## <a name="remarks"></a>Заметки

Этот элемент появился в Exchange Server 2013.
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |false  <br/> |
   

