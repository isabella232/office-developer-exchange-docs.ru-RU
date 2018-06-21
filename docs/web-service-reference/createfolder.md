---
title: CreateFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CreateFolder
api_type:
- schema
ms.assetid: 110bada1-517b-4bd6-870d-7086dc879e5d
description: Элемент CreateFolder определяет запрос на создание папки в хранилище Exchange.
ms.openlocfilehash: e30af23b8ed8669053b94be460d62fbf7abf24c9
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/21/2018
ms.locfileid: "19761869"
---
# <a name="createfolder"></a>CreateFolder

Элемент **CreateFolder** определяет запрос на создание папки в хранилище Exchange. 
  
```xml
<CreateFolder>
   <ParentFolderId/>
   <Folders/>
</CreateFolder>
```

 **CreateFolderType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) <br/> |Элемент, определяющий расположение, где будет создана новая папка.  <br/> |
|[Папки](folders-ex15websvcsotherref.md) <br/> |Элемент, содержащий все папках для создания.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

Нет.
  
## <a name="remarks"></a>Замечания

Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема сообщения  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[CreateFolder Operation](createfolder-operation.md)


[Создание папки (веб-служб Exchange)](http://msdn.microsoft.com/library/3b15b0ec-8691-45ed-9a24-a91ff732d6cf%28Office.15%29.aspx)

