---
title: ImListMigrationCompleted
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 6eed9502-5d9e-4345-ba23-3582ff487147
description: Элемент ImListMigrationCompleted указывает, содержит ли хранилище Exchange элементы для обмена мгновенными сообщениями, используемые клиентами обмена мгновенными сообщениями.
ms.openlocfilehash: 09f37d6e3663aab7cb98fc922f727ddd604f2acd
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44456026"
---
# <a name="imlistmigrationcompleted"></a>ImListMigrationCompleted

Элемент **ImListMigrationCompleted** указывает, содержит ли хранилище Exchange элементы для обмена мгновенными сообщениями, используемые клиентами обмена мгновенными сообщениями. 
  
```XML
<ImListMigrationCompleted>true | false</ImListMigrationCompleted>
```

 **Boolean**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

Отсутствуют.
  
### <a name="parent-elements"></a>Родительские элементы

[сетимлистмигратионкомплетед](setimlistmigrationcompleted.md)
  
## <a name="text-value"></a>Текстовое значение

Текстовое значение **true** для элемента **ImListMigrationCompleted** указывает на то, что хранилище контактов для обмена мгновенными сообщениями было перенесено в хранилище Exchange. Значение **false** указывает, что хранилище контактов для обмена мгновенными сообщениями не было перенесено. 
  
## <a name="remarks"></a>Примечания

Этот элемент появился в Exchange Server 2013.
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages. xsd  <br/> |
|Может быть пустым  <br/> ||
   

