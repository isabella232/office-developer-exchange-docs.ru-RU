---
title: FolderIds
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FolderIds
api_type:
- schema
ms.assetid: 3ff9d15a-7220-4785-ae6b-583a7eb82005
description: Элемент FolderIds содержит массив идентификаторов папок, которые используются для определения папок для копирования, перемещение, получение, удаление или отслеживание уведомлений о событиях.
ms.openlocfilehash: 911a74ca778ee988c270c16c67620a40656d82d8
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762623"
---
# <a name="folderids"></a>FolderIds

Элемент **FolderIds** содержит массив идентификаторов папок, которые используются для определения папок для копирования, перемещение, получение, удаление или отслеживание уведомлений о событиях. 
  
```xml
<FolderIds>
   <FolderId/>
   <DistinguishedFolderId/>
</FolderIds>
```

 **NonEmptyArrayOfBaseFolderIdsType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[FolderId](folderid.md) <br/> |Содержит идентификатор и ключ изменения папки.  <br/> |
|[DistinguishedFolderId](distinguishedfolderid.md) <br/> |Идентифицирует папок Microsoft Exchange Server, которые можно ссылаться по имени.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[GetFolder](getfolder.md) <br/> |Определяет запрос на получение папки из хранилища Exchange.  <br/> Ниже приведен выражение XPath для этого элемента.`/GetFolder` <br/> |
|[DeleteFolder](deletefolder.md) <br/> |Определяет запрос на удаление папок из хранилища Exchange.  <br/> Ниже приведен выражение XPath для этого элемента.`/DeleteFolder` <br/> |
|[EmptyFolder](emptyfolder.md) <br/> |Определяет запрос на удаление папок из хранилища Exchange.  <br/> Ниже приведен выражение XPath для этого элемента.`/EmptyFolder` <br/> |
|[MoveFolder](movefolder.md) <br/> |Определяет запрос на перемещение в папку в хранилище Exchange.  <br/> Ниже приведен выражение XPath для этого элемента.`/MoveFolder` <br/> |
|[CopyFolder](copyfolder.md) <br/> |Определяет запрос для копирования в папку в хранилище Exchange.  <br/> Ниже приведен выражение XPath для этого элемента.`/CopyFolder` <br/> |
|[PushSubscriptionRequest](pushsubscriptionrequest.md) <br/> |Представляет подписка на подписку на уведомления о принудительной события.  <br/> |
|[PullSubscriptionRequest](pullsubscriptionrequest.md) <br/> |Представляет подписка на подписку на уведомления о событий на основе репликации по запросу.  <br/> |
   
## <a name="remarks"></a>Замечания

Схема, описывающая этот элемент находится в виртуальном каталоге EWS компьютера, на котором выполняется Microsoft Exchange Server с установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages и http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема сообщения; Типы схемы  <br/> |
|Файл проверки  <br/> |Messages.xsd; Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[GetFolder Operation](getfolder-operation.md)
  
[Операция DeleteFolder](deletefolder-operation.md)
  
[Операция MoveFolder](movefolder-operation.md)
  
[Операция CopyFolder](copyfolder-operation.md)
  
[Операции подписки](subscribe-operation.md)

