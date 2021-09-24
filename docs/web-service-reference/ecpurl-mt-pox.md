---
title: EcpUrl-mt (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
ms.assetid: 5221745b-572c-44a5-afdb-41b58af44971
description: Элемент EcpUrl-mt указывает частичный URL-адрес, который можно сочетать со значением элемента EcpUrl (POX) для создания URL-адреса, который можно использовать для доступа к настройкам отслеживания сообщений электронной почты для пользователя с включенной почтой.
ms.openlocfilehash: bb0a60f3b3a2d65421164e40537e7514df20e357
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59520817"
---
# <a name="ecpurl-mt-pox"></a>EcpUrl-mt (POX)

Элемент **EcpUrl-mt** указывает частичный URL-адрес, который можно сочетать со значением элемента [EcpUrl (POX)](ecpurl-pox.md) для создания URL-адреса, который можно использовать для доступа к настройкам отслеживания сообщений электронной почты для пользователя с включенной почтой. 
  
[AutoDiscover (POX)](autodiscover-pox.md)
  
[Response (POX)](response-pox.md)
  
[Account (POX)](account-pox.md)
  
[Protocol (POX)](protocol-pox.md)
  
[EcpUrl-mt (POX)](ecpurl-mt-pox.md)
  
```XML
<EcpUrl-mt/>
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

Текстовое значение представляет частичный URL-адрес, который можно сочетать со значением [элемента EcpUrl (POX)](ecpurl-pox.md) для создания URL-адреса, который можно использовать для доступа к настройкам отслеживания электронной почты для пользователя. Значение элемента **EcpUrl-mt** содержит параметры, содержащиеся в символах < и >, которые заменяются клиентом, как показано в следующей таблице. 
  
|**Параметр**|**Замена**|
|:-----|:-----|
| _IsOwa_ <br/> |n  <br/> |
| _MsgID_ <br/> |Идентификатор сообщения в Интернете, отслеживаемого в загоне Message-ID.  <br/> |
| _Mbx_ <br/> |SMTP-адрес владельца почтового ящика.  <br/> |
| _Sender_ <br/> |SMTP-адрес отправщика сообщения.  <br/> |
   
## <a name="remarks"></a>Заметки

Элемент **EcpUrl-mt** является необязательным детским элементом элемента **Protocol.** 
  
## <a name="see-also"></a>См. также



[Элементы XML автооткрытия POX для Exchange](pox-autodiscover-xml-elements-for-exchange.md)

