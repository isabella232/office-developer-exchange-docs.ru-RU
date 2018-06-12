---
title: Идентификатора вложения AttachmentId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AttachmentId
api_type:
- schema
ms.assetid: 55a5fd77-60d1-40fa-8144-770600cedc6a
description: Элемент идентификатора вложения AttachmentId определяет вложение элемента или файла. Данный элемент используется в CreateAttachment ответы.
ms.openlocfilehash: 2910503d1661ca3aaeeb4e319deb39f6b57c5c0a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761509"
---
# <a name="attachmentid"></a>Идентификатора вложения AttachmentId

Элемент **идентификатора вложения AttachmentId** определяет вложение элемента или файла. Данный элемент используется в CreateAttachment ответы. 
  
```xml
<AttachmentId Id="" RootItemId="" RootItemChangeKey="" />
```

 **AttachmentIdType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|
  **Id** <br/> |Указывает уникальный идентификатор вложения.  <br/> |
|**RootItemId** <br/> |Указывает уникальный идентификатор корневого элемента хранилища, к которому подключен вложение.  <br/> |
|**RootItemChangeKey** <br/> |Идентифицирует ключ изменения корневого элемента хранилища, к которому подключен вложение.  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[ItemAttachment](itemattachment.md) <br/> |Представляет собой элемент Exchange, подключенный к другой элемент Exchange.  <br/> |
|[FileAttachment](fileattachment.md) <br/> |Представляет файл, подключенный к элементу в хранилище Exchange.  <br/> |
   
## <a name="remarks"></a>Замечания

Обратите внимание на то, что при создании вложения, изменить ключ корневого элемента изменяется важно.
  
Элемент [идентификатора вложения AttachmentId (GetAttachment и DeleteAttachment)](attachmentid-getattachment-and-deleteattachment.md) используется в DeleteAttachment и GetAttachment запросов. 
  
Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

