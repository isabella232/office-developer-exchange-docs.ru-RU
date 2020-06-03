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
ms.openlocfilehash: a0ff3fcb82e7f18837af5a6f5daa16e90043034d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460689"
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

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

[DisplayName (нонемптистрингтипе)](displayname-nonemptystringtype.md)  |  [GroupType](grouptype.md)  |  [Ексчанжестореид](exchangestoreid.md)  |  [Мемберкоррелатионкэй](membercorrelationkey.md)  |  [Екстендедпропертиес (нонемптяррайофекстендедпропертитипе)](extendedproperties-nonemptyarrayofextendedpropertytype.md)  |  [SmtpAddress](smtpaddress.md)
  
### <a name="parent-elements"></a>Родительские элементы

[Groups (аррайофимграуптипе)](groups-arrayofimgrouptype.md)  |  [Адддистрибутионграуптоимлистреспонсе](adddistributiongrouptoimlistresponse.md)  |  [Аддимграупреспонсе](addimgroupresponse.md)
  
## <a name="remarks"></a>Примечания

Этот элемент появился в Exchange Server 2013.
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages. xsd  <br/> |
|Может быть пустым  <br/> ||
   

