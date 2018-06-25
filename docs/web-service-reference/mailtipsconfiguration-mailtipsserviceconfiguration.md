---
title: MailTipsConfiguration (MailTipsServiceConfiguration)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MailTipsConfiguration
api_type:
- schema
ms.assetid: 9a34515e-815b-4c61-b118-d5f66b80238f
description: Элемент MailTipsConfiguration содержит сведения о конфигурации службы для службы советы почты.
ms.openlocfilehash: ea92af3ebb2d2f720e5823c5317d09d5bcdb3978
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834321"
---
# <a name="mailtipsconfiguration-mailtipsserviceconfiguration"></a>MailTipsConfiguration (MailTipsServiceConfiguration)

Элемент **MailTipsConfiguration** содержит сведения о конфигурации службы для службы советы почты. 
  
```XML
<MailTipsConfiguration>
   <MailTipsEnabled/>
   <MaxRecipientsPerGetMailTipsRequest/>
   <MaxMessageSize/>
   <LargeAudienceThreshold/>
   <ShowExternalRecipientCount/>
   <InternalDomains/>
</MailTipsConfiguration>
```

 **MailTipsServiceConfiguration**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[MailTipsEnabled](mailtipsenabled.md) <br/> |Указывает, доступна ли служба советы почты. Этот элемент обязательный.  <br/> |
|[MaxRecipientsPerGetMailTipsRequest](maxrecipientspergetmailtipsrequest.md) <br/> |Указывает максимальное количество получателей, которые могут передаваться [GetMailTips операции](getmailtips-operation.md). Этот элемент обязательный.  <br/> |
|[MaxMessageSize](maxmessagesize.md) <br/> |Представляет максимальный размер сообщения, можно принять получателя. Этот элемент обязательный.  <br/> |
|[LargeAudienceThreshold](largeaudiencethreshold.md) <br/> |Представляет большая аудитория пороговое значение для клиента. Этот элемент обязательный.  <br/> |
|[ShowExternalRecipientCount](showexternalrecipientcount.md) <br/> |Указывает ли объекты-получатели [GetMailTips операции](getmailtips-operation.md) для отображения почтовые подсказки, которые указывают число внешних получателей, к которым адресовано сообщение. Этот элемент обязательный.  <br/> |
|[InternalDomains (SmtpDomainList)](internaldomains-smtpdomainlist.md) <br/> |Определяет список внутренних доменов SMTP организации. Этот элемент обязательный.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[ServiceConfigurationResponseMessageType](serviceconfigurationresponsemessagetype.md) <br/> |Содержит параметры конфигурации службы.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Нет.
  
## <a name="remarks"></a>Замечания

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

