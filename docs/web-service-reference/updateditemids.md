---
title: UpdatedItemIds
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 9199aeb2-abdf-40c5-8743-40b61853c951
description: Элемент UpdatedItemIds указывает идентификаторы обновленных элементов напоминаний.
ms.openlocfilehash: 59e17e32d5df3f8a6000b05899f2fe0c5de2ec00
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59538613"
---
# <a name="updateditemids"></a>UpdatedItemIds

Элемент **UpdatedItemIds** указывает идентификаторы обновленных элементов напоминаний. 
  
```XML
<UpdatedItemIds>
   <ItemId></ItemId>
</UpdatedItemIds>

```

 **NonEmptyArrayOfItemIdsType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

[ItemId](itemid.md)
  
### <a name="parent-elements"></a>Родительские элементы

[PerformReminderActionResponse](performreminderactionresponse.md)
  
## <a name="remarks"></a>Заметки

Этот элемент появился в Exchange Server 2013.
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
Если операция [PerformReminderAction](performreminderaction-operation.md) не завершилась успешно или на сервере не были внесены изменения, элемент **UpdatedItemIds** возвращается как пустое значение. 
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |True  <br/> |
   
## <a name="see-also"></a>См. также



[PerformReminderActionResponse](performreminderactionresponse.md)


- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

