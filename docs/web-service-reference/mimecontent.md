---
title: MimeContent
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- MimeContent
api_type:
- schema
ms.assetid: 4f472a08-5653-4c54-ba65-831dfe32f20f
description: Элемент MimeContent содержит поток ASCII MIME объекта, который представлен в формате base64Binary и поддерживает [RFC2045].
ms.openlocfilehash: 43040f241008010620ff4f1018cc5410a7a00e42
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59542073"
---
# <a name="mimecontent"></a>MimeContent

Элемент **MimeContent** содержит поток ASCII MIME объекта, который представлен в формате base64Binary и поддерживает [[RFC2045].](http://www.rfc-editor.org/rfc/rfc2045.txt)
  
```xml
<MimeContent CharacterSet="" />
```

 **MimeContentType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|**CharacterSet** <br/> |Если установлено, значение этого атрибута игнорируется сервером.  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

[CalendarItem](calendaritem.md)  |  [Контакт](contact.md)  |  [DistributionList](distributionlist.md)  |  [Item](item.md)  |  [MeetingCancellation](meetingcancellation.md)  |  [MeetingMessage](meetingmessage.md)  |  [MeetingRequest](meetingrequest.md)  |  [MeetingResponse](meetingresponse.md)  |  [Сообщение](message-ex15websvcsotherref.md)  |  [RemoveItem](removeitem.md)  |  [Задача](task.md)
  
## <a name="text-value"></a>Текстовое значение

Если этот элемент используется, необходимо текстовое значение, представляюще поток MIME base64Binary.
  
## <a name="remarks"></a>Заметки

Содержимое сообщения проходит следующие три уровня кодии перед хранением в **значении MimeContent:** 
  
1. Текст сообщения — это кодировое тело, например iso-2022-jp для японских символов.
    
2. Поток MIME — это кодификат ASCII текста сообщения для элемента **MimeContent** или кодификат UTF8 текста сообщения для элемента [MimeContentUTF8.](mimecontentutf8.md) 
    
3. XML-документ — это всегда базовый поток ASCII в потоке MIME, где символы , такие как ', которые имеют значение для XML, скрыты от \< XML-парсеров.
    
Каждый уровень не зависит от уровня, предшествующего ему.
  
Элемент **MimeContent может** содержать те же данные, что и другие свойства, возвращаемые с элементом. 
  
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

