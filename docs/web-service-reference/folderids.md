---
title: фолдеридс
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
description: Элемент Фолдеридс содержит массив идентификаторов папок, которые используются для идентификации папок для копирования, перемещения, получения, удаления или отслеживания уведомлений о событиях.
ms.openlocfilehash: ff0476f72c7da088bd2b39f58ab560dcc82197e4
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530995"
---
# <a name="folderids"></a>фолдеридс

Элемент **фолдеридс** содержит массив идентификаторов папок, которые используются для идентификации папок для копирования, перемещения, получения, удаления или отслеживания уведомлений о событиях. 
  
```xml
<FolderIds>
   <FolderId/>
   <DistinguishedFolderId/>
</FolderIds>
```

 **нонемптяррайофбасефолдеридстипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[FolderId](folderid.md) <br/> |Содержит идентификатор и ключ изменения папки.  <br/> |
|[дистингуишедфолдерид](distinguishedfolderid.md) <br/> |Определяет папки Microsoft Exchange Server, на которые можно ссылаться по имени.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[GetFolder](getfolder.md) <br/> |Определяет запрос на получение папки из хранилища Exchange.  <br/> Ниже приведено выражение XPath для этого элемента:`/GetFolder` <br/> |
|[DeleteFolder](deletefolder.md) <br/> |Определяет запрос на удаление папок из хранилища Exchange.  <br/> Ниже приведено выражение XPath для этого элемента:`/DeleteFolder` <br/> |
|[EmptyFolder](emptyfolder.md) <br/> |Определяет запрос на удаление папок из хранилища Exchange.  <br/> Ниже приведено выражение XPath для этого элемента:`/EmptyFolder` <br/> |
|[MoveFolder](movefolder.md) <br/> |Определяет запрос на перемещение папки в хранилище Exchange.  <br/> Ниже приведено выражение XPath для этого элемента:`/MoveFolder` <br/> |
|[CopyFolder](copyfolder.md) <br/> |Определяет запрос на копирование папки в хранилище Exchange.  <br/> Ниже приведено выражение XPath для этого элемента:`/CopyFolder` <br/> |
|[пушсубскриптионрекуест](pushsubscriptionrequest.md) <br/> |Представляет подписку на подписку на уведомления о событиях на основе push-уведомлений.  <br/> |
|[пуллсубскриптионрекуест](pullsubscriptionrequest.md) <br/> |Представляет подписку на подписку на уведомления о событиях по запросу.  <br/> |
   
## <a name="remarks"></a>Примечания

Схема, описывающая этот элемент, находится в виртуальном каталоге EWS компьютера, на котором работает сервер Microsoft Exchange с установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages и https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема сообщений; Схема Types  <br/> |
|Файл проверки  <br/> |Messages. xsd; Types. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция GetFolder](getfolder-operation.md)
  
[Операция DeleteFolder](deletefolder-operation.md)
  
[Операция MoveFolder](movefolder-operation.md)
  
[Операция CopyFolder](copyfolder-operation.md)
  
[Операции подписки](subscribe-operation.md)

