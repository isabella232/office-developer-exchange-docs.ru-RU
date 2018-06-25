---
title: GetAttachment
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetAttachment
api_type:
- schema
ms.assetid: 9443cf96-b451-4530-b868-490dff798673
description: Элемент GetAttachment является корневым элементом в запросе для получения вложения из хранилища Exchange.
ms.openlocfilehash: fb639c86a0654e8f9e9601310f7c2f5b0fc7d729
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762698"
---
# <a name="getattachment"></a>GetAttachment

Элемент **GetAttachment** является корневым элементом в запросе для получения вложения из хранилища Exchange. 
  
```xml
<GetAttachment>
   <AttachmentShape/>
   <AttachmentIds/>
</GetAttachment>
```

 **GetAttachmentType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[AttachmentShape](attachmentshape.md) <br/> |Определяет дополнительные расширенные свойства элемента для возврата в ответ на запрос [GetAttachment](getattachment.md) . Этот элемент является необязательным.  <br/> |
|[AttachmentIds](attachmentids.md) <br/> |Содержит массив идентификаторов вложения.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

Нет.
  
## <a name="remarks"></a>Замечания

Элемент [AttachmentShape](attachmentshape.md) не требуется для идентификации свойства, возвращаемого в ответе. [Операция GetAttachment](getattachment-operation.md) возвращает имя, ContentType, ContentId, ContentLocation и свойства содержимого для вложенных файлов. Для вложений элемента возвращаемого свойства — это имя, ContentType, ContentId, ContentLocation и все вложенные свойства элемента. Это эквивалентно использованию фигуры базовый AllProperties в запросе [GetItem](getitem.md) . 
  
Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция GetAttachment](getattachment-operation.md)
  
[GetAttachmentResponse](getattachmentresponse.md)

