---
title: Флаг
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 7b47bc74-a60d-4308-8674-5d52444a1753
description: Элемент Flag указывает флаг для элемента почтового ящика.
ms.openlocfilehash: 7229a26181ee9baf80be5c32c0ef99483310ccb3
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44466264"
---
# <a name="flag"></a>Флаг

Элемент **Flag** указывает флаг для элемента почтового ящика. 
  
```XML
<Flag>
    <FlagStatus/>
    <StartDate/>
    <DueDate/>
    <CompleteDate/>
</Flag>
```

 **флагтипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[FlagStatus](flagstatus.md) <br/> |Содержит сводный статус флагов для элементов в текущей папке.  <br/> |
|[StartDate](startdate.md) <br/> |Представляет дату начала элемента.  <br/> |
|[DueDate](duedate.md) <br/> |Представляет дату выполнения элемента.  <br/> |
|[комплетедате](completedate.md) <br/> |Представляет дату завершения элемента.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[конверсатионактион](conversationaction.md) <br/> |Содержит одно действие, которое будет применено к одной беседе.  <br/> |
|[Ресурс](item.md) <br/> |Представляет общий элемент в хранилище Exchange.  <br/> |
   
## <a name="remarks"></a>Примечания

Этот элемент появился в Exchange Server 2013.
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема типа  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> ||
   
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

