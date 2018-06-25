---
title: MimeContent
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MimeContent
api_type:
- schema
ms.assetid: 4f472a08-5653-4c54-ba65-831dfe32f20f
description: Элемент MimeContent содержит ASCII MIME-поток объекта, который представлен в формате base64Binary и поддерживает [RFC2045].
ms.openlocfilehash: 60f2d42f09347611559137c494d93036f1192829
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834465"
---
# <a name="mimecontent"></a>MimeContent

Элемент **MimeContent** содержит ASCII MIME-поток объекта, который представлен в формате base64Binary и поддерживает [[RFC2045]](http://www.rfc-editor.org/rfc/rfc2045.txt).
  
```xml
<MimeContent CharacterSet="" />
```

 **MimeContentType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|**CharacterSet** <br/> |Если задано, значение этого атрибута игнорируется сервером.  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

[Элемента календаря, имеющего](calendaritem.md) | [контакт](contact.md) | [DistributionList](distributionlist.md) | [элемента](item.md) | [MeetingCancellation](meetingcancellation.md) | [MeetingMessage](meetingmessage.md) | [MeetingRequest](meetingrequest.md)  |  [ MeetingResponse](meetingresponse.md) | [сообщение](message-ex15websvcsotherref.md) | [RemoveItem](removeitem.md) | [задач](task.md)
  
## <a name="text-value"></a>Текстовое значение

Текстовое значение, представляющее потока MIME base64Binary является обязательным, если данный элемент используется.
  
## <a name="remarks"></a>Замечания

Содержимое сообщения проходит через кодировки перед сохранением в значении **MimeContent** трех уровней: 
  
1. Текст сообщения — это тело кодирования, такие как iso-2022-jp для японского языка символов.
    
2. Поток MIME — это ASCII кодирования текста сообщения для элемента **MimeContent** или кодировки UTF8 текста сообщения для элемента [MimeContentUTF8](mimecontentutf8.md) . 
    
3. XML-документ — это всегда в кодировке base64 поток ASCII потока MIME, где символы, такие как "\<", значимых XML, скрыты от анализаторы XML.
    
Каждый уровень вне зависимости от уровня, предшествующего его.
  
Элемент **MimeContent** может содержать те же данные, содержащие другие свойства, возвращаемые с элементом. 
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

