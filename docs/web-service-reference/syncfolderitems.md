---
title: SyncFolderItems
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SyncFolderItems
api_type:
- schema
ms.assetid: 463ed78c-bf82-4cd8-971a-d18425e9e7be
description: Элемент SyncFolderItems определяет запрос для синхронизации элементов в папке хранилища Exchange.
ms.openlocfilehash: 368e19babfccaeab40380103495c63d30647905c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19840126"
---
# <a name="syncfolderitems"></a>SyncFolderItems

Элемент **SyncFolderItems** определяет запрос для синхронизации элементов в папке хранилища Exchange. 
  
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
|[ItemShape](itemshape.md) <br/> |Определяет свойства элемента и содержимого для включения в SyncFolderItems ответа. Этот элемент обязательный.  <br/> |
|[SyncFolderId](syncfolderid.md) <br/> |Представляет папку, содержащую элементы для синхронизации. Этот элемент обязательный.  <br/> |
|[Состояние](syncstate-ex15websvcsotherref.md) <br/> |Содержит формы кодировки Base64 данных синхронизации, который обновляется после каждого успешного запроса. Используется для определения состояния синхронизации. Этот элемент является необязательным.  <br/> |
|[Пропуск](ignore.md) <br/> |Определяет элементы, чтобы пропустить во время синхронизации. Этот элемент является необязательным.  <br/> |
|[MaxChangesReturned](maxchangesreturned.md) <br/> |Описывает максимальное число изменений, которые могут возвращаться в ответ синхронизации. Этот элемент обязательный.  <br/> |
|[SyncScope](syncscope.md) <br/> |Указывает, будет ли только что элементов или элементы и сведения, папки, связанной возвращаются в синхронизации ответа. Этот элемент является необязательным.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

Нет.
  
## <a name="remarks"></a>Замечания

Схема, описывающая этот элемент находится в виртуальном каталоге EWS компьютера, на котором выполняется Microsoft Exchange Server с установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема сообщения  <br/> |
|Файл проверки  <br/> |messages.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция SyncFolderItems](syncfolderitems-operation.md)


- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

