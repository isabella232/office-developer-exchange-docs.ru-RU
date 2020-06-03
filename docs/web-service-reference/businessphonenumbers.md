---
title: бусинессфоненумберс
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: ecbe4f1c-1c9e-44e0-a8f7-08c160a0fddb
description: Элемент Бусинессфоненумберс указывает массив номеров рабочих телефонов и идентификаторы их исходных атрибутов для связанного пользователя.
ms.openlocfilehash: 8713af3ad302a2940cab247ff7188e55e8021ca0
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461620"
---
# <a name="businessphonenumbers"></a>бусинессфоненумберс

Элемент **бусинессфоненумберс** указывает массив номеров рабочих телефонов и идентификаторы их исходных атрибутов для связанного пользователя. 
  
```XML
<BusinessPhoneNumbers>
    <Value></Value>
    <Attributions></Attributions>
</BusinessPhoneNumbers>
```

 **аррайоффоненумбераттрибутедвалуестипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Значение (Персонафоненумбертипе)](value-personaphonenumbertype.md) <br/> |Указывает номер телефона и тип сведений, а также связанный с набором сопоставлений.  <br/> |
|[Атрибуты (Аррайофвалуеаттрибутионстипе)](attributions-arrayofvalueattributionstype.md) <br/> |Задает массив атрибутов для связанного элемента **value** .  <br/> |
   
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

