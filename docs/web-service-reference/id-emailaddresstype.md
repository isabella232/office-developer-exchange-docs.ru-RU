---
title: ID (EmailAddressType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Id
api_type:
- schema
ms.assetid: 3e1e37b5-5469-4447-ad1f-c2c6d4e0482f
description: Элемент ID определяет комнату для собраний в организации Exchange Server.
ms.openlocfilehash: 5cd62f6f4e5912d2ecccda352be15c6a3b24e06c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833847"
---
# <a name="id-emailaddresstype"></a>ID (EmailAddressType)

Элемент **ID** определяет комнату для собраний в организации Exchange Server. 
  
[Комната](room.md)
  
[ID (EmailAddressType)](id-emailaddresstype.md)
  
```xml
<Id>
   <Name/>
   <EmailAddress/>
   <RoutingType/>
   <MailboxType/>
   <ItemId/>
</Id>
```

 **EmailAddressType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Имя (EmailAddressType)](name-emailaddresstype.md) <br/> |Определяет имя комнаты для собраний. Этот элемент является необязательным.  <br/> |
|[EmailAddress (Нонемптистрингтипе)](emailaddress-nonemptystringtype.md) <br/> |Определяет SMTP-адрес комнаты для собраний. Этот элемент является необязательным.  <br/> |
|[Раутингтипе (EmailAddress)](routingtype-emailaddress.md) <br/> |Определяет маршрутизацию, используемую для почтового ящика. По умолчанию используется протокол SMTP. Этот элемент является необязательным.  <br/> |
|[MailboxType](mailboxtype.md) <br/> |Определяет тип почтового ящика пользователя почтового ящика. Этот элемент является необязательным.  <br/> |
|[Идентификатор](itemid.md) <br/> |Определяет идентификатор контакта или частный список рассылки для получателей из папки "Контакты" пользователя. Этот элемент является необязательным.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Комната](room.md) <br/> |Определяет комнату для собраний в организации Exchange Server.  <br/> |
   
## <a name="remarks"></a>Примечания

Схема, описывающая этот элемент, находится в каталоге EWS компьютера под управлением Microsoft Exchange Server, на котором установлена роль сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция GetRooms](getrooms-operation.md)


- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

