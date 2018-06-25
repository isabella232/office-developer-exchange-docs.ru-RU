---
title: Запрос автообнаружения POX для Exchange
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 75671b1d-f35b-497b-8d8c-706f3f2535fd
description: Запрос автообнаружения содержит запросов для настройки доступа пользователя клиента.
ms.openlocfilehash: 48d6c30946e75936ed93a6f4507d8a8d3ae47d40
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834865"
---
# <a name="pox-autodiscover-request-for-exchange"></a>Запрос автообнаружения POX для Exchange

Запрос автообнаружения содержит запросов для настройки доступа пользователя клиента.
  
## <a name="autodiscover-request-example"></a>Пример запроса службы автообнаружения

### <a name="description"></a>Описание

В следующем примере XML показано тело запроса службы автообнаружения.
  
### <a name="code"></a>Программа

```XML
<Autodiscover xmlns="http://schemas.microsoft.com/exchange/autodiscover/outlook/requestschema/2006">
   <Request>
     <EMailAddress>user@contoso.com</EMailAddress>
     <AcceptableResponseSchema>http://schemas.microsoft.com/exchange/autodiscover/outlook/responseschema/2006a</AcceptableResponseSchema>
   </Request>
 </Autodiscover>
```

### <a name="request-headers"></a>Заголовки запросов

Следующие заголовки HTTP не являются обязательными при отправке запросов автообнаружения.
  
**В таблице 1. Заголовки HTTP-запроса**

|**Header**|**Описание**|
|:-----|:-----|
|X-MapiHttpCapability  <br/> |Если этот параметр указан и задайте значение «1» указывает, что клиент запрашивает сведения, которые можно использовать для подключения к серверу с помощью протокола MAPI/HTTP. Этот заголовок можно применять для клиентов, использующих протокол MAPI/HTTP.  <br/> |
|X-ClientCanHandle  <br/> |Этот заголовок содержит список разделенных запятой возможности, поддерживаемые клиентом. Допустимые значения указаны в таблице 2.  <br/> |
   
**В таблице 2. Значения заголовка X-ClientCanHandle**

|**Значение X-ClientCanHandle (без учета регистра)**|**Минимальная версия**|**Описание**|
|:-----|:-----|:-----|
|Согласование  <br/> |15.00.0995.014  <br/> |Если это значение — этот параметр указан, сервер в элементе [AuthPackage (POX)](authpackage-pox.md) вернет значение «Согласование», если сервер настроен на прием проверки подлинности согласование. Если это значение не указан, сервер не будет возвращать значение «Согласование» в элементе **AuthPackage** .  <br/> |
|ExHttpInfo  <br/> |15.00.0995.014  <br/> |Если это значение — этот параметр указан, сервер возвращает элемент [Протокола (POX)](protocol-pox.md) с помощью элемента [Типа (POX)](type-pox.md) значение «EXHTTP», если сервер настроен на прием подключений RPC/HTTP. Если это значение не указан, сервер не будет возвращать элемент **протокола** с **типом** элемента, задайте значение «EXHTTP».  <br/> |
   
### <a name="request-elements"></a>Элементы запроса

В тексте запроса используются следующие элементы:
  
- [Автообнаружение (POX)](autodiscover-pox.md)
    
- [Запрос (POX)](request-pox.md)
    
- [AcceptableResponseSchema (POX)](acceptableresponseschema-pox.md)
    
- [EMailAddress (POX)](emailaddress-pox.md)
    
> [!NOTE]
> Элемент [LegacyDN (POX)](legacydn-pox.md) можно использовать вместо элемента [EMailAddress (POX)](emailaddress-pox.md) . 
  
### <a name="version-differences"></a>Различия версий

Заголовок X-MapiHttpCapability доступна в Office 365 и Exchange Online и локальной версии Exchange, начиная с построения 15.00.0847.032 (Exchange Server 2013 с пакетом обновления 1).
  
Заголовок X-ClientCanHandle доступна в Office 365 и Exchange Online и локальной версии Exchange, начиная с построения 15.00.0995.014.
  
## <a name="see-also"></a>См. также



[POX ответа службы автообнаружения для Exchange](pox-autodiscover-response-for-exchange.md)


[Служба POX автоматического обнаружения веб-ссылки для Exchange](pox-autodiscover-web-service-reference-for-exchange.md)
  
[Элементы XML автоматического обнаружения POX для Exchange](pox-autodiscover-xml-elements-for-exchange.md)

