---
title: ажентексекутион
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
api_name:
- agentExecution
api_type:
- schema
ms.assetid: 600c4690-941c-45af-a906-5528748d09cd
description: 'Дата последнего изменения: 17 сентября 2015 г.'
ms.openlocfilehash: 457257e59fb37659daf2f91b0fa5dfced5c48c03
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44446492"
---
# <a name="agentexecution"></a>ажентексекутион
  
**Применимо к:** Exchange Server 2013 
  
Элемент **ажентексекутион** определяет время в миллисекундах, в течение которого сервер клиентского доступа или почтовых ящиков должен подождать, пока агент вернется из события, прежде чем запишет в журнал событий. 
  
- [configuration](configuration.md)  
- [текущего](monitoring.md)
- [ажентексекутион](agentexecution.md)
  
```XML
<agentExecution timeLimitInMilliseconds="" />
```

**Ажентексекутионтипе (complexType)**

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|**тимелимитинмиллисекондс** <br/> |Положительное целое число, задающее время ожидания (в миллисекундах) ожидания агентом возврата из события до записи предупреждения в журнал событий. Если это значение слишком мало, производительность может снизиться. Предлагаемое значение для этого атрибута — 300 000, равное 5 минутам.  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

Отсутствуют.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[текущего](monitoring.md) <br/> |Содержит сведения о конфигурации, определяющие, как и когда внешняя служба транспорта или служба транспорта наблюдает за установленными агентами.  <br/> |
   
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Namespace  <br/> |В этом файле не определено пространство имен.  <br/> |
|Имя схемы  <br/> |Недоступно.  <br/> |
|Файл проверки  <br/> |Недоступно.  <br/> |
|Может быть пустым  <br/> |Неверно.  <br/> |
   
## <a name="see-also"></a>См. также

- [Элементы файла конфигурации агентов для Exchange 2013](agents-configuration-file-elements-for-exchange-2013.md)

