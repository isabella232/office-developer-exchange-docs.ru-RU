---
title: исаутоматикрепли
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsAutomaticReply
api_type:
- schema
ms.assetid: 280e9baf-199d-422c-8fdf-1d0751a3e77d
description: Элемент Исаутоматикрепли указывает, должны ли входящие сообщения относиться к автоматическому ответу, чтобы применить условие или исключение.
ms.openlocfilehash: 7521dbbb458cf7683b52b2fe4fddacd276b40256
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44455564"
---
# <a name="isautomaticreply"></a>исаутоматикрепли

Элемент **исаутоматикрепли** указывает, должны ли входящие сообщения относиться к автоматическому ответу, чтобы применить условие или исключение. 
  
```XML
<IsAutomaticReply> true | false</IsAutomaticReply>
```

 **Boolean**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

Отсутствуют.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Условия](conditions.md) <br/> |Представляет условия, которые, если удовлетворены, запускают действия правила для правила.  <br/> |
|[Исключения](exceptions.md) <br/> |Представляет все доступные условия исключения правила для правила папки "Входящие".  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение **true** указывает, что сообщение должно относиться к автоматическому ответу, чтобы применить условие или исключение. Значение **false** указывает, что сообщение не обязательно должно быть автоматическим ответом для того, чтобы условие или исключение применялось. 
  
## <a name="remarks"></a>Примечания

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages. xsd  <br/> |
|Может быть пустым  <br/> |True  <br/> |
   
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

