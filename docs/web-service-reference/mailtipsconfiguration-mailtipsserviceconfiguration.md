---
title: MailTipsConfiguration (MailTipsServiceConfiguration)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- MailTipsConfiguration
api_type:
- schema
ms.assetid: 9a34515e-815b-4c61-b118-d5f66b80238f
description: Элемент MailTipsConfiguration содержит сведения о конфигурации службы для службы советов почты.
ms.openlocfilehash: eb86291572f6854710d01badcee2db24406844c6
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59524037"
---
# <a name="mailtipsconfiguration-mailtipsserviceconfiguration"></a>MailTipsConfiguration (MailTipsServiceConfiguration)

Элемент **MailTipsConfiguration содержит** сведения о конфигурации службы для службы советов почты. 
  
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
|[MailTipsEnabled](mailtipsenabled.md) <br/> |Указывает, доступна ли служба советов почты. Этот элемент обязательный.  <br/> |
|[MaxRecipientsPerGetMailTipsRequest](maxrecipientspergetmailtipsrequest.md) <br/> |Указывает максимальное число получателей, которые могут быть переданы в [операцию GetMailTips.](getmailtips-operation.md) Этот элемент обязательный.  <br/> |
|[MaxMessageSize](maxmessagesize.md) <br/> |Представляет максимальный размер сообщения, который может принять получатель. Этот элемент обязательный.  <br/> |
|[LargeAudienceThreshold](largeaudiencethreshold.md) <br/> |Представляет порог большой аудитории для клиента. Этот элемент обязательный.  <br/> |
|[ShowExternalRecipientCount](showexternalrecipientcount.md) <br/> |Указывает, должны ли пользователи операции [GetMailTips](getmailtips-operation.md) показывать советы по почте, которые указывают количество внешних получателей, к которым адресовано сообщение. Этот элемент обязательный.  <br/> |
|[InternalDomains (SmtpDomainList)](internaldomains-smtpdomainlist.md) <br/> |Определяет список внутренних доменов SMTP организации. Этот элемент обязательный.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[ServiceConfigurationResponseMessageType](serviceconfigurationresponsemessagetype.md) <br/> |Содержит параметры конфигурации службы.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Нет.
  
## <a name="remarks"></a>Заметки

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

