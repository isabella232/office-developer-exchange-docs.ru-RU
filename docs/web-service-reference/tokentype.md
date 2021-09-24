---
title: TokenType
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 83c650eb-7ab8-480c-a7c9-df60072ee042
description: Элемент TokenType указывает тип маркера.
ms.openlocfilehash: a51ddfdd097a94370168077b9eca8be2e0581603
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59523323"
---
# <a name="tokentype"></a>TokenType

Элемент **TokenType** указывает тип маркера. 
  
```XML
<TokenType> CallerIdentity | ExtensionCallback | ScopedToken </TokenType>
```

 **ClientAccessTokenType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

[TokenRequest](tokenrequest.md)  |  [Маркер](token.md)
  
## <a name="text-value"></a>Текстовое значение

Текстовое значение элемента **TokenType** — это тип маркера. Текстовое значение **объекта CallerId указывает,** что маркер является маркером удостоверения вызывающего пользователя. Текстовое значение **ExtensionCallback** указывает, что маркер для вызова расширения. Текстовое значение **ScopedToken** указывает, что маркер клиентского доступа является маркером с областью действия. 
  
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
   

