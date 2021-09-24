---
title: SharingFolderId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- SharingFolderId
api_type:
- schema
ms.assetid: 5ad37ceb-2922-4420-9051-c29d0d57c420
description: Элемент SharingFolderId представляет идентификатор локальной папки в отношениях общего доступа.
ms.openlocfilehash: 9f26efa394341c8ead895a1d8e898cb48d9c2cb9
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59540442"
---
# <a name="sharingfolderid"></a>SharingFolderId

Элемент **SharingFolderId** представляет идентификатор локальной папки в отношениях общего доступа. 
  
```xml
<SharingFolderId Id="" ChangeKey="" />
```

 **FolderIdType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|Id  <br/> |Содержит строку, которая идентифицирует папку в Exchange магазине. Этот атрибут является обязательным.  <br/> |
|ChangeKey  <br/> |Содержит строку, определяемую версией папки, идентифицируемой атрибутом Id. Этот атрибут является необязательным. Используйте этот атрибут, чтобы убедиться, что используется правильная версия папки.  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[RefreshSharingFolder](refreshsharingfolder.md) <br/> |Определяет запрос на обновление указанной локальной папки.  <br/> |
|[GetSharingFolderResponse](getsharingfolderresponse.md) <br/> |Определяет ответ на запрос [операции GetSharingFolder.](getsharingfolder-operation.md)  <br/> |
|[GetSharingFolderResponseMessage](getsharingfolderresponsemessage.md) <br/> |Содержит состояние и результат одного запроса [операции GetSharingFolder.](getsharingfolder-operation.md)  <br/> |
   
## <a name="remarks"></a>Заметки

Схема, описываемая этим элементом, расположена в виртуальном каталоге IIS, Exchange веб-службы компьютера, на котором Microsoft Exchange Server установлена роль сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

