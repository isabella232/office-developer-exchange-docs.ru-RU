---
title: OldFolderId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- OldFolderId
api_type:
- schema
ms.assetid: da554a97-ab87-4950-9fc4-26b1972381bb
description: Элемент OldFolderId содержит исходный идентификатор папки, которая была перемещена или скопирована.
ms.openlocfilehash: 42260822870a0a9bac565c20447a5c29c3daccce
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59541947"
---
# <a name="oldfolderid"></a>OldFolderId

Элемент **OldFolderId** содержит исходный идентификатор папки, которая была перемещена или скопирована. 
  
```xml
<OldFolderId Id="" ChangeKey=""/>
```

 **FolderIdType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|**Id** <br/> |Содержит строку, которая идентифицирует папку в Exchange магазине. Этот атрибут является обязательным.  <br/> |
|**ChangeKey** <br/> |Содержит строку, определяемую версией папки, идентифицируемой атрибутом Id. Этот атрибут является необязательным. Используйте этот атрибут, чтобы убедиться, что используется правильная версия папки.  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[CopiedEvent](copiedevent.md) <br/> |Представляет событие, в котором копируется элемент или папка.  <br/> |
|[MovedEvent](movedevent.md) <br/> |Представляет событие, в котором элемент или папка перемещаются из одной родительской папки в другую родительную.  <br/> |
   
## <a name="remarks"></a>Заметки

Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операции подписки](subscribe-operation.md)
  
[Операция GetEvents](getevents-operation.md)
  
[Операция Unsubscribe](unsubscribe-operation.md)


- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

