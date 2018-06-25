---
title: PolicyTipsEnabled
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 16409652-21e4-4bd3-9373-67e1882236b4
description: Элемент PolicyTipsEnabled указывает, включены ли подсказки политики.
ms.openlocfilehash: 683131a5cefd6757faf582324f312b01fd9ddb33
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834838"
---
# <a name="policytipsenabled"></a>PolicyTipsEnabled

Элемент **PolicyTipsEnabled** указывает, включены ли подсказки политики. 
  
```XML
<PolicyTipsEnabled> true | false </PolicyTipsEnabled>
```

 **Boolean**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

[MailTipsConfiguration (MailTipsServiceConfiguration)](mailtipsconfiguration-mailtipsserviceconfiguration.md)
  
## <a name="text-value"></a>Текстовое значение

Текстовое значение **true** для элемента **PolicyTipsEnabled** указывает, что советы по политикам разрешены для почтового ящика. Значение **false** указывает подсказок политики не включены для почтового ящика. 
  
## <a name="remarks"></a>Замечания

Этот элемент появился в Exchange Server 2013.
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> ||
   

