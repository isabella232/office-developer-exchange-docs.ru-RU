---
title: моведевент
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MovedEvent
api_type:
- schema
ms.assetid: 572f8b40-dfa8-47bc-b0c1-e1a7138506fd
description: Элемент Моведевент представляет событие, в котором элемент или папка перемещаются из одной родительской папки в другую.
ms.openlocfilehash: 1f8fb57dba7edb769fe0dd658d89c032dccf8c5f
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530410"
---
# <a name="movedevent"></a>моведевент

Элемент **моведевент** представляет событие, в котором элемент или папка перемещаются из одной родительской папки в другую. 
  
```xml
<MovedEvent>
   <Watermark/>
   <TimeStamp/>
   <ItemId/>
   <ParentFolderId/>
   <OldItemId/>
   <OldParentFolderId/>
</MovedEvent>
```

```xml
<MovedEvent>
   <Watermark/>
   <TimeStamp/>
   <FolderId/>
   <ParentFolderId/>
   <OldFolderId/>
   <OldParentFolderId/>
</MovedEvent>
```


**моведкопиедевенттипе**

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Watermark](watermark.md) <br/> |Представляет закладку Events в таблице событий почтовых ящиков.  <br/> |
|[Метка времени](timestamp.md) <br/> |Представляет метку времени для события перемещения элемента/почтового ящика папки.  <br/> |
|[FolderId](folderid.md) <br/> |Представляет идентификатор перемещенной папки.  <br/> |
|[Идентификатор](itemid.md) <br/> |Представляет идентификатор перемещенного элемента.  <br/> |
|[ParentFolderId](parentfolderid.md) <br/> |Представляет идентификатор папки, содержащей перемещенный элемент или папку.  <br/> |
|[олдфолдерид](oldfolderid.md) <br/> |Содержит идентификатор исходной папки перед ее перемещением или копированием.  <br/> |
|[олдитемид](olditemid.md) <br/> |Содержит уникальный идентификатор исходного элемента перед его перемещением.  <br/> |
|[олдпарентфолдерид](oldparentfolderid.md) <br/> |Содержит идентификатор исходной родительской папки для перемещенного элемента или папки.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Уведомление](notification-ex15websvcsotherref.md) <br/> |Содержит сведения о подписке и событиях, произошедших с момента последнего уведомления.  <br/> |
   
## <a name="remarks"></a>Примечания

Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Операции подписки](subscribe-operation.md) 
- [Операция GetEvents](getevents-operation.md) 
- [Операция по отмене подписки](unsubscribe-operation.md)

