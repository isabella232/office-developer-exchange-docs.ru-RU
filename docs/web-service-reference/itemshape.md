---
title: итемшапе
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
description: Элемент Итемшапе определяет набор свойств, возвращаемых операцией GetItem, операцией FindItem или ответом операции SyncFolderItems.
ms.openlocfilehash: ffb666ee331b55a4f04cad076c705e4bec980e03
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458126"
---
# <a name="itemshape"></a>итемшапе

Элемент **итемшапе** определяет набор свойств, возвращаемых [операцией GetItem](getitem-operation.md), [операцией FindItem](finditem-operation.md)или ответом [операции SyncFolderItems](syncfolderitems-operation.md) . 
  
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

 **итемреспонсешапетипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[басешапе](baseshape.md) <br/> |Определяет базовую конфигурацию свойств, возвращаемых в ответе элемента или папки.  <br/> |
|[инклудемимеконтент](includemimecontent.md) <br/> |Указывает, будет ли в ответе возвращено содержимое MIME для элемента с многоцелевыми почтовыми расширениями.  <br/> |
|[BodyType](bodytype.md) <br/> |Определяет способ форматирования основного текста в отклике.  <br/> |
|[ConvertHtmlCodePageToUTF8](converthtmlcodepagetoutf8.md) <br/> |Указывает, преобразуется ли текст HTML элемента в формат UTF8.  <br/> |
|[филтерхтмлконтент](filterhtmlcontent.md) <br/> |Указывает, включена ли фильтрация HTML-содержимого.  <br/> |
|[аддитионалпропертиес](additionalproperties.md) <br/> |Определяет дополнительные свойства, возвращаемые в ответе.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[GetItem](getitem.md) <br/> |Определяет запрос на извлечение элементов из почтового ящика в хранилище Exchange.  <br/> Ниже приведено выражение XPath для этого элемента:  <br/>  `/GetItem` <br/> |
|[FindItem](finditem.md) <br/> |Определяет запрос на поиск всех элементов, которые содержатся в папке.  <br/> Ниже приведено выражение XPath для этого элемента:  <br/>  `/FindItem` <br/> |
|[SyncFolderItems](syncfolderitems.md) <br/> |Определяет запрос на синхронизацию элементов в папке хранилища Exchange.  <br/> Ниже приведено выражение XPath для этого элемента:  <br/>  `/SyncFolderItems` <br/> |
   
## <a name="text-value"></a>Текстовое значение

Нет.
  
## <a name="remarks"></a>Примечания

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция GetItem](getitem-operation.md)
  
[Операция FindItem](finditem-operation.md)
  
[Операция SyncFolderItems](syncfolderitems-operation.md)


- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

