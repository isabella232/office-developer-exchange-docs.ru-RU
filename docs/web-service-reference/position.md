---
title: Position
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 46726ebb-a403-4793-8378-282aa7dc39d0
description: Элемент позиции указывает положение сущности, извлеченные из сообщения.
ms.openlocfilehash: 4bd8f3088891e918e13d5ef1ec8e3e5217cb3fa1
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834853"
---
# <a name="position"></a>Position

Элемент **позиции** указывает положение сущности, извлеченные из сообщения. 
  
```XML
<Position> LatestReply | Other | Subject | Signature </Position>
```

 **EmailPositionType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

[UrlEntity](urlentity.md) | [AddressEntity](addressentity.md) | [EmailAddressEntity](emailaddressentity.md) | [MeetingSuggestion](meetingsuggestion.md) | [контакт (ContactType)](contact-contacttype.md) | [Телефон (PhoneEntityType)](phone-phoneentitytype.md)  |  [ TaskSuggestion](tasksuggestion.md)
  
## <a name="text-value"></a>Текстовое значение

Текстовое значение элемента **положение** — расположение источник извлеченный объект в исходного сообщения. Приведены значения параметра текст для элемента **положение** . 
  
- **LatestReply** - извлеченный объект исходит от последнего ответа на сообщение. 
    
- **Другие** - извлеченный объект исходит от undefined часть сообщения. 
    
- **Тема** - извлеченный объект исходит от теме сообщения. 
    
- **Подпись** - извлеченный объект исходит от подпись сообщения. 
    
## <a name="remarks"></a>Замечания

Этот элемент появился в Exchange Server 2013.
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> ||
   

