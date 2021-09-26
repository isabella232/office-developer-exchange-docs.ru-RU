---
title: UsePOPAuth (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: 28f552d8-6bb8-49b4-a45c-b2053670f1cc
description: Элемент UsePOPAuth указывает, используются ли сведения о проверке подлинности для учетной записи типа POP3 для протокола простой передачи почты (SMTP).
ms.openlocfilehash: 354c027bf40ddf30cda472eb4ca0d018dca64f9c
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59542626"
---
# <a name="usepopauth-pox"></a>UsePOPAuth (POX)

Элемент **UsePOPAuth** указывает, используются ли сведения о проверке подлинности для учетной записи типа POP3 для протокола простой передачи почты (SMTP). 
  
[AutoDiscover (POX)](autodiscover-pox.md)
  
[Response (POX)](response-pox.md)
  
[Account (POX)](account-pox.md)
  
[Protocol (POX)](protocol-pox.md)
  
[UsePOPAuth (POX)](usepopauth-pox.md)
  
```xml
<UsePOPAuth>on or off</UsePOPAuth>
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
|[Protocol (POX)](protocol-pox.md) <br/> |Содержит спецификации для подключения клиента к компьютеру, на Microsoft Exchange Server 2007 г., на который установлена роль сервера клиентского доступа.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение указывает, используются ли сведения о проверке подлинности для учетной записи типа POP3 для SMTP. Возможные значения **включаем и** **отключаем.**
  
## <a name="remarks"></a>Заметки

Элемент **UsePOPAuth** используется только в том случае, если [Type (POX)](type-pox.md) является SMTP. 
  
## <a name="see-also"></a>См. также



[Элементы XML автооткрытия POX для Exchange](pox-autodiscover-xml-elements-for-exchange.md)

