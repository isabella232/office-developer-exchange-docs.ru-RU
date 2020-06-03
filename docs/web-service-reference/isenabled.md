---
title: IsEnabled
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsEnabled
api_type:
- schema
ms.assetid: c7e3035e-a4ef-4c11-8cb0-214790a554ff
description: Элемент Enable указывает, включено ли правило.
ms.openlocfilehash: 7a150dc4a27cf4ff7da9825d1daae2b747088539
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44455312"
---
# <a name="isenabled"></a>IsEnabled

Элемент **Enable** указывает, включено ли правило. 
  
```XML
<IsEnabled/>
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
|[Правило (RuleType)](rule-ruletype.md) <br/> |Представляет правило в почтовом ящике пользователя.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение **true** указывает, что правило включено и может быть выполнено. Значение **false** указывает, что правило не может быть выполнено. 
  
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

