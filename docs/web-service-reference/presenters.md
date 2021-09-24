---
title: Докладчики
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 01057872-4f1a-4246-86ba-73d10ef854a0
description: Элемент Presenters указывает презентаторы для собрания в Интернете.
ms.openlocfilehash: 1c9bf9093450e675245b647c98d7b1d00101ce9e
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59519144"
---
# <a name="presenters"></a>Докладчики

Элемент **Presenters** указывает презентаторы для собрания в Интернете. 
  
```XML
<Presenters> Disabled | Internal | Everyone </Presenters>
```

 **PresentersType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

[OnlineMeetingSettings](onlinemeetingsettings.md)
  
## <a name="text-value"></a>Текстовое значение

Текстовое значение **элемента Presenters** — это тип пользователей, которые могут быть презентатором для собрания в Интернете. Текстовые значения элемента **Presenters** описаны в следующей таблице. 
  
**Текстовые значения элементов presenters**

|**Значение**|**Описание**|
|:-----|:-----|
|Отключено  <br/> |Presenters are disabled.  <br/> |
|Внутренний  <br/> |Только внутренние участники могут быть презентаторами.  <br/> |
|Все пользователи  <br/> |Любой участник может быть презентером.  <br/> |
   
## <a name="remarks"></a>Заметки

Этот элемент появился в Exchange Server 2013.
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> ||
   

