---
title: DomainResponses (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: d9c7fd91-22cd-4c72-a841-25cb9d415e0c
description: Элемент DomainResponses содержит массив ответ для каждого домена запрошенные параметры.
ms.openlocfilehash: 77a3efc1605337ab436f6aea2b61a67f22e4f8ce
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762213"
---
# <a name="domainresponses-soap"></a>DomainResponses (SOAP)

Элемент **DomainResponses** содержит массив ответ для каждого домена запрошенные параметры. 
  
```XML
<DomainResponses>
   <DomainResponse/>
</DomainResponses>
```

 **ArrayOfDomainResponse**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[DomainResponse (SOAP)](domainresponse-soap.md) <br/> |Содержит запрошенные параметры для конкретного домена.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[GetDomainSettingsResponse (SOAP)](getdomainsettingsresponse-soap.md) <br/> |Представляет ответ на запрос [операции GetDomainSettings (SOAP)](getdomainsettings-operation-soap.md) для домена и возвращает параметры домена.  <br/> |
|[Ответ (GetDomainSettings) (SOAP)](response-getdomainsettingssoap.md) <br/> |Представляет ответ на звонок [GetDomainSettings операции (SOAP)](getdomainsettings-operation-soap.md) для отдельного домена.  <br/> |
   
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

- [Операция GetDomainSettings (SOAP)](getdomainsettings-operation-soap.md)

