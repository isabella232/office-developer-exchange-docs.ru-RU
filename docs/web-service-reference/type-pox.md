---
title: Type (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: 9a627244-554f-4223-b9d8-a601b81a4a1a
description: Элемент Type определяет тип настроенной учетной записи почты.
ms.openlocfilehash: bb92913071509fec46736341bce56b1a00730f6b
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59517527"
---
# <a name="type-pox"></a>Type (POX)

Элемент **Type** определяет тип настроенной учетной записи почты. 
  
[AutoDiscover (POX)](autodiscover-pox.md)
  
[Response (POX)](response-pox.md)
  
[Account (POX)](account-pox.md)
  
[Protocol (POX)](protocol-pox.md)
  
[Type (POX)](type-pox.md)
  
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
|[Protocol (POX)](protocol-pox.md) <br/> |Содержит спецификации для подключения клиента к Exchange серверу.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение представляет тип учетной записи почты. В следующей таблице перечислены возможные значения.
  
|**Значение**|**Описание**|
|:-----|:-----|
|EXCH  <br/> |Протокол, используемый для подключения к серверу, Exchange RPC.  <br/> |
|EXHTTP  <br/> |Протокол, используемый для подключения к соединениям RPC/HTTP сервера.  <br/> |
|EXPR  <br/> |Протокол, используемый для подключения к серверу, Exchange RPC над HTTP с помощью прокси-сервера RPC.  <br/> Это применимо только в том случае, если элемент [AccountType (POX)](accounttype-pox.md) настроен на электронную почту.  <br/> |
|WEB  <br/> |К электронной почте можно получить доступ из веб-браузера с помощью URL-адреса, указанного в элементе [Server (POX).](server-pox.md)  <br/> Это применимо только в том случае, если элемент [AccountType (POX)](accounttype-pox.md) настроен на электронную почту.  <br/> |
   
### <a name="version-differences"></a>Различия версий

Office 365, Exchange Online и локальной версии Exchange начиная со сборки 15.00.0995.014 возвращают значение "EXHTTP" только в том случае, если сервер настроен на прием подключений RPC/HTTP, а клиент включает в себя загон [X-ClientCanHandle,](pox-autodiscover-request-for-exchange.md) содержащий "ExHttpInfo". 
  
## <a name="see-also"></a>См. также



[Элементы XML автооткрытия POX для Exchange](pox-autodiscover-xml-elements-for-exchange.md)

