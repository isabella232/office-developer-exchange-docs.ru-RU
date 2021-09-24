---
title: TokenType (ClientAccessTokenType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 96103f15-a3e0-497c-af21-90adbf9a4b14
description: Элемент TokenType определяет тип маркера клиентского доступа, который будет возвращен в ответе GetClientAccessToken.
ms.openlocfilehash: 967d64796799147876ef6443b40b16154b55c01a
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59523358"
---
# <a name="tokentype-clientaccesstokentype"></a>TokenType (ClientAccessTokenType)

Элемент **TokenType** определяет тип маркера клиентского доступа, который будет возвращен в **ответе GetClientAccessToken.** 
  
```XML
<TokenType>CallerIdentity | ExtensionCallback | ScopedToken</TokenType>
```

 **ClientAccessTokenType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

[TokenRequest](tokenrequest.md)  |  [Маркер (ClientAccessTokenType)](token-clientaccesstokentype.md)
  
## <a name="text-value"></a>Текстовое значение

Текстовое значение **callerIdentity означает,** что возвращается маркер клиентского доступа к удостоверениям вызывающего пользователя. Текстовое значение **ExtensionCallback** указывает, что возвращается маркер клиентского доступа к продлению обратного вызова. Текстовое значение **ScopedToken** указывает, что маркер клиентского доступа — это маркер с областью действия. 
  
## <a name="remarks"></a>Заметки

Этот элемент появился в Exchange Server 2013.
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |false  <br/> |
   

