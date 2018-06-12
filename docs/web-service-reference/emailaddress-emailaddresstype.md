---
title: EmailAddress (EmailAddressType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 0cdabfcb-7658-4c7d-bb03-1e776ed11e43
description: Элемент EmailAddress указывает полностью разрешенной SMTP-адрес для почтового ящика сайта или связанного пользователя.
ms.openlocfilehash: c31a37fc0dbdcc2b501b82346a17a0a3b4775556
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762274"
---
# <a name="emailaddress-emailaddresstype"></a>EmailAddress (EmailAddressType)

Элемент **EmailAddress** указывает полностью разрешенной SMTP-адрес для почтового ящика сайта или связанного пользователя. 
  
```xml
<EmailAddress>
    <Name></Name>
    <EmailAddress></EmailAddress>
    <RoutingType></RoutingType>
    <MailboxType></MailboxType>
    <ItemId></ItemId>
</EmailAddress>
```

 **EmailAddressType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Имя (строка)](name-string.md) <br/> |Указывает имя уточнения поиска или ключ или имя электронной почты пользователя.  <br/> |
|[EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) <br/> |Определяет основной SMTP-адрес пользователя почтового ящика.  <br/> |
|[RoutingType (EmailAddressType)](routingtype-emailaddresstype.md) <br/> |Указывает тип маршрутизации адресом электронной почты.  <br/> |
|[MailboxType](mailboxtype.md) <br/> |Представляет тип почтового ящика, который соответствует адресу электронной почты.  <br/> |
|[Идентификатор элемента](itemid.md) <br/> |Содержит уникальный идентификатор и меняет ключ элемента в хранилище Exchange.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Пользователь](persona.md) <br/> |Задает набор пользователя данные, возвращаемые запросом **GetPersona** .  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Нет.
  
## <a name="remarks"></a>Замечания

Этот элемент является необязательным.
  
Элемент **EmailAddress** используется для клиентов, относящихся к Exchange Online и версий Microsoft Exchange Server, начиная с Exchange 2013. 
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема типа  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> ||
   
## <a name="see-also"></a>См. также

- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

