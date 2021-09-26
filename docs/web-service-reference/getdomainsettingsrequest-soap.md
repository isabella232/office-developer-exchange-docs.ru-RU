---
title: GetDomainSettingsRequest (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: 5ac0ff6d-9e02-4e4c-973d-cd9e076661d5
description: Элемент GetDomainSettingsRequest представляет запрос операции GetDomainSettings (SOAP).
ms.openlocfilehash: 4c222c6832b5be7da598de3390d13123749f8b0f
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59544994"
---
# <a name="getdomainsettingsrequest-soap"></a>GetDomainSettingsRequest (SOAP)

Элемент **GetDomainSettingsRequest** представляет запрос операции [GetDomainSettings (SOAP).](getdomainsettings-operation-soap.md) 
  
```XML
<GetDomainSettingsRequest>
   <Domains/>
   <RequestedSettings/>
   <RequestedVersion/>
</GetDomainSettingsRequest>
```

 **GetDomainSettingsRequest**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Domains (SOAP)](domains-soap.md) <br/> |Представляет коллекцию идентификаторов домена.  <br/> |
|[RequestedSettings (SOAP)](requestedsettings-soap.md) <br/> |Содержит имена запрашиваемого параметра конфигурации домена.  <br/> |
|[RequestedVersion (SOAP)](requestedversion-soap.md) <br/> |Указывает версию сервера, которую будет использовать поставщик.  <br/> |
   
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



[Операция GetDomainSettings (SOAP)](getdomainsettings-operation-soap.md)

