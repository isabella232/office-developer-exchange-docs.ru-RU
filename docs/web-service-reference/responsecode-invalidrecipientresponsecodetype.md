---
title: Респонсекоде (ИнвалидреЦипиентреспонсекодетипе)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ResponseCode
api_type:
- schema
ms.assetid: 582e9caa-d2bc-4be1-a460-739294f9ef18
description: Элемент Респонсекоде предоставляет сведения о причине неправильного получателя.
ms.openlocfilehash: d78de64de7725007ec51a55dad13d1cc892a25e6
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529723"
---
# <a name="responsecode-invalidrecipientresponsecodetype"></a>Респонсекоде (ИнвалидреЦипиентреспонсекодетипе)

Элемент **респонсекоде** предоставляет сведения о причине неправильного получателя. 
  
```XML
<ResponseCode>OtherError or RecipientOrganizationNotFederated or CannotObtainTokenFromSTS or SystemPolicyBlocksSharingWithThisRecipient or RecipientOrganizationFederatedWithUnknownTokenIssuer</ResponseCode>
```

 **инвалидреЦипиентреспонсекодетипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

Отсутствуют.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[инвалидреЦипиент](invalidrecipient.md) <br/> |Содержит SMTP-адрес недопустимого получателя и сведения о почему получатель является недопустимым.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

В следующей таблице приведены возможные значения для элемента **респонсекоде** . 
  
|**Code**|**Описание**|
|:-----|:-----|
|осереррор  <br/> |Указывает на то, что ошибка не указана другим кодом ответа на сообщение об ошибке.  <br/> |
|реЦипиенторганизатионнотфедератед  <br/> |Указывает, что отношение общего доступа недоступно в Организации, указанной в SMTP-адресе электронной почты получателя.  <br/> |
|каннотобтаинтокенфромстс  <br/> |Указывает, что при получении маркера безопасности от сервера маркеров возникла проблема.  <br/> |
|системполициблокксшарингвиссисреЦипиент  <br/> |Указывает, что системный администратор установил системную политику, которая блокирует общий доступ для указанного получателя.  <br/> |
|реЦипиенторганизатионфедератедвисункновнтокениссуер  <br/> |Указывает, что служба безопасного токена, используемая указанным получателем, неизвестна.  <br/> |
   
## <a name="remarks"></a>Примечания

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция GetSharingMetadata](getsharingmetadata-operation.md)


- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

