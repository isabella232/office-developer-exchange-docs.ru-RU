---
title: Item (UploadItemType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: ab7058f2-615f-4393-a0d4-af76727f37e9
description: Элемент Item представляет один элемент для отправки в почтовый ящик.
ms.openlocfilehash: bd4681a19df2018db9e54ee39095cd602662650a
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59514447"
---
# <a name="item-uploaditemtype"></a>Item (UploadItemType)

Элемент **Item** представляет один элемент для отправки в почтовый ящик. 
  
[UploadItems](uploaditems.md)
  
[Items (NonEmptyArrayOfUploadItemsType)](items-nonemptyarrayofuploaditemstype.md)
  
[Item (UploadItemType)](item-uploaditemtype.md)
  
```XML
<Item CreateAction="" IsAssociated="">
   <ParentFolderId/>
   <ItemId/>
   <Data/>
</Item>
```

 **UploadItemType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|**CreateAction** <br/> |Указывает действие для отправки элемента в почтовый ящик. Этот атрибут является обязательным.  <br/> |
|**IsAssociated** <br/> |Указывает, является ли загруженный элемент связанным элементом папки. Этот атрибут является значением Boolean. Значение true **указывает,** что элемент — это связанный с папкой элемент. Этот атрибут является необязательным.  <br/> |
   
#### <a name="createaction-attribute"></a>Атрибут CreateAction

|**Значение**|**Описание**|
|:-----|:-----|
|**CreateNew** <br/> |Указывает, что в почтовый ящик загружается новая копия исходного элемента. Элемент [ItemId](itemid.md) не должен присутствовать, если используется значение CreateNew. Идентификатор нового элемента возвращается в ответ.  <br/> |
|**Обновление** <br/> |Указывает, что элемент, указанный **элементом ItemId,** будет обновлен. Ошибка возвращается, если элемента **ItemId** нет или элемент не существует в папке, идентифицированной [элементом ParentFolderId.](parentfolderid.md)  <br/> |
|**UpdateOrCreate** <br/> |Указывает, что сначала предпринята попытка обновления элемента. Если элемент не существует в папке, указанной элементом **ParentFolderId,** создается новый элемент.  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[ParentFolderId](parentfolderid.md) <br/> |Представляет идентификатор родительской папки, в которой создается новый элемент или содержит элемент для обновления.  <br/> |
|[ItemId](itemid.md) <br/> |Содержит уникальный идентификатор и ключ изменения элемента для создания или обновления в Exchange магазине.  <br/> |
|[Data (base64Binary)](data-base64binary.md) <br/> |Содержит данные одного элемента для отправки в почтовый ящик.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Items (NonEmptyArrayOfUploadItemsType)](items-nonemptyarrayofuploaditemstype.md) <br/> |Содержит массив элементов для отправки в почтовый ящик.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Нет.
  
## <a name="remarks"></a>Заметки

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.Этот элемент появился в Exchange Server 2010 с пакетом обновления 1 (SP1).
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция ExportItems](exportitems-operation.md)
  
[Операция UploadItems](uploaditems-operation.md)

