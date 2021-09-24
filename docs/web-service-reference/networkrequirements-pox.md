---
title: NetworkRequirements (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: 1555fd2e-05b6-4b94-907b-dae9174049d9
description: Элемент NetworkRequirements содержит критерии, используемые для определения того, подключен ли клиентский компьютер к сети, которая соответствует требованиям поставщика интернет-услуг (ISP) для подключения к серверу.
ms.openlocfilehash: 07a258ad48b74c614ce367db0f893ed884cf3f75
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59509518"
---
# <a name="networkrequirements-pox"></a>NetworkRequirements (POX)

Элемент **NetworkRequirements** содержит критерии, используемые для определения того, подключен ли клиентский компьютер к сети, которая соответствует требованиям поставщика интернет-услуг (ISP) для подключения к серверу. 
  
[AutoDiscover (POX)](autodiscover-pox.md)
  
[Response (POX)](response-pox.md)
  
[Account (POX)](account-pox.md)
  
[Protocol (POX)](protocol-pox.md)
  
[NetworkRequirements (POX)](networkrequirements-pox.md)
  
```xml
<NetworkRequirements>
   <IPv4Start/>
   <IPv4End/>
   <IPv6Start/>
   <IPv6End/>
</NetworkRequirements>
```

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[IPv4Start (POX)](ipv4start-pox.md) <br/> |Определяет начало диапазона IP-адресов версии 4 (IPv4), используемых для идентификации компьютера в сети.  <br/> |
|[IPv4End (POX)](ipv4end-pox.md) <br/> |Определяет конец диапазона IP-адресов версии 4 (IPv4), используемых для идентификации компьютера в сети.  <br/> |
|[IPv6Start (POX)](ipv6start-pox.md) <br/> |Определяет начало диапазона IP-адресов версии 6 (IPv6), используемых для идентификации компьютера в сети.  <br/> |
|[IPv6End (POX)](ipv6end-pox.md) <br/> |Определяет конец диапазона IP-адресов версии 6 (IPv6), используемых для идентификации компьютера в сети.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Protocol (POX)](protocol-pox.md) <br/> |Содержит спецификации для подключения клиента к компьютеру, на Microsoft Exchange Server 2007 г., на который установлена роль сервера клиентского доступа.  <br/> |
   
## <a name="remarks"></a>Заметки

Если клиент электронной почты не соответствует требованиям сети, он должен попробовать другие типы протоколов. Интернет-пользователи могут предоставлять один набор серверов с тегами [Protocol (POX),](protocol-pox.md) которые не требуют проверки подлинности, но должны быть в сети интернет-пользователей. Интернет-пользователи могут перечислить другой набор серверов, которые требуют проверки подлинности, но не должны быть в определенной сети. 
  
Элемент **NetworkRequirements** необязателен. 
  
## <a name="see-also"></a>См. также



[Элементы XML автооткрытия POX для Exchange](pox-autodiscover-xml-elements-for-exchange.md)

