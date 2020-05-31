---
title: инвалидреЦипиент
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- InvalidRecipient
api_type:
- schema
ms.assetid: 9e2d3433-22d7-444b-9883-e5649297d8fe
description: Элемент ИнвалидреЦипиент содержит SMTP-адрес недопустимого получателя и сведения о том, почему получатель не является допустимым.
ms.openlocfilehash: 800056666e486e9337dcd1c2786f7e6db1e060bb
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833961"
---
# <a name="invalidrecipient"></a>инвалидреЦипиент

Элемент **инвалидреЦипиент** содержит SMTP-адрес недопустимого получателя и сведения о том, почему получатель не является допустимым. 
  
```XML
<InvalidRecipient>
   <SmtpAddress/>
   <ResponseCode/>
   <MessageText/>
</InvalidRecipient>

```

 **инвалидреЦипиенттипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[SmtpAddress](smtpaddress.md) <br/> |Содержит SMTP-адрес недопустимого получателя. Этот элемент обязательный.  <br/> |
|[Респонсекоде (ИнвалидреЦипиентреспонсекодетипе)](responsecode-invalidrecipientresponsecodetype.md) <br/> |Предоставляет код ошибки, определяющий конкретную ошибку, обнаруженную в запросе. Этот элемент обязательный.  <br/> |
|[мессажетекст](messagetext.md) <br/> |Предоставляет текстовое описание состояния отклика. Этот элемент является необязательным.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[инвалидреЦипиентс](invalidrecipients.md) <br/> |Представляет недопустимые получатели запроса на общий доступ к папке.  <br/> |
   
## <a name="remarks"></a>Примечания

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция GetSharingMetadata](getsharingmetadata-operation.md)


- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

