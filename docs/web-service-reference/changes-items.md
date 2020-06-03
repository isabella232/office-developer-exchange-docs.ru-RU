---
title: Изменения (элементы)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Changes
api_type:
- schema
ms.assetid: d3139fef-0455-4b89-babd-5d6783b50a58
description: Элемент Changes содержит массив последовательности типов изменений, которые представляют типы различий между элементами на клиенте и элементами на сервере Exchange.
ms.openlocfilehash: 6fda7b5602f172bae84ad7b211db2811def4f883
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463267"
---
# <a name="changes-items"></a>Изменения (элементы)

Элемент **Changes** содержит массив последовательности типов изменений, которые представляют типы различий между элементами на клиенте и элементами на сервере Exchange. 
  
[синкфолдеритемсреспонсе](syncfolderitemsresponse.md)
  
[респонсемессажес](responsemessages.md)
  
[синкфолдеритемсреспонсемессаже](syncfolderitemsresponsemessage.md)
  
[Изменения (элементы)](changes-items.md)
  
```xml
<Changes>
   <Create/>
   <Update/>
   <Delete/>
</Changes>
```

 **синкфолдеритемсчанжестипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Create (Итемсинк)](create-itemsync.md) <br/> |Определяет один элемент, который необходимо создать в локальном хранилище клиента.  <br/> |
|[Обновление (Итемсинк)](update-itemsync.md) <br/> |Определяет один элемент для обновления в локальном хранилище клиента.  <br/> |
|[Delete (Итемсинк)](delete-itemsync.md) <br/> |Определяет один элемент, который необходимо удалить в локальном хранилище клиента.  <br/> |
|[реадфлагчанже](readflagchange.md) <br/> |Возвращается в ответах [операции SyncFolderItems](syncfolderitems-operation.md) при чтении элемента. Это свойство доступно только для чтения.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[синкфолдеритемсреспонсемессаже](syncfolderitemsresponsemessage.md) <br/> |Содержит состояние и результат запроса [операции SyncFolderItems](syncfolderitems-operation.md) .  <br/> |
   
## <a name="remarks"></a>Примечания

Схема, описывающая этот элемент, находится в виртуальном каталоге EWS компьютера под управлением Microsoft Exchange Server 2010, на котором установлена роль сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция SyncFolderItems](syncfolderitems-operation.md)


- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

