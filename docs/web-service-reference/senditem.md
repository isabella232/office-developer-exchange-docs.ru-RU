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
ms.lasthandoff: 06/11/2018
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

 **SendItemType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|**SaveItemToFolder** <br/> |Определяет, является ли копия отправленного элемента сохраняется. Сохранить действие зависит от значение **SaveItemToFolder** и [SavedItemFolderId](saveditemfolderid.md) элемент присутствует в запросе. Этот элемент обязательный.  <br/> |
   
#### <a name="saveitemtofolder-attribute"></a>Атрибут SaveItemToFolder

|**Значение**|**Описание**|
|:-----|:-----|
|**значение true** <br/> |Если элемент [SavedItemFolderId](saveditemfolderid.md) не задан, элемент сохраняется в папке «Отправленные». При наличии элемент [SavedItemFolderId](saveditemfolderid.md) элемент сохраняется в папке, указанной с помощью элемента [SavedItemFolderId](saveditemfolderid.md) .  <br/> |
|**false** <br/> |Если элемент [SavedItemFolderId](saveditemfolderid.md) не задан, элемент не сохраняются. При наличии элемент [SavedItemFolderId](saveditemfolderid.md) возврату ошибки будут возвращены с элементом [ResponseCode](responsecode.md) , который содержит значение **ErrorInvalidSendItemSaveSettings** .  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Что ItemID](itemids.md) <br/> |Содержит уникальные идентификаторы элементов, элементы вхождений и повторяющиеся основные элементы, используемые для удаления, отправка, получение, перемещение и копирование элементов в хранилище Exchange.  <br/> |
|[SavedItemFolderId](saveditemfolderid.md) <br/> |Определяет папку назначения для операций, обновление, отправка и создания элементов в хранилище Exchange.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

Нет.
  
## <a name="remarks"></a>Замечания

При отправке элемента в этой папке, отправленный элемент удаляется и поместите его копию в этой папке.
  
Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[SendItem Operation](senditem-operation.md)

