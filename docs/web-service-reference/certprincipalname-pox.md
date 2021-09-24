---
title: CertPrincipalName (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: a24092c9-58be-4008-92c4-68ec5c6c0fa6
description: Элемент CertPrincipalName указывает основное имя сертификата Secure Sockets Layer (SSL), необходимое для подключения к организации Microsoft Exchange Server 2007 г. с помощью SSL.
ms.openlocfilehash: 69ee49cdad09032c269ffbbcc918044daf61cb9b
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59523253"
---
# <a name="certprincipalname-pox"></a>CertPrincipalName (POX)

Элемент **CertPrincipalName** указывает основное имя сертификата Secure Sockets Layer (SSL), необходимое для подключения к организации Microsoft Exchange Server 2007 г. с помощью SSL. 
  
[AutoDiscover (POX)](autodiscover-pox.md)
  
[Response (POX)](response-pox.md)
  
[Account (POX)](account-pox.md)
  
[Protocol (POX)](protocol-pox.md)
  
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
|[Protocol (POX)](protocol-pox.md) <br/> |Содержит спецификации для подключения клиента к компьютеру 2007 Exchange 2007 года с установленной ролью сервера клиентского доступа.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

В текстовом значении указывается основное имя сертификата SSL, необходимое для подключения к организации Microsoft Exchange с помощью SSL.
  
## <a name="remarks"></a>Заметки

Если элемент **CertPrincipalName** не указан, по умолчанию задан msstd:SERVER, где SERVER — это значение, указанное в элементе [Server (POX).](server-pox.md) Например, если сервер указывается как example.com и **CertPrincipalName** остается пустым с включенной [SSL (POX),](ssl-pox.md) по умолчанию значение **CertPrincipalName** будет msstd:example.com. 
  
Если **ничего** не указано, Windows будет проверять основное имя сертификата в соответствии с сведениями, найденными в разделе [Основные](https://go.microsoft.com/fwlink/?LinkId=93417) имена в MSDN. 
  
## <a name="see-also"></a>См. также



[Элементы XML автооткрытия POX для Exchange](pox-autodiscover-xml-elements-for-exchange.md)

