---
title: AttachmentId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- AttachmentId
api_type:
- schema
ms.assetid: 55a5fd77-60d1-40fa-8144-770600cedc6a
description: Элемент AttachmentId определяет элемент или вложение файла. Этот элемент используется в ответах CreateAttachment.
ms.openlocfilehash: a6363fad4e7ef9f0c21377f2c1ea8c19c494cdef
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59522021"
---
# <a name="attachmentid"></a>AttachmentId

Элемент **AttachmentId** определяет элемент или вложение файла. Этот элемент используется в ответах CreateAttachment. 
  
```xml
<AttachmentId Id="" RootItemId="" RootItemChangeKey="" />
```

 **AttachmentIdType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|**Id** <br/> |Определяет уникальный идентификатор вложения.  <br/> |
|**RootItemId** <br/> |Определяет уникальный идентификатор элемента корневого магазина, к которому присоединено вложение.  <br/> |
|**RootItemChangeKey** <br/> |Определяет ключ изменения элемента корневого магазина, к которому присоединено вложение.  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[ItemAttachment](itemattachment.md) <br/> |Представляет элемент Exchange, присоединенный к другому элементу Exchange.  <br/> |
|[FileAttachment](fileattachment.md) <br/> |Представляет файл, присоединенный к элементу в Exchange магазине.  <br/> |
   
## <a name="remarks"></a>Заметки

Важно отметить, что при создания вложения изменяется ключ изменения корневого элемента.
  
Элемент [AttachmentId (GetAttachment и DeleteAttachment)](attachmentid-getattachment-and-deleteattachment.md) используется в запросах DeleteAttachment и GetAttachment. 
  
Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

