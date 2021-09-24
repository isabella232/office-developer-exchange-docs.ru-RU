---
title: Value (EmailAddressType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 24eaa473-0024-47e2-b7d2-051d5dd4f53c
description: Элемент Value указывает значение emailAddress, связанного с массивом атрибуций.
ms.openlocfilehash: 21859c6cc4c05e55029758ce25bdf312b5f084fa
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59522518"
---
# <a name="value-emailaddresstype"></a>Value (EmailAddressType)

Элемент **Value** указывает значение **emailAddress,** связанного с массивом атрибуций. 
  
```XML
<Value>
   <Name/>
   <EmailAddress/>
   <RoutingType/>
   <MailboxType/>
   <ItemId/>
   <OriginalDisplayName/>
</Value>
```

**EmailAddressType**

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

[Имя (строка)](name-string.md)  |  [EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md)  |  [RoutingType (EmailAddressType)](routingtype-emailaddresstype.md)  |  [Почтовый ящикType](mailboxtype.md)  |  [ItemId](itemid.md)  |  [OriginalDisplayName](originaldisplayname.md)
  
### <a name="parent-elements"></a>Родительские элементы

[EmailAddressAttributedValue](emailaddressattributedvalue.md)
  
## <a name="remarks"></a>Заметки

Этот элемент появился в Exchange Server 2013.
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |false  <br/> |
   

