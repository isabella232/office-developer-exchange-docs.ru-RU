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
description: Запрос автообнаружения содержит запрос для конфигурации клиентского доступа пользователя.
ms.openlocfilehash: b2138f9813c7b75aef9afb90089b9b874aac7532
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461669"
---
# <a name="pox-autodiscover-request-for-exchange"></a>Запрос автообнаружения POX для Exchange

Запрос автообнаружения содержит запрос для конфигурации клиентского доступа пользователя.
  
## <a name="autodiscover-request-example"></a>Пример запроса автообнаружения

### <a name="description"></a>Description

В приведенном ниже примере XML-кода показан текст запроса автообнаружения.
  
### <a name="code"></a>Код

```XML
<Autodiscover xmlns="https://schemas.microsoft.com/exchange/autodiscover/outlook/requestschema/2006">
   <Request>
     <EMailAddress>user@contoso.com</EMailAddress>
     <AcceptableResponseSchema>https://schemas.microsoft.com/exchange/autodiscover/outlook/responseschema/2006a</AcceptableResponseSchema>
   </Request>
 </Autodiscover>
```

### <a name="request-headers"></a>Заголовки запросов

Следующие заголовки HTTP необязательны при отправке запросов автообнаружения.
  
**Таблица 1. Заголовки HTTP-запросов**

|**Header**|**Описание**|
|:-----|:-----|
|X — Мапихттпкапабилити  <br/> |Если указано значение "1", клиент запрашивает сведения, которые можно использовать для подключения к серверу с помощью протокола MAPI/HTTP. Этот заголовок применяется для клиентов, которые реализуют протокол MAPI/HTTP.  <br/> |
|X — Клиентканхандле  <br/> |Этот заголовок содержит разделенный запятыми список возможностей, поддерживаемых клиентом. Возможные значения указаны в таблице 2.  <br/> |
   
**Таблица 2. Значения заголовков X – Клиентканхандле**

|**Значение X-Клиентканхандле (без учета регистра)**|**Минимальная версия сервера**|**Описание**|
|:-----|:-----|:-----|
|Подключение  <br/> |15.00.0995.014  <br/> |Если задано это значение, сервер возвратит значение "Negotiate" в элементе [ауспаккаже (POX)](authpackage-pox.md) , если сервер настроен для приема проверки подлинности согласования. Если это значение отсутствует, сервер не возвратит значение "Negotiate" в элементе **ауспаккаже** .  <br/> |
|ексхттпинфо  <br/> |15.00.0995.014  <br/> |Если это значение задано, сервер возвратит элемент [протокола (POX)](protocol-pox.md) с элементом [Type (POX)](type-pox.md) со значением "ексхттп", если сервер НАСТРОЕН для приема подключений RPC/HTTP. Если это значение отсутствует, сервер не возвращает элемент **Protocol** , у которого для элемента **Type** задано значение "ексхттп".  <br/> |
   
### <a name="request-elements"></a>Элементы Request

В тексте запроса используются следующие элементы:
  
- [Служба автообнаружения (POX)](autodiscover-pox.md)
    
- [Запрос (POX)](request-pox.md)
    
- [Акцептаблереспонсесчема (POX)](acceptableresponseschema-pox.md)
    
- [EMailAddress (POX)](emailaddress-pox.md)
    
> [!NOTE]
> Элемент [LegacyDN (POX)](legacydn-pox.md) можно использовать вместо элемента [EMailAddress (POX)](emailaddress-pox.md) . 
  
### <a name="version-differences"></a>Различия версий

Заголовок X-Мапихттпкапабилити доступен в Office 365, Exchange Online и локальных версиях Exchange, начиная с сборки 15.00.0847.032 (Exchange Server 2013 с пакетом обновления 1 (SP1)).
  
Заголовок X-Клиентканхандле доступен в Office 365, Exchange Online и локальных версиях Exchange, начиная с сборки 15.00.0995.014.
  
## <a name="see-also"></a>См. также



[Отклик автообнаружения POX для Exchange](pox-autodiscover-response-for-exchange.md)


[Справочник по веб-службе автообнаружения POX для Exchange](pox-autodiscover-web-service-reference-for-exchange.md)
  
[XML-элементы автообнаружения POX для Exchange](pox-autodiscover-xml-elements-for-exchange.md)

