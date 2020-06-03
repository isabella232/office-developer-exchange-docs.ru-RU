---
title: усерпараметерс
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: bad7311f-7ecd-4f0c-b8e7-dd8f7d378f55
description: Элемент Усерпараметерс содержит список включенных и отключенных расширений клиентов.
ms.openlocfilehash: 76bf858adfb6d2ef76a25c234117131752c60d7b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44526755"
---
# <a name="userparameters"></a>усерпараметерс

Элемент **усерпараметерс** содержит список включенных и отключенных расширений клиентов. 
  
```XML
<UserParameters UserId="" EnabledOnly="">
   <UserEnabledExtensions/>
   <UserDisabledExtensions/>
</UserParameters>
```

 **жетклиентекстенсионусерпараметерстипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|UserId  <br/> |Текстовое значение атрибута **UserID** — идентификатор пользователя.  <br/> |
|енабледонли  <br/> |Текстовое значение **енабледонли** указывает, содержит ли отклик только включенные расширения.  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

[Усеренабледекстенсионс](userenabledextensions.md)  |  [Усердисабледекстенсионс](userdisabledextensions.md)
  
### <a name="parent-elements"></a>Родительские элементы

[жетклиентекстенсион](getclientextension.md)
  
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
   

