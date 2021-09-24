---
title: ModifiedEvent
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- ModifiedEvent
api_type:
- schema
ms.assetid: ca1309f4-2df7-4289-811c-75c3db0e7072
description: Элемент ModifiedEvent представляет событие, в котором изменен элемент или папка.
ms.openlocfilehash: 92002c2824168687e6984913dbf46ee85da921e7
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59539361"
---
# <a name="modifiedevent"></a>ModifiedEvent

Элемент **ModifiedEvent** представляет событие, в котором изменен элемент или папка. 
  
```xml
<ModifiedEvent>
   <Watermark/>
   <TimeStamp/>
   <FolderId/>
   <ParentFolderId/>
   <UnreadCount/>
</ModifiedEvent>
```

```xml
<ModifiedEvent>
   <Watermark/>
   <TimeStamp/>
   <ItemId/> 
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
|[Watermark](watermark.md) <br/> |Представляет закладки событий в таблице событий почтового ящика.  <br/> |
|[TimeStamp](timestamp.md) <br/> |Представляет время события измененного элемента или почтового ящика папки.  <br/> |
|[FolderId](folderid.md) <br/> |Представляет идентификатор измененной папки.  <br/> |
|[ItemId](itemid.md) <br/> |Представляет идентификатор измененного элемента.  <br/> |
|[ParentFolderId](parentfolderid.md) <br/> |Представляет идентификатор родительской папки измененного элемента или папки.  <br/> |
|[UnreadCount](unreadcount.md) <br/> |Представляет количество непрочитанные элементы в данной папке.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Уведомление](notification-ex15websvcsotherref.md) <br/> |Содержит сведения о подписке и событиях, произошедших с момента последнего уведомления.  <br/> |
   
## <a name="remarks"></a>Заметки

Для каждой модификации элемента в папке создаются два измененных события. Одно событие имеет отношение к измененным элементам. Другое событие имеет отношение к родительской папке элемента. Это та же папка, в которую была создана подписка. Событие, связанное с папкой, используется для связи потенциального изменения свойства [UnreadCount](unreadcount.md) в папке. 
  
Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Операции подписки](subscribe-operation.md)  
- [Операция GetEvents](getevents-operation.md)  
- [Операция Unsubscribe](unsubscribe-operation.md)

