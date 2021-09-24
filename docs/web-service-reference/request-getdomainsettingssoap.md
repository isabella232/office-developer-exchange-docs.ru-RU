---
title: Request (GetDomainSettings) (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: 3ea026fc-74f1-4118-86ae-908ed4f82a4b
description: Элемент Request содержит запрос на возвращение параметров домена.
ms.openlocfilehash: fbee6479b844ac9026b0cfc0218cdc542ea0f2fd
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59540547"
---
# <a name="request-getdomainsettings-soap"></a>Request (GetDomainSettings) (SOAP)

Элемент **Request** содержит запрос на возвращение параметров домена. 
  
```xml
<Request>
   <Domains/>
   <RequestedSettings/>
</Request>
```

 **GetDomainSettingsRequest**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Domains (SOAP)](domains-soap.md) <br/> |Представляет домены, конфигурации для которых возвращаются в операции [GetDomainSettings (SOAP)](getdomainsettings-operation-soap.md) или домены, федерационные в операции [GetFederationInformation (SOAP).](getfederationinformation-operation-soap.md)  <br/> |
|[RequestedSettings (SOAP)](requestedsettings-soap.md) <br/> |Содержит имена параметров запрашиваемой конфигурации.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[GetDomainSettingsRequestMessage (SOAP)](getdomainsettingsrequestmessage-soap.md) <br/> |Представляет запрос [на операцию GetDomainSettings (SOAP).](getdomainsettings-operation-soap.md)  <br/> |
   
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

