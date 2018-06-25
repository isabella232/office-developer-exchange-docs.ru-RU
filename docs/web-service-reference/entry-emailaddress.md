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
description: Элемент представляет адрес электронной почты контакта.
ms.openlocfilehash: 1852584e507c38da030815c37f85f7c4af4e2ba4
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762366"
---
# <a name="entry-emailaddress"></a>Запись (EmailAddress)

**Элемент** представляет адрес электронной почты контакта. 
  
```XML
<Entry Key="" Name="" RoutingType="" MailboxType="" />
```

**EmailAddressDictionaryEntryType**

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|**Key** <br/> | Указывает адрес электронной почты.<br/><br/>Ниже приведены возможные значения этого атрибута.<br/><br/>-EmailAddress1  <br/>-EmailAddress2  <br/>-EmailAddress3 <br/><br/>  Этот атрибут является обязательным.  <br/> |
|**Имя** <br/> |Определяет имя почтового ящика пользователя. Этот атрибут является необязательным.  <br/> |
|**RoutingType** <br/> |Определяет маршрутизации, используемый для почтового ящика. Значение по умолчанию — SMTP. Этот атрибут является необязательным.  <br/> |
|**MailboxType** <br/> |Определяет тип почтового ящика пользователя почтового ящика. Этот атрибут является необязательным.  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[EmailAddresses](emailaddresses.md) <br/> |Представляет коллекцию адреса электронной почты контакта.  <br/> |
   
## <a name="remarks"></a>Замечания

Этот элемент появился в Exchange Server 2013.
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

