---
title: Отдел операций
manager: sethgros
ms.date: 09/17/2015
ms.audience: ITPro
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Operations
api_type:
- schema
ms.assetid: d8cd41b1-28ae-4c95-9ff6-8b25c8e18306
description: Элемент Operations содержит массив операций правил, которые можно выполнять в почтовом ящике.
ms.openlocfilehash: 48679c9c7c0482ab53d3af5c661dc6efe513e637
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59518073"
---
# <a name="operations"></a>Отдел операций

Элемент **Operations** содержит массив операций правил, которые можно выполнять в почтовом ящике. 
  
[UpdateInboxRules](updateinboxrules.md)
  
```XML
<Operations>
    <CreateRuleOperation/>
    <SetRuleOperation/>
    <DeleteRuleOperation/>
</Operations>
```

 **ArrayOfRuleOperationsType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[CreateRuleOperation](createruleoperation.md) <br/> |Представляет операцию по созданию нового правила "Входящие".  <br/> |
|[SetRuleOperation](setruleoperation.md) <br/> |Представляет операцию по обновлению правила "Входящие".  <br/> |
|[DeleteRuleOperation](deleteruleoperation.md) <br/> |Представляет операцию по удалите правило "Входящие".  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[UpdateInboxRules](updateinboxrules.md) <br/> |Определяет запрос на обновление правил "Входящие" в почтовом ящике в серверном магазине.  <br/> |
   
## <a name="remarks"></a>Заметки

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция UpdateInboxRules](updateinboxrules-operation.md)


- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

