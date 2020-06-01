---
title: текущего
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
api_name:
- monitoring
api_type:
- schema
ms.assetid: 350d7b46-9260-41a7-8613-3cb8cc1b29a5
description: 'Дата последнего изменения: 17 сентября 2015 г.'
ms.openlocfilehash: 5614ac2c6428da9b6845769a9335486d3ded5754
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44455830"
---
# <a name="monitoring"></a>текущего
  
**Применимо к:** Exchange Server 2013
  
Элемент **Monitor** содержит сведения о конфигурации, которые определяют, как и когда внешняя служба транспорта или служба транспорта наблюдает за установленными агентами. 
  
- [configuration](configuration.md)  
- [мексрунтиме](mexruntime.md)  
- [текущего](monitoring.md)
  
```XML
<monitoring>
   <agentExecution/>
   <messageSnapshot/>
</monitoring>
```

**Мониторингтипе (complexType)**

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[ажентексекутион](agentexecution.md) <br/> |Определяет время в миллисекундах для клиентского доступа или сервера почтовых ящиков для ожидания возврата агентом из события перед записью в журнал событий.  <br/> |
|[мессажеснапшот](messagesnapshot.md) <br/> |Содержит атрибут, указывающий, включена ли функция трассировки конвейера для клиентского доступа или сервера почтовых ящиков.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[мексрунтиме](mexruntime.md) <br/> |Содержит элементы, определяющие сведения о конфигурации для мониторинга агентов и сведения о конфигурации для установленных агентов SMTP и маршрутизации.  <br/> |
   
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Namespace  <br/> |В этом файле не определено пространство имен.  <br/> |
|Имя схемы  <br/> |Недоступно.  <br/> |
|Файл проверки  <br/> |Недоступно.  <br/> |
|Может быть пустым  <br/> |Неверно.  <br/> |
   
## <a name="see-also"></a>См. также

- [Элементы файла конфигурации агентов для Exchange 2013](agents-configuration-file-elements-for-exchange-2013.md)

