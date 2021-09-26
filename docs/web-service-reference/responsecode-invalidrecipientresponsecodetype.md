---
title: ResponseCode (InvalidRecipientResponseCodeType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- ResponseCode
api_type:
- schema
ms.assetid: 582e9caa-d2bc-4be1-a460-739294f9ef18
description: Элемент ResponseCode предоставляет сведения о том, почему получатель является недействительным.
ms.openlocfilehash: 33cd05aca672e250f288aec72d876734132d2e36
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59544810"
---
# <a name="responsecode-invalidrecipientresponsecodetype"></a>ResponseCode (InvalidRecipientResponseCodeType)

Элемент **ResponseCode** предоставляет сведения о том, почему получатель является недействительным. 
  
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

В следующей таблице перечислены возможные значения элемента **ResponseCode.** 
  
|**Code**|**Описание**|
|:-----|:-----|
|OtherError  <br/> |Указывает, что ошибка не указана другим кодом ответа на ошибку.  <br/> |
|RecipientOrganizationNotFederated  <br/> |Указывает, что связь общего доступа недоступна с организацией, указанной в smTP-адресе электронной почты получателя.  <br/> |
|CannotObtainTokenFromSTS  <br/> |Указывает, что возникла проблема с получением маркера безопасности с сервера маркеров.  <br/> |
|SystemPolicyBlocksSharingWithThisRecipient  <br/> |Указывает, что системный администратор установил системную политику, которая блокирует общий доступ к указанному получателю.  <br/> |
|RecipientOrganizationFederatedWithUnknownTokenIssuer  <br/> |Указывает, что служба безопасного маркера, используемая указанным получателем, неизвестна.  <br/> |
   
## <a name="remarks"></a>Заметки

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция GetSharingMetadata](getsharingmetadata-operation.md)


- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

