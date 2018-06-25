---
title: UserIds
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UserIds
api_type:
- schema
ms.assetid: 78a09c3a-1646-4c55-95a2-1109fb11e1c6
description: UserIds, который содержит массив делегирование пользователей, позволяющее получить или удалить из почтового ящика участника. Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).
ms.openlocfilehash: 277ae96fdbc30f1b39ef20553e10ff1de3ff7a8b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19840424"
---
# <a name="userids"></a>UserIds

Элемент **UserIds** содержит массив делегат пользователям получить или удалить из почтового ящика участника. Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1). 
  
```xml
<UserIds>
   <UserId/>
</UserIds>
```

 **ArrayOfUserIdType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Идентификатор пользователя](userid.md) <br/> |Определяет делегат для получения или удалить из почтового ящика участника. Этот элемент появился в Exchange 2007 с пакетом обновления 1.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[GetDelegate](getdelegate.md) <br/> |Определяет запрос на получение сведений о делегатов к почтовому ящику. Этот элемент появился в Exchange 2007 с пакетом обновления 1.  <br/> |
|[RemoveDelegate](removedelegate.md) <br/> |Определяет запрос для удаления делегатов из почтового ящика. Этот элемент появился в Exchange 2007 с пакетом обновления 1.  <br/> |
   
## <a name="remarks"></a>Замечания

Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция GetDelegate](getdelegate-operation.md)
  
[Операция RemoveDelegate](removedelegate-operation.md)


- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

