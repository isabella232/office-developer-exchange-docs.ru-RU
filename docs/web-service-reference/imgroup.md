---
title: Группа
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: ab7b884e-ecf1-4e58-86ec-856b13a95f2b
description: Элемент "Группа" представляет группу мгновенных сообщений.
ms.openlocfilehash: 2a444158dbc6a73b1aee7b306cc251d33d005c43
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833890"
---
# <a name="imgroup"></a>Группа

Элемент " **Группа** " представляет группу мгновенных сообщений. 
  
```XML
<ImGroup>
   <DisplayName/>
   <GroupType/>
   <ExchangeStoreId/>
   <MemberCorrelationKey/>
   <ExtendedProperties/>
   <SmtpAddress/>
</ImGroup>
```

 **имграуптипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

[DisplayName (нонемптистрингтипе)](displayname-nonemptystringtype.md) | [groupType](grouptype.md) | [ексчанжестореид](exchangestoreid.md) | [мемберкоррелатионкэй](membercorrelationkey.md) | [екстендедпропертиес (нонемптяррайофекстендедпропертитипе)](extendedproperties-nonemptyarrayofextendedpropertytype.md) | [SmtpAddress](smtpaddress.md)
  
### <a name="parent-elements"></a>Родительские элементы

[Groups (аррайофимграуптипе)](groups-arrayofimgrouptype.md) | [адддистрибутионграуптоимлистреспонсе](adddistributiongrouptoimlistresponse.md) | [аддимграупреспонсе](addimgroupresponse.md)
  
## <a name="remarks"></a>Примечания

Этот элемент появился в Exchange Server 2013.
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages. xsd  <br/> |
|Может быть пустым  <br/> ||
   

