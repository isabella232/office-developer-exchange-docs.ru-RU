---
title: нониндексаблеитемдетаил
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: a26d4c02-f1bd-40c4-9257-5db45e839f17
description: Элемент Нониндексаблеитемдетаил указывает подробные сведения об элементе, который невозможно индексировать.
ms.openlocfilehash: ef1bd072a44b42b501a3016c394b89fe6ab25bf0
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834543"
---
# <a name="nonindexableitemdetail"></a>нониндексаблеитемдетаил

Элемент **нониндексаблеитемдетаил** указывает подробные сведения об элементе, который невозможно индексировать. 
  
```XML
<NonIndexableItemDetail>
   <ItemId/>
   <ErrorCode/>
   <ErrorDescription/>
   <IsPartiallyIndexed/>
   <IsPermanentFailure/>
   <SortValue/>
   <AttemptCount/>
   <LastAttemptTime/>
   <AdditionalInfo/>
</NonIndexableItemDetail>
```

 **нониндексаблеитемдетаилтипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

[ItemId](itemid.md) | [ErrorCode (итеминдексеррортипе)](errorcode-itemindexerrortype.md) | [еррордескриптион](errordescription.md) | [испартиаллиндексед](ispartiallyindexed.md) | [исперманентфаилуре](ispermanentfailure.md) | [AttemptCount](attemptcount.md)[SortValue](sortvalue.md) | [AdditionalInfo](additionalinfo.md) сортвалуе AttemptCount | [LastAttemptTime](lastattempttime.md)AdditionalInfo | 
  
### <a name="parent-elements"></a>Родительские элементы

[Элементы (Аррайофнониндексаблеитемдетаилстипе)](items-arrayofnonindexableitemdetailstype.md)
  
## <a name="remarks"></a>Примечания

Этот элемент появился в Exchange Server 2013.
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> ||
   

