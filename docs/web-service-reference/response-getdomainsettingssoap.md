---
title: Response (GetDomainSettings) (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: a5b052df-93bd-4fe1-ac30-83de9a3dfcd7
description: Элемент Response представляет ответ на вызов GetDomainSettings для отдельного домена.
ms.openlocfilehash: e8f76127d5e812bc6805430544fe334eabd29ffa
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59540554"
---
# <a name="response-getdomainsettings-soap"></a>Response (GetDomainSettings) (SOAP)

Элемент **Response** представляет ответ на вызов **GetDomainSettings для** отдельного домена. 
  
```XML
<Response>
   <DomainResponses/>
   <ErrorCode/>
   <ErrorMessage/>
</Response>
```

 **GetDomainSettingsResponse**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[DomainResponses (SOAP)](domainresponses-soap.md) <br/> |Содержит ответ для каждого домена, запрашиваемой в **запросе GetDomainSettings.**  <br/> |
|[ErrorCode (SOAP)](errorcode-soap.md) <br/> |Содержит код ошибки, связанный с ответом, если это применимо.  <br/> |
|[ErrorMessage (SOAP)](errormessage-soap.md) <br/> |Содержит сообщение об ошибке, связанное с ответом, если применимо.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[GetDomainSettingsResponseMessage (SOAP)](getdomainsettingsresponsemessage-soap.md) <br/> |Возвращает звоняму параметры конфигурации домена.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Нет.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Имя схемы  <br/> |Схема автооткрытия  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |True  <br/> |
   
## <a name="see-also"></a>См. также



[Операция GetDomainSettings (SOAP)](getdomainsettings-operation-soap.md)

