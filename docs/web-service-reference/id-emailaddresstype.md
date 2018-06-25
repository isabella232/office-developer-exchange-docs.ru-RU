---
title: Идентификатор (EmailAddressType)
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
description: Элемент Id идентифицирует конференц-зала в пределах организации Exchange server.
ms.openlocfilehash: 5cd62f6f4e5912d2ecccda352be15c6a3b24e06c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833847"
---
# <a name="id-emailaddresstype"></a>Идентификатор (EmailAddressType)

Элемент **Id** идентифицирует конференц-зала в пределах организации Exchange server. 
  
[Комнаты](room.md)
  
[Идентификатор (EmailAddressType)](id-emailaddresstype.md)
  
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

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Имя (EmailAddressType)](name-emailaddresstype.md) <br/> |Определяет имя зала. Этот элемент является необязательным.  <br/> |
|[EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) <br/> |Определяет адрес Simple Mail Transfer Protocol (SMTP) конференц-зала. Этот элемент является необязательным.  <br/> |
|[RoutingType (EmailAddress)](routingtype-emailaddress.md) <br/> |Определяет маршрутизации, используемый для почтового ящика. Значение по умолчанию — SMTP. Этот элемент является необязательным.  <br/> |
|[MailboxType](mailboxtype.md) <br/> |Определяет тип почтового ящика пользователя почтового ящика. Этот элемент является необязательным.  <br/> |
|[Идентификатор элемента](itemid.md) <br/> |Определяет идентификатор элемента контакта или список рассылки закрытый для получателей из папки Контакты. Этот элемент является необязательным.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Комнаты](room.md) <br/> |Определяет конференц-зала в организации Exchange server.  <br/> |
   
## <a name="remarks"></a>Замечания

Схема, описывающая этот элемент находится в каталоге EWS компьютера, на котором выполняется Microsoft Exchange Server с установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция GetRooms](getrooms-operation.md)


- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

