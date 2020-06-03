---
title: Запись (EmailAddress)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Entry
api_type:
- schema
ms.assetid: b028c5c7-3494-4ecd-96d1-78783daa660f
description: Элемент entry представляет один адрес электронной почты контакта.
ms.openlocfilehash: 766d67cda10b02c07a7677e541fddfc38a4285cf
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459646"
---
# <a name="entry-emailaddress"></a>Запись (EmailAddress)

Элемент **entry** представляет один адрес электронной почты контакта. 
  
```XML
<Entry Key="" Name="" RoutingType="" MailboxType="" />
```

**емаиладдрессдиктионарентритипе**

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|**Key** <br/> | Определяет адрес электронной почты.<br/><br/>Ниже приведены возможные значения для этого атрибута.<br/><br/>- EmailAddress1  <br/>- EmailAddress2  <br/>- EmailAddress3 <br/><br/>  Этот атрибут является обязательным.  <br/> |
|**имя** <br/> |Определяет имя пользователя почтового ящика. Этот атрибут является необязательным.  <br/> |
|**раутингтипе** <br/> |Определяет маршрутизацию, используемую для почтового ящика. По умолчанию используется протокол SMTP. Этот атрибут является необязательным.  <br/> |
|**MailboxType** <br/> |Определяет тип почтового ящика пользователя почтового ящика. Этот атрибут является необязательным.  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

Отсутствуют.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[EmailAddresses](emailaddresses.md) <br/> |Представляет коллекцию адресов электронной почты контакта.  <br/> |
   
## <a name="remarks"></a>Примечания

Этот элемент появился в Exchange Server 2013.
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

