---
title: EmailAddress (EmailAddressType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 0cdabfcb-7658-4c7d-bb03-1e776ed11e43
description: Элемент EmailAddress указывает полностью решенный SMTP-адрес для почтового ящика сайта или связанного с ним лица.
ms.openlocfilehash: 76b279a82f6f277d9f231866437359ceae46df59
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59545260"
---
# <a name="emailaddress-emailaddresstype"></a>EmailAddress (EmailAddressType)

Элемент **EmailAddress** указывает полностью решенный SMTP-адрес для почтового ящика сайта или связанного с ним лица. 
  
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
|[Name (строка)](name-string.md) <br/> |Указывает имя или ключ поиска или имя пользователя электронной почты.  <br/> |
|[EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) <br/> |Определяет основной SMTP-адрес пользователя почтового ящика.  <br/> |
|[RoutingType (EmailAddressType)](routingtype-emailaddresstype.md) <br/> |Указывает тип маршрутивки адреса электронной почты.  <br/> |
|[MailboxType](mailboxtype.md) <br/> |Представляет тип почтового ящика, который представлен адресом электронной почты.  <br/> |
|[ItemId](itemid.md) <br/> |Содержит уникальный идентификатор и ключ изменения элемента в Exchange магазине.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Роль](persona.md) <br/> |Указывает набор данных persona, возвращаемого по запросу **GetPersona.**  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Нет.
  
## <a name="remarks"></a>Заметки

Этот элемент является необязательным.
  
Элемент **EmailAddress** применим для клиентов, которые Exchange Online и версии Microsoft Exchange Server начиная с Exchange 2013 года. 
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема типа  <br/> |
|Файл проверки  <br/> |types.xsd  <br/> |
|Может быть пустым  <br/> ||
   
## <a name="see-also"></a>См. также

- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

