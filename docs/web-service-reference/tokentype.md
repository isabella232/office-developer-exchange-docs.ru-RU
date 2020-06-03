---
title: токентипе
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 83c650eb-7ab8-480c-a7c9-df60072ee042
description: Элемент Токентипе указывает тип маркера.
ms.openlocfilehash: a42849dce9ed0253c3c5d4d4e899367b8e105594
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459884"
---
# <a name="tokentype"></a>токентипе

Элемент **токентипе** указывает тип маркера. 
  
```XML
<TokenType> CallerIdentity | ExtensionCallback | ScopedToken </TokenType>
```

 **клиентакцесстокентипетипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

Отсутствуют.
  
### <a name="parent-elements"></a>Родительские элементы

[Токенрекуест](tokenrequest.md)  |  [Token (маркер](token.md) )
  
## <a name="text-value"></a>Текстовое значение

Текстовое значение элемента **токентипе** — тип маркера. Текстовое значение **каллеридентити** указывает на то, что маркер является маркером удостоверения звонящего. Текстовое значение **екстенсионкаллбакк** указывает, что маркер предназначен для обратного вызова расширения. Текстовое значение **скопедтокен** указывает на то, что маркер клиентского доступа является маркером с областью действия. 
  
## <a name="remarks"></a>Примечания

Этот элемент появился в Exchange Server 2013.
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |false  <br/> |
   

