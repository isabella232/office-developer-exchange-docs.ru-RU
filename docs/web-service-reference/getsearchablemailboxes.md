---
title: GetSearchableMailboxes
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 949871f7-0d10-498e-84aa-f0652f1193be
description: Элемент GetSearchableMailboxes содержит запрос на поиск списка почтовых ящиков, на которые клиент имеет разрешение на выполнение поиска по обнаружению электронных сообщений.
ms.openlocfilehash: 7c5902af3e0aa88c77a8e13d7c4ec521aa444d6b
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59515847"
---
# <a name="getsearchablemailboxes"></a>GetSearchableMailboxes

Элемент **GetSearchableMailboxes** содержит запрос на поиск списка почтовых ящиков, на которые клиент имеет разрешение на выполнение поиска по обнаружению электронных сообщений. 
  
```XML
<GetSearchableMailboxes>
   <SearchFilter/>
   <ExpandGroupMembership/>
</GetSearchableMailboxes>
```

 **GetSearchableMailboxesType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

[SearchFilter](searchfilter.md)  |  [ExpandGroupMembership](expandgroupmembership.md)
  
### <a name="parent-elements"></a>Родительские элементы

Нет.
  
## <a name="remarks"></a>Заметки

Этот элемент появился в Exchange Server 2013.
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |messages.xsd  <br/> |
|Может быть пустым  <br/> ||
   

