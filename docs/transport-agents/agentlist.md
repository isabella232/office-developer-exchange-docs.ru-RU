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
ms.openlocfilehash: 99e4e24c3bca77c7e7d5f2c59bb21cee1317fed2
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44446394"
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

Отсутствуют.
  
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

