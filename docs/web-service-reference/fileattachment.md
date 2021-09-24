---
title: FileAttachment
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- FileAttachment
api_type:
- schema
ms.assetid: 3ecea174-73d1-47fd-8917-6065cef1d565
description: Элемент FileAttachment представляет файл, присоединенный к элементу в Exchange магазине.
ms.openlocfilehash: 66424fefafd2084bf0b6f45881089448593e621d
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59518500"
---
# <a name="fileattachment"></a>FileAttachment

Элемент **FileAttachment** представляет файл, присоединенный к элементу в Exchange магазине. 
  
```XML
<FileAttachment>
   <AttachmentId/>
   <Name/>
   <ContentType/>
   <ContentId/>
   <ContentLocation/>
   <Size/>
   <LastModifiedTime/>
   <IsInline/>
   <IsContactPhoto/>
   <Content/>
</FileAttachment>
```

 **FileAttachmentType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[AttachmentId](attachmentid.md) <br/> |Определяет вложение файла.  <br/> |
|[Name (AttachmentType)](name-attachmenttype.md) <br/> |Представляет имя вложения.  <br/> |
|[ContentType](contenttype.md) <br/> |Описывает тип многоцелевых расширений интернет-почты (MIME) контента вложений.  <br/> |
|[ContentId](contentid.md) <br/> |Представляет идентификатор для содержимого вложения. [ContentId](contentid.md) можно задать любому значению строки. Приложения могут использовать [ContentId для](contentid.md) реализации собственных механизмов идентификации.  <br/> |
|[ContentLocation](contentlocation.md) <br/> |Содержит идентификатор единого ресурса (URI), соответствующий расположению содержимого вложения.  <br/> |
|[Размер](size.md) <br/> |Представляет размер в bytes вложения файла.  <br/> |
|[LastModifiedTime](lastmodifiedtime.md) <br/> |Представляет, когда вложение файла было изменено в последний раз.  <br/> |
|[IsInline](isinline.md) <br/> |Представляет, отображается ли вложение внутри элемента.  <br/> |
|[IsContactPhoto](iscontactphoto.md) <br/> |Указывает, является ли вложение файла контактным изображением.  <br/> |
|[Статья](content.md) <br/> |Содержит содержимое вложения файла с кодом Base64.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Вложения](attachments-ex15websvcsotherref.md) <br/> |Содержит элементы или файлы, присоединенные к элементу в Exchange магазине.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Нет.
  
## <a name="remarks"></a>Заметки

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

