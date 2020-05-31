---
title: InternetMessageHeader
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- InternetMessageHeader
api_type:
- schema
ms.assetid: c70675f8-6feb-4c89-ba48-bce0479b308b
description: Элемент InternetMessageHeader представляет заголовок Интернет-сообщения для данного заголовка в коллекции заголовков. Чтобы получить всю коллекцию заголовков сообщений Интернета, используйте свойство PR_TRANSPORT_MESSAGE_HEADERS. Для получения дополнительных сведений о службах EWS и заголовках сообщений Интернета Сижеттинг в службах EWS, MIME и отсутствующих заголовках сообщений через Интернет.
ms.openlocfilehash: 9457cdabe99c0adcb8183cbc039cc86db881fec7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833952"
---
# <a name="internetmessageheader"></a>InternetMessageHeader

Элемент **InternetMessageHeader** представляет заголовок Интернет-сообщения для данного заголовка в коллекции заголовков. Чтобы получить всю коллекцию заголовков сообщений Интернета, используйте свойство **PR_TRANSPORT_MESSAGE_HEADERS** . Дополнительные сведения о службах EWS и заголовках сообщений в Интернете приведены в статье "как заголовки сообщений Интернета в [EWS, MIME и отсутствующие заголовки сообщений в Интернете](http://msdn.microsoft.com/en-us/library/exchange/hh545614%28v=exchg.140%29.aspx)".
  
```XML
<InternetMessageHeader HeaderName=""/>
```

 **интернесеадертипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|**хеадернаме** <br/> |Определяет имя заголовка.  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[InternetMessageHeaders](internetmessageheaders.md) <br/> |Представляет коллекцию всех заголовков сообщений Интернета, которые находятся в элементе почтового ящика.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение представляет значение заголовка.
  
## <a name="remarks"></a>Примечания

Ниже приведено определение расширенного свойства управляемого API EWS для свойства **PR_TRANSPORT_MESSAGE_HEADERS** . 
  
```cs
ExtendedPropertyDefinition transportMsgHdr = new ExtendedPropertyDefinition(0x007D, MapiPropertyType.String);
```

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


[EWS, MIME и отсутствующие заголовки сообщений Интернета](http://msdn.microsoft.com/en-us/library/exchange/hh545614%28v=exchg.140%29.aspx)

