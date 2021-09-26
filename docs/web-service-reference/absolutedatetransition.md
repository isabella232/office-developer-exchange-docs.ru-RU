---
title: AbsoluteDateTransition
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- AbsoluteDateTransition
api_type:
- schema
ms.assetid: 8f5731eb-bed0-45bf-ba89-4aaf20c34a39
description: Элемент AbsoluteDateTransition представляет переход часовой пояс, который происходит в определенную дату и в определенное время.
ms.openlocfilehash: c0d4e28d8ecefaaa72ded50ab3022666d74ce479
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59542549"
---
# <a name="absolutedatetransition"></a>AbsoluteDateTransition

Элемент **AbsoluteDateTransition представляет** переход часовой пояс, который происходит в определенную дату и в определенное время. 
  
```xml
<AbsoluteDateTransition>
   <To/>
   <DateTime/>
</AbsoluteDateTransition>
```

**AbsoluteDateTransitionType**

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[To](to.md) <br/> |Указывает период [или](period.md) [TransitionsGroup,](transitionsgroup.md) которые должны быть объектом перехода часового пояса.  <br/> |
|[DateTime](datetime.md) <br/> |Представляет дату и время перехода часовой зоны.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Transitions](transitions.md) <br/> |Представляет коллекцию переходов часового пояса.  <br/> |
|[TransitionsGroup](transitionsgroup.md) <br/> |Представляет коллекцию переходов часового пояса.  <br/> |
   
## <a name="remarks"></a>Заметки

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

