---
title: OWAUrl (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 450b86a1-1722-49f5-b541-16c1edc3db7a
description: Элемент OWAUrl описывает URL-адрес и схемы проверки подлинности, используемый для доступа к на конкретном компьютере, на котором выполняется Microsoft Exchange Server 2007, который имеет роль сервера клиентского доступа установлен, на котором размещается веб-клиент Outlook.
ms.openlocfilehash: 93d03506e2a74aa1b4ef6d2a49ccbda01cfc1f9a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19834673"
---
# <a name="owaurl-pox"></a>OWAUrl (POX)

Элемент **OWAUrl** описывает URL-адрес и схемы проверки подлинности, используемый для доступа к на конкретном компьютере, на котором выполняется Microsoft Exchange Server 2007, который имеет роль сервера клиентского доступа установлен, на котором размещается веб-клиент Outlook. 
  
[Автообнаружение (POX)](autodiscover-pox.md)
  
[Ответ (POX)](response-pox.md)
  
[Учетная запись (POX)](account-pox.md)
  
[Протокол (POX)](protocol-pox.md)
  
[Внутренний (POX)](internal-pox.md)
  
[OWAUrl (POX)](owaurl-pox.md)
  
```xml
<OWAUrl AuthenticationMethod=""/>
```

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|**AuthenticationMethod** <br/> |Описываются методы проверки подлинности для доступа к Outlook Web Access.  <br/> |
   
#### <a name="authenticationmethod-attribute"></a>Атрибут AuthenticationMethod

|**Значение**|**Описание**|
|:-----|:-----|
|WindowsIntegrated  <br/> |Встроенная проверка подлинности Windows.  <br/> |
|FBA  <br/> |Проверка подлинности на основе форм.  <br/> |
|NTLM  <br/> |Проверка подлинности NTLM.  <br/> |
|Дайджест-проверка  <br/> |Дайджест-проверки подлинности.  <br/> |
|Общая  <br/> |Обычная проверка подлинности.  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Внутренний (POX)](internal-pox.md) <br/> |Содержит коллекцию Outlook Web Access URL-адреса, клиент может подключиться к, когда в сети брандмауэра.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение представляет URL-адрес для службы Outlook Web Access на сервере клиентского доступа.
  
## <a name="see-also"></a>См. также



[Элементы XML автоматического обнаружения POX для Exchange](pox-autodiscover-xml-elements-for-exchange.md)

