---
title: InternalUrl (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 4649baa9-eec9-426d-952b-361818c25fe0
description: Элемент InternalUrl содержит URL-адрес для подключения клиента на сервер адресной книги или почтового ящика пользователя из внутренней организации пользователя с помощью протокола MAPI/HTTP.
ms.openlocfilehash: 3823236081961128b31bb2c0f563062897c55814
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833950"
---
# <a name="internalurl-pox"></a>InternalUrl (POX)

Элемент **InternalUrl** содержит URL-адрес для подключения клиента на сервер адресной книги или почтового ящика пользователя из внутренней организации пользователя с помощью протокола MAPI/HTTP. 
  
```XML
<InternalUrl/>
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
|[AddressBook (POX)](addressbook-pox.md) <br/> |Содержит спецификации для подключения клиента к сервер адресной книги с помощью протокола MAPI/HTTP.  <br/> |
|[MailStore (POX)](mailstore-pox.md) <br/> |Содержит спецификации для подключения клиента к почтовому ящику пользователя с помощью протокола MAPI/HTTP.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение представляет URL-адрес, который можно использовать для доступа к сервер адресной книги или почтового ящика пользователя из внутренней организации пользователя.
  
## <a name="remarks"></a>Замечания

Элемент **InternalUrl** могут быть представлены в соответствии с элементом [Протокола (POX)](protocol-pox.md) со значением атрибута **типа** «mapiHttp». 
  
Элемент **InternalUrl** доступен для клиентов, использующих протокол MAPI/HTTP и конечного Exchange Online, Exchange Online в составе Office 365 и локальной версии Exchange, начиная с построения 15.00.0847.032 (Exchange Server 2013 с пакетом обновления 1) . 
  
## <a name="see-also"></a>См. также



[Элементы XML автоматического обнаружения POX для Exchange](pox-autodiscover-xml-elements-for-exchange.md)

