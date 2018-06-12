---
title: GetDomainSettingsRequest (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 5ac0ff6d-9e02-4e4c-973d-cd9e076661d5
description: Элемент GetDomainSettingsRequest представляет запрос операции GetDomainSettings операции (SOAP).
ms.openlocfilehash: 4de525a9ba47a0d9afb0d6db9200fe32845f31d0
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762755"
---
# <a name="getdomainsettingsrequest-soap"></a>GetDomainSettingsRequest (SOAP)

Элемент **GetDomainSettingsRequest** представляет запрос операции [GetDomainSettings операции (SOAP)](getdomainsettings-operation-soap.md) . 
  
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
|[Домены (SOAP)](domains-soap.md) <br/> |Представляет коллекцию идентификаторов домена.  <br/> |
|[RequestedSettings (SOAP)](requestedsettings-soap.md) <br/> |Содержит имена параметров конфигурации запрошенного домена.  <br/> |
|[RequestedVersion (SOAP)](requestedversion-soap.md) <br/> |Указывает версию сервера, который будет использоваться поставщик.  <br/> |
   
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



[Операция GetDomainSettings (SOAP)](getdomainsettings-operation-soap.md)

