---
title: DomainResponses (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: d9c7fd91-22cd-4c72-a841-25cb9d415e0c
description: Элемент DomainResponses содержит массив ответов для параметров каждого запрашиваемого домена.
ms.openlocfilehash: 307cae0aca0f34b0a33edd41248f8f572f2a80af
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59540112"
---
# <a name="domainresponses-soap"></a>DomainResponses (SOAP)

Элемент **DomainResponses** содержит массив ответов для параметров каждого запрашиваемого домена. 
  
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
|[DomainResponse (SOAP)](domainresponse-soap.md) <br/> |Содержит заданные параметры для указанного домена.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[GetDomainSettingsResponse (SOAP)](getdomainsettingsresponse-soap.md) <br/> |Представляет ответ на запрос [операции GetDomainSettings (SOAP)](getdomainsettings-operation-soap.md) для домена и возвращает параметры домена.  <br/> |
|[Response (GetDomainSettings) (SOAP)](response-getdomainsettingssoap.md) <br/> |Представляет ответ на вызов [операции GetDomainSettings (SOAP)](getdomainsettings-operation-soap.md) для отдельного домена.  <br/> |
   
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

- [Операция GetDomainSettings (SOAP)](getdomainsettings-operation-soap.md)

