---
title: FreeBusyAccessEnabled (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
ms.assetid: 8d2d3276-b180-424e-a707-7256d14a1776
description: Элемент FreeBusyAccessEnabled представляет флаг FreeBusyAccessEnabled(). Элемент FreeBusyAccessEnabled используется только для внутреннего использования. Этот элемент не используется клиентами.
ms.openlocfilehash: faf51798ba211b4219a3f2abee3b3e5e9ce4ab29
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59530222"
---
# <a name="freebusyaccessenabled-soap"></a>FreeBusyAccessEnabled (SOAP)

Элемент **FreeBusyAccessEnabled** представляет флаг **FreeBusyAccessEnabled().** Элемент **FreeBusyAccessEnabled** используется только для внутреннего использования. Этот элемент не используется клиентами. 
  
```XML
<FreeBusyAccessEnabled>true | false</FreeBusyAccessEnabled>
```

 **Boolean**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[OrganizationRelationshipSettings (SOAP)](organizationrelationshipsettings-soap.md) <br/> |Представляет список отношений организации для одной организации.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение, истинное для элемента **FreeBusyAccessEnabled,** указывает на то, что связь общего доступа должна использоваться для получения бесплатных загруженных сведений от пользователей в организации.  Значение false **указывает** на то, что связь общего доступа должна быть подавлена. 
  
## <a name="remarks"></a>Заметки

Используйте этот элемент, чтобы разрешить или подавлять бесплатные или загруженные сведения с сервера. 
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Имя схемы  <br/> |Схема автооткрытия  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |True  <br/> |
   
## <a name="see-also"></a>См. также



[Операция GetOrganizationRelationshipSettings (SOAP)](getorganizationrelationshipsettings-operation-soap.md)

