---
title: Тип (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 9a627244-554f-4223-b9d8-a601b81a4a1a
description: Элемент Type определяет тип настроенной почтовой учетной записи.
ms.openlocfilehash: 6e1349769c6a5349304f576419e0c609d3edd9a0
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19840247"
---
# <a name="type-pox"></a>Тип (POX)

Элемент **Type** определяет тип настроенной почтовой учетной записи. 
  
[Служба автообнаружения (POX)](autodiscover-pox.md)
  
[Ответ (POX)](response-pox.md)
  
[Учетная запись (POX)](account-pox.md)
  
[Протокол (POX)](protocol-pox.md)
  
[Тип (POX)](type-pox.md)
  
```XML
<Type>WEB or EXCH or EXPR or EXHTTP</Type>
```

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Протокол (POX)](protocol-pox.md) <br/> |Содержит спецификации для подключения клиента к серверу Exchange Server.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение представляет тип учетной записи почты. В приведенной ниже таблице перечислены возможные значения.
  
|**Значение**|**Описание**|
|:-----|:-----|
|EXCH  <br/> |Протокол, используемый для подключения к серверу, — RPC RPC.  <br/> |
|ексхттп  <br/> |Протокол, используемый для подключения к серверу RPC/HTTP-подключениям.  <br/> |
|ВЫРАЖЕН  <br/> |Протокол, используемый для подключения к серверу, — это Exchange RPC через HTTP с использованием прокси-сервера RPC.  <br/> Этот параметр применяется, только если для элемента [AccountType (POX)](accounttype-pox.md) задано значение email.  <br/> |
|WEB  <br/> |Доступ к электронной почте осуществляется из веб-браузера с помощью URL-адреса, указанного в элементе [Server (POX)](server-pox.md) .  <br/> Этот параметр применяется, только если для элемента [AccountType (POX)](accounttype-pox.md) задано значение email.  <br/> |
   
### <a name="version-differences"></a>Различия версий

Office 365, Exchange Online и локальная версия Exchange, начиная с сборки 15.00.0995.014, возвращают значение "ЕКСХТТП" только в том случае, если сервер настроен на прием подключений RPC/HTTP, а клиент содержит заголовок [X-клиентканхандле](pox-autodiscover-request-for-exchange.md) , который содержит "ексхттпинфо". 
  
## <a name="see-also"></a>См. также



[XML-элементы автообнаружения POX для Exchange](pox-autodiscover-xml-elements-for-exchange.md)

