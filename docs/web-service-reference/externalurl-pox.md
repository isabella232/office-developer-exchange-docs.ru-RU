---
title: ExternalUrl (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 3b647d88-6feb-40d7-9299-b2ca47b707db
description: Элемент ExternalUrl содержит URL-адрес для подключения клиента на сервер адресной книги или почтового ящика пользователя из за пределами организации пользователя с помощью протокола MAPI/HTTP.
ms.openlocfilehash: 603e2109e7b3c98acdd4cbc13df81ed9717630ec
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762512"
---
# <a name="externalurl-pox"></a>ExternalUrl (POX)

Элемент **ExternalUrl** содержит URL-адрес для подключения клиента на сервер адресной книги или почтового ящика пользователя из за пределами организации пользователя с помощью протокола MAPI/HTTP. 
  
```XML
<ExternalUrl/>
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

Текстовое значение представляет URL-адрес, который можно использовать для доступа к сервер адресной книги или почтового ящика пользователя из за пределами организации пользователя.
  
## <a name="remarks"></a>Замечания

Элемент **ExternalUrl** могут быть представлены в соответствии с элементом [Протокола (POX)](protocol-pox.md) со значением атрибута **типа** «mapiHttp». 
  
Элемент **ExternalUrl** доступен для клиентов, использующих протокол MAPI/HTTP и конечного Exchange Online, Exchange Online в составе Office 365 и локальной версии Exchange, начиная с построения 15.00.0847.032 (Exchange Server 2013 с пакетом обновления 1) . 
  
## <a name="see-also"></a>См. также



[Элементы XML автоматического обнаружения POX для Exchange](pox-autodiscover-xml-elements-for-exchange.md)

