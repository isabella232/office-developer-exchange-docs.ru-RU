---
title: SentToOrCcMe
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- SentToOrCcMe
api_type:
- schema
ms.assetid: ca43e05d-df37-485b-9276-34678025f2b7
description: Элемент SentToOrCcMe указывает, должен ли владелец почтового ящика быть в свойстве ToRecipients или CcRecipients входящих сообщений, чтобы применить условие или исключение.
ms.openlocfilehash: 0e9dddf53c2b671613a5a4c20e3b845a5d38c247
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59510892"
---
# <a name="senttoorccme"></a>SentToOrCcMe

Элемент **SentToOrCcMe** указывает, должен ли владелец почтового ящика быть в свойстве **ToRecipients** или **CcRecipients** входящих сообщений, чтобы применить условие или исключение. 
  
```XML
<SentToOrCcMe>true | false</SentToOrCcMe>
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
|[Исключения](exceptions.md) <br/> |Представляет все доступные условия исключения правил для правила "Входящие".  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение  true указывает, что владелец почтового ящика должен быть в свойстве **ToRecipients** или **CcRecipients** входящих сообщений, чтобы применить условие или исключение. Значение false  указывает, что владелец почтового ящика не должен быть в свойстве **ToRecipients** или **CcRecipients** входящих сообщений, чтобы применить условие или исключение. 
  
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

