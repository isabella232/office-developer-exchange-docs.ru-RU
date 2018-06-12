---
title: мониторинг
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
description: 'Последнее изменение: 17 сентября 2015'
ms.openlocfilehash: 1b5484467def0bf3d22ba0707357977d5ed461ff
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761313"
---
# <a name="monitoring"></a>мониторинг
  
**Применимо к:** Exchange Server 2013
  
Элемент **мониторинга** содержит сведения о конфигурации, который определяет, как и когда транспортная служба переднего плана или службу транспорта отслеживает агентов, которые устанавливаются. 
  
- [Конфигурация](configuration.md)  
- [mexRuntime](mexruntime.md)  
- [мониторинг](monitoring.md)
  
```XML
<monitoring>
   <agentExecution/>
   <messageSnapshot/>
</monitoring>
```

**monitoringType (complexType)**

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[agentExecution](agentexecution.md) <br/> |Задает время в миллисекундах для клиентского доступа или сервера почтовых ящиков ожидания агента для возврата из события перед записывает в журнал событий.  <br/> |
|[messageSnapshot](messagesnapshot.md) <br/> |Содержит атрибут, который указывает, включена ли функция конвейерной трассировки для клиентского доступа и сервера почтовых ящиков.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[mexRuntime](mexruntime.md) <br/> |Содержит элементы, определяющие данные конфигурации для наблюдение за агентом и данные конфигурации для SMTP и агенты маршрутизации, которые устанавливаются.  <br/> |
   
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |Этот файл не определяет пространство имен.  <br/> |
|Имя схемы  <br/> |Компонент недоступен.  <br/> |
|Файл проверки  <br/> |Компонент недоступен.  <br/> |
|Может быть пустым  <br/> |false  <br/> |
   
## <a name="see-also"></a>См. также

- [Элементы файла конфигурации агентов для Exchange 2013](agents-configuration-file-elements-for-exchange-2013.md)

