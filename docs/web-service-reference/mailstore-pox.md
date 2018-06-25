---
title: MailStore (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: af338f99-9e62-4124-9bff-8d7cc2008161
description: Элемент MailStore содержит спецификации для подключения клиента к почтовому ящику пользователя с помощью протокола MAPI/HTTP.
ms.openlocfilehash: 4c82c7b61752cf7d91287a3968f6c642f4943855
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834301"
---
# <a name="mailstore-pox"></a>MailStore (POX)

Элемент **MailStore** содержит спецификации для подключения клиента к почтовому ящику пользователя с помощью протокола MAPI/HTTP. 
  
[Автообнаружение (POX)](autodiscover-pox.md)
  
[Ответ (POX)](response-pox.md)
  
[Учетная запись (POX)](account-pox.md)
  
[Протокол (POX)](protocol-pox.md)
  
[MailStore (POX)](mailstore-pox.md)
  
```XML
<MailStore>
   <ExternalUrl/>
   <InternalUrl/>
</MailStore>
```

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[ExternalUrl (POX)](externalurl-pox.md) <br/> |Содержит URL-адрес, который должен использоваться для доступа к почтового ящика пользователя из за пределами сети организации с помощью протокола MAPI/HTTP.  <br/> |
|[InternalUrl (POX)](internalurl-pox.md) <br/> |Содержит URL-адрес, который должен использоваться для доступа к почтового ящика пользователя из внутри сети организации с помощью протокола MAPI/HTTP.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Протокол (POX)](protocol-pox.md) <br/> |Содержит спецификации для подключения клиента к серверу клиентского доступа.  <br/> |
   
## <a name="remarks"></a>Замечания

Элемент **MailStore** присутствует в соответствии с элементом [Протокола (POX)](protocol-pox.md) со значением атрибута **типа** «mapiHttp». 
  
Элемент **MailStore** доступен для клиентов, использующих протокол MAPI/HTTP и конечного Exchange Online, Exchange Online в составе Office 365 и локальной версии Exchange, начиная с построения 15.00.0847.032 (Exchange Server 2013 с пакетом обновления 1). 
  
## <a name="see-also"></a>См. также



[Элементы XML автоматического обнаружения POX для Exchange](pox-autodiscover-xml-elements-for-exchange.md)

