---
title: base64FolderId (веб-служба единой системы обмена СООБЩЕНИЯМИ)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- base64FolderId
api_type:
- schema
ms.assetid: 662f8f2f-49a7-4c7a-9065-98a02a49cfcd
description: Элемент base64FolderId содержит идентификатор папки, чтобы указать в качестве папки электронной почты по умолчанию, из которого единой системы обмена сообщениями считывает этих сообщений по телефону в запросе SetTelephoneAccessFolderEmail операции (веб-служба единой системы обмена СООБЩЕНИЯМИ).
ms.openlocfilehash: 7d710542418a717c6fcad243a22682e5840ebbd2
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761546"
---
# <a name="base64folderid-um-web-service"></a>base64FolderId (веб-служба единой системы обмена СООБЩЕНИЯМИ)

Элемент **base64FolderId** содержит идентификатор папки, чтобы указать в качестве папки электронной почты по умолчанию, из которого единой системы обмена сообщениями считывает этих сообщений по телефону в запрос [SetTelephoneAccessFolderEmail операции (веб-служба единой системы обмена СООБЩЕНИЯМИ)](settelephoneaccessfolderemail-operation-um-web-service.md) . 
  
[SetTelephoneAccessFolderEmail (веб-служба единой системы обмена СООБЩЕНИЯМИ)](settelephoneaccessfolderemail-um-web-service.md)
  
[base64FolderId (веб-служба единой системы обмена СООБЩЕНИЯМИ)](base64folderid-um-web-service.md)
  
```xml
<base64FolderId/>
```

 **string**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[SetTelephoneAccessFolderEmail (веб-служба единой системы обмена СООБЩЕНИЯМИ)](settelephoneaccessfolderemail-um-web-service.md) <br/> |Определяет запрос, чтобы задать папку телефонного доступа электронной почты.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение является обязательным. Текстовое значение представляет идентификатор MAPI папки.
  
## <a name="remarks"></a>Замечания

Чтобы задать папку телефонного доступа электронной почты, с помощью [операции SetTelephoneAccessFolderEmail (веб-служба единой системы обмена СООБЩЕНИЯМИ)](settelephoneaccessfolderemail-operation-um-web-service.md).
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Сообщения  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[SetTelephoneAccessFolderEmail (веб-служба единой системы обмена СООБЩЕНИЯМИ)](settelephoneaccessfolderemail-um-web-service.md)
  
[Операция SetTelephoneAccessFolderEmail (веб-служба единой системы обмена СООБЩЕНИЯМИ)](settelephoneaccessfolderemail-operation-um-web-service.md)
  
[FindFolder Operation](findfolder-operation.md)
  
[FindItem Operation](finditem-operation.md)

