---
title: SharedFolderId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- SharedFolderId
api_type:
- schema
ms.assetid: 21181ba3-9626-4284-9717-0b1c16948e8f
description: Элемент SharedFolderId представляет идентификатор общей папки локального идентификатора папок, для которого должен быть возвращен запрос на операцию GetSharingFolder.
ms.openlocfilehash: 7e47ba49abed99bdb3cfd00eb43d2ef276d4ef37
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59545974"
---
# <a name="sharedfolderid"></a>SharedFolderId

Элемент **SharedFolderId** представляет идентификатор общей папки локального идентификатора папок, для которого должен быть возвращен запрос на операцию [GetSharingFolder.](getsharingfolder-operation.md) 
  
```xml
<SharedFolderId/>
```

 **NonEmptyStringType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[GetSharingFolder](getsharingfolder.md) <br/> |Определяет запрос для получения локального идентификатора папки указанной общей папки.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение представляет строку, представляющую идентификатор общей папки, локальный идентификатор папки, для которого должен быть возвращен запрос на операцию [GetSharingFolder.](getsharingfolder-operation.md) 
  
## <a name="remarks"></a>Заметки

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция GetSharingFolder](getsharingfolder-operation.md)


- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

