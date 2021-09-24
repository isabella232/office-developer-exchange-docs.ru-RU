---
title: Response (GetOrganizationRelationship) (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
ms.assetid: e6bbe800-3cbc-48b2-87b3-2043f575e88b
description: Элемент Response содержит сведения о реагировании на операции GetOrganizationRelationshipSettings (SOAP). Элемент Response используется только для внутреннего использования. Этот элемент не используется клиентами.
ms.openlocfilehash: 4aed4721fd443c5068055f4d802793e7cd1be14d
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59514153"
---
# <a name="response-getorganizationrelationship-soap"></a>Response (GetOrganizationRelationship) (SOAP)

Элемент **Response** содержит сведения о реагировании [на операции GetOrganizationRelationshipSettings (SOAP).](getorganizationrelationshipsettings-operation-soap.md) Элемент **Response** используется только для внутреннего использования. Этот элемент не используется клиентами. 
  
```XML
<GetOrganizationRelationshipSettingsResponse>
   <ErrorCode/>
   <ErrorMessage/>
   <OrganizationRelationshipSettingsCollection/>
</GetOrganizationRelationshipSettingResponse>
```

 **GetOrganizationRelationshipSettingsResponse**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[ErrorCode (SOAP)](errorcode-soap.md) <br/> |Представляет код ошибки, возвращаемый службой автооткрытия.  <br/> |
|[ErrorMessage (SOAP)](errormessage-soap.md) <br/> |Представляет сообщение, связанное с кодом ошибки, который возвращается службой автооткрытия.  <br/> |
|[OrganizationRelationshipSettingsCollection (SOAP)](organizationrelationshipsettingscollection-soap.md) <br/> |Представляет список организаций, которые соответствуют запросу.  <br/> |
   
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



[Операция GetOrganizationRelationshipSettings (SOAP)](getorganizationrelationshipsettings-operation-soap.md)

