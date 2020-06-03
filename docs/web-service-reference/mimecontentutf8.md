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
ms.openlocfilehash: a9214bda876c1aadac5b026b3adf38faea8ef17a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530431"
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

Отсутствуют.
  
### <a name="parent-elements"></a>Родительские элементы

[Календаритем](calendaritem.md)  |  [Contact (контакт](contact.md)  |  ) [Дистрибутионлист](distributionlist.md)  |  [Элемент](item.md)  |  [Митингканцеллатион](meetingcancellation.md)  |  [Митингмессаже](meetingmessage.md)  |  [Свойство meetingrequest](meetingrequest.md)  |  [Митингреспонсе](meetingresponse.md)  |  [Message (сообщение](message-ex15websvcsotherref.md)  |  ) [RemoveItem](removeitem.md)  |  [Task (задача](task.md) )
  
## <a name="text-value"></a>Текстовое значение

Текстовое значение, представляющее поток MIME base64Binary, является обязательным при использовании этого элемента.
  
## <a name="remarks"></a>Примечания

Содержимое сообщения проходит через три указанных ниже уровня кодирования, прежде чем он будет сохранен в значении **MimeContentUTF8** : 
  
1. Текст сообщения — это кодировка текста, например ISO-2022-JP для японских символов.
    
2. Поток MIME — это кодировка UTF8 текста сообщения для элемента **MimeContentUTF8** или кодировка ASCII текста сообщения для элемента [сохранитьmimecontent](mimecontent.md) . 
    
3. XML-документ — это всегда зашифрованный поток ASCII потока MIME, в котором символы, такие как ' \< ', которые являются осмысленными для XML, скрыты из синтаксических анализаторов XML.
    
Каждый уровень не зависит от уровня, который предшествует ему.
  
Элемент **MimeContentUTF8** может содержать те же данные, что и другие свойства, возвращаемые с элементом. 
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
### <a name="version-differences"></a>Различия версий

Этот элемент доступен в версиях Exchange, начинающихся с сборки 15.00.0986.00.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

