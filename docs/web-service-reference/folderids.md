---
title: FolderIds
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- FolderIds
api_type:
- schema
ms.assetid: 3ff9d15a-7220-4785-ae6b-583a7eb82005
description: Элемент FolderIds содержит массив идентификаторов папок, используемых для идентификации папок для копирования, перемещения, получения, удаления или мониторинга уведомлений о событиях.
ms.openlocfilehash: 7c0cf46d5fdaf35ec72cf3b5750b51edc5a8bfe0
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59518367"
---
# <a name="folderids"></a>FolderIds

Элемент **FolderIds** содержит массив идентификаторов папок, используемых для идентификации папок для копирования, перемещения, получения, удаления или мониторинга уведомлений о событиях. 
  
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
|[DistinguishedFolderId](distinguishedfolderid.md) <br/> |Определяет Microsoft Exchange Server папки, на которые можно ссылаться по имени.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[GetFolder](getfolder.md) <br/> |Определяет запрос на получения папки из Exchange магазина.  <br/> Ниже приводится выражение XPath к этому элементу:  `/GetFolder` <br/> |
|[DeleteFolder](deletefolder.md) <br/> |Определяет запрос на удаление папок из Exchange магазина.  <br/> Ниже приводится выражение XPath к этому элементу:  `/DeleteFolder` <br/> |
|[EmptyFolder](emptyfolder.md) <br/> |Определяет запрос на удаление папок из Exchange магазина.  <br/> Ниже приводится выражение XPath к этому элементу:  `/EmptyFolder` <br/> |
|[MoveFolder](movefolder.md) <br/> |Определяет запрос на перемещение папки в Exchange магазине.  <br/> Ниже приводится выражение XPath к этому элементу:  `/MoveFolder` <br/> |
|[CopyFolder](copyfolder.md) <br/> |Определяет запрос на копирование папки в Exchange магазине.  <br/> Ниже приводится выражение XPath к этому элементу:  `/CopyFolder` <br/> |
|[PushSubscriptionRequest](pushsubscriptionrequest.md) <br/> |Представляет подписку на подписку на push-уведомление о событиях.  <br/> |
|[PullSubscriptionRequest](pullsubscriptionrequest.md) <br/> |Представляет подписку на подписку на уведомление о событиях на основе тяги.  <br/> |
   
## <a name="remarks"></a>Заметки

Схема, описываемая этим элементом, расположена в виртуальном каталоге компьютера EWS, на Microsoft Exchange Server установлена роль сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages и https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема сообщений; Схема типов  <br/> |
|Файл проверки  <br/> |Messages.xsd; Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция GetFolder](getfolder-operation.md)
  
[Операция DeleteFolder](deletefolder-operation.md)
  
[Операция MoveFolder](movefolder-operation.md)
  
[Операция CopyFolder](copyfolder-operation.md)
  
[Операции подписки](subscribe-operation.md)

