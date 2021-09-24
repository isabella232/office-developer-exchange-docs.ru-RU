---
title: Position
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 46726ebb-a403-4793-8378-282aa7dc39d0
description: Элемент Position указывает положение объекта, извлеченного из сообщения.
ms.openlocfilehash: 6b4e7c12bbcf12b8804619caa508f5c2c0bc4eda
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59515294"
---
# <a name="position"></a>Position

Элемент **Position** указывает положение объекта, извлеченного из сообщения. 
  
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

[UrlEntity](urlentity.md)  |  [AddressEntity](addressentity.md)  |  [EmailAddressEntity](emailaddressentity.md)  |  [MeetingSuggestion](meetingsuggestion.md)  |  [Контакт (ContactType)](contact-contacttype.md)  |  [Телефон (PhoneEntityType)](phone-phoneentitytype.md)  |  [TaskSuggestion](tasksuggestion.md)
  
## <a name="text-value"></a>Текстовое значение

Текстовое значение элемента **Position** — это расположение, в котором извлекаемая сущность возникла в исходных сообщениях. Текстовые значения элемента **Position:** 
  
- **LatestReply** — извлеченная сущность возникает из последнего ответа на сообщение. 
    
- **Другое** — извлекаемая сущность возникает из неопределяемой части сообщения. 
    
- **Subject** — извлекаемая сущность берет свое начало из темы сообщения. 
    
- **Подпись** — извлекаемая сущность возникает из подписи сообщения. 
    
## <a name="remarks"></a>Заметки

Этот элемент появился в Exchange Server 2013.
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> ||
   

