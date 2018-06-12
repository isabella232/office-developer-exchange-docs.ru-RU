---
title: Ответ (GetFederationInformation) (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: ca48a4b3-5006-4bb7-973e-d9137ce67e16
description: Элемент Response с информацией GetFederationInformation операции (SOAP) ответа.
ms.openlocfilehash: 946cba56d7503a0e20ec59640f4f1258c00a844e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19835171"
---
# <a name="response-getfederationinformation-soap"></a>Ответ (GetFederationInformation) (SOAP)

Элемент **ответа** содержит сведения ответа [GetFederationInformation операции (SOAP)](getfederationinformation-operation-soap.md) . 
  
```XML
<Response>
   <ErrorCode/>
   <ErrorMessage/>
   <ApplicationUri/>
   <Domains/>
</Response>
```

 **GetFederationInformationResponse**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Код ошибки (SOAP)](errorcode-soap.md) <br/> |Представляет код ошибки, возвращаемые службой автообнаружения.  <br/> |
|[Сообщение об ошибке (SOAP)](errormessage-soap.md) <br/> |Представляет сообщение, связанное с кодом ошибки, возвращаемые службой автообнаружения.  <br/> |
|[ApplicationUri (SOAP)](applicationuri-soap.md) <br/> |Определяет расположение приложения.  <br/> |
|[Домены (SOAP)](domains-soap.md) <br/> |Представляет коллекцию домена, конфигурации, для которого возвращаются в [операции GetDomainSettings (SOAP)](getdomainsettings-operation-soap.md)или домены, которые организации федеративных в ходе [операции GetFederationInformation (SOAP)](getfederationinformation-operation-soap.md).  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[GetFederationInformationResponseMessage (SOAP)](getfederationinformationresponsemessage-soap.md) <br/> |Определяет ответ на запрос [операции GetFederationInformation (SOAP)](getfederationinformation-operation-soap.md) .  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Нет.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Имя схемы  <br/> |Схема службы автообнаружения  <br/> |
|Файл проверки  <br/> |messages.xsd  <br/> |
|Может быть пустым  <br/> |True  <br/> |
   
## <a name="see-also"></a>См. также



[Операция GetFederationInformation (SOAP)](getfederationinformation-operation-soap.md)

