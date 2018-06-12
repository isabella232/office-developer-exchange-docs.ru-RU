---
title: CertPrincipalName (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: a24092c9-58be-4008-92c4-68ec5c6c0fa6
description: Элемент CertPrincipalName указывает Secure Sockets Layer (SSL) имя участника сертификата, который необходим для подключения к организации Microsoft Exchange Server 2007 с помощью протокола SSL.
ms.openlocfilehash: d2766b16a3e8a1bcd013de332d9c07f709fcf949
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761676"
---
# <a name="certprincipalname-pox"></a>CertPrincipalName (POX)

Элемент **CertPrincipalName** указывает Secure Sockets Layer (SSL) имя участника сертификата, который необходим для подключения к организации Microsoft Exchange Server 2007 с помощью протокола SSL. 
  
[Автообнаружение (POX)](autodiscover-pox.md)
  
[Ответ (POX)](response-pox.md)
  
[Учетная запись (POX)](account-pox.md)
  
[Протокол (POX)](protocol-pox.md)
  
[CertPrincipalName (POX)](certprincipalname-pox.md)
  
```xml
<CertPrincipalName>none or servername</CertPrinicpalName>
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
|[Протокол (POX)](protocol-pox.md) <br/> |Содержит спецификации для подключения клиентского компьютера, на котором работает с установленной ролью сервера клиентского доступа Exchange 2007.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение указывает имя участника сертификата SSL, которые требуются для подключения к Microsoft Exchange в организации с помощью протокола SSL.
  
## <a name="remarks"></a>Замечания

Если элемент **CertPrincipalName** не указан, по умолчанию имеет значение msstd:SERVER, где сервер — это значение, которое задано в элементе [Сервера (POX)](server-pox.md) . Например если сервер указан как example.com и **CertPrincipalName** оставлено пустым с включенным [SSL (POX)](ssl-pox.md) , значение по умолчанию **CertPrincipalName** будет msstd:example.com. 
  
Если **он не задан,** Windows будет проверять имя участника сертификата в соответствии с сведения, содержащиеся в разделе [Имена участников](http://go.microsoft.com/fwlink/?LinkId=93417) на сайте MSDN. 
  
## <a name="see-also"></a>См. также



[Элементы XML автоматического обнаружения POX для Exchange](pox-autodiscover-xml-elements-for-exchange.md)

