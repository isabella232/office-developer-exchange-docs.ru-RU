---
title: messageSnapshot
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
api_name:
- messageSnapshot
api_type:
- schema
ms.assetid: f157e44c-b950-463f-b086-31d5da94b7ff
description: 'Последнее изменение: 17 сентября 2015'
ms.openlocfilehash: 4b814def8eef8fb452d2e754c5f6787d644055f7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761314"
---
# <a name="messagesnapshot"></a>messageSnapshot

**Применимо к:** Exchange Server 2013
  
Элемент **messageSnapshot** содержит атрибут, который указывает, включена ли функция конвейерной трассировки для Exchange server с клиентского доступа или установлена роль сервера почтовых ящиков. 
  
- [Конфигурация](configuration.md)  
- [mexRuntime](mexruntime.md) 
- [мониторинг](monitoring.md) 
- [messageSnapshot](messagesnapshot.md)
  
```XML
<messageSnapshot enabled="" />
```

**messageSnapshotType (Boolean)**

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|**включено** <br/> |Логическое значение, указывающее, включена ли функция конвейерной трассировки для клиентского доступа и сервера почтовых ящиков. Значение равно **true** , если включена конвейерной трассировки. в противном случае — значение равно **false** или элемент не существует.  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[мониторинг](monitoring.md) <br/> |Содержит сведения о конфигурации, который определяет, как и когда транспортная служба отслеживает агентов, которые устанавливаются.  <br/> |
   
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |Этот файл не определяет пространство имен.  <br/> |
|Имя схемы  <br/> |Компонент недоступен.  <br/> |
|Файл проверки  <br/> |Компонент недоступен.  <br/> |
|Может быть пустым  <br/> |false  <br/> |
   
## <a name="see-also"></a>См. также

- [Элементы файла конфигурации агентов для Exchange 2013](agents-configuration-file-elements-for-exchange-2013.md)

