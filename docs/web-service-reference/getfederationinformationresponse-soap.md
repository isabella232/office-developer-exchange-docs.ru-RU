---
title: GetFederationInformationResponse (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: 2033c14f-dcc8-43c2-9fd9-a51946ec7055
description: Элемент GetFederationInformationResponse содержит ответ операции GetFederationInformation (SOAP).
ms.openlocfilehash: 20d00f047acae6c9eba1347ae7e8110656fefb4b
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59529881"
---
# <a name="getfederationinformationresponse-soap"></a>GetFederationInformationResponse (SOAP)

Элемент **GetFederationInformationResponse** содержит ответ [операции GetFederationInformation (SOAP).](getfederationinformation-operation-soap.md) 
  
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
|[ErrorCode (SOAP)](errorcode-soap.md) <br/> |Представляет код ошибки, возвращаемый службой автооткрытия.  <br/> |
|[ErrorMessage (SOAP)](errormessage-soap.md) <br/> |Представляет сообщение, связанное с кодом ошибки, который возвращается службой автооткрытия.  <br/> |
|[ApplicationUri (SOAP)](applicationuri-soap.md) <br/> |Определяет расположение приложения.  <br/> |
|[TokenIssuers (SOAP)](tokenissuers-soap.md) <br/> |Представляет коллекцию маркеров безопасности, содержащих идентификаторы и конечные точки службы маркеров безопасности.  <br/> |
|[Domains (SOAP)](domains-soap.md) <br/> |Представляет домены, конфигурации для которых возвращаются в операции [GetDomainSettings (SOAP)](getdomainsettings-operation-soap.md) **GetDomainSettings** или домены, федерационные в операции [GetFederationInformation (SOAP)](getfederationinformation-operation-soap.md) **GetFederationInformation.**  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

Нет.
  
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



[Операция GetFederationInformation (SOAP)](getfederationinformation-operation-soap.md)

