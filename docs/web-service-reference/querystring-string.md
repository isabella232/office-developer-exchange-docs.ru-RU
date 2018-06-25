---
title: Строка запроса (строка)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f81b1b3d-9fe4-4ab3-b517-42e4207fa596
description: Элемент строки запроса указывает набор значений, возвращаемых, соответствующих строки запроса в запрос операции FindPeople. Поиск по не указан строки запроса возвращает все элементы в указанной папке.
ms.openlocfilehash: 9c5c733adcec1496e36986fd720b56b0a0274593
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834935"
---
# <a name="querystring-string"></a>Строка запроса (строка)

Элемент **строки запроса** указывает набор значений, возвращаемых, соответствующих строки запроса в запрос [FindPeople операции](findpeople-operation.md) . Поиск по не указан **строки запроса** возвращает все элементы в указанной папке. 
  
```XML
<QueryString/> 
```

 **string**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[FindPeople](findpeople.md) <br/> |Содержит аргументы для [FindPeople операции](findpeople-operation.md) поиска.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение **строки запроса** представляет запрос почтового ящика, выполненные с помощью подмножество [Расширенного синтаксиса запроса (AQS)](http://msdn.microsoft.com/en-us/library/aa965711%28VS.85%29.aspx). Сведения о синтаксисе для этого элемента содержатся [строки запроса (QueryStringType)](querystring-querystringtype.md).
  
## <a name="remarks"></a>Замечания

Этот элемент появился в Exchange Server 2013.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция FindPeople](findpeople-operation.md)


- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

