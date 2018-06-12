---
title: Элемент (UploadItemType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: ab7058f2-615f-4393-a0d4-af76727f37e9
description: Элемент представляет один элемент для передачи в почтовый ящик.
ms.openlocfilehash: 8fecef9a2368a44e38633eb9fddaa8197620f6a1
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19834138"
---
# <a name="item-uploaditemtype"></a>Элемент (UploadItemType)

**Элемент** представляет один элемент для передачи в почтовый ящик. 
  
[UploadItems](uploaditems.md)
  
[Элементы (NonEmptyArrayOfUploadItemsType)](items-nonemptyarrayofuploaditemstype.md)
  
[Элемент (UploadItemType)](item-uploaditemtype.md)
  
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
|**CreateAction** <br/> |Указывает действие для отправки элемента в почтовом ящике. Этот атрибут является обязательным.  <br/> |
|**IsAssociated** <br/> |Указывает, будет ли загруженного элемента — элемент папки, связанной. Этот атрибут является значение типа Boolean. Значение **true** указывает, что элемент — папка, связанный элемент. Этот атрибут является необязательным.  <br/> |
   
#### <a name="createaction-attribute"></a>Атрибут действие создания

|**Значение**|**Описание**|
|:-----|:-----|
|**CreateNew** <br/> |Указывает, что новую копию исходного элемента передается в почтовый ящик. Элемент [ItemId](itemid.md) не должна быть этот параметр указан, если используется значение CreateNew. Идентификатор нового элемента возвращаемого в ответе.  <br/> |
|**обновление**. <br/> |Указывает, что элемент, указанный в параметре элемент **ItemId** будут обновлены. Если элемент **ItemId** не существует, или если элемент не существует в папку, указанную в элементе [ParentFolderId](parentfolderid.md) , возвращается ошибка.  <br/> |
|**UpdateOrCreate** <br/> |Указывает, сначала предпринята попытка обновить элемент. Если элемент не существует в папке, заданной в элементе **ParentFolderId** , будет создан новый элемент.  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[ParentFolderId](parentfolderid.md) <br/> |Представляет идентификатор родительской папки, где создается новый элемент или, содержащее элемент, который требуется обновить.  <br/> |
|[Идентификатор элемента](itemid.md) <br/> |Содержит уникальный идентификатор и меняет ключ элемента для создания или обновления в хранилище Exchange.  <br/> |
|[Данные (base64Binary)](data-base64binary.md) <br/> |Содержит данные одного элемента для передачи в почтовый ящик.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Элементы (NonEmptyArrayOfUploadItemsType)](items-nonemptyarrayofuploaditemstype.md) <br/> |Содержит массив элемент загружается в почтовый ящик.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Нет.
  
## <a name="remarks"></a>Замечания

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.Этот элемент появился в Exchange Server 2010 с пакетом обновления 1 (SP1).
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция ExportItems](exportitems-operation.md)
  
[Операция UploadItems](uploaditems-operation.md)

