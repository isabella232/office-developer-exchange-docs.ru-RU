---
title: SearchFilter
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 1a7ee364-b7da-4197-aab2-57134537109a
description: Элемент SearchFilter содержит строки запроса для фильтрации почтовые ящики которого требуется получить из GetSearchableMailboxes запроса.
ms.openlocfilehash: b71d8dd862e9338afc145545df4cd29e8bcc3dc8
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19835285"
---
# <a name="searchfilter"></a>SearchFilter

Элемент **SearchFilter** содержит строки запроса для фильтрации почтовые ящики которого требуется получить из **GetSearchableMailboxes** запроса. 
  
```XML
<SearchFilter></SearchFilter>
```

 **string**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

[GetSearchableMailboxes](getsearchablemailboxes.md)
  
## <a name="text-value"></a>Текстовое значение

Текстовое значение элемента **SearchFilter** — это строка запроса к почтовым ящикам фильтр для поиска обнаружения. 
  
## <a name="remarks"></a>Замечания

Этот элемент появился в Exchange Server 2013.
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> ||
   
