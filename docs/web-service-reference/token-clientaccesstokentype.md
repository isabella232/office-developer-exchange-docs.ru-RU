---
title: Маркер (ClientAccessTokenType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: cddd6075-06b6-4858-9ffa-9db4d9d9b030
description: Элемент маркер указывает маркера доступа клиента.
ms.openlocfilehash: 2e1f401141aef07a57a214968f6a6bafdf71f0dc
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19840203"
---
# <a name="token-clientaccesstokentype"></a>Маркер (ClientAccessTokenType)

**Маркер** элемент указывает маркера доступа клиента. 
  
```XML
<Token>
   <Id/>
   <TokenType/>
   <TokenValue/>
   <TTL/>
</Token>
```

 **ClientAccessTokenType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

[Идентификатор (String)](id-string.md) | [TokenType](tokentype.md) | [TokenValue](tokenvalue.md) | [TTL](ttl.md)
  
### <a name="parent-elements"></a>Родительские элементы

[GetClientAccessTokenResponseMessage](getclientaccesstokenresponsemessage.md)
  
## <a name="remarks"></a>Замечания

Этот элемент появился в Exchange Server 2013.
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> ||
   

