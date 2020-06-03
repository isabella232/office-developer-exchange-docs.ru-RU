---
title: Строка запроса (строка)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f81b1b3d-9fe4-4ab3-b517-42e4207fa596
description: Элемент QueryString указывает набор значений, которые должны быть возвращены, чтобы соответствовать строке запроса в запросе операции FindPeople. Поиск без указания строки запроса возвращает все элементы из указанной папки.
ms.openlocfilehash: ec025f86d3e6fb74810e9c539eba102d05adbb93
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465326"
---
# <a name="querystring-string"></a>Строка запроса (строка)

Элемент **QueryString** указывает набор значений, которые должны быть возвращены, чтобы соответствовать строке запроса в запросе [операции FindPeople](findpeople-operation.md) . Поиск без указания **строки запроса** возвращает все элементы из указанной папки. 
  
```XML
<QueryString/> 
```

 **строка**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

Отсутствуют.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[FindPeople](findpeople.md) <br/> |Содержит аргументы для поиска [операции FindPeople](findpeople-operation.md) .  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение **QueryString** представляет запрос почтового ящика, выполненный с помощью подмножества [расширенного синтаксиса запросов (AQS)](https://msdn.microsoft.com/library/aa965711%28VS.85%29.aspx). Сведения о синтаксисе этого элемента см. в статье [QueryString (куеристрингтипе)](querystring-querystringtype.md).
  
## <a name="remarks"></a>Примечания

Этот элемент появился в Exchange Server 2013.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция FindPeople](findpeople-operation.md)


- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

