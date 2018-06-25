---
title: GetFederationInformationResponse (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 2033c14f-dcc8-43c2-9fd9-a51946ec7055
description: Элемент GetFederationInformationResponse содержит ответа GetFederationInformation операции (SOAP).
ms.openlocfilehash: 28b002b45968278ad4c7160b4eed29721422646d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762788"
---
# <a name="getfederationinformationresponse-soap"></a>GetFederationInformationResponse (SOAP)

Элемент **GetFederationInformationResponse** содержит ответа [GetFederationInformation операции (SOAP)](getfederationinformation-operation-soap.md) . 
  
```XML
<GetFederationInformationResponse>
   <ErrorCode/>
   <ErrorMessage/>
   <TokenIssuers/>
   <ApplicationUri/>
   <Domains/>
</GetFederationInformationResponse>
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
|[TokenIssuers (SOAP)](tokenissuers-soap.md) <br/> |Представляет коллекцию маркеров безопасности, которые содержат идентификаторы службы маркеров безопасности и конечных точек.  <br/> |
|[Домены (SOAP)](domains-soap.md) <br/> |Представляет доменов, конфигурации, для которого возвращаются в ходе операции [GetDomainSettings операции (SOAP)](getdomainsettings-operation-soap.md) **GetDomainSettings** или домены, которым организации федеративных в ходе [операции GetFederationInformation (SOAP)](getfederationinformation-operation-soap.md) Операция **GetFederationInformation** .  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

Нет.
  
## <a name="text-value"></a>Текстовое значение

Нет.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Имя схемы  <br/> |Схема службы автообнаружения  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |True  <br/> |
   
## <a name="see-also"></a>См. также



[Операция GetFederationInformation (SOAP)](getfederationinformation-operation-soap.md)

