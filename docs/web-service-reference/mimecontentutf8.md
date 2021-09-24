---
title: MimeContentUTF8
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 31544c95-5231-4b57-958c-2a689464d29b
description: Элемент MimeContentUTF8 содержит поток MIME UTF-8 объекта, который представлен в формате base64Binary и поддерживает интернационализацию адресов электронной почты и [RFC6530].
ms.openlocfilehash: f0ab38368d3a18be38f63c86183a238e2fd0a474
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59540757"
---
# <a name="mimecontentutf8"></a>MimeContentUTF8

Элемент **MimeContentUTF8** содержит поток MIME UTF-8 объекта, который представлен в формате base64Binary и поддерживает интернационализацию адресов электронной почты [и [RFC6530].](http://www.rfc-editor.org/rfc/rfc6530.txt)
  
```XML
<MimeContentUTF8 CharacterSet="" />
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

Если этот элемент используется, требуется текстовое значение, представляюще поток MIME base64binary.
  
## <a name="remarks"></a>Заметки

Содержимое сообщения перед хранением в значении **MimeContentUTF8** проходит следующие три уровня кодификинга: 
  
1. Текст сообщения — это кодировое тело, например iso-2022-jp для японских символов.
    
2. Поток MIME — это кодификат текста сообщения UTF8 для элемента **MimeContentUTF8** или кодификация ASCII текста сообщения для элемента [MimeContent.](mimecontent.md) 
    
3. XML-документ — это всегда базовый поток ASCII в потоке MIME, где символы , такие как ', которые имеют значение для XML, скрыты от \< XML-парсеров.
    
Каждый уровень не зависит от уровня, предшествующего ему.
  
Элемент **MimeContentUTF8** может содержать те же данные, что и другие свойства, возвращаемые с элементом. 
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
### <a name="version-differences"></a>Различия версий

Этот элемент доступен в версиях Exchange начиная с сборки 15.00.0986.00.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

