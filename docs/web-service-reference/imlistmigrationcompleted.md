---
title: ImListMigrationCompleted
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 6eed9502-5d9e-4345-ba23-3582ff487147
description: Элемент ImListMigrationCompleted указывает, содержится ли в Exchange элементов обмена мгновенными сообщениями, используемых клиентами мгновенных сообщений.
ms.openlocfilehash: b55f3d72259897d7bdf46b351421b0148a41b93e
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59514615"
---
# <a name="imlistmigrationcompleted"></a>ImListMigrationCompleted

Элемент **ImListMigrationCompleted** указывает, содержит ли Exchange хранилище элементы обмена мгновенными сообщениями, используемые клиентами обмена мгновенными сообщениями. 
  
```XML
<ImListMigrationCompleted>true | false</ImListMigrationCompleted>
```

 **Boolean**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

[SetImListMigrationCompleted](setimlistmigrationcompleted.md)
  
## <a name="text-value"></a>Текстовое значение

Текстовое значение true **для** элемента **ImListMigrationCompleted** указывает, что хранилище контактов мгновенных сообщений было перенесено в Exchange хранилище. Значение false **указывает** на то, что хранилище мгновенных контактов сообщений не было перенесено. 
  
## <a name="remarks"></a>Заметки

Этот элемент появился в Exchange Server 2013.
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> ||
   

