---
title: RemoveItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RemoveItem
api_type:
- schema
ms.assetid: 766878e3-9007-454f-8501-45139bc5c0e2
description: Элемент RemoveItem представляет объект Response, который используется для удаления элемента собрания при получении сообщения Митингканцеллатион.
ms.openlocfilehash: c0cd5c1f9894287ee78c2f7a65b8f4d3b943414e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467692"
---
# <a name="removeitem"></a>RemoveItem

Элемент **RemoveItem** представляет объект Response, который используется для удаления элемента собрания при получении сообщения митингканцеллатион. 
  
```xml
<RemoveItem ObjectName="">
   <ReferenceItemId/>
</RemoveItem>
```

 **ремовеитемтипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|**ObjectName** <br/> |Представляет имя класса объекта ответа RemoveItem в виде строки на английском языке.  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[референцеитемид](referenceitemid.md) <br/> |Определяет элемент, на который ссылается объект ответа RemoveItem.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Элементы (Нонемптяррайофаллитемстипе)](items-nonemptyarrayofallitemstype.md) <br/> |Содержит массив элементов для создания в папке, определяемой элементом [ParentFolderId (таржетфолдеридтипе)](parentfolderid-targetfolderidtype.md) .  <br/> |
|[респонсеобжектс](responseobjects.md) <br/> |Содержит коллекцию всех объектов ответа, связанных с элементом в хранилище Exchange.  <br/> |
   
## <a name="remarks"></a>Примечания

 **RemoveItem** является допустимым только для [митингканцеллатион](meetingcancellation.md). В противном случае возникает ошибка.
  
> [!NOTE]
> [ItemClass](itemclass.md) для отмены собрания — IPM. Schedule. Meeting. Canceled. 
  
Чтобы удалить объект [свойство meetingrequest](meetingrequest.md) и связанный с ним [Календаритем](calendaritem.md), вместо **RemoveItem**используйте объект отклика [деклинеитем](declineitem.md) .
  
 **RemoveItem** не поддерживается для делегированного доступа. 
  
Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

