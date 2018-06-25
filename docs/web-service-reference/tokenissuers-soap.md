---
title: TokenIssuers (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 26c55228-184e-4340-bd80-f86be56f3e7a
description: Элементы TokenIssuers представляет коллекцию TokenIssuer (SOAP).
ms.openlocfilehash: b070d85b32d5bce8461ac4e930329f237885bad7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19840208"
---
# <a name="tokenissuers-soap"></a>TokenIssuers (SOAP)

Элементы **TokenIssuers** представляет коллекцию [TokenIssuer (SOAP)](tokenissuer-soap.md) . 
  
```XML
<TokenIssuers>
    <TokenIssuer/>
</TokenIssuers>
```

 **TokenIssuers**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[TokenIssuer (SOAP)](tokenissuer-soap.md) <br/> |Указывает [Uri (SOAP)](uri-soap.md) и [Конечной точки (SOAP)](endpoint-soap.md) для службы маркеров безопасности.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[GetFederationInformationResponse (SOAP)](getfederationinformationresponse-soap.md) <br/> |Содержит ответ [GetFederationInformation операции (SOAP)](getfederationinformation-operation-soap.md) .  <br/> |
   
## <a name="remarks"></a>Замечания

**TokenIssuers** представляет коллекцию элементов [TokenIssuer (SOAP)](tokenissuer-soap.md) для использования в автоматического обнаружения. 
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Имя схемы  <br/> |Схема службы автообнаружения  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |True  <br/> |
   
## <a name="see-also"></a>См. также



[Ссылки веб-службу автообнаружения для Exchange](autodiscover-web-service-reference-for-exchange.md)
  
[Элементы XML автоматического обнаружения SOAP для Exchange 2013](soap-autodiscover-xml-elements-for-exchange-2013.md)

