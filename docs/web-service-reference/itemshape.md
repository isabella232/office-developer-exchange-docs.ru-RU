---
title: ItemShape
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- ItemShape
api_type:
- schema
ms.assetid: c5604161-bbc0-40bc-ad75-ff7e837d745f
description: Элемент ItemShape определяет набор свойств, возвращаемого в операции GetItem, операции FindItem или syncFolderItems.
ms.openlocfilehash: d6cc1efc85a8a22e12f2a3616fe949b72b3bba33
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59519396"
---
# <a name="itemshape"></a>ItemShape

Элемент **ItemShape** определяет набор свойств, возвращаемого в операции [GetItem, операции FindItem](finditem-operation.md)или [syncFolderItems.](syncfolderitems-operation.md) [](getitem-operation.md) 
  
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
|[BaseShape](baseshape.md) <br/> |Определяет базовую конфигурацию свойств, возвращаемую в ответ элемента или папки.  <br/> |
|[IncludeMimeContent](includemimecontent.md) <br/> |Указывает, возвращается ли в ответ многоцелевой контент расширения интернет-почты (MIME) элемента.  <br/> |
|[BodyType](bodytype.md) <br/> |Определяет форматирование текста тела в ответе.  <br/> |
|[ConvertHtmlCodePageToUTF8](converthtmlcodepagetoutf8.md) <br/> |Указывает, преобразуется ли тело HTML-элемента в UTF8.  <br/> |
|[FilterHtmlContent](filterhtmlcontent.md) <br/> |Указывает, включена ли фильтрация контента HTML.  <br/> |
|[AdditionalProperties](additionalproperties.md) <br/> |Определяет дополнительные свойства, возвращаемые в ответ.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[GetItem](getitem.md) <br/> |Определяет запрос на извлечение элементов из почтового ящика в Exchange магазине.  <br/> Ниже приводится выражение XPath к этому элементу:  <br/>  `/GetItem` <br/> |
|[FindItem](finditem.md) <br/> |Определяет запрос на поиск всех элементов, содержащихся в папке.  <br/> Ниже приводится выражение XPath к этому элементу:  <br/>  `/FindItem` <br/> |
|[SyncFolderItems](syncfolderitems.md) <br/> |Определяет запрос на синхронизацию элементов в Exchange папке.  <br/> Ниже приводится выражение XPath к этому элементу:  <br/>  `/SyncFolderItems` <br/> |
   
## <a name="text-value"></a>Текстовое значение

Нет.
  
## <a name="remarks"></a>Заметки

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция GetItem](getitem-operation.md)
  
[Операция FindItem](finditem-operation.md)
  
[Операция SyncFolderItems](syncfolderitems-operation.md)


- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

