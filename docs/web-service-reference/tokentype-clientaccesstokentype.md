---
title: Токентипе (Клиентакцесстокентипе)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 96103f15-a3e0-497c-af21-90adbf9a4b14
description: Элемент Токентипе определяет тип маркера клиентского доступа, который будет возвращен в ответе GetClientAccessToken.
ms.openlocfilehash: c9adb60acf76fefebd58e2fd3bc899332a63dbee
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19840213"
---
# <a name="tokentype-clientaccesstokentype"></a>Токентипе (Клиентакцесстокентипе)

Элемент **токентипе** определяет тип маркера клиентского доступа, который будет возвращен в ответе **GetClientAccessToken** . 
  
```XML
<TokenType>CallerIdentity | ExtensionCallback | ScopedToken</TokenType>
```

 **клиентакцесстокентипетипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

[Маркер токенрекуест](tokenrequest.md) | [(клиентакцесстокентипе)](token-clientaccesstokentype.md)
  
## <a name="text-value"></a>Текстовое значение

Текстовое значение **каллеридентити** означает, что возвращается маркер доступа клиента идентификации звонящего. Текстовое значение **екстенсионкаллбакк** указывает на то, что маркер доступа клиента обратного вызова для расширения возвращается. Текстовое значение **скопедтокен** указывает на то, что маркер клиентского доступа является маркером с областью действия. 
  
## <a name="remarks"></a>Примечания

Этот элемент появился в Exchange Server 2013.
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |false  <br/> |
   

