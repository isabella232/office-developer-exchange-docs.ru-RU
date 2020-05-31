---
title: FileAttachment
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FileAttachment
api_type:
- schema
ms.assetid: 3ecea174-73d1-47fd-8917-6065cef1d565
description: Элемент FileAttachment представляет файл, присоединенный к элементу в хранилище Exchange.
ms.openlocfilehash: 5ce7aef753313aa9430f640bb3c26f652b8c1c43
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762542"
---
# <a name="fileattachment"></a>FileAttachment

Элемент **FileAttachment** представляет файл, присоединенный к элементу в хранилище Exchange. 
  
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

 **филеаттачменттипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[AttachmentId](attachmentid.md) <br/> |Определяет вложенный файл.  <br/> |
|[Имя (AttachmentType)](name-attachmenttype.md) <br/> |Представляет имя вложения.  <br/> |
|[ContentType](contenttype.md) <br/> |Описание многоцелевого расширения почты в Интернете (MIME) для содержимого вложения.  <br/> |
|[ContentId](contentid.md) <br/> |Представляет идентификатор для содержимого вложения. Идентификатору [ContentId](contentid.md) можно присвоить любое строковое значение. Приложения могут использовать идентификаторы [ContentId](contentid.md) для реализации собственных механизмов идентификации.  <br/> |
|[ContentLocation](contentlocation.md) <br/> |Содержит универсальный код ресурса (URI), соответствующий расположению содержимого вложения.  <br/> |
|[Размер](size.md) <br/> |Представляет размер вложенного файла в байтах.  <br/> |
|[LastModifiedTime](lastmodifiedtime.md) <br/> |Представляет время последнего изменения вложенного файла.  <br/> |
|[IsInline](isinline.md) <br/> |Указывает, отображается ли вложение встроенным в элементе.  <br/> |
|[исконтактфото](iscontactphoto.md) <br/> |Указывает, является ли вложение изображением контакта.  <br/> |
|[Статья](content.md) <br/> |Содержит содержимое вложенного файла в кодировке Base64.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Вложения](attachments-ex15websvcsotherref.md) <br/> |Содержит элементы или файлы, вложенные в элемент в хранилище Exchange.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Нет.
  
## <a name="remarks"></a>Примечания

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

