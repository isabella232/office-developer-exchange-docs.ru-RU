---
title: DeleteItems
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- DeleteItems
api_type:
- schema
ms.assetid: a5898bfc-f5ae-451d-9713-3e55864c690c
description: Элемент DeleteItems указывает, какие элементы в папке пользователь имеет разрешение на удаление. Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).
ms.openlocfilehash: d41e44c3cc0996ab5933eafaf1087cf30d7944a3
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59546674"
---
# <a name="deleteitems"></a>DeleteItems

Элемент **DeleteItems** указывает, какие элементы в папке пользователь имеет разрешение на удаление. Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1). 
  
```xml
<DeleteItems>None or Owned or All</DeleteItems>
```

 **PermissionActionType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Разрешение](permission.md) <br/> |Определяет доступ пользователя к папке. Этот элемент появился в Exchange 2007 с пакетом обновления 1.  <br/> |
|[CalendarPermission](calendarpermission.md) <br/> |Определяет доступ пользователя к папке календаря. Этот элемент появился в Exchange 2007 с пакетом обновления 1.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

В следующей таблице перечислены возможные значения элемента **DeleteItems.** 
  
**Текстовые значения элементов DeleteItems**

|**Значение**|**Описание**|
|:-----|:-----|
|Нет  <br/> |Указывает, что пользователь не имеет разрешения на удаление элементов в папке.  <br/> |
|Owned  <br/> |Указывает, что у пользователя есть разрешение на удаление элементов, которые принадлежат пользователю в папке.  <br/> |
|Все  <br/> |Указывает, что у пользователя есть разрешение на удаление всех элементов в папке.  <br/> |
   
## <a name="remarks"></a>Заметки

Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)
- [Setting Folder-Level Permissions](https://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

