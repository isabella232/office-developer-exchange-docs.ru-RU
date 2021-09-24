---
title: OWAUrl (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: 450b86a1-1722-49f5-b541-16c1edc3db7a
description: Элемент OWAUrl описывает схему URL-адреса и проверки подлинности, которая используется для доступа к определенному компьютеру, который работает Microsoft Exchange Server 2007 г., на котором установлена роль сервера клиентского доступа, на котором Outlook веб-Outlook доступ.
ms.openlocfilehash: fbd61eb75018c57dada40f5ed7472379d365e752
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59534893"
---
# <a name="owaurl-pox"></a>OWAUrl (POX)

Элемент **OWAUrl** описывает схему URL-адреса и проверки подлинности, которая используется для доступа к определенному компьютеру, который работает Microsoft Exchange Server 2007 г., на котором установлена роль сервера клиентского доступа, на котором Outlook веб-доступ. 
  
[AutoDiscover (POX)](autodiscover-pox.md)
  
[Response (POX)](response-pox.md)
  
[Account (POX)](account-pox.md)
  
[Protocol (POX)](protocol-pox.md)
  
[Internal (POX)](internal-pox.md)
  
[OWAUrl (POX)](owaurl-pox.md)
  
```xml
<OWAUrl AuthenticationMethod=""/>
```

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|**AuthenticationMethod** <br/> |Описывает методы проверки подлинности для доступа Outlook веб-доступа.  <br/> |
   
#### <a name="authenticationmethod-attribute"></a>Атрибут AuthenticationMethod

|**Значение**|**Описание**|
|:-----|:-----|
|WindowsIntegrated  <br/> |Интегрированная Windows проверки подлинности.  <br/> |
|FBA  <br/> |Проверка подлинности на основе форм.  <br/> |
|NTLM;  <br/> |Проверка подлинности NTLM.  <br/> |
|Дайджест  <br/> |Дайджест проверки подлинности.  <br/> |
|Базовый  <br/> |Обычная проверка подлинности.  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Internal (POX)](internal-pox.md) <br/> |Содержит коллекцию URL Outlook веб-доступа, к которую клиент может подключиться, когда находится внутри брандмауэра.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение представляет URL-адрес для Outlook веб-доступа на сервере клиентского доступа.
  
## <a name="see-also"></a>См. также



[Элементы XML автооткрытия POX для Exchange](pox-autodiscover-xml-elements-for-exchange.md)

