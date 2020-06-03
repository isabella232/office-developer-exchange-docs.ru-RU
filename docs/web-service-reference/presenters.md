---
title: Выступающих
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 01057872-4f1a-4246-86ba-73d10ef854a0
description: Элемент Presenter указывает докладчиков для собрания по сети.
ms.openlocfilehash: 0236457020dfc4684569e84d3d54e357af00d102
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529912"
---
# <a name="presenters"></a>Выступающих

Элемент **Presenter** указывает докладчиков для собрания по сети. 
  
```XML
<Presenters> Disabled | Internal | Everyone </Presenters>
```

 **пресентерстипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

Отсутствуют.
  
### <a name="parent-elements"></a>Родительские элементы

[онлинемитингсеттингс](onlinemeetingsettings.md)
  
## <a name="text-value"></a>Текстовое значение

Текстовое значение элемента **Presenters** — это тип пользователей, которые могут быть выступающими для собрания по сети. Текстовые значения для элемента **Presenter** описаны в следующей таблице. 
  
**Текстовые значения элементов выступающих**

|**Значение**|**Описание**|
|:-----|:-----|
|Отключено  <br/> |Выступающие отключены.  <br/> |
|Внутренний  <br/> |Докладчиками могут быть только внутренние участники.  <br/> |
|Все  <br/> |Любой участник может быть докладчиком.  <br/> |
   
## <a name="remarks"></a>Примечания

Этот элемент появился в Exchange Server 2013.
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> ||
   

