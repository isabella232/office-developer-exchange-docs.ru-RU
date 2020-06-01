---
title: EmailAddress (Жетперсонатипе)
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 052055b5-4630-40ed-9b24-9e7f4bf7ba1d
description: Элемент EmailAddress (Жетперсонатипе) указывает адрес электронной почты, связанный с персонажом.
ms.openlocfilehash: b58f61202cd94ff282b21138b47b40887b38752a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463456"
---
# <a name="emailaddress-getpersonatype"></a>EmailAddress (Жетперсонатипе)

Элемент **EmailAddress (жетперсонатипе)** указывает адрес электронной почты, связанный с персонажом. 
  
```XML
<EmailAddress>
    <Name></Name>
    <EmailAddress></EmailAddress>
    <RoutingType></RoutingType>
    <MailboxType></MailboxType>
    <ItemId></ItemId>
    <OriginalDisplayName></OriginalDisplayName>
</EmailAddress>>
```

 **EmailAddressType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

[Имя (строка)](name-string.md)  |  [EmailAddress (нонемптистрингтипе)](emailaddress-nonemptystringtype.md)  |  [Раутингтипе (EmailAddressType)](routingtype-emailaddresstype.md)  |  [MailboxType](mailboxtype.md)  |  [ItemId](itemid.md)  |  [Оригиналдисплайнаме](originaldisplayname.md)
  
### <a name="parent-elements"></a>Родительские элементы

[GetPersona](getpersona.md)
  
## <a name="remarks"></a>Примечания

Этот элемент появился в Exchange Server 2013 с пакетом обновления 1 (SP1).
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages. xsd  <br/> |
|Может быть пустым  <br/> |True  <br/> |
   
## <a name="see-also"></a>См. также

- [GetPersona](getpersona.md)
- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

