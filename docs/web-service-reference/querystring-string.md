---
title: QueryString (строка)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: f81b1b3d-9fe4-4ab3-b517-42e4207fa596
description: Элемент QueryString указывает набор возвращающихся значений, которые соответствуют строке запроса в запросе операции FindPeople. Поиск без заданного queryString возвращает все элементы из указанной папки.
ms.openlocfilehash: 6dfd4b5552511e2551baf5ce645f82d4f74e5499
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59523736"
---
# <a name="querystring-string"></a>QueryString (строка)

Элемент **QueryString** указывает набор возвращающихся значений, которые соответствуют строке запроса в [запросе операции FindPeople.](findpeople-operation.md) Поиск без **заданного queryString** возвращает все элементы из указанной папки. 
  
```XML
<QueryString/> 
```

 **строка**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[FindPeople](findpeople.md) <br/> |Содержит аргументы для поиска [операции FindPeople.](findpeople-operation.md)  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое **значение QueryString** представляет запрос почтовых ящиков, сделанный с помощью подмножество [Расширенный синтаксис запросов (AQS).](https://msdn.microsoft.com/library/aa965711%28VS.85%29.aspx) Сведения о синтаксисе для этого элемента см. в [обзоре QueryString (QueryStringType).](querystring-querystringtype.md)
  
## <a name="remarks"></a>Заметки

Этот элемент появился в Exchange Server 2013.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция FindPeople](findpeople-operation.md)


- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

