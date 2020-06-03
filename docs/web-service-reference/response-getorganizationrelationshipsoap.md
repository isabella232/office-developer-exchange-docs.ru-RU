---
title: Отклик (Жеторганизатионрелатионшип) (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: e6bbe800-3cbc-48b2-87b3-2043f575e88b
description: Элемент Response содержит сведения об отклике операции Жеторганизатионрелатионшипсеттингс (SOAP). Элемент Response предназначен только для внутреннего использования. Этот элемент не используется клиентами.
ms.openlocfilehash: 55f8cd549f40b780b2e7438634a851a2c3854f40
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467944"
---
# <a name="response-getorganizationrelationship-soap"></a>Отклик (Жеторганизатионрелатионшип) (SOAP)

Элемент **Response** содержит сведения об отклике [операции жеторганизатионрелатионшипсеттингс (SOAP)](getorganizationrelationshipsettings-operation-soap.md) . Элемент **Response** предназначен только для внутреннего использования. Этот элемент не используется клиентами. 
  
```XML
<GetOrganizationRelationshipSettingsResponse>
   <ErrorCode/>
   <ErrorMessage/>
   <OrganizationRelationshipSettingsCollection/>
</GetOrganizationRelationshipSettingResponse>
```

 **жеторганизатионрелатионшипсеттингсреспонсе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[ErrorCode (SOAP)](errorcode-soap.md) <br/> |Представляет код ошибки, возвращенный службой автообнаружения.  <br/> |
|[ErrorMessage (SOAP)](errormessage-soap.md) <br/> |Представляет сообщение, связанное с кодом ошибки, возвращаемым службой автообнаружения.  <br/> |
|[Организатионрелатионшипсеттингсколлектион (SOAP)](organizationrelationshipsettingscollection-soap.md) <br/> |Представляет список отношений Организации, которые совпадают с запросом.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

Отсутствуют.
  
## <a name="text-value"></a>Текстовое значение

Отсутствуют.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Имя схемы  <br/> |Схема автообнаружения  <br/> |
|Файл проверки  <br/> |Messages. xsd  <br/> |
|Может быть пустым  <br/> |True  <br/> |
   
## <a name="see-also"></a>См. также



[Операция Жеторганизатионрелатионшипсеттингс (SOAP)](getorganizationrelationshipsettings-operation-soap.md)

