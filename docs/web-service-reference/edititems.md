---
title: EditItems
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- EditItems
api_type:
- schema
ms.assetid: 1cb14493-c999-4d66-b82c-ecb410dc1c00
description: Элемент EditItems указывает, какие элементы в папке пользователь имеет разрешение на редактирование. Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).
ms.openlocfilehash: 51c038cf93d43fffe785b1946a52c8bcb5c1c302
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59538263"
---
# <a name="edititems"></a>EditItems

Элемент **EditItems** указывает, какие элементы в папке пользователь имеет разрешение на редактирование. Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1). 
  
```xml
<EditItems>None or Owned or All</EditItems>
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

В следующей таблице перечислены возможные значения элемента **EditItems.** 
  
**Текстовые значения элементов EditItems**

|**Значение**|**Описание**|
|:-----|:-----|
|Нет  <br/> |Указывает, что пользователь не имеет разрешения на редактирование элементов в папке.  <br/> |
|Owned  <br/> |Указывает, что у пользователя есть разрешение на редактирование элементов, которые принадлежат пользователю в папке.  <br/> |
|Все  <br/> |Указывает, что у пользователя есть разрешение на редактирование всех элементов в папке.  <br/> |
   
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

