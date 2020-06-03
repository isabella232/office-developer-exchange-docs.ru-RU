---
title: Retentionpolicytag используется
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f46679d0-9236-41e2-8624-72300079c67c
description: Элемент Retentionpolicytag используется указывает политику хранения для элемента почтового ящика.
ms.openlocfilehash: 3ece841e14e6cf11ab15e4a4d8b83a778ae32e46
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465179"
---
# <a name="retentionpolicytag"></a>Retentionpolicytag используется

Элемент **retentionpolicytag используется** указывает политику хранения для элемента почтового ящика. 
  
```XML
<RetentionPolicyTag>
   <DisplayName/>
   <RetentionId/>
   <RetentionPeriod/>
   <Type/>
   <RetentionAction/>
   <Description/>
   <IsVisible/>
   <OptedInto/>
   <IsArchive/>
</RetentionPolicyTag>
```

 **ретентионполицитагтипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

[DisplayName (строка)](displayname-string.md)  |  [RetentionId](retentionid.md)  |  [Ретентионпериод](retentionperiod.md)  |  [Тип (елкфолдертипе)](type-elcfoldertype.md)  |  [RetentionAction](retentionaction.md)  |  [Description (описание](description.md)  |  ) [Отображается](isvisible.md)  |  [Оптединто](optedinto.md)  |  [Archive](isarchive.md)
  
### <a name="parent-elements"></a>Родительские элементы

[ретентионполицитагс](retentionpolicytags.md)
  
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
   

