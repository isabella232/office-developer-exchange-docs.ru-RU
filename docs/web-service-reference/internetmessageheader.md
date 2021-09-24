---
title: InternetMessageHeader
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- InternetMessageHeader
api_type:
- schema
ms.assetid: c70675f8-6feb-4c89-ba48-bce0479b308b
description: Элемент InternetMessageHeader представляет заголовок интернет-сообщений для данного заголовок в коллекции заголовок. Чтобы получить всю коллекцию заглавных сообщений в Интернете, используйте свойство PR_TRANSPORT_MESSAGE_HEADERS. Дополнительные сведения о руководителях EWS и интернет-сообщений см. в дополнительных сведениях о загонах интернет-сообщений в EWS, MIME и отсутствующих загонах сообщений в Интернете.
ms.openlocfilehash: 4b3072611e8a3debf87ce2a023f4f68ee4487185
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59541086"
---
# <a name="internetmessageheader"></a>InternetMessageHeader

Элемент **InternetMessageHeader** представляет заголовок интернет-сообщений для данного заголовок в коллекции заголовок. Чтобы получить всю коллекцию загона интернет-сообщений, используйте **свойство PR_TRANSPORT_MESSAGE_HEADERS.** Дополнительные сведения о EWS и загонах интернет-сообщений см. в "Получение заглавных сообщений в Интернете в [EWS, MIME и](https://msdn.microsoft.com/library/exchange/hh545614%28v=exchg.140%29.aspx)отсутствующих загонах сообщений в Интернете.
  
```XML
<InternetMessageHeader HeaderName=""/>
```

 **InternetHeaderType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|**HeaderName** <br/> |Определяет имя загона.  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[InternetMessageHeaders](internetmessageheaders.md) <br/> |Представляет коллекцию всех заглавных сообщений в Интернете, содержащихся в элементе в почтовом ящике.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение представляет значение для загона.
  
## <a name="remarks"></a>Заметки

Ниже приводится расширенное определение расширенного свойства управляемого API **PR_TRANSPORT_MESSAGE_HEADERS** EWS. 
  
```cs
ExtendedPropertyDefinition transportMsgHdr = new ExtendedPropertyDefinition(0x007D, MapiPropertyType.String);
```

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


[EWS, MIME и отсутствующие заглавные сообщения в Интернете](https://msdn.microsoft.com/library/exchange/hh545614%28v=exchg.140%29.aspx)

