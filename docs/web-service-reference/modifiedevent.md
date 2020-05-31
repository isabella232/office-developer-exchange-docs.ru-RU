---
title: модифиедевент
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
description: Элемент Модифиедевент представляет событие, в котором изменяется элемент или папка.
ms.openlocfilehash: 2e9fb870396d49efb5cdf307a502b4111c2e507e
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/28/2018
ms.locfileid: "21353814"
---
# <a name="modifiedevent"></a>модифиедевент

Элемент **модифиедевент** представляет событие, в котором изменяется элемент или папка. 
  
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

**модифиедевенттипе**

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Watermark](watermark.md) <br/> |Представляет закладку события в таблице событий почтовых ящиков.  <br/> |
|[Метка времени](timestamp.md) <br/> |Представляет метку времени для измененного события элемента или почтового ящика папки.  <br/> |
|[FolderId](folderid.md) <br/> |Представляет идентификатор измененной папки.  <br/> |
|[Идентификатор](itemid.md) <br/> |Представляет идентификатор измененного элемента.  <br/> |
|[ParentFolderId](parentfolderid.md) <br/> |Представляет идентификатор родительской папки измененного элемента или папки.  <br/> |
|[унреадкаунт](unreadcount.md) <br/> |Представляет количество непрочитанных элементов в заданной папке.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Уведомление](notification-ex15websvcsotherref.md) <br/> |Содержит сведения о подписке и событиях, произошедших с момента последнего уведомления.  <br/> |
   
## <a name="remarks"></a>Примечания

Для каждого изменения элемента в папке создается два измененных события. Одно событие относится к измененному элементу. Другое событие относится к родительской папке элемента. Это та же папка, в которой была создана подписка. Событие, связанное с папкой, используется для передачи потенциального изменения свойству [унреадкаунт](unreadcount.md) в папке. 
  
Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Операции подписки](subscribe-operation.md)  
- [Операция GetEvents](getevents-operation.md)  
- [Операция по отмене подписки](unsubscribe-operation.md)

