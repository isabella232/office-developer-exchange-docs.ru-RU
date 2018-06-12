---
title: agentExecution
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
description: 'Последнее изменение: 17 сентября 2015'
ms.openlocfilehash: 5848d52a68c8c3f747614015e49becb34bc4cfd8
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761283"
---
# <a name="agentexecution"></a>agentExecution
  
**Применимо к:** Exchange Server 2013 
  
Элемент **agentExecution** определяет время, в миллисекундах для сервера клиентского доступа или почтовых ящиков ожидания агента для возврата из события перед записывает в журнал событий. 
  
- [Конфигурация](configuration.md)  
- [мониторинг](monitoring.md)
- [agentExecution](agentexecution.md)
  
```XML
<agentExecution timeLimitInMilliseconds="" />
```

**agentExecutionType (complexType)**

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|**timeLimitInMilliseconds** <br/> |Значение положительное целое число, указывающее время в миллисекундах для сервера ожидания агента для возврата из события до предупреждения о записи в журнал событий. Если это значение слишком мало, это может привести к производительности. Предлагаемое значение этого атрибута — 300 000, что составляет 5 минут.  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[мониторинг](monitoring.md) <br/> |Содержит сведения о конфигурации, который определяет, как и когда служба транспорта переднего плана или службу транспорта отслеживает агентов, которые устанавливаются.  <br/> |
   
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |Этот файл не определяет пространство имен.  <br/> |
|Имя схемы  <br/> |Компонент недоступен.  <br/> |
|Файл проверки  <br/> |Компонент недоступен.  <br/> |
|Может быть пустым  <br/> |false  <br/> |
   
## <a name="see-also"></a>См. также

- [Элементы файла конфигурации агентов для Exchange 2013](agents-configuration-file-elements-for-exchange-2013.md)

