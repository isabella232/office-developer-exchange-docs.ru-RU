---
title: Оваурл (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 450b86a1-1722-49f5-b541-16c1edc3db7a
description: Элемент Оваурл описывает URL-адрес и схему проверки подлинности, которая используется для доступа к определенному компьютеру под управлением Microsoft Exchange Server 2007 с установленной ролью сервера клиентского доступа, на котором размещена служба Outlook Web Access.
ms.openlocfilehash: 93d03506e2a74aa1b4ef6d2a49ccbda01cfc1f9a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834673"
---
# <a name="owaurl-pox"></a>Оваурл (POX)

Элемент **оваурл** описывает URL-адрес и схему проверки подлинности, которая используется для доступа к определенному компьютеру под управлением Microsoft Exchange Server 2007 с установленной ролью сервера клиентского доступа, на котором размещена служба Outlook Web Access. 
  
[Служба автообнаружения (POX)](autodiscover-pox.md)
  
[Ответ (POX)](response-pox.md)
  
[Учетная запись (POX)](account-pox.md)
  
[Протокол (POX)](protocol-pox.md)
  
[Internal (POX)](internal-pox.md)
  
[Оваурл (POX)](owaurl-pox.md)
  
```xml
<OWAUrl AuthenticationMethod=""/>
```

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|**Параметр authenticationmethod** <br/> |Описывает методы проверки подлинности для доступа к Outlook Web Access.  <br/> |
   
#### <a name="authenticationmethod-attribute"></a>Атрибут AuthenticationMethod

|**Значение**|**Описание**|
|:-----|:-----|
|виндовсинтегратед  <br/> |Встроенная проверка подлинности Windows.  <br/> |
|FBA  <br/> |Проверка подлинности на основе форм.  <br/> |
|NTLM;  <br/> |Проверка подлинности NTLM.  <br/> |
|Digest  <br/> |Дайджест-проверка подлинности.  <br/> |
|Базовая  <br/> |Обычная проверка подлинности.  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Internal (POX)](internal-pox.md) <br/> |Содержит коллекцию URL-адресов Outlook Web Access, к которым клиент может подключаться, если он находится в брандмауэре.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение представляет URL-адрес службы Outlook Web Access на сервере клиентского доступа.
  
## <a name="see-also"></a>См. также



[XML-элементы автообнаружения POX для Exchange](pox-autodiscover-xml-elements-for-exchange.md)

