---
title: JournalFolderPermissionLevel
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- JournalFolderPermissionLevel
api_type:
- schema
ms.assetid: 564525fa-cd95-4c1a-9d6c-3806be664579
description: Элемент JournalFolderPermissionLevel содержит разрешения для папки Journal по умолчанию. Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).
ms.openlocfilehash: 0237048e61fbae12a1341cef33e5ca30ebc0c838
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59524968"
---
# <a name="journalfolderpermissionlevel"></a>JournalFolderPermissionLevel

Элемент **JournalFolderPermissionLevel содержит** разрешения для папки Journal по умолчанию. Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1). 
  
```xml
<JournalFolderPermissionLevel>
   None or Editor or Reviewer or Author or Custom
</JournalFolderPermissionLevel>
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
|Нет  <br/> |У пользователя делегирования нет разрешений на доступ к папке Journal.  <br/> |
|Reviewer  <br/> |Пользователь делегирования может читать элементы в папке Journal.  <br/> |
|Автор  <br/> |Пользователь делегирования может читать и создавать элементы в папке Журнал.  <br/> |
|Редактор  <br/> |Пользователь делегирования может читать, создавать и изменять элементы в папке Journal.  <br/> |
|Пользовательский сервер  <br/> |Пользователь делегирования имеет настраиваемые разрешения доступа к папке Journal.  <br/> |
   
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



[Операция AddDelegate](adddelegate-operation.md)
  
[Операция UpdateDelegate](updatedelegate-operation.md)


- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)


[Добавление делегатов](https://msdn.microsoft.com/library/3a744150-66a3-4a13-9433-793603ba5038%28Office.15%29.aspx)

