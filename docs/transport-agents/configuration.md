---
title: configuration
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
api_name:
- configuration
api_type:
- schema
ms.assetid: 6fc04e4d-657a-4999-9431-186ccb7832b5
description: 'Последнее изменение: 17 сентября 2015'
ms.openlocfilehash: 342e52e879534b6a130d286d358138c6095e4563
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761287"
---
# <a name="configuration"></a>configuration
  
**Применимо к:** Exchange Server 2013
  
Элемент **конфигурации** является корневым элементом для файла конфигурации агентов. 
  
- [Конфигурация](configuration.md) 
- [mexRuntime](mexruntime.md)
  
```XML
<configuration>
      <mexRuntime/>
</configuration>
```

**configurationType (complexType)**

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[mexRuntime](mexruntime.md) <br/> |Содержит элементы, определяющие данные конфигурации для наблюдение за агентом и данные конфигурации для SMTP и агенты маршрутизации, которые устанавливаются.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

Нет.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |Этот файл не определяет пространство имен.  <br/> |
|Имя схемы  <br/> |Компонент недоступен.  <br/> |
|Файл проверки  <br/> |Компонент недоступен.  <br/> |
|Может быть пустым  <br/> |false  <br/> |
   
## <a name="see-also"></a>См. также

- [Элементы файла конфигурации агентов для Exchange 2013](agents-configuration-file-elements-for-exchange-2013.md)

