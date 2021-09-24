---
title: IsManagedFoldersRoot
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- IsManagedFoldersRoot
api_type:
- schema
ms.assetid: 00823fb9-bf8b-49bb-8e1b-d698c6d4063f
description: Элемент IsManagedFoldersRoot указывает, является ли управляемый папка корнем для всех управляемых папок.
ms.openlocfilehash: 85c806f1bb3f3613f8faf33b763e2a8c20f5ef40
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59539495"
---
# <a name="ismanagedfoldersroot"></a>IsManagedFoldersRoot

Элемент **IsManagedFoldersRoot** указывает, является ли управляемый папка корнем для всех управляемых папок. 
  
```xml
<IsManagedFoldersRoot/>
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
|[ManagedFolderInformation](managedfolderinformation.md) <br/> |Содержит сведения об управляемой папке.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Если этот элемент присутствует, необходимо текстовое значение, представляю которое представляет значение Boolean. Значение true **указывает,** что папка является корневой папкой управляемой папки; значение false **указывает,** что папка не является корневой папкой управляемой папки. 
  
## <a name="remarks"></a>Заметки

Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

