---
title: SendItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SendItem
api_type:
- schema
ms.assetid: a966da19-b05a-4504-ac98-91acc1667b9a
description: Элемент SendItem является корневым элементом в запросе на отправку элемента в хранилище Exchange.
ms.openlocfilehash: c5ce52ee4643219aa31ae59e8b7d40d7a904c8ab
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835340"
---
# <a name="senditem"></a>SendItem

Элемент **SendItem** является корневым элементом в запросе на отправку элемента в хранилище Exchange. 
  
```xml
<SendItem SaveItemToFolder="">
   <ItemIds/>
   <SavedItemFolderId/>
</SendItem>
```

 **сендитемтипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|**савеитемтофолдер** <br/> |Определяет, будет ли сохранена копия отправленного элемента. Действие Save зависит от значения **савеитемтофолдер** и наличия элемента [саведитемфолдерид](saveditemfolderid.md) в запросе. Этот элемент обязательный.  <br/> |
   
#### <a name="saveitemtofolder-attribute"></a>Атрибут Савеитемтофолдер

|**Значение**|**Описание**|
|:-----|:-----|
|**относится** <br/> |Если элемент [саведитемфолдерид](saveditemfolderid.md) отсутствует, элемент сохраняется в папке "Отправленные". Если присутствует элемент [саведитемфолдерид](saveditemfolderid.md) , он сохраняется в папке, указанной элементом [саведитемфолдерид](saveditemfolderid.md) .  <br/> |
|**значения** <br/> |Если элемент [саведитемфолдерид](saveditemfolderid.md) отсутствует, элемент не сохраняется. Если присутствует элемент [саведитемфолдерид](saveditemfolderid.md) , возвращается ответ об ошибке с элементом [респонсекоде](responsecode.md) , содержащим значение **ерроринвалидсендитемсавесеттингс** .  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[итемидс](itemids.md) <br/> |Содержит уникальные идентификаторы элементов, элементы вхождений и повторяющиеся элементы шаблона, которые используются для удаления, отправки, получения, перемещения или копирования элементов в хранилище Exchange.  <br/> |
|[саведитемфолдерид](saveditemfolderid.md) <br/> |Определяет целевую папку для операций обновления, отправки и создания элементов в хранилище Exchange.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

Нет.
  
## <a name="remarks"></a>Примечания

При отправке элемента в папке "Отправленные" элемент удаляется, а его копия помещается в папку "Отправленные".
  
Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция SendItem](senditem-operation.md)

