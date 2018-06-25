---
title: NotSentToMe
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- NotSentToMe
api_type:
- schema
ms.assetid: 7cb63269-622c-4198-9a21-f5a021bf6901
description: Элемент NotSentToMe указывает, должно ли не быть владельца почтового ящика в свойстве ToRecipients входящих сообщений в порядке для условие или исключение для применения.
ms.openlocfilehash: 917648f811855961877d1aba4924573e95e3962a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834555"
---
# <a name="notsenttome"></a>NotSentToMe

Элемент **NotSentToMe** указывает, должно ли не быть владельца почтового ящика в свойстве **ToRecipients** входящих сообщений в порядке для условие или исключение для применения. 
  
```xml
<NotSentToMe>true | false</NotSentToMe>
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
|[Исключения](exceptions.md) <br/> |Представляет исключения, которые представляют все доступные правила условия исключений для правила папки «Входящие».  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение **true,** указывает, что владелец почтового ящика не должна быть в свойстве **ToRecipients** входящих сообщений в порядке для условие или исключение для применения. Значение **false** указывает, что владелец почтового ящика должны быть в свойстве **ToRecipients** входящих сообщений в порядке для условие или исключение для применения. 
  
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

