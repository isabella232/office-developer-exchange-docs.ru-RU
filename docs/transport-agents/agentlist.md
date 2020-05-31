---
title: ажентлист
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
api_name:
- agentList
api_type:
- schema
ms.assetid: e877b7ef-e303-4270-964d-8d116ff2a865
description: 'Дата последнего изменения: 17 сентября 2015 г.'
ms.openlocfilehash: 7dd9d48356932c82dbc048a85b9f02437c6366de
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761285"
---
# <a name="agentlist"></a>ажентлист
  
**Применимо к:** Exchange Server 2013
  
Элемент **ажентлист** содержит элемент [Agent](agent.md) для каждого установленного агента. 
  
- [configuration](configuration.md)
- [мексрунтиме](mexruntime.md)
- [ажентлист](agentlist.md)
  
```XML
<agentList>
      <agent/>
</agentList>
```

**Ажентлисттипе (complexType)**

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[агента](agent.md) <br/> |Содержит сведения о конфигурации установленного агента.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[мексрунтиме](mexruntime.md) <br/> |Содержит элементы, определяющие сведения о конфигурации для мониторинга агентов и сведения о конфигурации установленных агентов.  <br/> |
   
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Namespace  <br/> |В этом файле не определено пространство имен.  <br/> |
|Имя схемы  <br/> |Недоступно.  <br/> |
|Файл проверки  <br/> |Недоступно.  <br/> |
|Может быть пустым  <br/> |Неверно.  <br/> |
   
## <a name="see-also"></a>См. также

- [Элементы файла конфигурации агентов для Exchange 2013](agents-configuration-file-elements-for-exchange-2013.md)

