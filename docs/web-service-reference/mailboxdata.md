---
title: MailboxData
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MailboxData
api_type:
- schema
ms.assetid: e9e3f50c-5a7b-49c7-a9ea-117959c08352
description: Элемент MailboxData представляет отдельного пользователя почтового ящика и параметры для типа возвращаемых данных о пользователе почтового ящика.
ms.openlocfilehash: bfcb8c01d40af81097c7d9868006fe9b7b5519d4
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467251"
---
# <a name="mailboxdata"></a>MailboxData

Элемент **MailboxData** представляет отдельного пользователя почтового ящика и параметры для типа возвращаемых данных о пользователе почтового ящика. 
  
- [жетусераваилабилитирекуест](getuseravailabilityrequest.md)
  
- [маилбоксдатааррай](mailboxdataarray.md)
  
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

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Электронная почта (EmailAddressType)](email-emailaddresstype.md) <br/> |Представляет пользователя почтового ящика для запроса GetUserAvailability.  <br/> |
|[AttendeeType](attendeetype.md) <br/> |Представляет тип участника, идентифицированного в элементе [электронной почты (EmailAddressType)](email-emailaddresstype.md) . Используется в запросах предложений о собрании.  <br/> |
|[ексклудеконфликтс](excludeconflicts.md) <br/> |Указывает, следует ли возвращать предлагаемые времена для календарных ситуаций, в которых возникает конфликт между участниками.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[маилбоксдатааррай](mailboxdataarray.md) <br/> |Содержит список почтовых ящиков, в которых запрашиваются сведения о доступности.  <br/> XPath для этого элемента:  <br/>  `/GetUserAvailabilityRequest/MailboxDataArray[i]` <br/> |
   
## <a name="remarks"></a>Примечания

Клиентское приложение может определять один или несколько элементов **MailboxData** . 
  
> [!NOTE]
> Схема, описывающая этот элемент, находится в виртуальном каталоге EWS компьютера, на котором установлен сервер Exchange Server 2007 с ролью сервера клиентского доступа. 
  
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
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Операция GetUserAvailability](getuseravailability-operation.md)
- [жетусераваилабилитирекуест](getuseravailabilityrequest.md)
- [Getting User Availability](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

