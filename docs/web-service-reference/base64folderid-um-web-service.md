---
title: base64FolderId (веб-служба единой системы обмена сообщениями)
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
description: Элемент base64FolderId содержит идентификатор папки, которую необходимо указать в качестве папки электронной почты по умолчанию, из которой единая система обмена сообщениями читает сообщения по телефону, в запросе веб-службы единой системы обмена сообщениями SetTelephoneAccessFolderEmail.
ms.openlocfilehash: ea31c7a0f93188e563bf95c4a3e6e91f0866746c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458049"
---
# <a name="base64folderid-um-web-service"></a>base64FolderId (веб-служба единой системы обмена сообщениями)

Элемент **base64FolderId** содержит идентификатор папки, которую необходимо указать в качестве папки электронной почты по умолчанию, из которой единая система обмена сообщениями читает сообщения по телефону, в запросе [веб-службы единой системы обмена](settelephoneaccessfolderemail-operation-um-web-service.md) сообщениями SetTelephoneAccessFolderEmail. 
  
[SetTelephoneAccessFolderEmail (веб-служба единой системы обмена сообщениями)](settelephoneaccessfolderemail-um-web-service.md)
  
[base64FolderId (веб-служба единой системы обмена сообщениями)](base64folderid-um-web-service.md)
  
```xml
<base64FolderId/>
```

 **строка**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Нет
  
### <a name="child-elements"></a>Дочерние элементы

Отсутствуют.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[SetTelephoneAccessFolderEmail (веб-служба единой системы обмена сообщениями)](settelephoneaccessfolderemail-um-web-service.md) <br/> |Определяет запрос на установку папки электронной почты для телефонного доступа.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Необходимо указать текстовое значение. Текстовое значение представляет идентификатор MAPI папки.
  
## <a name="remarks"></a>Примечания

Чтобы задать папку электронной почты для телефонного доступа, используйте [операцию SetTelephoneAccessFolderEmail (веб-служба единой системы обмена сообщениями)](settelephoneaccessfolderemail-operation-um-web-service.md).
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Сообщения  <br/> |
|Файл проверки  <br/> |Messages. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[SetTelephoneAccessFolderEmail (веб-служба единой системы обмена сообщениями)](settelephoneaccessfolderemail-um-web-service.md)
  
[Операция SetTelephoneAccessFolderEmail (веб-служба единой системы обмена сообщениями)](settelephoneaccessfolderemail-operation-um-web-service.md)
  
[Операция FindFolder](findfolder-operation.md)
  
[Операция FindItem](finditem-operation.md)

