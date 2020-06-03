---
title: InternalUrl (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 4649baa9-eec9-426d-952b-361818c25fe0
description: Элемент InternalUrl содержит URL-адрес для подключения клиента к серверу адресной книги или почтового ящика пользователя внутри организации пользователя с помощью протокола MAPI/HTTP.
ms.openlocfilehash: 9c6ba621a681ec54d88089de6b7ae1eefdebc679
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465578"
---
# <a name="internalurl-pox"></a>InternalUrl (POX)

Элемент **InternalUrl** содержит URL-адрес для подключения клиента к серверу адресной книги или почтового ящика пользователя внутри организации пользователя с помощью протокола MAPI/HTTP. 
  
```XML
<InternalUrl/>
```

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

Отсутствуют.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[AddressBook (POX)](addressbook-pox.md) <br/> |Содержит спецификации для подключения клиента к серверу адресной книги с помощью протокола MAPI/HTTP.  <br/> |
|[Маилсторе (POX)](mailstore-pox.md) <br/> |Содержит спецификации для подключения клиента к почтовому ящику пользователя с помощью протокола MAPI/HTTP.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение представляет собой URL-адрес, который можно использовать для доступа к почтовому ящику сервера адресной книги или пользователя из Организации.
  
## <a name="remarks"></a>Примечания

Элемент **InternalUrl** может присутствовать в отклике, у которого есть элемент [Protocol (POX)](protocol-pox.md) со значением атрибута **Type** "возможно". 
  
Элемент **InternalUrl** доступен для клиентов, которые реализуют протокол MAPI/HTTP и целевую среду Exchange Online, Exchange Online в составе Office 365, а локальные версии Exchange, начиная с сборки 15.00.0847.032 (Exchange Server 2013 SP1). 
  
## <a name="see-also"></a>См. также



[XML-элементы автообнаружения POX для Exchange](pox-autodiscover-xml-elements-for-exchange.md)

