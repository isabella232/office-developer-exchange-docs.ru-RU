---
title: agentExecution
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- agentExecution
api_type:
- schema
ms.assetid: 600c4690-941c-45af-a906-5528748d09cd
description: 'Последнее изменение: 17 сентября 2015 г.'
ms.openlocfilehash: 04a53e2698c66326943bcd083c775b53f5c6d5d5
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59513061"
---
# <a name="agentexecution"></a>agentExecution
  
**Применяется к:** Exchange Server 2013 г. 
  
Элемент **agentExecution** определяет время, в миллисекундном периоде, когда клиентский доступ или сервер почтовых ящиков будут ждать, пока агент вернется из события до записи в журнал событий. 
  
- [configuration](configuration.md)  
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
|**timeLimitInMilliseconds** <br/> |Положительное значение integer, которое указывает время, в миллисекунды, для сервера, чтобы ждать агента, чтобы вернуться из события, прежде чем он пишет предупреждение в журнал событий. Производительность может снизиться, если это значение слишком мало. Рекомендуемые значения для этого атрибута — 300 000, что равно 5 минутам.  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[мониторинг](monitoring.md) <br/> |Содержит сведения о конфигурации, определяя, как и когда служба переднего транспорта или служба транспорта отслеживает установленные агенты.  <br/> |
   
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |Этот файл не определяет пространство имен.  <br/> |
|Имя схемы  <br/> |Недоступно.  <br/> |
|Файл проверки  <br/> |Недоступно.  <br/> |
|Может быть пустым  <br/> |Неверно.  <br/> |
   
## <a name="see-also"></a>См. также

- [Элементы конфигурации файлов агентов для Exchange 2013 г.](agents-configuration-file-elements-for-exchange-2013.md)

