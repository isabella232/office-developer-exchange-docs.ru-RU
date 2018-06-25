---
title: ResponseCode (InvalidRecipientResponseCodeType)
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
description: Элемент ResponseCode предоставляет сведения о почему получатель является недопустимым.
ms.openlocfilehash: 3bff99dd1ac6603ce31d5ceb074e73ef48190bb2
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835186"
---
# <a name="responsecode-invalidrecipientresponsecodetype"></a>ResponseCode (InvalidRecipientResponseCodeType)

Элемент **ResponseCode** предоставляет сведения о почему получатель является недопустимым. 
  
```XML
<ResponseCode>OtherError or RecipientOrganizationNotFederated or CannotObtainTokenFromSTS or SystemPolicyBlocksSharingWithThisRecipient or RecipientOrganizationFederatedWithUnknownTokenIssuer</ResponseCode>
```

 **InvalidRecipientResponseCodeType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[InvalidRecipient](invalidrecipient.md) <br/> |Содержит SMTP-адрес недопустимого получателя и сведения о почему получатель является недопустимым.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

В следующей таблице приведены возможные значения для элемента **ResponseCode** . 
  
|**Код**|**Описание**|
|:-----|:-----|
|OtherError  <br/> |Указывает, что ошибки не указан с другой код ошибки.  <br/> |
|RecipientOrganizationNotFederated  <br/> |Указывает, что отношение общего доступа не доступен с организацией, указанного в поле адрес электронной почты получателя SMTP.  <br/> |
|CannotObtainTokenFromSTS  <br/> |Указывает, что возникла проблема получение маркера безопасности на основе сервера маркеров.  <br/> |
|SystemPolicyBlocksSharingWithThisRecipient  <br/> |Указывает, что системный администратор значение системной политики, который блокирует общий доступ для указанного получателя.  <br/> |
|RecipientOrganizationFederatedWithUnknownTokenIssuer  <br/> |Указывает, что службы маркеров безопасности, используемый для указанного получателя неизвестно.  <br/> |
   
## <a name="remarks"></a>Замечания

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция GetSharingMetadata](getsharingmetadata-operation.md)


- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

