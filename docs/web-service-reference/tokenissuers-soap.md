---
title: TokenIssuers (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
ms.assetid: 26c55228-184e-4340-bd80-f86be56f3e7a
description: Элементы TokenIssuers представляют коллекцию TokenIssuer (SOAP).
ms.openlocfilehash: 68ff3ed515b346a84734596fae6fe127768b4476
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59520404"
---
# <a name="tokenissuers-soap"></a>TokenIssuers (SOAP)

Элементы **TokenIssuers** представляют коллекцию [TokenIssuer (SOAP).](tokenissuer-soap.md) 
  
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
|[TokenIssuer (SOAP)](tokenissuer-soap.md) <br/> |Указывает [Uri (SOAP)](uri-soap.md) и [Endpoint (SOAP)](endpoint-soap.md) для службы маркеров безопасности.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[GetFederationInformationResponse (SOAP)](getfederationinformationresponse-soap.md) <br/> |Содержит [ответ операции GetFederationInformation (SOAP).](getfederationinformation-operation-soap.md)  <br/> |
   
## <a name="remarks"></a>Заметки

**TokenIssuers представляет** коллекцию элементов [TokenIssuer (SOAP),](tokenissuer-soap.md) которые будут использоваться в автооткрытии. 
  
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

