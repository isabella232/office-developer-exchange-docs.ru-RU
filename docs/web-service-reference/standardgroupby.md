---
title: стандардграупби
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- StandardGroupBy
api_type:
- schema
ms.assetid: 04a84f71-b7eb-44dc-ac2c-ed504b52c463
description: Элемент Стандардграупби представляет стандартные механизмы группирования и агрегирования для операции сгруппированной операции FindItem.
ms.openlocfilehash: 3e135feba322979de3d66d5a45d423654ccc9100
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467559"
---
# <a name="standardgroupby"></a>стандардграупби

Элемент **стандардграупби** представляет стандартные механизмы группирования и агрегирования для операции сгруппированной операции FindItem. 
  
[FindItem](finditem.md)
  
[дистингуишедграупби](distinguishedgroupby.md)
  
[стандардграупби](standardgroupby.md)
  
```xml
<StandardGroupBy/>
```

 **стандардграупбитипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

Отсутствуют.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[дистингуишедграупби](distinguishedgroupby.md) <br/> |Предоставляет стандартные группирования для запросов FindItem.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Необходимо указать текстовое значение. Для этого элемента можно использовать только значение **ConversationTopic**. **ConversationTopic** группы по сообщению: ConversationTopic и статистические выражения для элемента: DateTimeReceived (Maximum). Дополнительные сведения о агрегации приведены в разделе [аггрегатеон](aggregateon.md).
  
## <a name="remarks"></a>Примечания

Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция FindItem](finditem-operation.md)
  
[FindItem](finditem.md)


[Поиск элементов](https://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

