---
title: ResolutionSet
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- ResolutionSet
api_type:
- schema
ms.assetid: 43d5b876-0e87-4414-9b1d-bff1c1ec825c
description: Элемент ResolutionSet содержит массив разрешений для неоднозначного имени.
ms.openlocfilehash: f77b8a94871aa7827c98a3bb15fdf4a3a35c7c55
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59521748"
---
# <a name="resolutionset"></a>ResolutionSet

Элемент **ResolutionSet** содержит массив разрешений для неоднозначного имени. 
  
[ResolveNamesResponse](resolvenamesresponse.md)
  
[ResponseMessages](responsemessages.md)
  
[ResolveNamesResponseMessage](resolvenamesresponsemessage.md)
  
[ResolutionSet](resolutionset.md)
  
```xml
<ResolutionSet IndexedPagingOffset="" NumeratorOffset="" AbsoluteDenominator="" IncludesLastItemInRange="" TotalItemsInView="">
   <Resolution/>
</ResolutionSet>
```

 **ArrayOfResolutionType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|**IndexedPagingOffset** <br/> |Представляет следующий индекс, который следует использовать для следующего запроса при использовании индексного представления страницы.  <br/> |
|**NumeratorOffset** <br/> |Представляет новое значение числительную цифру, используемую для следующего запроса при использовании представлений страниц фракции.  <br/> |
|**AbsoluteDenominator** <br/> |Представляет следующий знаменатель, который будет использовать для следующего запроса при использовании представлений страниц фракции.  <br/> |
|**IncludesLastItemInRange** <br/> |Этот атрибут будет верным, если в текущих результатах содержится последний элемент запроса, чтобы дополнительная прогона не требовалась.  <br/> |
|**TotalItemsInView** <br/> |Представляет общее количество элементов в представлении.  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Решение](resolution.md) <br/> |Содержит одну разрешенную сущность.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[ResolveNamesResponseMessage](resolvenamesresponsemessage.md) <br/> |Содержит состояние и результат запроса ResolveNames.  <br/> |
   
## <a name="remarks"></a>Заметки

Элемент **ResolutionSet** может содержать не более 100 разрешенных сущностями. 
  
Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[ResolveNames](resolvenames.md)
  
[ResolveNamesResponse](resolvenamesresponse.md)
  
[Операция ResolveNames](resolvenames-operation.md)


- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

