---
title: messageSnapshot
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- messageSnapshot
api_type:
- schema
ms.assetid: f157e44c-b950-463f-b086-31d5da94b7ff
description: 'Последнее изменение: 17 сентября 2015 г.'
ms.openlocfilehash: 2ac38dd3f50b5d9d070262f3daffb72b02df5d82
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59525458"
---
# <a name="messagesnapshot"></a>messageSnapshot

**Применяется к:** Exchange Server 2013 г.
  
Элемент **messageSnapshot** содержит атрибут, который указывает, включена ли функция отслеживания конвейера для сервера Exchange, на который установлен клиентский доступ или установлена роль сервера почтовых ящиков. 
  
- [configuration](configuration.md)  
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
|**enabled** <br/> |Значение Boolean, которое указывает, включена ли функция трассиры конвейера для клиентского доступа или сервера почтовых ящиков. Значение **верно, если** включена трассировка конвейера; в противном случае значение является **ложным** или элемент не присутствует.  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[мониторинг](monitoring.md) <br/> |Содержит сведения о конфигурации, определяя, как и когда транспортная служба отслеживает установленные агенты.  <br/> |
   
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |Этот файл не определяет пространство имен.  <br/> |
|Имя схемы  <br/> |Недоступно.  <br/> |
|Файл проверки  <br/> |Недоступно.  <br/> |
|Может быть пустым  <br/> |Неверно.  <br/> |
   
## <a name="see-also"></a>См. также

- [Элементы конфигурации файлов агентов для Exchange 2013 г.](agents-configuration-file-elements-for-exchange-2013.md)

