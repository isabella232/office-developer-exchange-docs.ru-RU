---
title: FindMailboxStatisticsByKeywordsResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: d3835800-8887-43db-9a8a-fe3cfea7a863
description: Элемент FindMailboxStatisticsByKeywordsResponseMessage указывает сообщение ответа на запрос FindMailboxStatisticsByKeywords.
ms.openlocfilehash: f41a44ebb90b59c7458162dffe445bbeba7c2ba0
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59513719"
---
# <a name="findmailboxstatisticsbykeywordsresponsemessage"></a>FindMailboxStatisticsByKeywordsResponseMessage

Элемент **FindMailboxStatisticsByKeywordsResponseMessage** указывает сообщение ответа на запрос **FindMailboxStatisticsByKeywords.** 
  
```XML
<FindMailboxStatisticsByKeywordsResponseMessage ResponseClass=" Success | Warning | Error ">
    <MailboxStatisticsSearchResult/>
    <MessageText/>
    <ResponseCode/>
    <DescriptiveLinkKey/>
    <MessageXml/>
</FindMailboxStatisticsByKeywordsResponseMessage>
```

 **FindMailboxStatisticsByKeywordsResponseMessageType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|ResponseClass  <br/> |Указывает класс отклика.  <br/> |
   
#### <a name="responseclass"></a>ResponseClass

|**Значение**|**Описание**|
|:-----|:-----|
|Успешно  <br/> |Указывает на успех.  <br/> |
|Предупреждение  <br/> |Указывает предупреждение.  <br/> |
|Error  <br/> |Указывает на ошибку.  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[MailboxStatisticsSearchResult](mailboxstatisticssearchresult.md) <br/> |Указывает результат поиска почтовых ящиков.  <br/> |
|[MessageText](messagetext.md) <br/> |Предоставляет текстовое описание состояния отклика.  <br/> |
|[ResponseCode](responsecode.md) <br/> |Предоставляет сведения о состоянии запроса.  <br/> |
|[DescriptiveLinkKey](descriptivelinkkey.md) <br/> |В настоящее время неиспользированы и зарезервированы для использования в будущем.  <br/> |
|[MessageXml](messagexml.md) <br/> |Предоставляет дополнительные сведения об отклике с ошибкой.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[ResponseMessages](responsemessages.md) <br/> |Указывает массив ответных сообщений.  <br/> |
   
## <a name="remarks"></a>Заметки

Этот элемент появился в Exchange Server 2013.
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема сообщения  <br/> |
|Файл проверки  <br/> |messages.xsd  <br/> |
|Может быть пустым  <br/> ||
   
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

