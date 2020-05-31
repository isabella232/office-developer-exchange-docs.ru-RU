---
title: исмитингреспонсе
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsMeetingResponse
api_type:
- schema
ms.assetid: 85090943-81c6-4fbe-a2db-007dced6a4cf
description: Элемент Исмитнгреспонсекуест указывает, должны ли входящие сообщения быть ответом на приглашение на собрание, чтобы применялось условие или исключение.
ms.openlocfilehash: 9040859452a48916a969b6d8e4e370b5785c1c1a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834053"
---
# <a name="ismeetingresponse"></a>исмитингреспонсе

Элемент **исмитнгреспонсекуест** указывает, должны ли входящие сообщения быть ответом на приглашение на собрание, чтобы применялось условие или исключение. 
  
```XML
<IsMeetingResponse/>true | false</IsMeetingResponse>
```

 **Boolean**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Условия](conditions.md) <br/> |Представляет условия, которые, если удовлетворены, запускают действия правила для правила.  <br/> |
|[Исключения](exceptions.md) <br/> |Представляет все доступные условия исключения правила для правила папки "Входящие".  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение **true** указывает, что сообщение должно быть ответом на приглашение на собрание, чтобы применялось условие или исключение. Текстовое значение **false** указывает, что сообщение не должно быть ответом на приглашение на собрание, чтобы применялось условие или исключение. 
  
## <a name="remarks"></a>Примечания

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages. xsd  <br/> |
|Может быть пустым  <br/> |True  <br/> |
   
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

