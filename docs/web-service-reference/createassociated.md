---
title: CreateAssociated
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CreateAssociated
api_type:
- schema
ms.assetid: 742a6136-6015-4924-bae4-f3868127e966
description: Элемент CreateAssociated указывает ли клиента можно создать таблицу связанного содержимого. Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).
ms.openlocfilehash: ec6e55ed2423ff5849f6d19aee29f790572ddda6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761854"
---
# <a name="createassociated"></a>CreateAssociated

Элемент **CreateAssociated** указывает ли клиента можно создать таблицу связанного содержимого. Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1). 
  
```xml
<CreateAssociated>true or false</CreateAssociated>
```

 **boolean**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[EffectiveRights](effectiverights.md) <br/> |Содержит правами клиент, построенный на параметры разрешений для элемента или папки. Этот элемент появился в Exchange 2007 с пакетом обновления 1.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение **true,** указывает, что клиент может создать таблицу связанного содержимого. 
  
## <a name="remarks"></a>Замечания

Это свойство используется только для объектов папки.
  
Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)


[Setting Folder-Level Permissions](http://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

