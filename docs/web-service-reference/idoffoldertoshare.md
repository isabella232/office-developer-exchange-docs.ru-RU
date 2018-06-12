---
title: IdOfFolderToShare
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IdOfFolderToShare
api_type:
- schema
ms.assetid: 199d1839-f061-4070-a977-874b0c08e5be
description: Элемент IdOfFolderToShare представляет идентификатор папки на сервере, который будет использоваться.
ms.openlocfilehash: 1e3e53819f23bbc5753ac21b9e3ea6593ac4826c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833853"
---
# <a name="idoffoldertoshare"></a>IdOfFolderToShare

Элемент **IdOfFolderToShare** представляет идентификатор папки на сервере, который будет использоваться. 
  
```
<IdOfFolderToShare Id="" ChangeKey="" />
```

 **FolderIdType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|Id  <br/> |Содержит строку, которая определяет папке в хранилище Exchange. Этот атрибут является обязательным.  <br/> |
|ChangeKey  <br/> |Содержит строку, которая определяет к папке, которая определена в атрибуте Id версии. Этот атрибут является необязательным. Этот атрибут используется, чтобы убедиться в том, что используется правильный версии папки.  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[GetSharingMetadata](getsharingmetadata.md) <br/> |Определяет запрос на получение маркера непрозрачный проверки подлинности, идентифицирующее приглашение к совместному использованию.  <br/> |
   
## <a name="remarks"></a>Замечания

Схема, описывающая этот элемент находится в IIS виртуального каталога веб-служб Exchange узлов компьютера, на котором выполняется Microsoft Exchange Server, на наличие установлена роль сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция GetSharingMetadata](getsharingmetadata-operation.md)


- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

