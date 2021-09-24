---
title: TokenIssuer (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
ms.assetid: 2d7be675-626c-4173-89e9-e32beef81ad5
description: Элемент TokenIssuer указывает Uri (SOAP) и Endpoint (SOAP) для службы маркеров безопасности.
ms.openlocfilehash: ea1c93493e4f47a6f2551c24586e54614f4f45e6
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59527267"
---
# <a name="tokenissuer-soap"></a>TokenIssuer (SOAP)

Элемент **TokenIssuer** указывает [Uri (SOAP)](uri-soap.md) и [Endpoint (SOAP)](endpoint-soap.md) для службы маркеров безопасности. 
  
```XML
<TokenIssuer>
   <Uri/>
   <Endpoint/>
</TokenIssuer>
```

 **TokenIssuer**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Uri (SOAP)](uri-soap.md) <br/> |URI службы маркеров безопасности, выдав маркер безопасности.  <br/> |
|[Endpoint (SOAP)](endpoint-soap.md) <br/> |URI конечной точки веб-службы.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[TokenIssuers (SOAP)](tokenissuers-soap.md) <br/> |Представляет коллекцию службы маркеров безопасности [Uri (SOAP)](uri-soap.md) и [Endpoint (SOAP).](endpoint-soap.md)  <br/> |
   
## <a name="remarks"></a>Заметки

Используйте элемент **TokenIssuer** для указания службы маркеров безопасности при использовании маркеров безопасности. 
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Имя схемы  <br/> |Схема автооткрытия  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |True  <br/> |
   
## <a name="see-also"></a>См. также



[Ссылка на веб-службу автооткрытия для Exchange](autodiscover-web-service-reference-for-exchange.md)
  
[Элементы XML автооткрытия SOAP для Exchange 2013 г.](soap-autodiscover-xml-elements-for-exchange-2013.md)

