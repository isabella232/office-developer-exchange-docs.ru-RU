---
title: Атрибуты (Аррайофперсонааттрибутионстипе)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f61d843c-bca5-4c88-9667-fd03d2a963a1
description: Элемент "атрибуты" определяет массив сведений о сопоставлении для одного или нескольких контактов или получателей Active Directory, собранных в связанный с ним пользователь.
ms.openlocfilehash: a9883e06a8adbd5c9d3bc7e1edd28c62418df653
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460325"
---
# <a name="attributions-arrayofpersonaattributionstype"></a>Атрибуты (Аррайофперсонааттрибутионстипе)

Элемент " **атрибуты** " определяет массив сведений о сопоставлении для одного или нескольких контактов или получателей Active Directory, собранных в связанный с ним пользователь. 
  
```XML
<Attributions>
    <Attribution></Attribution>
</Attributions>
```

 **аррайофперсонааттрибутионстипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Атрибуты (Персонааттрибутионтипе)](attribution-personaattributiontype.md) <br/> |Указывает экземпляр в массиве атрибутов для элемента **персонатипе** .  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Роль](persona.md) <br/> |Задает набор данных о пользователях, возвращаемых запросом к **другому человеку** .  <br/> |
   
## <a name="remarks"></a>Примечания

Этот элемент появился в Exchange Server 2013.
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема типа  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> ||
   
## <a name="see-also"></a>См. также

- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

