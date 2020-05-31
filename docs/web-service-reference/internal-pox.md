---
title: Internal (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 69c22546-ebd6-4a03-b0b4-bbac72ec5551
description: Внутренний элемент содержит коллекцию URL-адресов, которые клиент может использовать для подключения к Exchange из сети Организации.
ms.openlocfilehash: 0dc5b679af98b52f15ef3b40181c2d97f102f373
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833946"
---
# <a name="internal-pox"></a>Internal (POX)

**Внутренний** элемент содержит коллекцию URL-адресов, которые клиент может использовать для подключения к Exchange из сети Организации. 
  
[Служба автообнаружения (POX)](autodiscover-pox.md)
  
[Ответ (POX)](response-pox.md)
  
[Учетная запись (POX)](account-pox.md)
  
[Протокол (POX)](protocol-pox.md)
  
[Internal (POX)](internal-pox.md)
  
```xml
<Internal>
   <OWAUrl/>
   <Protocol>
      <Type/>
      <ASUrl/>
   </Protocol>
</Internal>
```

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Оваурл (POX)](owaurl-pox.md) <br/> |Описание URL-адреса и схемы проверки подлинности, которая используется для доступа к определенному компьютеру, на котором установлен сервер Microsoft Exchange Server с установленной ролью сервера клиентского доступа, на котором размещена служба Outlook Web Access.  <br/> |
|[Протокол (POX)](protocol-pox.md) <br/> |Содержит спецификации для подключения клиента к компьютеру, на котором установлен сервер Microsoft Exchange с установленной ролью сервера клиентского доступа. Этот элемент **Protocol** содержит только два дочерних элемента: [тип (POX)](type-pox.md) , указывающий протокол подключения, и элемент [асурл (POX)](asurl-pox.md) , указав конечную точку EWS для веб-службы доступности.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Протокол (POX)](protocol-pox.md) <br/> |Содержит спецификации для подключения клиента к компьютеру, на котором установлен сервер Microsoft Exchange с установленной ролью сервера клиентского доступа.  <br/> |
   
## <a name="remarks"></a>Примечания

**Внутренний** элемент — это необязательный дочерний элемент элемента **Protocol** . 
  
## <a name="see-also"></a>См. также



[XML-элементы автообнаружения POX для Exchange](pox-autodiscover-xml-elements-for-exchange.md)

