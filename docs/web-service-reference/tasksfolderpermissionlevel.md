---
title: TasksFolderPermissionLevel
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- TasksFolderPermissionLevel
api_type:
- schema
ms.assetid: 0f70b79b-3443-4048-b410-692d4e2464fc
description: Элемент TasksFolderPermissionLevel содержит разрешения для папки задач по умолчанию. Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).
ms.openlocfilehash: 49807896f9175bafbef106c41d1c9dff8f6178c4
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19840137"
---
# <a name="tasksfolderpermissionlevel"></a>TasksFolderPermissionLevel

Элемент **TasksFolderPermissionLevel** содержит разрешения для папки задач по умолчанию. Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1). 
  
```xml
<TasksFolderPermissionLevel>
   None or Editor or Reviewer or Author or Custom
</TasksFolderPermissionLevel>
```

**DelegateFolderPermissionLevelType**

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[DelegatePermissions](delegatepermissions.md) <br/> |Содержит параметры уровня разрешений делегат для пользователя. Этот элемент появился в Exchange 2007 с пакетом обновления 1.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

В следующей таблице перечислены текстовые значения, которые представляют уровни разрешений.
  
**Разрешение уровня текстовые значения**

|**Уровень разрешений**|**Описание**|
|:-----|:-----|
|Нет  <br/> |Делегата не имеет доступа к разрешений на папку.  <br/> |
|Редактор  <br/> |Делегат пользователь может читать элементы в папке задач.  <br/> |
|Author  <br/> |Делегата можно читать и создавать элементы в папке заданий.  <br/> |
|Редактор  <br/> |Делегата могут читать, создавать и изменять элементы в папке задач.  <br/> |
|Пользовательский сервер  <br/> |Делегата имеет пользовательские разрешения доступа к папке задачи.  <br/> |
   
## <a name="remarks"></a>Замечания

Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Операция AddDelegate](adddelegate-operation.md)
- [Операция UpdateDelegate](updatedelegate-operation.md)
- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)
- [Добавление делегатов](http://msdn.microsoft.com/library/3a744150-66a3-4a13-9433-793603ba5038%28Office.15%29.aspx)

