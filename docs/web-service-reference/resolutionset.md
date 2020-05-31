---
title: Авторешение
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ResolutionSet
api_type:
- schema
ms.assetid: 43d5b876-0e87-4414-9b1d-bff1c1ec825c
description: Элемент "набор решений" содержит массив разрешений для неоднозначного имени.
ms.openlocfilehash: ad7bd31c85051e8c80aea25aa9e6f2914cf0ad01
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835160"
---
# <a name="resolutionset"></a>Авторешение

Элемент "набор **решений** " содержит массив разрешений для неоднозначного имени. 
  
[ресолвенамесреспонсе](resolvenamesresponse.md)
  
[респонсемессажес](responsemessages.md)
  
[ресолвенамесреспонсемессаже](resolvenamesresponsemessage.md)
  
[Авторешение](resolutionset.md)
  
```xml
<ResolutionSet IndexedPagingOffset="" NumeratorOffset="" AbsoluteDenominator="" IncludesLastItemInRange="" TotalItemsInView="">
   <Resolution/>
</ResolutionSet>
```

 **аррайофресолутионтипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|**индекседпагингоффсет** <br/> |Представляет следующий индекс, который должен использоваться для следующего запроса при использовании индексированного представления страницы.  <br/> |
|**нумератороффсет** <br/> |Представляет новое значение числителя, которое будет использоваться для следующего запроса при использовании представлений страницы дробей.  <br/> |
|**абсолутеденоминатор** <br/> |Представляет следующий знаменатель, который будет использоваться для следующего запроса при использовании представлений страницы дробной части.  <br/> |
|**инклудесластитеминранже** <br/> |Этот атрибут будет иметь значение true, если текущие результаты содержат последний элемент в запросе, чтобы не требовалось дополнительное разбиение на страницы.  <br/> |
|**тоталитемсинвиев** <br/> |Представляет общее число элементов в представлении.  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Resolution](resolution.md) <br/> |Содержит одну разрешенную сущность.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[ресолвенамесреспонсемессаже](resolvenamesresponsemessage.md) <br/> |Содержит состояние и результат запроса ResolveNames.  <br/> |
   
## <a name="remarks"></a>Примечания

Элемент "набор **решений** " может содержать не более 100 разрешенных сущностей. 
  
Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[ResolveNames](resolvenames.md)
  
[ресолвенамесреспонсе](resolvenamesresponse.md)
  
[Операция ResolveNames](resolvenames-operation.md)


- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

