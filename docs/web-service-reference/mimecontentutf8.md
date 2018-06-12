---
title: MimeContentUTF8
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 31544c95-5231-4b57-958c-2a689464d29b
description: Элемент MimeContentUTF8 содержит MIME UTF-8-поток объекта, представленного в формате base64Binary и Интернационализация адрес электронной почты поддерживает и [RFC6530].
ms.openlocfilehash: 47599b6634738fd488e5b020f69e36d5fcf550a6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19834466"
---
# <a name="mimecontentutf8"></a>MimeContentUTF8

Элемент **MimeContentUTF8** содержит MIME UTF-8-поток объекта, который представлен в формате base64Binary и поддерживает Интернационализация адрес электронной почты и [[RFC6530]](http://www.rfc-editor.org/rfc/rfc6530.txt).
  
```XML
<MimeContentUTF8 CharacterSet="" />
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

Текстовое значение, представляющее потока MIME base64binary является обязательным, если данный элемент используется.
  
## <a name="remarks"></a>Замечания

Содержимое сообщения проходит через трех уровней кодировки перед сохранением в значении **MimeContentUTF8** : 
  
1. Текст сообщения — это тело кодирования, такие как iso-2022-jp для японского языка символов.
    
2. Поток MIME — это кодировки UTF8 текста сообщения для элемента **MimeContentUTF8** или кодировка текста сообщения для элемента [MimeContent](mimecontent.md) ASCII. 
    
3. XML-документ — это всегда в кодировке base64 поток ASCII потока MIME, где символы, такие как "\<", значимых XML, скрыты от анализаторы XML.
    
Каждый уровень вне зависимости от уровня, предшествующего его.
  
Элемент **MimeContentUTF8** может содержать те же данные, содержащие другие свойства, возвращаемые с элементом. 
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
### <a name="version-differences"></a>Различия версий

Этот элемент доступен в версиях Exchange, начиная с построения 15.00.0986.00.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

