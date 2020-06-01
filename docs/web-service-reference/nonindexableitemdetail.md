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
ms.openlocfilehash: 4fc4324501570402d22aa303d6af2a60b50b3cc6
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/01/2020
ms.locfileid: "44466740"
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

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

[ItemId](itemid.md)  |  [ErrorCode (итеминдексеррортипе)](errorcode-itemindexerrortype.md)  |  [Еррордескриптион](errordescription.md)  |  [Испартиаллиндексед](ispartiallyindexed.md)  |  [Исперманентфаилуре](ispermanentfailure.md)  |  [Сортвалуе](sortvalue.md)  |  [Аттемпткаунт](attemptcount.md)  |  [Ластаттемпттиме](lastattempttime.md)  |  [Аддитионалинфо](additionalinfo.md)
  
### <a name="parent-elements"></a>Родительские элементы

[Элементы (Аррайофнониндексаблеитемдетаилстипе)](items-arrayofnonindexableitemdetailstype.md)
  
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
   

