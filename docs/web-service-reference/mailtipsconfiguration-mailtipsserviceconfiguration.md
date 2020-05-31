---
title: Маилтипсконфигуратион (Маилтипссервицеконфигуратион)
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
description: Элемент Маилтипсконфигуратион содержит сведения о конфигурации службы для почтовых подсказок.
ms.openlocfilehash: ea92af3ebb2d2f720e5823c5317d09d5bcdb3978
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834321"
---
# <a name="mailtipsconfiguration-mailtipsserviceconfiguration"></a>Маилтипсконфигуратион (Маилтипссервицеконфигуратион)

Элемент **маилтипсконфигуратион** содержит сведения о конфигурации службы для почтовых подсказок. 
  
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

 **маилтипссервицеконфигуратион**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[маилтипсенаблед](mailtipsenabled.md) <br/> |Указывает, доступна ли служба советов по работе с почтой. Этот элемент обязательный.  <br/> |
|[максреЦипиентспержетмаилтипсрекуест](maxrecipientspergetmailtipsrequest.md) <br/> |Указывает максимальное количество получателей, которые могут быть переданы в операцию с помощью [подсказок](getmailtips-operation.md). Этот элемент обязательный.  <br/> |
|[MaxMessageSize](maxmessagesize.md) <br/> |Представляет максимальный размер сообщения, которое может принимать получатель. Этот элемент обязательный.  <br/> |
|[ларжеаудиенцесрешолд](largeaudiencethreshold.md) <br/> |Представляет пороговое значение большой аудитории для клиента. Этот элемент обязательный.  <br/> |
|[шовекстерналреЦипиенткаунт](showexternalrecipientcount.md) <br/> |Указывает, должны ли потребители [операции](getmailtips-operation.md) с подсказками отображать подсказки для почты, указывающие количество внешних получателей, на которые адресовано сообщение. Этот элемент обязательный.  <br/> |
|[Имена внутренних доменов (Смтпдомаинлист)](internaldomains-smtpdomainlist.md) <br/> |Определяет список внутренних доменов SMTP Организации. Этот элемент обязательный.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[сервицеконфигуратионреспонсемессажетипе](serviceconfigurationresponsemessagetype.md) <br/> |Содержит параметры конфигурации службы.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Нет.
  
## <a name="remarks"></a>Примечания

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

