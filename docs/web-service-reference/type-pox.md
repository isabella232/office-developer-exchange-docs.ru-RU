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
description: Элемент Type определяет тип учетной записи электронной почты настроена.
ms.openlocfilehash: 6e1349769c6a5349304f576419e0c609d3edd9a0
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19840247"
---
# <a name="type-pox"></a>Тип (POX)

Элемент **Type** определяет тип учетной записи электронной почты настроена. 
  
[Автообнаружение (POX)](autodiscover-pox.md)
  
[Ответ (POX)](response-pox.md)
  
[Учетная запись (POX)](account-pox.md)
  
[Протокол (POX)](protocol-pox.md)
  
[Тип (POX)](type-pox.md)
  
```XML
<Type>WEB or EXCH or EXPR or EXHTTP</Type>
```

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Протокол (POX)](protocol-pox.md) <br/> |Содержит спецификации для подключения клиента к серверу Exchange.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение представляет тип учетной записи почты. В следующей таблице приведены возможные значения.
  
|**Значение**|**Описание**|
|:-----|:-----|
|EXCH  <br/> |Протокол, используемый для подключения к серверу используется Exchange RPC.  <br/> |
|EXHTTP  <br/> |Протокол, используемый для подключения RPC/HTTP-подключений сервера.  <br/> |
|ВЫРАЖЕНИЕ  <br/> |Протокол, используемый для подключения к серверу — Exchange RPC через HTTP, прокси-сервер RPC.  <br/> Это применимо только если для элемента [AccountType (POX)](accounttype-pox.md) в электронной почты.  <br/> |
|WEB  <br/> |Для доступа к электронной почты из веб-браузера с помощью URL-адреса, указанного в элементе [Сервера (POX)](server-pox.md) .  <br/> Это применимо только если для элемента [AccountType (POX)](accounttype-pox.md) в электронной почты.  <br/> |
   
### <a name="version-differences"></a>Различия версий

Office 365, Exchange Online и локальной версии Exchange, начиная с построения 15.00.0995.014 возвращаемое значение «EXHTTP» только в том случае, если сервер настроен на прием RPC/HTTP-подключений и клиент включает в себя заголовок [X-ClientCanHandle](pox-autodiscover-request-for-exchange.md) , содержит «ExHttpInfo». 
  
## <a name="see-also"></a>См. также



[Элементы XML автоматического обнаружения POX для Exchange](pox-autodiscover-xml-elements-for-exchange.md)

