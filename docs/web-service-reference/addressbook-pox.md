---
title: AddressBook (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
ms.assetid: b2d62fd0-741c-4a41-9762-cc7d0ff01c9c
description: Элемент AddressBook содержит спецификации для подключения клиента к серверу адресной книги с помощью протокола MAPI/HTTP.
ms.openlocfilehash: 28de1d41146b082c8b7f82c868fbbed1ce2c483e
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59546800"
---
# <a name="addressbook-pox"></a>AddressBook (POX)

Элемент **AddressBook** содержит спецификации для подключения клиента к серверу адресной книги с помощью протокола MAPI/HTTP. 
  
[AutoDiscover (POX)](autodiscover-pox.md)
  
[Response (POX)](response-pox.md)
  
[Account (POX)](account-pox.md)
  
[Protocol (POX)](protocol-pox.md)
  
[AddressBook (POX)](addressbook-pox.md)
  
```XML
<AddressBook>
   <ExternalUrl/>
   <InternalUrl/>
</AddressBook>
```

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[ExternalUrl (POX)](externalurl-pox.md) <br/> |Содержит URL-адрес, который должен использоваться для доступа к адресной книге из-за пределов сети организации с помощью протокола MAPI/HTTP.  <br/> |
|[InternalUrl (POX)](internalurl-pox.md) <br/> |Содержит URL-адрес, который должен использоваться для доступа к адресной книге из сети организации с помощью протокола MAPI/HTTP.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Protocol (POX)](protocol-pox.md) <br/> |Содержит спецификации для подключения клиента к серверу клиентского доступа.  <br/> |
   
## <a name="remarks"></a>Заметки

Элемент **AddressBook** присутствует в ответе, который имеет элемент [Protocol (POX)](protocol-pox.md) со значением **атрибута Type** "mapiHttp". 
  
Элемент **AddressBook** доступен клиентам, реализующими протокол MAPI/HTTP и целевой Exchange Online, Exchange Online в составе Office 365 и локальной версии Exchange начиная со сборки 15.00.0847.032 (Exchange Server 2013 SP1). 
  
## <a name="see-also"></a>См. также

- [Элементы XML автооткрытия POX для Exchange](pox-autodiscover-xml-elements-for-exchange.md)

