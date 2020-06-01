---
title: мексрунтиме
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
api_name:
- mexRuntime
api_type:
- schema
ms.assetid: eabb2f12-10a7-4ce2-ae4b-9c04010c765f
description: 'Дата последнего изменения: 17 сентября 2015 г.'
ms.openlocfilehash: f192965a8375eb46d1ca5b46d3b768a3299c284d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44461837"
---
# <a name="mexruntime"></a>мексрунтиме
  
**Применимо к:** Exchange Server 2013
  
Элемент **мексрунтиме** содержит элементы, определяющие сведения о конфигурации для мониторинга агентов и сведения о конфигурации агентов маршрутизации SMTP и маршрутизации, которые установлены. 
  
- [configuration](configuration.md)  
- [мексрунтиме](mexruntime.md)
  
```XML
<mexRuntime>
   <monitoring/>
   <agentList/>
</mexRuntime>
```

**Мексрунтиметипе (complexType)**

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[текущего](monitoring.md) <br/> |Содержит сведения о конфигурации, определяющие, как и когда транспортный монитор устанавливает агенты.  <br/> |
|[ажентлист](agentlist.md) <br/> |Содержит элемент [Agent](agent.md) для каждого установленного агента.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[configuration](configuration.md) <br/> |Корневой элемент для файла конфигурации агентов.  <br/> |
   
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Namespace  <br/> |В этом файле не определено пространство имен.  <br/> |
|Имя схемы  <br/> |Недоступно.  <br/> |
|Файл проверки  <br/> |Недоступно.  <br/> |
|Может быть пустым  <br/> |Неверно.  <br/> |
   
## <a name="see-also"></a>См. также

- [Элементы файла конфигурации агентов для Exchange 2013](agents-configuration-file-elements-for-exchange-2013.md)

