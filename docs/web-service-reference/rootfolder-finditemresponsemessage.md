---
title: RootFolder (FindItemResponseMessage)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RootFolder
api_type:
- schema
ms.assetid: 187e009f-efaa-42a8-8962-329a645213ab
description: Элемент RootFolder содержит результаты поиска в одной корневой папке во время операции FindItem.
ms.openlocfilehash: ea17369ef4efc4112a738b430c8f0dbab3886341
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19835254"
---
# <a name="rootfolder-finditemresponsemessage"></a>RootFolder (FindItemResponseMessage)

Элемент **RootFolder** содержит результаты поиска в одной корневой папке во время [операции FindItem](finditem-operation.md).
  
```xml
<RootFolder IndexedPagingOffset="" NumeratorOffset="" AbsoluteDenominator="" IncludesLastItemInRange="" TotalItemsInView="">
   <Items/>
   <Groups/>
</RootFolder>
```

 **FindItemParentType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|**IndexedPagingOffset** <br/> |Представляет следующий индекс, который следует использовать для следующего запроса при использовании индексированного представления разбиение на страницы.  <br/> |
|**NumeratorOffset** <br/> |Представляет новое значение перечислителя использовать для следующего запроса при использовании просмотров страниц дроби.  <br/> |
|**AbsoluteDenominator** <br/> |Представляет Далее делителя для использования в следующем запросе при выполнении дробная разбиение на страницы.  <br/> |
|**IncludesLastItemInRange** <br/> |Указывает, содержат ли текущие результаты последнего элемента в запросе, таким образом, что дальнейшей постраничного просмотра не требуется.  <br/> |
|**TotalItemsInView** <br/> |Представляет общее число элементов, которые ограничение игнорируется. В сгруппированных [операции FindItem](finditem-operation.md)атрибут **TotalItemsInView** возвращает общее число элементов в представлении, а также общее число групп.  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Элементы](items.md) <br/> |Содержит массив найденных элементов, у которых критерии поиска, определенные в запросе на [операции FindItem](finditem-operation.md) .  <br/> |
|[Группы](groups.md) <br/> |Содержит коллекцию найдено групп, у которых поиска и объединение критериям, заданным в запрос [FindItem операции](finditem-operation.md) .  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[FindItemResponseMessage](finditemresponsemessage.md) <br/> |Содержит состояние и результат [операции FindItem](finditem-operation.md) запроса.  <br/> |
   
## <a name="remarks"></a>Замечания

Схема, описывающая этот элемент находится в виртуальном каталоге EWS компьютера, на котором работает Exchange Server с установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[FindItem Operation](finditem-operation.md)
  
[IndexedPagingOffset](https://msdn.microsoft.com/library/ExchangeWebServices.FindItemParentType.IndexedPagingOffset.aspx)
  
[NumeratorOffset](https://msdn.microsoft.com/library/ExchangeWebServices.FindItemParentType.NumeratorOffset.aspx)
  
[AbsoluteDenominator](https://msdn.microsoft.com/library/ExchangeWebServices.FindItemParentType.AbsoluteDenominator.aspx)
  
[IncludesLastItemInRange](https://msdn.microsoft.com/library/ExchangeWebServices.FindItemParentType.IncludesLastItemInRange.aspx)
  
[TotalItemsInView](https://msdn.microsoft.com/library/ExchangeWebServices.FindItemParentType.TotalItemsInView.aspx)


[Поиск элементов](http://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

