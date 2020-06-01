---
title: мессажеснапшот
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
description: 'Дата последнего изменения: 17 сентября 2015 г.'
ms.openlocfilehash: 8a58444580c803efb7312df95d75d697bc42e8e0
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44461844"
---
# <a name="messagesnapshot"></a>мессажеснапшот

**Применимо к:** Exchange Server 2013
  
Элемент **мессажеснапшот** содержит атрибут, указывающий, включена ли функция трассировки конвейера для сервера Exchange, на котором установлена роль сервера клиентского доступа или сервера почтовых ящиков. 
  
- [configuration](configuration.md)  
- [мексрунтиме](mexruntime.md) 
- [текущего](monitoring.md) 
- [мессажеснапшот](messagesnapshot.md)
  
```XML
<messageSnapshot enabled="" />
```

**Мессажеснапшоттипе (Boolean)**

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|**enabled** <br/> |Логическое значение, которое указывает, включена ли функция трассировки конвейера для клиентского доступа или сервера почтовых ящиков. Значение **true** , если включена трассировка конвейера; в противном случае — значение **false** или элемент отсутствует.  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

Отсутствуют.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[текущего](monitoring.md) <br/> |Содержит сведения о конфигурации, определяющие, как и когда служба транспорта наблюдает за установленными агентами.  <br/> |
   
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Namespace  <br/> |В этом файле не определено пространство имен.  <br/> |
|Имя схемы  <br/> |Недоступно.  <br/> |
|Файл проверки  <br/> |Недоступно.  <br/> |
|Может быть пустым  <br/> |Неверно.  <br/> |
   
## <a name="see-also"></a>См. также

- [Элементы файла конфигурации агентов для Exchange 2013](agents-configuration-file-elements-for-exchange-2013.md)

