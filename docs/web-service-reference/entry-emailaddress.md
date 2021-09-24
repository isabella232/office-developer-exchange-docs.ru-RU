---
title: Entry (EmailAddress)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Entry
api_type:
- schema
ms.assetid: b028c5c7-3494-4ecd-96d1-78783daa660f
description: Элемент Entry представляет единый адрес электронной почты для контакта.
ms.openlocfilehash: 96351a82e113f2c4aa73776e89e1eb7e7a683433
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59520670"
---
# <a name="entry-emailaddress"></a>Entry (EmailAddress)

Элемент **Entry** представляет единый адрес электронной почты для контакта. 
  
```XML
<Entry Key="" Name="" RoutingType="" MailboxType="" />
```

**EmailAddressDictionaryEntryType**

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|**Ключ** <br/> | Определяет адрес электронной почты.<br/><br/>Возможные значения для этого атрибута:<br/><br/>- EmailAddress1  <br/>- EmailAddress2  <br/>- EmailAddress3 <br/><br/>  Этот атрибут является обязательным.  <br/> |
|**Имя** <br/> |Определяет имя пользователя почтового ящика. Этот атрибут является необязательным.  <br/> |
|**RoutingType** <br/> |Определяет маршрутику, используемую для почтового ящика. По умолчанию значение SMTP. Этот атрибут является необязательным.  <br/> |
|**MailboxType** <br/> |Определяет тип почтового ящика пользователя почтового ящика. Этот атрибут является необязательным.  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[EmailAddresses](emailaddresses.md) <br/> |Представляет коллекцию адресов электронной почты для контакта.  <br/> |
   
## <a name="remarks"></a>Заметки

Этот элемент появился в Exchange Server 2013.
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

