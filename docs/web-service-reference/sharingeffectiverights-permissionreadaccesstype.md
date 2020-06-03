---
title: Шаринжеффективеригхтс (Пермиссионреадакцесстипе)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SharingEffectiveRights
api_type:
- schema
ms.assetid: 808bb4a1-aa2d-48c5-94b3-551b52c348bd
description: Элемент Шаринжеффективеригхтс указывает разрешения, которые есть у пользователя для данных контакта, к которым предоставлен общий доступ.
ms.openlocfilehash: 64b1e6d831068e9699e9cd47693e74919e0416a5
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44526664"
---
# <a name="sharingeffectiverights-permissionreadaccesstype"></a>Шаринжеффективеригхтс (Пермиссионреадакцесстипе)

Элемент **шаринжеффективеригхтс** указывает разрешения, которые есть у пользователя для данных контакта, к которым предоставлен общий доступ. 
  
```XML
<SharingEffectiveRights>None | FullDetails</SharingEffectiveRights >
```

 **пермиссионреадакцесстипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

Отсутствуют.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[контактсфолдер](contactsfolder.md) <br/> |Представляет папку "Контакты", содержащуюся в почтовом ящике.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

В следующей таблице приведены возможные значения для элемента **шаринжеффективеригхтс** . 
  
**Текстовые значения элементов Шаринжеффективеригхтс**

|**Значение**|**Описание**|
|:-----|:-----|
|Нет  <br/> |Указывает, что у пользователя нет разрешения на чтение элементов в папке.  <br/> |
|фуллдетаилс  <br/> |Указывает, что у пользователя есть разрешение на чтение всех элементов в папке.  <br/> |
   
## <a name="remarks"></a>Примечания

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

