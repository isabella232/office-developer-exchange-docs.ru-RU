---
title: SyncFolderItems
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- SyncFolderItems
api_type:
- schema
ms.assetid: 463ed78c-bf82-4cd8-971a-d18425e9e7be
description: Элемент SyncFolderItems определяет запрос на синхронизацию элементов в папке Exchange магазине.
ms.openlocfilehash: a3e5aa83335a6bc29b832021e227e6adad4092bf
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59513285"
---
# <a name="syncfolderitems"></a>SyncFolderItems

Элемент **SyncFolderItems** определяет запрос на синхронизацию элементов в папке Exchange магазина. 
  
```xml
<SyncFolderItems>
   <ItemShape/>
   <SyncFolderId/>
   <SyncState/>
   <Ignore/>
   <MaxChangesReturned/>   <SyncScope/>
</SyncFolderItems>
```

 **SyncFolderItemsType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[ItemShape](itemshape.md) <br/> |Определяет свойства и содержимое элемента, которые необходимо включить в ответ SyncFolderItems. Этот элемент обязательный.  <br/> |
|[SyncFolderId](syncfolderid.md) <br/> |Представляет папку, которая содержит элементы для синхронизации. Этот элемент обязательный.  <br/> |
|[SyncState](syncstate-ex15websvcsotherref.md) <br/> |Содержит кодированную базовую форму данных синхронизации, обновляемую после каждого успешного запроса. Это используется для определения состояния синхронизации. Этот элемент является необязательным.  <br/> |
|[Ignore](ignore.md) <br/> |Определяет элементы, которые необходимо пропустить во время синхронизации. Этот элемент является необязательным.  <br/> |
|[MaxChangesReturned](maxchangesreturned.md) <br/> |Описывает максимальное количество изменений, которые могут быть возвращены в ответ на синхронизацию. Этот элемент обязательный.  <br/> |
|[SyncScope](syncscope.md) <br/> |Указывает, возвращаются ли в ответ синхронизации только элементы или элементы и связанные с ними папки. Этот элемент является необязательным.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

Нет.
  
## <a name="remarks"></a>Заметки

Схема, описываемая этим элементом, расположена в виртуальном каталоге компьютера EWS, на Microsoft Exchange Server установлена роль сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |схема сообщений  <br/> |
|Файл проверки  <br/> |messages.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция SyncFolderItems](syncfolderitems-operation.md)


- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

