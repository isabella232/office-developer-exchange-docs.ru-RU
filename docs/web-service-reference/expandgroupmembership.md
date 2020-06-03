---
title: експандграупмембершип
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 8989e96b-8fa1-4858-93b2-2cbdb30b9ca9
description: Элемент Експандграупмембершип указывает, следует ли расширять членство в группе, возвращенной из запроса GetSearchableMailboxes.
ms.openlocfilehash: 8a94aa3da165ecc13282127e75c8d166f3972ead
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44456908"
---
# <a name="expandgroupmembership"></a>експандграупмембершип

Элемент **експандграупмембершип** указывает, следует ли расширять членство в группе, возвращенной из запроса **GetSearchableMailboxes** . 
  
```XML
<ExpandGroupMembership>true | false</ExpandGroupMembership>
```

 **Boolean**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

Отсутствуют.
  
### <a name="parent-elements"></a>Родительские элементы

[GetDiscoverySearchConfiguration](getdiscoverysearchconfiguration.md)  |  [GetSearchableMailboxes](getsearchablemailboxes.md)
  
## <a name="text-value"></a>Текстовое значение

Текстовое значение **true** для элемента **експандграупелемент** указывает на то, что членство в группе развернуто. Значение **false** указывает, что членство в группе не разворачивается для отображения членов группы. 
  
## <a name="remarks"></a>Примечания

Этот элемент появился в Exchange Server 2013.
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |messages. xsd  <br/> |
|Может быть пустым  <br/> |false  <br/> |
   

