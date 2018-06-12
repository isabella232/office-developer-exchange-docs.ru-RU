---
title: ItemShape
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ItemShape
api_type:
- schema
ms.assetid: c5604161-bbc0-40bc-ad75-ff7e837d745f
description: Элемент ItemShape определяет набор свойств для возвращения операции GetItem, FindItem операции или операции SyncFolderItems ответа.
ms.openlocfilehash: 95174a85a8fa05cb2612e1289d46c8db32b6e052
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19834191"
---
# <a name="itemshape"></a>ItemShape

Элемент **ItemShape** определяет набор свойств, возвращаемых в ответе [операции GetItem](getitem-operation.md), [FindItem операции](finditem-operation.md)или [операции SyncFolderItems](syncfolderitems-operation.md) . 
  
```XML
<ItemShape>
   <BaseShape/>
   <IncludeMimeContent/>
   <BodyType/>
   <FilterHtmlContent/>
   <ConvertHtmlCodePageToUTF8/>
   <AdditionalProperties/>
</ItemShape>
```

 **ItemResponseShapeType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[BaseShape](baseshape.md) <br/> |Определяет базовую конфигурацию свойства, возвращаемые в элемент или папку ответ.  <br/> |
|[IncludeMimeContent](includemimecontent.md) <br/> |Указывает, является ли содержимое Multipurpose Internet Mail Extensions (MIME) элементов возвращаемого в ответе.  <br/> |
|[BodyType](bodytype.md) <br/> |Определяет способ форматирования основного текста в ответе.  <br/> |
|[ConvertHtmlCodePageToUTF8](converthtmlcodepagetoutf8.md) <br/> |Указывает, будет ли HTML-тела элемента преобразуется в UTF8.  <br/> |
|[FilterHtmlContent](filterhtmlcontent.md) <br/> |Указывает, включена ли фильтрация содержимого в формате HTML.  <br/> |
|[AdditionalProperties](additionalproperties.md) <br/> |Определяет дополнительные свойства, возвращаемые в ответе.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[GetItem](getitem.md) <br/> |Определяет запрос на получение элементов из почтового ящика в хранилище Exchange.  <br/> Ниже приведен выражение XPath для этого элемента.  <br/>  `/GetItem` <br/> |
|[FindItem](finditem.md) <br/> |Определяет запрос для поиска всех элементов, содержащихся в папке.  <br/> Ниже приведен выражение XPath для этого элемента.  <br/>  `/FindItem` <br/> |
|[SyncFolderItems](syncfolderitems.md) <br/> |Определяет запрос для синхронизации элементов в папке хранилища Exchange.  <br/> Ниже приведен выражение XPath для этого элемента.  <br/>  `/SyncFolderItems` <br/> |
   
## <a name="text-value"></a>Текстовое значение

Нет.
  
## <a name="remarks"></a>Замечания

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[GetItem Operation](getitem-operation.md)
  
[FindItem Operation](finditem-operation.md)
  
[Операция SyncFolderItems](syncfolderitems-operation.md)


- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

