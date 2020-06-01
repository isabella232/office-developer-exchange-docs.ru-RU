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
description: Элемент GetAttachment является корневым элементом запроса для получения вложения из хранилища Exchange.
ms.openlocfilehash: d03d086ff443db87b0104a2ec83599eb9eaea6b9
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463981"
---
# <a name="getattachment"></a>GetAttachment

Элемент **GetAttachment** является корневым элементом запроса для получения вложения из хранилища Exchange. 
  
```xml
<GetAttachment>
   <AttachmentShape/>
   <AttachmentIds/>
</GetAttachment>
```

 **жетаттачменттипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[аттачментшапе](attachmentshape.md) <br/> |Определяет дополнительные свойства расширенного элемента, которые возвращаются в ответ на запрос [GetAttachment](getattachment.md) . Этот элемент является необязательным.  <br/> |
|[аттачментидс](attachmentids.md) <br/> |Содержит массив идентификаторов вложений.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

Нет.
  
## <a name="remarks"></a>Примечания

Элемент [аттачментшапе](attachmentshape.md) не требуется для определения свойств, возвращаемых в ответе. [Операция GetAttachment](getattachment-operation.md) возвращает имя, ContentType, ContentId, ContentLocation и свойства содержимого для вложенных файлов. Для вложений элемента возвращаемыми свойствами являются имя, ContentType, идентификатор ContentId, ContentLocation и все свойства вложенного элемента. Это эквивалентно использованию базовой фигуры Аллпропертиес в запросе [GetItem](getitem.md) . 
  
Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция GetAttachment](getattachment-operation.md)
  
[жетаттачментреспонсе](getattachmentresponse.md)

