---
title: IsNDR
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsNDR
api_type:
- schema
ms.assetid: 194f5836-7793-463a-a090-4386d1c2487a
description: Элемент IsNDR указывает, должен ли входящих сообщений отчеты о недоставке (NDR) в порядке для условие или исключение для применения.
ms.openlocfilehash: 651590d055a0532c904dbf6c481dca2f899d673f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834056"
---
# <a name="isndr"></a>IsNDR

Элемент **IsNDR** указывает, должен ли входящих сообщений отчеты о недоставке (NDR) в порядке для условие или исключение для применения. 
  
```XML
<IsNDR>true | false</IsNDR>
```

 **Boolean**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Условия](conditions.md) <br/> |Представляет условия, которые, если удовлетворены, запускают действия правила для правила.  <br/> |
|[Исключения](exceptions.md) <br/> |Представляет доступных исключение условий для правила папки «Входящие».  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение **true,** указывает, что сообщения должны быть отчета о Недоставке, чтобы условие или исключение можно применить. Значение **false** указывает, что сообщение не должна быть отчета о Недоставке, чтобы условие или исключение можно применить. 
  
## <a name="remarks"></a>Замечания

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |True  <br/> |
   
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

