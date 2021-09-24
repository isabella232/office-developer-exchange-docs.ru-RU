---
title: EcpUrl-tmHiding (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
ms.assetid: 9b9ae15b-3ac1-45ac-85ba-38c7231fe508
description: Элемент EcpUrl-tmHiding указывает частичный URL-адрес, который можно сочетать со значением элемента EcpUrl (POX) для создания URL-адреса, который можно использовать для отписки пользователя из почтового ящика сайта.
ms.openlocfilehash: d8e8ced554b96f1a0cd554d3d601970d5f47019b
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59514736"
---
# <a name="ecpurl-tmhiding-pox"></a>EcpUrl-tmHiding (POX)

Элемент **EcpUrl-tmHiding** указывает частичный URL-адрес, который можно сочетать со значением [элемента EcpUrl (POX)](ecpurl-pox.md) для создания URL-адреса, который можно использовать для отписки пользователя из почтового ящика сайта. 
  
[AutoDiscover (POX)](autodiscover-pox.md)
  
[Response (POX)](response-pox.md)
  
[Account (POX)](account-pox.md)
  
[Protocol (POX)](protocol-pox.md)
  
[EcpUrl-tmHiding (POX)](ecpurl-tmhiding-pox.md)
  
```XML
<EcpUrl-tmHiding/>
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
|[Protocol (POX)](protocol-pox.md) <br/> |Содержит спецификации для подключения клиента к компьютеру, на Microsoft Exchange Server установлена роль сервера клиентского доступа.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение представляет частичный URL-адрес, который может сочетаться со значением [элемента EcpUrl (POX)](ecpurl-pox.md) для создания URL-адреса, который можно использовать для отписки пользователя из почтового ящика сайта. Значение элемента **EcpUrl-tmHiding** содержит параметры, содержащиеся в символах "<" и ">", которые заменяются клиентом, как показано в следующей таблице. 
  
|**Параметр**|**Замена**|
|:-----|:-----|
| _Id_ <br/> |Адрес электронной почты SMTP или отличительное имя X500 почтового ящика сайта.  <br/> |
   
## <a name="remarks"></a>Заметки

Элемент **EcpUrl-tmHiding** является необязательным детским элементом элемента **Protocol.** 
  
## <a name="see-also"></a>См. также



[Элементы XML автооткрытия POX для Exchange](pox-autodiscover-xml-elements-for-exchange.md)

