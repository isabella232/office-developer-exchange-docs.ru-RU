---
title: MailboxData
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- MailboxData
api_type:
- schema
ms.assetid: e9e3f50c-5a7b-49c7-a9ea-117959c08352
description: Элемент MailboxData представляет отдельного пользователя почтового ящика и параметры типа данных, которые будут возвращены о пользователе почтового ящика.
ms.openlocfilehash: 62c8c816fc0b0e0c6831d468d90e7303fb72d9be
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59546135"
---
# <a name="mailboxdata"></a>MailboxData

Элемент **MailboxData** представляет отдельного пользователя почтового ящика и параметры типа данных, которые будут возвращены о пользователе почтового ящика. 
  
- [GetUserAvailabilityRequest](getuseravailabilityrequest.md)
  
- [MailboxDataArray](mailboxdataarray.md)
  
- [MailboxData](mailboxdata.md)
  
```xml
<MailboxData>
   <Email>...</Email>
   <AttendeeType>...</AttendeeType>
   <ExcludeConflicts>...</ExcludeConflicts>
<MailboxData>
```

**MailboxData**

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Email (EmailAddressType)](email-emailaddresstype.md) <br/> |Представляет пользователя почтового ящика для запроса GetUserAvailability.  <br/> |
|[AttendeeType](attendeetype.md) <br/> |Представляет тип участника, идентифицированного в [элементе Email (EmailAddressType).](email-emailaddresstype.md) Это используется в запросах на предложения собрания.  <br/> |
|[ExcludeConflicts](excludeconflicts.md) <br/> |Указывает, следует ли возвращать рекомендуемые время для календарного времени, которое конфликтуется между участниками.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[MailboxDataArray](mailboxdataarray.md) <br/> |Содержит список почтовых ящиков для запроса сведений о доступности.  <br/> XPath для этого элемента:  <br/>  `/GetUserAvailabilityRequest/MailboxDataArray[i]` <br/> |
   
## <a name="remarks"></a>Заметки

Клиентская приложение может определить один для многих **элементов MailboxData.** 
  
> [!NOTE]
> Схема, описываемая этим элементом, расположена в виртуальном каталоге компьютера EWS, который работает Exchange Server 2007 г., где установлена роль сервера клиентского доступа. 
  
## <a name="example"></a>Пример

```xml
<MailboxDataArray>
  <MailboxData xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
    <Email>
      <Name></Name>
      <Address>someone@ExServer.example.com</Address>
      <RoutingType>SMTP</RoutingType>
    </Email>
    <AttendeeType>Organizer</AttendeeType>
    <ExcludeConflicts>false</ExcludeConflicts>
  </MailboxData>
</MailboxDataArray>
```

## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Операция GetUserAvailability](getuseravailability-operation.md)
- [GetUserAvailabilityRequest](getuseravailabilityrequest.md)
- [Getting User Availability](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

