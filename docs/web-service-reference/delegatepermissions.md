---
title: делегатепермиссионс
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DelegatePermissions
api_type:
- schema
ms.assetid: 292badc7-bab3-4368-9d7c-9a8b7edb279b
description: Элемент Делегатепермиссионс содержит параметры делегированного уровня разрешений для пользователя. Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).
ms.openlocfilehash: 319592b6c3386a07b3094115c335c7fb8ffe1130
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762008"
---
# <a name="delegatepermissions"></a>делегатепермиссионс

Элемент **делегатепермиссионс** содержит параметры делегированного уровня разрешений для пользователя. Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1). 
  
```xml
<DelegatePermissions>
   <CalendarFolderPermissionLevel/>
   <TasksFolderPermissionLevel/>
   <InboxFolderPermissionLevel/>
   <ContactsFolderPermissionLevel/>
   <NotesFolderPermissionLevel/>
   <JournalFolderPermissionLevel/>
</DelegatePermissions>
```

**делегатепермиссионстипе**

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[календарфолдерпермиссионлевел](calendarfolderpermissionlevel.md) <br/> |Содержит разрешения для папки календаря по умолчанию. Этот элемент появился в Exchange 2007 с пакетом обновления 1.  <br/> |
|[тасксфолдерпермиссионлевел](tasksfolderpermissionlevel.md) <br/> |Содержит разрешения для папки задач по умолчанию. Этот элемент появился в Exchange 2007 с пакетом обновления 1.  <br/> |
|[инбоксфолдерпермиссионлевел](inboxfolderpermissionlevel.md) <br/> |Содержит разрешения для папки "Входящие", используемой по умолчанию. Этот элемент появился в Exchange 2007 с пакетом обновления 1.  <br/> |
|[контактсфолдерпермиссионлевел](contactsfolderpermissionlevel.md) <br/> |Содержит разрешения для папки "Контакты" по умолчанию. Этот элемент появился в Exchange 2007 с пакетом обновления 1.  <br/> |
|[нотесфолдерпермиссионлевел](notesfolderpermissionlevel.md) <br/> |Содержит разрешения для папки заметок по умолчанию. Этот элемент появился в Exchange 2007 с пакетом обновления 1.  <br/> |
|[жаурналфолдерпермиссионлевел](journalfolderpermissionlevel.md) <br/> |Содержит разрешения для папки журнала по умолчанию. Этот элемент появился в Exchange 2007 с пакетом обновления 1.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[делегатеусер](delegateuser.md) <br/> |Определяет одного делегата для добавления или обновления в почтовом ящике. Этот элемент появился в Exchange 2007 с пакетом обновления 1.  <br/> |
   
## <a name="remarks"></a>Примечания

Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Операция AddDelegate](adddelegate-operation.md) 
- [Операция UpdateDelegate](updatedelegate-operation.md)
- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)
- [Добавление делегатов](http://msdn.microsoft.com/library/3a744150-66a3-4a13-9433-793603ba5038%28Office.15%29.aspx)

