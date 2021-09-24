---
title: ReturnNewItemIds
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: aeef79e4-31e1-4213-b627-9bac676be018
description: Элемент ReturnNewItemIds указывает, возвращаются ли идентификаторы элементов новых элементов в ответе.
ms.openlocfilehash: 93ff4e37c56c3583e81711ba7e3582706d9ef940
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59512382"
---
# <a name="returnnewitemids"></a>ReturnNewItemIds

Элемент **ReturnNewItemIds** указывает, возвращаются ли идентификаторы элементов новых элементов в ответе. 
  
```XML
<ReturnNewItemIds/>
```

 **xs:boolean**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[CopyItem](copyitem.md) <br/> |Определяет запрос на копирование элемента в почтовом ящике в Exchange магазине.  <br/> |
|[MoveItem](moveitem.md) <br/> |Определяет запрос на перемещение элемента в Exchange магазине.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое **значение, истинное** для элемента **ReturnNewItemIds,** указывает, что новые идентификаторы элементов возвращаются в ответ. Значение false **указывает,** что идентификаторы новых элементов не возвращаются в ответе. 
  
## <a name="remarks"></a>Заметки

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.Этот элемент появился в Exchange Server 2010 с пакетом обновления 1 (SP1).
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема сообщения  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   

