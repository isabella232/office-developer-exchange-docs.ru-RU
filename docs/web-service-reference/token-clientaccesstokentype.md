---
title: Маркер (Клиентакцесстокентипе)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: cddd6075-06b6-4858-9ffa-9db4d9d9b030
description: Элемент Token указывает маркер клиентского доступа.
ms.openlocfilehash: d195e81d8d20eb2288e921c640c7b2898a5341ab
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467867"
---
# <a name="token-clientaccesstokentype"></a>Маркер (Клиентакцесстокентипе)

Элемент **Token** указывает маркер клиентского доступа. 
  
```XML
<Token>
   <Id/>
   <TokenType/>
   <TokenValue/>
   <TTL/>
</Token>
```

 **клиентакцесстокентипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

[ID (строка)](id-string.md)  |  [Токентипе](tokentype.md)  |  [Токенвалуе](tokenvalue.md)  |  [Срок жизни](ttl.md)
  
### <a name="parent-elements"></a>Родительские элементы

[жетклиентакцесстокенреспонсемессаже](getclientaccesstokenresponsemessage.md)
  
## <a name="remarks"></a>Примечания

Этот элемент появился в Exchange Server 2013.
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> ||
   

