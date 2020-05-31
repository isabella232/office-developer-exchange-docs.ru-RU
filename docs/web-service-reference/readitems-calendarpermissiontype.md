---
title: ReadItems (Календарпермиссионтипе)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ReadItems
api_type:
- schema
ms.assetid: bec01982-26a1-4373-b1e6-2e0c838d83c4
description: Элемент ReadItems указывает, имеет ли пользователь разрешение на чтение элементов в папке "Календарь". Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).
ms.openlocfilehash: 532b90c47cca7117a89d59e7012436268be9ebb0
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834964"
---
# <a name="readitems-calendarpermissiontype"></a>ReadItems (Календарпермиссионтипе)

Элемент **ReadItems** указывает, имеет ли пользователь разрешение на чтение элементов в папке "Календарь". Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1). 
  
```xml
<ReadItems>None or TimeOnly or TimeAndSubjectAndLocation or FullDetails</ReadItems>
```

 **календарпермиссионреадакцесстипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[календарпермиссион](calendarpermission.md) <br/> |Определяет доступ пользователя к папке календаря. Этот элемент появился в Exchange 2007 с пакетом обновления 1.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

В следующей таблице приведены возможные значения для элемента **ReadItems** . 
  
**Текстовые значения элементов ReadItems**

|**Значение**|**Описание**|
|:-----|:-----|
|Нет  <br/> |Указывает, что у пользователя нет разрешения на просмотр элементов в календаре.  <br/> |
|тимеонли  <br/> |Указывает, что у пользователя есть разрешение на просмотр сведений о занятости в календаре.  <br/> |
|тимеандсубжектандлокатион  <br/> |Указывает, что пользователь имеет разрешение на просмотр сведений о занятости в календаре и теме и местоположении встреч.  <br/> |
|фуллдетаилс  <br/> |Указывает, что у пользователя есть разрешение на просмотр всех элементов календаря, в том числе сведения о занятости, теме, местоположении и сведения о встречах.  <br/> |
   
## <a name="remarks"></a>Примечания

Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)


[Setting Folder-Level Permissions](http://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

