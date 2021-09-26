---
title: GetHoldOnMailboxesResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 0f7d0d90-d418-4ce9-8cea-afe8f14728c3
description: Элемент GetHoldOnMailboxesResponseMessage указывает сообщение ответа для запроса GetHoldOnMailboxes.
ms.openlocfilehash: 124975139f901f6e54a29a447455b89fc0272aa7
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59546282"
---
# <a name="getholdonmailboxesresponsemessage"></a>GetHoldOnMailboxesResponseMessage

Элемент **GetHoldOnMailboxesResponseMessage** указывает сообщение ответа для запроса **GetHoldOnMailboxes.** 
  
```XML
<GetHoldOnMailboxesResponseMessage ResponseClass=" Success | Warning | Error ">
    <MailboxHoldResult/>
    <MessageText/>
    <ResponseCode/>
    <DescriptiveLinkKey/>
    <MessageXml/>
</GetHoldOnMailboxesResponseMessage>
```

 **GetHoldOnMailboxesResponseMessageType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|ResponseClass  <br/> |Указывает класс ответа.  <br/> |
   
#### <a name="responseclass"></a>ResponseClass

|**Значение**|**Описание**|
|:-----|:-----|
|Успешно  <br/> |Указывает на успех.  <br/> |
|Предупреждение  <br/> |Указывает предупреждение.  <br/> |
|Error  <br/> |Указывает на ошибку.  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[MailboxHoldResult](mailboxholdresult.md) <br/> |Содержит результат запроса **GetHoldOnMailboxes.**  <br/> |
|[DescriptiveLinkKey](descriptivelinkkey.md) <br/> |В настоящее время неиспользированы и зарезервированы для использования в будущем.  <br/> |
|[MessageText](messagetext.md) <br/> |Предоставляет текстовое описание состояния отклика.  <br/> |
|[MessageXml](messagexml.md) <br/> |Предоставляет дополнительные сведения об отклике с ошибкой.  <br/> |
|[ResponseCode](responsecode.md) <br/> |Предоставляет сведения о состоянии запроса.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[ResponseMessages](responsemessages.md) <br/> |Содержит сообщения ответа для запроса Exchange веб-служб (EWS).  <br/> |
   
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

