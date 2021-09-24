---
title: ProgrammaticAccessAllowed
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: a1fc7dff-a303-4809-b7f4-9672f86c183c
description: Элемент ProgrammaticAccessAllowed указывает, включен ли программный доступ для управляемых данных с правами.
ms.openlocfilehash: 3e7f16a148fe1d81bbf942c098591f108529d456
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59523848"
---
# <a name="programmaticaccessallowed"></a>ProgrammaticAccessAllowed

Элемент **ProgrammaticAccessAllowed** указывает, включен ли программный доступ для управляемых данных с правами. 
  
```XML
<ProgrammaticAccessAllowed> true | false </ProgrammaticAccessAllowed>
```

 **Boolean**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

[RightsManagementLicenseData](rightsmanagementlicensedata.md)
  
## <a name="text-value"></a>Текстовое значение

Значение текста, **истинное** для элемента **ProgrammaticAccessAllowed,** указывает на программный доступ к данным. Значение false **указывает** на то, что данные не доступны программным образом. 
  
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
   

