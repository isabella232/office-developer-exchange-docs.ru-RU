---
title: Изменения (иерархия)
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
ms.assetid: 918a0d1f-90a5-4eef-9592-07e15bef94e6
description: Элемент Changes содержит упорядоченный массив типов изменений, представляющий тип различий между папками на клиенте и папками на компьютере, на котором работает Microsoft Exchange Server 2007.
ms.openlocfilehash: a296d87f23e85d42b4c8c858e92eddfb586a8324
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463274"
---
# <a name="changes-hierarchy"></a>Изменения (иерархия)

Элемент **Changes** содержит упорядоченный массив типов изменений, представляющий тип различий между папками на клиенте и папками на компьютере, на котором работает Microsoft Exchange Server 2007. 
  
[синкфолдерхиерарчиреспонсе](syncfolderhierarchyresponse.md)
  
[респонсемессажес](responsemessages.md)
  
[синкфолдерхиерарчиреспонсемессаже](syncfolderhierarchyresponsemessage.md)
  
[Изменения (иерархия)](changes-hierarchy.md)
  
```xml
<Changes>
   <Create/>
   <Update/>
   <Delete/>
</Changes>
```

 **синкфолдерхиерарчичанжестипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Create (Фолдерсинк)](create-foldersync.md) <br/> |Определяет одну папку для создания в локальном хранилище клиента.  <br/> |
|[Обновление (Фолдерсинк)](update-foldersync.md) <br/> |Определяет одну папку для обновления в локальном хранилище клиента.  <br/> |
|[Delete (Фолдерсинк)](delete-foldersync.md) <br/> |Определяет одну папку для удаления в локальном хранилище клиента.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[синкфолдерхиерарчиреспонсемессаже](syncfolderhierarchyresponsemessage.md) <br/> |Содержит состояние и результат запроса SyncFolderHierarchy.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение, представляющее логическое значение является обязательным.
  
## <a name="remarks"></a>Примечания

Схема, описывающая этот элемент, находится в виртуальном каталоге EWS компьютера Exchange 2007, на котором установлена роль сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция SyncFolderHierarchy](syncfolderhierarchy-operation.md)


[Справка по службам EWS для Exchange](ews-reference-for-exchange.md)
  
- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

