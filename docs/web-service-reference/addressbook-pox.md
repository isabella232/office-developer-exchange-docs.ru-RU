---
title: AddressBook (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: b2d62fd0-741c-4a41-9762-cc7d0ff01c9c
description: Элемент AddressBook содержит спецификации для подключения клиента к серверу адресной книги с помощью протокола MAPI/HTTP.
ms.openlocfilehash: 0967ac123cd3bb0086fd004ea0d0d37c08d2e037
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463638"
---
# <a name="addressbook-pox"></a>AddressBook (POX)

Элемент **addressBook** содержит спецификации для подключения клиента к серверу адресной книги с помощью протокола MAPI/HTTP. 
  
[Служба автообнаружения (POX)](autodiscover-pox.md)
  
[Ответ (POX)](response-pox.md)
  
[Учетная запись (POX)](account-pox.md)
  
[Протокол (POX)](protocol-pox.md)
  
[AddressBook (POX)](addressbook-pox.md)
  
```XML
<AddressBook>
   <ExternalUrl/>
   <InternalUrl/>
</AddressBook>
```

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[ExternalUrl (POX)](externalurl-pox.md) <br/> |Содержит URL-адрес, который должен использоваться для доступа к адресной книге извне сети Организации с помощью протокола MAPI/HTTP.  <br/> |
|[InternalUrl (POX)](internalurl-pox.md) <br/> |Содержит URL-адрес, который должен использоваться для доступа к адресной книге из сети Организации с помощью протокола MAPI/HTTP.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Протокол (POX)](protocol-pox.md) <br/> |Содержит спецификации для подключения клиента к серверу клиентского доступа.  <br/> |
   
## <a name="remarks"></a>Примечания

Элемент **addressBook** присутствует в отклике, у которого есть элемент [Protocol (POX)](protocol-pox.md) со значением атрибута **Type** "возможно". 
  
Элемент **addressBook** доступен для клиентов, которые реализуют протокол MAPI/HTTP и целевую среду Exchange Online, Exchange Online в составе Office 365, а локальные версии Exchange, начиная с сборки 15.00.0847.032 (Exchange Server 2013 SP1). 
  
## <a name="see-also"></a>См. также

- [XML-элементы автообнаружения POX для Exchange](pox-autodiscover-xml-elements-for-exchange.md)

