---
title: GetClientAccessTokenResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 45ca2500-ceab-4c98-9576-cb9e158e5896
description: Элемент GetClientAccessTokenResponseMessage указывает сообщение ответа на запрос GetClientAccessToken.
ms.openlocfilehash: 16fe684dd48f77156ed88d02a6ae7b8f3312cd87
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762714"
---
# <a name="getclientaccesstokenresponsemessage"></a>GetClientAccessTokenResponseMessage

Элемент **GetClientAccessTokenResponseMessage** указывает сообщение ответа на запрос **GetClientAccessToken** . 
  
```XML
<GetClientAccessTokenResponseMessage ResponseClass=" Success | Warning | Error ">
    <Token/>
    <MessageText/>
    <ResponseCode/>
    <DescriptiveLinkKey/>
    <MessageXml/>
</GetClientAccessTokenResponseMessage>
```

 **GetClientAccessTokenResponseMessageType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|ResponseClass  <br/> |Указывает класс ответа.  <br/> |
   
#### <a name="responseclass"></a>ResponseClass

|**Значение**|**Описание**|
|:-----|:-----|
|Успешное выполнение  <br/> |Означает успешное выполнение.  <br/> |
|Предупреждающая  <br/> |Указывает на предупреждение.  <br/> |
|Ошибка  <br/> |Отображается сообщение об ошибке.  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Маркер (ClientAccessTokenType)](token-clientaccesstokentype.md) <br/> |Задает маркер доступа клиентов.  <br/> |
|[DescriptiveLinkKey](descriptivelinkkey.md) <br/> |В настоящее время используется и зарезервировано для будущего использования.  <br/> |
|[MessageText](messagetext.md) <br/> |Предоставляет текстовое описание состояния ответа.  <br/> |
|[MessageXml](messagexml.md) <br/> |Предоставляет дополнительные сведения об ошибке ответа.  <br/> |
|[ResponseCode](responsecode.md) <br/> |Предоставляет сведения о состоянии о запросе.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[ResponseMessages](responsemessages.md) <br/> |Содержит сообщения ответа на запрос веб-служб Exchange (EWS).  <br/> |
   
## <a name="remarks"></a>Замечания

Этот элемент появился в Exchange Server 2013.
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема сообщения  <br/> |
|Файл проверки  <br/> |messages.xsd  <br/> |
|Может быть пустым  <br/> ||
   
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

