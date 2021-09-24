---
title: SyncScope
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- SyncScope
api_type:
- schema
ms.assetid: e0ca231f-0374-4844-8d4c-ada8da167920
description: Элемент SyncScope указывает, возвращаются ли в ответ синхронизации только элементы или элементы и связанные с ними папки.
ms.openlocfilehash: 5e5d19809cea1f8f244444c09615ee888fea05be
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59538900"
---
# <a name="syncscope"></a>SyncScope

Элемент **SyncScope** указывает, возвращаются ли в ответ синхронизации только элементы или элементы и связанные с ними папки. 
  
```xml
<SyncScope>NormalItems or NormalAndAssociatedItems</SyncScope>
```

 **SyncFolderItemsScopeType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[SyncFolderItems](syncfolderitems.md) <br/> |Элемент, который определяет запрос для синхронизации элементов в Exchange папке.  <br/> Ниже приводится выражение XPath к этому элементу:  <br/> /SyncFolderItems  <br/> |
   
## <a name="text-value"></a>Текстовое значение

В следующей таблице перечислены возможные значения элемента **SyncScope.** 
  
**Значения элементов SyncScope**

|**Значение**|**Описание**|
|:-----|:-----|
|NormalItems  <br/> |Указывает, что только элементы в папке возвращаются в ответ на синхронизацию.  <br/> |
|NormalAndAssociatedItems  <br/> |Указывает, что в ответ на синхронизацию возвращаются как элементы в папке, так и связанные с ней данные.  <br/> |
   
## <a name="remarks"></a>Заметки

Схема, описываемая этим элементом, расположена в виртуальном каталоге компьютера EWS, на Microsoft Exchange Server установлена роль сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция SyncFolderItems](syncfolderitems-operation.md)


- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

