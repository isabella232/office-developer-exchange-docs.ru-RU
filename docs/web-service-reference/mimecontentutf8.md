---
title: MimeContentUTF8
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 31544c95-5231-4b57-958c-2a689464d29b
description: Элемент MimeContentUTF8 содержит MIME-поток в кодировке UTF-8 объекта, представленный в формате base64Binary и поддерживающий международную связь с адресами электронной почты и [RFC6530].
ms.openlocfilehash: 47599b6634738fd488e5b020f69e36d5fcf550a6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834466"
---
# <a name="mimecontentutf8"></a>MimeContentUTF8

Элемент **MimeContentUTF8** содержит MIME-поток в кодировке UTF-8 объекта, представленный в формате base64Binary и поддерживающий международную связь с адресами электронной почты и [[RFC6530]](http://www.rfc-editor.org/rfc/rfc6530.txt).
  
```XML
<MimeContentUTF8 CharacterSet="" />
```

 **мимеконтенттипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|**CharacterSet** <br/> |Если этот параметр установлен, то значение этого атрибута игнорируется сервером.  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

[Календаритем](calendaritem.md) | [Contact](contact.md) | [Item](item.md) | [Message](message-ex15websvcsotherref.md)[DistributionList](distributionlist.md) |  | [Task](task.md) [MeetingCancellation](meetingcancellation.md) | [RemoveItem](removeitem.md)[MeetingRequest](meetingrequest.md)[MeetingResponse](meetingresponse.md)[MeetingMessage](meetingmessage.md)дистрибутионлист Item | митингканцеллатион митингмессаже свойство meetingrequest | митингреспонсе Message RemoveItem Task |  | 
  
## <a name="text-value"></a>Текстовое значение

Текстовое значение, представляющее поток MIME base64Binary, является обязательным при использовании этого элемента.
  
## <a name="remarks"></a>Примечания

Содержимое сообщения проходит через три указанных ниже уровня кодирования, прежде чем он будет сохранен в значении **MimeContentUTF8** : 
  
1. Текст сообщения — это кодировка текста, например ISO-2022-JP для японских символов.
    
2. Поток MIME — это кодировка UTF8 текста сообщения для элемента **MimeContentUTF8** или кодировка ASCII текста сообщения для элемента [сохранитьmimecontent](mimecontent.md) . 
    
3. XML-документ — это всегда зашифрованный поток ASCII потока MIME, в котором символы, такие как '\<', которые являются осмысленными для XML, скрыты из синтаксических анализаторов XML.
    
Каждый уровень не зависит от уровня, который предшествует ему.
  
Элемент **MimeContentUTF8** может содержать те же данные, что и другие свойства, возвращаемые с элементом. 
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
### <a name="version-differences"></a>Различия версий

Этот элемент доступен в версиях Exchange, начинающихся с сборки 15.00.0986.00.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

