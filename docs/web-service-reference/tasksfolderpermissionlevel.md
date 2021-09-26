---
title: TasksFolderPermissionLevel
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- TasksFolderPermissionLevel
api_type:
- schema
ms.assetid: 0f70b79b-3443-4048-b410-692d4e2464fc
description: Элемент TasksFolderPermissionLevel содержит разрешения для папки Задачи по умолчанию. Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).
ms.openlocfilehash: 991b13f9a9f95805b13312712b1f6c5941033c46
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59543872"
---
# <a name="tasksfolderpermissionlevel"></a>TasksFolderPermissionLevel

Элемент **TasksFolderPermissionLevel** содержит разрешения для папки Задачи по умолчанию. Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1). 
  
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
|[DelegatePermissions](delegatepermissions.md) <br/> |Содержит параметры уровня разрешений делегата для пользователя. Этот элемент появился в Exchange 2007 с пакетом обновления 1.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

В следующей таблице перечислены текстовые значения, которые представляют уровни разрешений.
  
**Текстовые значения уровня разрешений**

|**Уровень разрешений**|**Описание**|
|:-----|:-----|
|Нет  <br/> |У пользователя делегирования нет разрешений доступа к папке Задачи.  <br/> |
|Reviewer  <br/> |Пользователь делегирования может читать элементы в папке Задачи.  <br/> |
|Автор  <br/> |Пользователь делегирования может читать и создавать элементы в папке Задачи.  <br/> |
|Редактор  <br/> |Пользователь делегирования может читать, создавать и изменять элементы в папке Задачи.  <br/> |
|Пользовательский сервер  <br/> |Пользователь делегирования имеет пользовательские разрешения доступа к папке Задачи.  <br/> |
   
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

- [Операция AddDelegate](adddelegate-operation.md)
- [Операция UpdateDelegate](updatedelegate-operation.md)
- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)
- [Добавление делегатов](https://msdn.microsoft.com/library/3a744150-66a3-4a13-9433-793603ba5038%28Office.15%29.aspx)

