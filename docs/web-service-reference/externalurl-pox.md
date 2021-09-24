---
title: ExternalUrl (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
ms.assetid: 3b647d88-6feb-40d7-9299-b2ca47b707db
description: Элемент ExternalUrl содержит URL-адрес для подключения клиента к серверу адресной книги или почтовому ящику пользователя из-за пределов организации пользователя с помощью протокола MAPI/HTTP.
ms.openlocfilehash: 90aaf9cabedba4ea89e0ed47da010245006407ba
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59510075"
---
# <a name="externalurl-pox"></a>ExternalUrl (POX)

Элемент **ExternalUrl** содержит URL-адрес для подключения клиента к серверу адресной книги или почтовому ящику пользователя из-за пределов организации пользователя с помощью протокола MAPI/HTTP. 
  
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
|[AddressBook (POX)](addressbook-pox.md) <br/> |Содержит спецификации для подключения клиента к серверу адресной книги с помощью протокола MAPI/HTTP.  <br/> |
|[MailStore (POX)](mailstore-pox.md) <br/> |Содержит спецификации для подключения клиента к почтовому ящику пользователя с помощью протокола MAPI/HTTP.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение представляет URL-адрес, который можно использовать для доступа к серверу адресной книги или почтовому ящику пользователя за пределами организации пользователя.
  
## <a name="remarks"></a>Заметки

Элемент **ExternalUrl может** присутствовать в ответе с элементом [Протокола (POX)](protocol-pox.md) со значением атрибута **Type** "mapiHttp". 
  
Элемент **ExternalUrl** доступен клиентам, реализующими протокол MAPI/HTTP и целевой Exchange Online, Exchange Online в составе Office 365 и локальной версии Exchange начиная со сборки 15.00.0847.032 (Exchange Server 2013 SP1). 
  
## <a name="see-also"></a>См. также



[Элементы XML автооткрытия POX для Exchange](pox-autodiscover-xml-elements-for-exchange.md)

