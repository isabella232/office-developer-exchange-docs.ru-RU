---
title: делететипе
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DeleteType
api_type:
- schema
ms.assetid: 6e3136cd-9cb4-493a-aa85-9678f719002d
description: Элемент Делететипе указывает, как удаляются элементы в беседе.
ms.openlocfilehash: 199f7afc29fe866865509d2fb90d24944113d5c0
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44442635"
---
# <a name="deletetype"></a>делететипе

Элемент **делететипе** указывает, как удаляются элементы в беседе. 
  
- [ApplyConversationAction](applyconversationaction.md)  
- [конверсатионактионс](conversationactions.md)  
- [конверсатионактион](conversationaction.md)  
- [делететипе](deletetype.md)
  
```XML
<DeleteType> HardDelete | MoveToDeletedItems | SoftDelete </DeleteType>
```

 **диспосалтипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

Отсутствуют.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[конверсатионактион](conversationaction.md) <br/> |Содержит одно действие, которое будет применено к одной беседе.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение элемента **делететипе** указывает, как удаляются элементы в беседе. Ниже приведены возможные текстовые значения. 
  
- HardDelete — указывает, что элементы в беседе навсегда удаляются из базы данных почтовых ящиков.
    
- Моветоделетеитемс — указывает, что элементы в беседе перемещаются в папку "Удаленные".
    
- SoftDelete — указывает, что элементы в беседе перемещаются в мусорную корзину, если корзина включена.
    
## <a name="remarks"></a>Примечания

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.Этот элемент появился в Exchange Server 2010 с пакетом обновления 1 (SP1).
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Операция ApplyConversationAction](applyconversationaction-operation.md)
- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

