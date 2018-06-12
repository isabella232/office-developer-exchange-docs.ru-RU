---
title: DomainSetting (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: bad5399c-0762-4979-9c15-58cf4b7b6278
description: Элемент DomainSetting содержит параметры домена, возвращенных по запросу операции GetDomainSettings операции (SOAP).
ms.openlocfilehash: f1c7a30ee221c5f3ca1358d0f3c3aca5c3467159
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762219"
---
# <a name="domainsetting-soap"></a>DomainSetting (SOAP)

Элемент **DomainSetting** содержит параметры домена, возвращенных по запросу операции [операции GetDomainSettings (SOAP)](getdomainsettings-operation-soap.md) . 
  
```XML
<DomainSetting>
   <Name/>
</DomainSetting>
```

 **DomainSetting**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Имя (SOAP)](name-soap.md) <br/> |Представляет имя параметра.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[DomainSettings (SOAP)](domainsettings-soap.md) <br/> |Представляет параметры домена, которые были отправленными в запрос автообнаружения или возвращаемых ответа службы автообнаружения.  <br/> |
   
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

