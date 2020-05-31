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
ms.openlocfilehash: 4a34eedfc16d64cbfa67003ed23cf6eba2bb4bad
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761317"
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

Нет.
  
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

