---
title: Position
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 46726ebb-a403-4793-8378-282aa7dc39d0
description: Элемент Position указывает позицию объекта, извлеченного из сообщения.
ms.openlocfilehash: 9acd965c3e0c29f3fa91df338c0671749192b38b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465424"
---
# <a name="position"></a>Position

Элемент **position** указывает позицию объекта, извлеченного из сообщения. 
  
```XML
<Position> LatestReply | Other | Subject | Signature </Position>
```

 **емаилпоситионтипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

Отсутствуют.
  
### <a name="parent-elements"></a>Родительские элементы

[Урлентити](urlentity.md)  |  [Аддрессентити](addressentity.md)  |  [Емаиладдрессентити](emailaddressentity.md)  |  [Свойства meetingsuggestion](meetingsuggestion.md)  |  [Контактное лицо (контакттипе)](contact-contacttype.md)  |  [Телефон (фонинтититипе)](phone-phoneentitytype.md)  |  [TaskSuggestion](tasksuggestion.md)
  
## <a name="text-value"></a>Текстовое значение

Текстовое значение элемента **position** — это место, в котором извлеченная сущность была создана в исходном сообщении. Текстовые значения для элемента **position** : 
  
- **Латестрепли** — извлеченная сущность поступает из последнего ответа на сообщение. 
    
- **Другой** — извлеченная сущность поступает из неопределенной части сообщения. 
    
- **Subject** — извлеченная сущность поступает из темы сообщения. 
    
- **Подпись** — извлеченная сущность берется из подписи сообщения. 
    
## <a name="remarks"></a>Примечания

Этот элемент появился в Exchange Server 2013.
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> ||
   

