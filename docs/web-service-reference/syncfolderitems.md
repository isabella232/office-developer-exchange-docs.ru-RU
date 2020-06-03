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
description: Элемент SyncFolderItems определяет запрос на синхронизацию элементов в папке хранилища Exchange.
ms.openlocfilehash: 0fa5b1544d5627d1423287369e72f97662c28d12
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465151"
---
# <a name="syncfolderitems"></a>SyncFolderItems

Элемент **SyncFolderItems** определяет запрос на синхронизацию элементов в папке хранилища Exchange. 
  
```xml
<SyncFolderItems>
   <ItemShape/>
   <SyncFolderId/>
   <SyncState/>
   <Ignore/>
   <MaxChangesReturned/>   <SyncScope/>
</SyncFolderItems>
```

 **синкфолдеритемстипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[итемшапе](itemshape.md) <br/> |Определяет свойства и контент элемента, включаемые в ответ SyncFolderItems. Этот элемент обязательный.  <br/> |
|[синкфолдерид](syncfolderid.md) <br/> |Представляет папку, содержащую синхронизируемые элементы. Этот элемент обязательный.  <br/> |
|[синкстате](syncstate-ex15websvcsotherref.md) <br/> |Содержит форму синхронизации данных с кодировкой base64, которая обновляется после каждого успешного выполнения запроса. Используется для определения состояния синхронизации. Этот элемент является необязательным.  <br/> |
|[Ignore](ignore.md) <br/> |Определяет элементы, которые необходимо пропустить во время синхронизации. Этот элемент является необязательным.  <br/> |
|[максчанжесретурнед](maxchangesreturned.md) <br/> |Описывает максимальное число изменений, которые могут быть возвращены в ответе синхронизации. Этот элемент обязательный.  <br/> |
|[синкскопе](syncscope.md) <br/> |Указывает, будут ли в ответе синхронизации возвращаться только элементы, связанные с папкой и сведениями о них. Этот элемент является необязательным.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

Нет.
  
## <a name="remarks"></a>Примечания

Схема, описывающая этот элемент, находится в виртуальном каталоге EWS компьютера, на котором работает сервер Microsoft Exchange с установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |схема сообщений  <br/> |
|Файл проверки  <br/> |messages. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция SyncFolderItems](syncfolderitems-operation.md)


- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

