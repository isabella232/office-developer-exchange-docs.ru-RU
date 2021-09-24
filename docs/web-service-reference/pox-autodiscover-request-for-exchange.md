---
title: Запрос автооткрытия POX для Exchange
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: 75671b1d-f35b-497b-8d8c-706f3f2535fd
description: Запрос автооткрытия содержит запрос для конфигурации клиентского доступа пользователя.
ms.openlocfilehash: 8a0960dcff21276baf723512befacc4eca35950f
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59523868"
---
# <a name="pox-autodiscover-request-for-exchange"></a>Запрос автооткрытия POX для Exchange

Запрос автооткрытия содержит запрос для конфигурации клиентского доступа пользователя.
  
## <a name="autodiscover-request-example"></a>Пример запроса автооткрытия

### <a name="description"></a>Описание

В следующем примере XML показан орган запроса автонаружения.
  
### <a name="code"></a>Код

```XML
<Autodiscover xmlns="https://schemas.microsoft.com/exchange/autodiscover/outlook/requestschema/2006">
   <Request>
     <EMailAddress>user@contoso.com</EMailAddress>
     <AcceptableResponseSchema>https://schemas.microsoft.com/exchange/autodiscover/outlook/responseschema/2006a</AcceptableResponseSchema>
   </Request>
 </Autodiscover>
```

### <a name="request-headers"></a>Запрашивать заглавные

Следующие http-заголовки необязательны при отправке запросов автооткрытия.
  
**Таблица 1. Http request headers**

|**Header**|**Описание**|
|:-----|:-----|
|X-MapiHttpCapability  <br/> |Если присутствует и задается "1", указывает, что клиент запрашивает сведения, которые можно использовать для подключения к серверу с помощью протокола MAPI/HTTP. Этот заголик применим к клиентам, реализуемым протоколу MAPI/HTTP.  <br/> |
|X-ClientCanHandle  <br/> |В этом загородных загонах содержится список возможностей, поддерживаемых клиентом. Возможные значения указаны в таблице 2.  <br/> |
   
**Таблица 2. Значения загона X-ClientCanHandle**

|**Значение X-ClientCanHandle (нечувствительный к делу)**|**Минимальная версия сервера**|**Описание**|
|:-----|:-----|:-----|
|Согласование  <br/> |15.00.0995.014  <br/> |Если это значение присутствует, сервер возвращает значение "Согласование" в [элементе AuthPackage (POX),](authpackage-pox.md) если сервер настроен на согласование проверки подлинности. Если этого значения нет, сервер не возвращает значение "Negotiate" в **элементе AuthPackage.**  <br/> |
|ExHttpInfo  <br/> |15.00.0995.014  <br/> |Если это значение присутствует, сервер возвращает элемент [Protocol (POX)](protocol-pox.md) с элементом [Type (POX)](type-pox.md) с набором "EXHTTP", если сервер настроен на прием подключений RPC/HTTP. Если этого значения нет, сервер не возвращает элемент **Протокол** с элементом **Type,** заданной "EXHTTP".  <br/> |
   
### <a name="request-elements"></a>Элементы запроса

В теле запроса используются следующие элементы:
  
- [AutoDiscover (POX)](autodiscover-pox.md)
    
- [Request (POX)](request-pox.md)
    
- [AcceptableResponseSchema (POX)](acceptableresponseschema-pox.md)
    
- [EMailAddress (POX)](emailaddress-pox.md)
    
> [!NOTE]
> Элемент [LegacyDN (POX)](legacydn-pox.md) может использоваться на месте элемента [EMailAddress (POX).](emailaddress-pox.md) 
  
### <a name="version-differences"></a>Различия версий

Загон X-MapiHttpCapability доступен в Office 365, Exchange Online и локальной версии Exchange начиная с сборки 15.00.0847.032 (Exchange Server 2013 SP1).
  
Загон X-ClientCanHandle доступен в Office 365, Exchange Online и локальной версии Exchange начиная с сборки 15.00.0995.014.
  
## <a name="see-also"></a>См. также



[Ответ автооткрытия POX для Exchange](pox-autodiscover-response-for-exchange.md)


[Ссылка веб-службы автооткрытия POX для Exchange](pox-autodiscover-web-service-reference-for-exchange.md)
  
[Элементы XML автооткрытия POX для Exchange](pox-autodiscover-xml-elements-for-exchange.md)

