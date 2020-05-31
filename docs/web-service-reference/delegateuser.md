---
title: делегатеусер
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DelegateUser
api_type:
- schema
ms.assetid: aac4e74e-f69b-4c41-a0c9-489610330fbf
description: Элемент Делегатеусер определяет одного делегата для добавления или обновления в почтовом ящике или делегата, возвращенного в ответе управления представителями. Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).
ms.openlocfilehash: 72ddc313a5a76cd0345918cad63b7775ff85026b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762012"
---
# <a name="delegateuser"></a>делегатеусер

Элемент **делегатеусер** определяет одного делегата для добавления или обновления в почтовом ящике или делегата, возвращенного в ответе управления представителями. Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1). 
  
```xml
<DelegateUser>
   <UserId/>
   <DelegatePermissions/>
   <ReceiveCopiesOfMeetingMessages/>
   <ViewPrivateItems/>
</DelegateUser>
```

**делегатеусертипе**

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[UserId](userid.md) <br/> |Определяет делегата. Этот элемент появился в Exchange 2007 с пакетом обновления 1.  <br/> |
|[делегатепермиссионс](delegatepermissions.md) <br/> |Содержит параметры уровня разрешений делегата. Этот элемент появился в Exchange 2007 с пакетом обновления 1.  <br/> |
|[рецеивекопиесофмитингмессажес](receivecopiesofmeetingmessages.md) <br/> |Указывает, получает ли делегат копии сообщений, связанных с собранием, которые адресованы участнику. Этот элемент появился в Exchange 2007 с пакетом обновления 1.  <br/> |
|[виевприватеитемс](viewprivateitems.md) <br/> |Указывает, имеет ли представитель разрешение на просмотр частных элементов календаря в почтовом ящике субъекта. Этот элемент появился в Exchange 2007 с пакетом обновления 1.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[делегатеусерс](delegateusers.md) <br/> |Содержит идентификаторы делегатов, которые добавляются или обновляются в почтовом ящике.  <br/> |
|[делегатеусерреспонсемессажетипе](delegateuserresponsemessagetype.md) <br/> |Содержит сообщения ответа для операций управления делегированием. Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).  <br/> |
   
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

