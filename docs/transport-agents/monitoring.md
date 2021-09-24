---
title: monitoring
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- monitoring
api_type:
- schema
ms.assetid: 350d7b46-9260-41a7-8613-3cb8cc1b29a5
description: 'Последнее изменение: 17 сентября 2015 г.'
ms.openlocfilehash: 215737fb43e1dbef9b7dd11baea1d3f922df7d34
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59540370"
---
# <a name="monitoring"></a>monitoring
  
**Применяется к:** Exchange Server 2013 г.
  
Элемент **мониторинга** содержит сведения о конфигурации, определяющие, как и когда передняя транспортная служба или служба транспорта отслеживает установленные агенты. 
  
- [configuration](configuration.md)  
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
|[agentExecution](agentexecution.md) <br/> |Определяет время, в течение миллисекунд, когда клиентский доступ или сервер почтовых ящиков будут ждать возвращения агента из события перед записью в журнал событий.  <br/> |
|[messageSnapshot](messagesnapshot.md) <br/> |Содержит атрибут, который указывает, включена ли функция отслеживания конвейера для клиентского доступа или сервера почтовых ящиков.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[mexRuntime](mexruntime.md) <br/> |Содержит элементы, определяющие сведения о конфигурации для агентов мониторинга и конфигурации для установленных агентов SMTP и маршрутов.  <br/> |
   
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |Этот файл не определяет пространство имен.  <br/> |
|Имя схемы  <br/> |Недоступно.  <br/> |
|Файл проверки  <br/> |Недоступно.  <br/> |
|Может быть пустым  <br/> |Неверно.  <br/> |
   
## <a name="see-also"></a>См. также

- [Элементы конфигурации файлов агентов для Exchange 2013 г.](agents-configuration-file-elements-for-exchange-2013.md)

