---
title: NotSentToMe
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- NotSentToMe
api_type:
- schema
ms.assetid: 7cb63269-622c-4198-9a21-f5a021bf6901
description: Элемент NotSentToMe указывает, не должен ли владелец почтового ящика быть в свойстве ToRecipients входящих сообщений, чтобы применить условие или исключение.
ms.openlocfilehash: f3c2994778298c1c8a27626fb0d4b32d6d2963cb
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59518108"
---
# <a name="notsenttome"></a>NotSentToMe

Элемент **NotSentToMe** указывает, не должен ли владелец почтового ящика быть в свойстве **ToRecipients** входящих сообщений, чтобы применить условие или исключение. 
  
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

Текстовое значение **true** указывает, что владелец почтового ящика не должен быть в свойстве **ToRecipients** входящих сообщений, чтобы применить условие или исключение. Значение false  указывает, что владелец почтового ящика должен быть в свойстве **ToRecipients** входящих сообщений, чтобы применить условие или исключение. 
  
## <a name="remarks"></a>Заметки

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |True  <br/> |
   
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

