---
title: ModifiedEvent
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ModifiedEvent
api_type:
- schema
ms.assetid: ca1309f4-2df7-4289-811c-75c3db0e7072
description: ModifiedEvent элемент представляет событие, в котором изменения элемента или папки.
ms.openlocfilehash: fb464fb0a270d8ca7d33d40e5425e260970b2f1e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834482"
---
# <a name="modifiedevent"></a>ModifiedEvent

**ModifiedEvent** элемент представляет событие, в котором изменения элемента или папки. 
  
```xml
<ModifiedEvent>
   <Watermark/>
   <TimeStamp/>
   <FolderId/>
   <ParentFolderId/>
   <UnreadCount/>
</ModifiedEvent>
```

 **ModifiedEventType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Водяной знак](watermark.md) <br/> |Представляет закладку события в таблице событий почтового ящика.  <br/> |
|[Метка времени](timestamp.md) <br/> |Представляет отметки времени событии изменения элемента или папки почтового ящика.  <br/> |
|[FolderId](folderid.md) <br/> |Представляет идентификатор измененного папки.  <br/> |
|[Идентификатор элемента](itemid.md) <br/> |Представляет идентификатор измененного элемента.  <br/> |
|[ParentFolderId](parentfolderid.md) <br/> |Представляет идентификатор родительской папки изменения элемента или папки.  <br/> |
|[UnreadCount](unreadcount.md) <br/> |Представляет количество непрочитанных элементов в указанной папке.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Уведомление](notification-ex15websvcsotherref.md) <br/> |Содержит сведения о подписке и события, произошедшие с момента последнего уведомления.  <br/> |
   
## <a name="remarks"></a>Замечания

При каждом изменении элемента в папке создаются два события изменения. Одно событие предназначенных для изменения элемента. Другие события относится к папке родительского элемента. Это ту же папку, которая была создана подписка. Событие, связанное с папкой используется для взаимодействия потенциальных изменение свойства [UnreadCount](unreadcount.md) в общей папке. 
  
Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операции подписки](subscribe-operation.md)
  
[Операция GetEvents](getevents-operation.md)
  
[Отписаться операции](unsubscribe-operation.md)

