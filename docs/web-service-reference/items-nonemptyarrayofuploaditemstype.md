---
title: Элементы (Нонемптяррайофуплоадитемстипе)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Items
api_type:
- schema
ms.assetid: 402bfa6d-11d7-4547-b8bd-197e9922ab49
description: Элемент Items содержит массив элементов для отправки в почтовый ящик.
ms.openlocfilehash: 5c69134c1613b0a4595a6aa876fa09fde63043ea
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44441550"
---
# <a name="items-nonemptyarrayofuploaditemstype"></a>Элементы (Нонемптяррайофуплоадитемстипе)

Элемент **Items** содержит массив элементов для отправки в почтовый ящик. 
  
[UploadItems](uploaditems.md)
  
[Элементы (Нонемптяррайофуплоадитемстипе)](items-nonemptyarrayofuploaditemstype.md)
  
```XML
<Items>
   <Item/>
</Items>
```

 **нонемптяррайофуплоадитемстипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Элемент (Уплоадитемтипе)](item-uploaditemtype.md) <br/> |Представляет отдельный элемент для отправки в почтовый ящик.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[UploadItems](uploaditems.md) <br/> |Представляет запрос на отправку элементов в почтовый ящик.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Нет.
  
## <a name="remarks"></a>Примечания

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.Этот элемент появился в Exchange Server 2010 с пакетом обновления 1 (SP1).
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема сообщения  <br/> |
|Файл проверки  <br/> |Messages. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция ExportItems](exportitems-operation.md)
  
[Операция UploadItems](uploaditems-operation.md)

