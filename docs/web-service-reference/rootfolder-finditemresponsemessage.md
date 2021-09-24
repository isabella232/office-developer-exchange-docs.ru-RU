---
title: RootFolder (FindItemResponseMessage)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- RootFolder
api_type:
- schema
ms.assetid: 187e009f-efaa-42a8-8962-329a645213ab
description: Элемент RootFolder содержит результаты поиска одной корневой папки во время операции FindItem.
ms.openlocfilehash: 96fa9e162dde34394e7c34543dd25a6f018ae7de
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59527539"
---
# <a name="rootfolder-finditemresponsemessage"></a>RootFolder (FindItemResponseMessage)

Элемент **RootFolder** содержит результаты поиска одной корневой папки во время операции [FindItem.](finditem-operation.md)
  
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
|**IndexedPagingOffset** <br/> |Представляет следующий индекс, который следует использовать для следующего запроса при использовании проиндексного представления для проиндексации.  <br/> |
|**NumeratorOffset** <br/> |Представляет новое значение числительную цифру, используемую для следующего запроса при использовании представлений страниц фракции.  <br/> |
|**AbsoluteDenominator** <br/> |Представляет следующий знаменатель, который будет использовать для следующего запроса при дробной прогонах.  <br/> |
|**IncludesLastItemInRange** <br/> |Указывает, содержатся ли в текущих результатах последний элемент запроса, например, чтобы дальнейшая прогона не требовалась.  <br/> |
|**TotalItemsInView** <br/> |Представляет общее число элементов, которые проходят ограничение. В сгруппивной операции [FindItem](finditem-operation.md)атрибут **TotalItemsInView** возвращает общее количество элементов в представлении плюс общее число групп.  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Items](items.md) <br/> |Содержит массив найденных элементов, в запросе на операцию [FindItem](finditem-operation.md) определены критерии поиска.  <br/> |
|[Группы](groups.md) <br/> |Содержит коллекцию групп, которые имеют критерии поиска и агрегации, выявленные в запросе [операции FindItem.](finditem-operation.md)  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[FindItemResponseMessage](finditemresponsemessage.md) <br/> |Содержит состояние и результат запроса [операции FindItem.](finditem-operation.md)  <br/> |
   
## <a name="remarks"></a>Заметки

Схема, описываемая этим элементом, расположена в виртуальном каталоге компьютера EWS, который Exchange Server с установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция FindItem](finditem-operation.md)
  
[IndexedPagingOffset](https://msdn.microsoft.com/library/ExchangeWebServices.FindItemParentType.IndexedPagingOffset.aspx)
  
[NumeratorOffset](https://msdn.microsoft.com/library/ExchangeWebServices.FindItemParentType.NumeratorOffset.aspx)
  
[AbsoluteDenominator](https://msdn.microsoft.com/library/ExchangeWebServices.FindItemParentType.AbsoluteDenominator.aspx)
  
[IncludesLastItemInRange](https://msdn.microsoft.com/library/ExchangeWebServices.FindItemParentType.IncludesLastItemInRange.aspx)
  
[TotalItemsInView](https://msdn.microsoft.com/library/ExchangeWebServices.FindItemParentType.TotalItemsInView.aspx)


[Поиск элементов](https://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

