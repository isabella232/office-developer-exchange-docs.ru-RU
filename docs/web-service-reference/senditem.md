---
title: SendItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- SendItem
api_type:
- schema
ms.assetid: a966da19-b05a-4504-ac98-91acc1667b9a
description: Элемент SendItem — это корневой элемент в запросе на отправку элемента в Exchange магазине.
ms.openlocfilehash: 2d1613451e7f876f0b612a3249570412e40b4764
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59521622"
---
# <a name="senditem"></a>SendItem

Элемент **SendItem** — это корневой элемент в запросе на отправку элемента в Exchange магазине. 
  
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
|**SaveItemToFolder** <br/> |Определяет, сохранена ли копия отправленного элемента. Действие сохранения зависит от значения **SaveItemToFolder** и от того, присутствует ли в запросе элемент [SavedItemFolderId.](saveditemfolderid.md) Этот элемент обязательный.  <br/> |
   
#### <a name="saveitemtofolder-attribute"></a>Атрибут SaveItemToFolder

|**Значение**|**Описание**|
|:-----|:-----|
|**true** <br/> |Если элемента [SavedItemFolderId](saveditemfolderid.md) нет, элемент сохранен в папке Отправленные элементы. Если элемент [SavedItemFolderId](saveditemfolderid.md) присутствует, элемент сохранен в папке, указанной элементом [SavedItemFolderId.](saveditemfolderid.md)  <br/> |
|**false** <br/> |Если элемента [SavedItemFolderId](saveditemfolderid.md) нет, элемент не сохранен. Если элемент [SavedItemFolderId](saveditemfolderid.md) присутствует, ответ на ошибку возвращается с помощью элемента [ResponseCode,](responsecode.md) содержаного значение **ErrorInvalidSendItemSaveSaveSettings.**  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[ItemIds](itemids.md) <br/> |Содержит уникальные удостоверения элементов, элементов возникновения и повторяющихся элементов, используемых для удаления, отправки, получения, перемещения или копирования элементов в Exchange магазине.  <br/> |
|[SavedItemFolderId](saveditemfolderid.md) <br/> |Определяет целевую папку для операций, которые обновляют, отправляют и создают элементы в Exchange магазине.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

Нет.
  
## <a name="remarks"></a>Заметки

Если элемент в папке Отправленные элементы отправляется, отправленный элемент удаляется и его копия отправляется в папку Отправленные элементы.
  
Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция SendItem](senditem-operation.md)

