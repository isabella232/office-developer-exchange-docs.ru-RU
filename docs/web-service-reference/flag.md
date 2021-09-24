---
title: Flag
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 7b47bc74-a60d-4308-8674-5d52444a1753
description: Элемент Флаг указывает флаг на элементе почтового ящика.
ms.openlocfilehash: dffc550dc4235c2121b6641f3a6eac30594f75b3
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59513698"
---
# <a name="flag"></a>Flag

Элемент **Флаг** указывает флаг на элементе почтового ящика. 
  
```XML
<Flag>
    <FlagStatus/>
    <StartDate/>
    <DueDate/>
    <CompleteDate/>
</Flag>
```

 **FlagType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[FlagStatus](flagstatus.md) <br/> |Содержит агрегированное состояние флага для элементов в текущей папке.  <br/> |
|[StartDate](startdate.md) <br/> |Представляет дату начала элемента.  <br/> |
|[DueDate](duedate.md) <br/> |Представляет дату, когда должен быть элемент.  <br/> |
|[CompleteDate](completedate.md) <br/> |Представляет дату завершения элемента.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[ConversationAction](conversationaction.md) <br/> |Содержит одно действие, которое необходимо применить к одному разговору.  <br/> |
|[Элемент](item.md) <br/> |Представляет универсальный элемент в Exchange магазине.  <br/> |
   
## <a name="remarks"></a>Заметки

Этот элемент появился в Exchange Server 2013.
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема типа  <br/> |
|Файл проверки  <br/> |types.xsd  <br/> |
|Может быть пустым  <br/> ||
   
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

