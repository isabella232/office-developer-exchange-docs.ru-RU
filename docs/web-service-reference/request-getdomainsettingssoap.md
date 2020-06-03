---
title: Request (Жетдомаинсеттингс) (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 3ea026fc-74f1-4118-86ae-908ed4f82a4b
description: Элемент Request содержит запрос на возврат параметров домена.
ms.openlocfilehash: c5f666102be8aaeee001a23706732e9e6c44b560
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459590"
---
# <a name="request-getdomainsettings-soap"></a>Request (Жетдомаинсеттингс) (SOAP)

Элемент **request** содержит запрос на возврат параметров домена. 
  
```xml
<Request>
   <Domains/>
   <RequestedSettings/>
</Request>
```

 **жетдомаинсеттингсрекуест**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Домены (SOAP)](domains-soap.md) <br/> |Представляет домены конфигурации, для которых в операции [жетдомаинсеттингс (SOAP)](getdomainsettings-operation-soap.md) или доменах, в которых Организация имеет Федеративные результаты, в [операции жетфедератионинформатион (SOAP)](getfederationinformation-operation-soap.md).  <br/> |
|[Рекуестедсеттингс (SOAP)](requestedsettings-soap.md) <br/> |Содержит имена запрошенных параметров конфигурации.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Жетдомаинсеттингсрекуестмессаже (SOAP)](getdomainsettingsrequestmessage-soap.md) <br/> |Представляет запрос [операции жетдомаинсеттингс (SOAP)](getdomainsettings-operation-soap.md).  <br/> |
   
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



[Операция Жетдомаинсеттингс (SOAP)](getdomainsettings-operation-soap.md)

