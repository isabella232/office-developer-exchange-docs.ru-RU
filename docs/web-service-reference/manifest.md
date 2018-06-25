---
title: Манифест
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: af0d7435-fef6-4f0d-bd22-00e3fa576315
description: Элемент манифеста содержит файла манифеста приложения в кодировке base64.
ms.openlocfilehash: 7388e40a96a082666519d1c67af5b218b2b9ab01
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834343"
---
# <a name="manifest"></a>Манифест

Элемент **манифеста** содержит файла манифеста приложения в кодировке base64. 
  
```XML
<Manifest></Manifest>
```

 **base64Binary**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

[Манифесты](manifests.md) | [InstallApp](installapp.md) | [ClientExtension](clientextension.md)
  
## <a name="text-value"></a>Текстовое значение

Текстовое значение манифеста элемента — это ASCII представление base64 двоичной кодировке файла манифеста приложения клиента.
  
## <a name="remarks"></a>Замечания

Этот элемент появился в Exchange Server 2013.
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  

