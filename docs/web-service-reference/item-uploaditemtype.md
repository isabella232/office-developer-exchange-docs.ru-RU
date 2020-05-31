---
title: Элемент (Уплоадитемтипе)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: ab7058f2-615f-4393-a0d4-af76727f37e9
description: Элемент Item представляет отдельный элемент для отправки в почтовый ящик.
ms.openlocfilehash: 8fecef9a2368a44e38633eb9fddaa8197620f6a1
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834138"
---
# <a name="item-uploaditemtype"></a>Элемент (Уплоадитемтипе)

Элемент **Item** представляет отдельный элемент для отправки в почтовый ящик. 
  
[UploadItems](uploaditems.md)
  
[Элементы (Нонемптяррайофуплоадитемстипе)](items-nonemptyarrayofuploaditemstype.md)
  
[Элемент (Уплоадитемтипе)](item-uploaditemtype.md)
  
```XML
<Item CreateAction="" IsAssociated="">
   <ParentFolderId/>
   <ItemId/>
   <Data/>
</Item>
```

 **уплоадитемтипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|**CreateAction** <br/> |Задает действие для отправки элемента в почтовый ящик. Этот атрибут является обязательным.  <br/> |
|**Связанный** <br/> |Указывает, является ли отправленный элемент связанным с папкой. Этот атрибут является логическим значением. Значение **true** указывает, что элемент является элементом, связанным с папкой. Этот атрибут является необязательным.  <br/> |
   
#### <a name="createaction-attribute"></a>Атрибут CreateAction

|**Значение**|**Описание**|
|:-----|:-----|
|**CreateNew** <br/> |Указывает, что новая копия исходного элемента будет отправлена в почтовый ящик. Элемент [ItemId](itemid.md) не должен присутствовать, если используется значение CreateNew. В ответе возвращается идентификатор нового элемента.  <br/> |
|**обновление**. <br/> |Указывает, что элемент, указанный с помощью элемента **ItemId** , будет обновлен. Если элемент **ItemId** отсутствует или не существует в папке, указанной с помощью элемента [ParentFolderId](parentfolderid.md) , возвращается ошибка.  <br/> |
|**упдатеоркреате** <br/> |Указывает, что сначала выполняется попытка обновления элемента. Если элемент не существует в папке, указанной с помощью элемента **ParentFolderId** , создается новый элемент.  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[ParentFolderId](parentfolderid.md) <br/> |Представляет идентификатор родительской папки, в которой создается новый элемент, или содержащая обновляемый элемент.  <br/> |
|[Идентификатор](itemid.md) <br/> |Содержит уникальный идентификатор и ключ изменения элемента для создания или обновления в хранилище Exchange.  <br/> |
|[Data (base64Binary)](data-base64binary.md) <br/> |Содержит данные одного элемента для отправки в почтовый ящик.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Элементы (Нонемптяррайофуплоадитемстипе)](items-nonemptyarrayofuploaditemstype.md) <br/> |Содержит массив элементов для отправки в почтовый ящик.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Нет.
  
## <a name="remarks"></a>Примечания

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.Этот элемент появился в Exchange Server 2010 с пакетом обновления 1 (SP1).
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция ExportItems](exportitems-operation.md)
  
[Операция UploadItems](uploaditems-operation.md)

