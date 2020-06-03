---
title: Рутфолдер (Финдитемреспонсемессаже)
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
description: Элемент Рутфолдер содержит результаты поиска в одной корневой папке во время операции FindItem.
ms.openlocfilehash: 3bbab325dff26139739c50ef519b215aea620a0b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457132"
---
# <a name="rootfolder-finditemresponsemessage"></a>Рутфолдер (Финдитемреспонсемессаже)

Элемент **рутфолдер** содержит результаты поиска в одной корневой папке во время [операции FindItem](finditem-operation.md).
  
```xml
<RootFolder IndexedPagingOffset="" NumeratorOffset="" AbsoluteDenominator="" IncludesLastItemInRange="" TotalItemsInView="">
   <Items/>
   <Groups/>
</RootFolder>
```

 **финдитемпаренттипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|**индекседпагингоффсет** <br/> |Представляет следующий индекс, который должен использоваться для следующего запроса при использовании индексированного представления разбиения по страницам.  <br/> |
|**нумератороффсет** <br/> |Представляет новое значение числителя, которое будет использоваться для следующего запроса при использовании представлений страницы дробей.  <br/> |
|**абсолутеденоминатор** <br/> |Представляет следующий знаменатель, который будет использоваться для следующего запроса при выполнении дробного разбиения на страницы.  <br/> |
|**инклудесластитеминранже** <br/> |Указывает, содержат ли текущие результаты последний элемент в запросе, что не требуется для дальнейшей разбиения на страницы.  <br/> |
|**тоталитемсинвиев** <br/> |Представляет общее число элементов, которые прошли ограничение. В сгруппированной [операции FindItem](finditem-operation.md)атрибут **тоталитемсинвиев** возвращает общее число элементов в представлении, а также общее число групп.  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Items](items.md) <br/> |Содержит массив найденных элементов, которые содержат условия поиска, указанные в запросе [операции FindItem](finditem-operation.md) .  <br/> |
|[Groups](groups.md) <br/> |Содержит коллекцию найденных групп, которые содержат критерии поиска и объединения, указанные в запросе [операции FindItem](finditem-operation.md) .  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[финдитемреспонсемессаже](finditemresponsemessage.md) <br/> |Содержит состояние и результат запроса [операции FindItem](finditem-operation.md) .  <br/> |
   
## <a name="remarks"></a>Примечания

Схема, описывающая этот элемент, находится в виртуальном каталоге EWS компьютера, на котором установлен сервер Exchange Server с установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция FindItem](finditem-operation.md)
  
[индекседпагингоффсет](https://msdn.microsoft.com/library/ExchangeWebServices.FindItemParentType.IndexedPagingOffset.aspx)
  
[нумератороффсет](https://msdn.microsoft.com/library/ExchangeWebServices.FindItemParentType.NumeratorOffset.aspx)
  
[абсолутеденоминатор](https://msdn.microsoft.com/library/ExchangeWebServices.FindItemParentType.AbsoluteDenominator.aspx)
  
[инклудесластитеминранже](https://msdn.microsoft.com/library/ExchangeWebServices.FindItemParentType.IncludesLastItemInRange.aspx)
  
[тоталитемсинвиев](https://msdn.microsoft.com/library/ExchangeWebServices.FindItemParentType.TotalItemsInView.aspx)


[Поиск элементов](https://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

