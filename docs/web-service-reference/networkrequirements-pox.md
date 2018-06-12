---
title: NetworkRequirements (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 1555fd2e-05b6-4b94-907b-dae9174049d9
description: Элемент NetworkRequirements содержит критерии, используемые для определения, является ли на клиентском компьютере в сети, которая соответствует требованиям поставщика услуг Интернета (поставщика услуг Интернета) для подключения к серверу.
ms.openlocfilehash: f3abcff04cd4121b8dcc7ceff7658ad389e6d0b0
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19834529"
---
# <a name="networkrequirements-pox"></a>NetworkRequirements (POX)

Элемент **NetworkRequirements** содержит критерии, используемые для определения, является ли на клиентском компьютере в сети, которая соответствует требованиям поставщика услуг Интернета (поставщика услуг Интернета) для подключения к серверу. 
  
[Автообнаружение (POX)](autodiscover-pox.md)
  
[Ответ (POX)](response-pox.md)
  
[Учетная запись (POX)](account-pox.md)
  
[Протокол (POX)](protocol-pox.md)
  
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
|[IPv4Start (POX)](ipv4start-pox.md) <br/> |Определяет начало диапазона IP версии 4 (IPv4) адреса, которые используются для идентификации компьютера в сети.  <br/> |
|[IPv4End (POX)](ipv4end-pox.md) <br/> |Определяет конец диапазона IP версии 4 (IPv4) адреса, которые используются для идентификации компьютера в сети.  <br/> |
|[IPv6Start (POX)](ipv6start-pox.md) <br/> |Определяет начало диапазона IP-адресов версии 6 (IPv6) адреса, которые используются для идентификации компьютера в сети.  <br/> |
|[IPv6End (POX)](ipv6end-pox.md) <br/> |Определяет конец диапазона IP-адресов версии 6 (IPv6) адреса, которые используются для идентификации компьютера в сети.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Протокол (POX)](protocol-pox.md) <br/> |Содержит спецификации для подключения клиентского компьютера, на котором выполняется Microsoft Exchange Server 2007 с установленной ролью сервера клиентского доступа.  <br/> |
   
## <a name="remarks"></a>Замечания

Если клиентом электронной почты не соответствует требованиям сети, его следует попробуйте других типов протокола. Поставщики услуг Интернета можно указать один набор серверов с тегами [Протокола (POX)](protocol-pox.md) , которые не требуют проверки подлинности, но требуется быть в сети поставщика услуг Интернета. Поставщики услуг Интернета могут списки другой набор серверов, которые требуют проверки подлинности, но не обязательно должны быть в конкретной сети. 
  
Элемент **NetworkRequirements** является необязательным. 
  
## <a name="see-also"></a>См. также



[Элементы XML автоматического обнаружения POX для Exchange](pox-autodiscover-xml-elements-for-exchange.md)

