---
title: EcpUrl-aggr (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
ms.assetid: 0e7879e3-9b8f-4f23-8291-bacec0e479c0
description: Элемент EcpUrl-aggr указывает частичный URL-адрес, который может сочетаться со значением элемента EcpUrl (POX) для создания URL-адреса, который можно использовать для доступа к настройкам агрегации электронной почты для пользователя с включенной почтой.
ms.openlocfilehash: b959747f05f6921b43d3d50512202c6423e899aa
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59545280"
---
# <a name="ecpurl-aggr-pox"></a>EcpUrl-aggr (POX)

Элемент **EcpUrl-aggr** указывает частичный URL-адрес, который может сочетаться со значением [элемента EcpUrl (POX)](ecpurl-pox.md) для создания URL-адреса, который можно использовать для доступа к настройкам агрегации электронной почты для пользователя с включенной почтой. 
  
[AutoDiscover (POX)](autodiscover-pox.md)
  
[Response (POX)](response-pox.md)
  
[Account (POX)](account-pox.md)
  
[Protocol (POX)](protocol-pox.md)
  
[EcpUrl-aggr (POX)](ecpurl-aggr-pox.md)
  
```XML
<EcpUrl-aggr/>
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

Текстовое значение представляет частичный URL-адрес, который может сочетаться со значением элемента [EcpUrl (POX)](ecpurl-pox.md) для создания URL-адреса, который можно использовать для доступа к настройкам агрегации электронной почты для пользователя. 
  
## <a name="remarks"></a>Заметки

Элемент **EcpUrl-aggr** является необязательным детским элементом элемента **Protocol.** 
  
## <a name="see-also"></a>См. также



[Элементы XML автооткрытия POX для Exchange](pox-autodiscover-xml-elements-for-exchange.md)

