---
title: base64FolderId (веб-служба единой системы обмена сообщениями)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_name:
- base64FolderId
api_type:
- schema
ms.assetid: 662f8f2f-49a7-4c7a-9065-98a02a49cfcd
description: Элемент base64FolderId содержит идентификатор папки, который указывается как папка электронной почты по умолчанию, из которой единая система обмена сообщениями считывет сообщения по телефону в запросе операции SetTelephoneAccessFolderEmail (веб-служба единой системы обмена сообщениями).
ms.openlocfilehash: 149ad55d0ab09f57b0dc3ace7eb0e17c96265e3f
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59518934"
---
# <a name="base64folderid-um-web-service"></a>base64FolderId (веб-служба единой системы обмена сообщениями)

Элемент **base64FolderId** содержит идентификатор папки, который указывается как папка электронной почты по умолчанию, из которой единая система обмена сообщениями считывет сообщения по телефону в запросе [операции SetTelephoneAccessFolderEmail](settelephoneaccessfolderemail-operation-um-web-service.md) (веб-служба единой системы обмена сообщениями). 
  
[SetTelephoneAccessFolderEmail (веб-служба единой системы обмена сообщениями)](settelephoneaccessfolderemail-um-web-service.md)
  
[base64FolderId (веб-служба единой системы обмена сообщениями)](base64folderid-um-web-service.md)
  
```xml
<base64FolderId/>
```

 **строка**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[SetTelephoneAccessFolderEmail (веб-служба единой системы обмена сообщениями)](settelephoneaccessfolderemail-um-web-service.md) <br/> |Определяет запрос для набора папки электронной почты доступа к телефону.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Требуется текстовое значение. Текстовое значение представляет ID MAPI папки.
  
## <a name="remarks"></a>Заметки

Чтобы установить папку электронной почты для доступа к телефону, используйте операцию [SetTelephoneAccessFolderEmail (веб-служба um).](settelephoneaccessfolderemail-operation-um-web-service.md)
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Сообщения  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[SetTelephoneAccessFolderEmail (веб-служба единой системы обмена сообщениями)](settelephoneaccessfolderemail-um-web-service.md)
  
[Операция SetTelephoneAccessFolderEmail (веб-служба единой системы обмена сообщениями)](settelephoneaccessfolderemail-operation-um-web-service.md)
  
[Операция FindFolder](findfolder-operation.md)
  
[Операция FindItem](finditem-operation.md)

