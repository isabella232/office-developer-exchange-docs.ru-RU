---
title: копиедевент
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CopiedEvent
api_type:
- schema
ms.assetid: 82f2fcac-deaa-4ff8-801f-4fe28d8a19f5
description: Элемент Копиедевент представляет событие, в котором копируется элемент или папка.
ms.openlocfilehash: 928910ddbe0bf1e48549d1665ab373f7382366d1
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529247"
---
# <a name="copiedevent"></a>копиедевент

Элемент **копиедевент** представляет событие, в котором копируется элемент или папка. 
  
```xml
<CopiedEvent>
   <Watermark/>
   <TimeStamp/>
   <FolderId/>
   <ParentFolderId/>
   <OldFolderId/>
   <OldParentFolderId/>
</CopiedEvent>
```

```xml
<CopiedEvent>
   <Watermark/>
   <TimeStamp/>
   <ItemId/>
   <ParentFolderId/>
   <OldFolderId/>
   <OldParentFolderId/>
</CopiedEvent>
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
|[Метка времени](timestamp.md) <br/> |Представляет метку времени события копирования элемента или папки почтового ящика.  <br/> |
|[FolderId](folderid.md) <br/> |Представляет идентификатор папки.  <br/> |
|[Идентификатор](itemid.md) <br/> |Представляет идентификатор элемента.  <br/> |
|[ParentFolderId](parentfolderid.md) <br/> |Представляет идентификатор папки, содержащей копию.  <br/> |
|[олдфолдерид](oldfolderid.md) <br/> |Представляет идентификатор исходной папки перед ее копированием.  <br/> |
|[олдитемид](olditemid.md) <br/> |Содержит уникальный идентификатор исходного элемента перед его копированием.  <br/> |
|[олдпарентфолдерид](oldparentfolderid.md) <br/> |Содержит идентификатор исходной родительской папки для скопированного элемента или папки.  <br/> |
   
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
- [Использование подписок по запросу](https://msdn.microsoft.com/library/f956bc0e-2b25-4613-966b-54c65456897c%28Office.15%29.aspx) 
- [Пример приложения для push-уведомлений](https://msdn.microsoft.com/library/db1f8523-fa44-483f-bdb6-ab5939b52eee%28Office.15%29.aspx)

