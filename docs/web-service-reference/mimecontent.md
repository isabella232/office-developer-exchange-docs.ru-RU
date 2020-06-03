---
title: Сохранитьmimecontent
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
description: Элемент Сохранитьmimecontent содержит MIME-поток MIME объекта, представленного в формате base64Binary и поддерживающий [RFC2045].
ms.openlocfilehash: 039ef1245d48e4cf13141970921dd210f4bd7d06
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530438"
---
# <a name="mimecontent"></a>Сохранитьmimecontent

Элемент **сохранитьmimecontent** содержит MIME-поток MIME объекта, представленного в формате base64Binary и поддерживающий [[RFC2045]](http://www.rfc-editor.org/rfc/rfc2045.txt).
  
```xml
<MimeContent CharacterSet="" />
```

 **мимеконтенттипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|**CharacterSet** <br/> |Если этот параметр установлен, то значение этого атрибута игнорируется сервером.  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

Отсутствуют.
  
### <a name="parent-elements"></a>Родительские элементы

[Календаритем](calendaritem.md)  |  [Contact (контакт](contact.md)  |  ) [Дистрибутионлист](distributionlist.md)  |  [Элемент](item.md)  |  [Митингканцеллатион](meetingcancellation.md)  |  [Митингмессаже](meetingmessage.md)  |  [Свойство meetingrequest](meetingrequest.md)  |  [Митингреспонсе](meetingresponse.md)  |  [Message (сообщение](message-ex15websvcsotherref.md)  |  ) [RemoveItem](removeitem.md)  |  [Task (задача](task.md) )
  
## <a name="text-value"></a>Текстовое значение

Текстовое значение, представляющее поток MIME base64Binary, является обязательным при использовании этого элемента.
  
## <a name="remarks"></a>Примечания

Содержимое сообщения проходит через три указанных ниже уровня кодирования, прежде чем он будет сохранен в значении **сохранитьmimecontent** : 
  
1. Текст сообщения — это кодировка текста, например ISO-2022-JP для японских символов.
    
2. Поток MIME — это кодировка ASCII текста сообщения для элемента **сохранитьmimecontent** или кодировка UTF8 текста сообщения для элемента [MimeContentUTF8](mimecontentutf8.md) . 
    
3. XML-документ — это всегда зашифрованный поток ASCII потока MIME, в котором символы, такие как ' \< ', которые являются осмысленными для XML, скрыты из синтаксических анализаторов XML.
    
Каждый уровень не зависит от уровня, который предшествует ему.
  
Элемент **сохранитьmimecontent** может содержать те же данные, что и другие свойства, возвращаемые с элементом. 
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

