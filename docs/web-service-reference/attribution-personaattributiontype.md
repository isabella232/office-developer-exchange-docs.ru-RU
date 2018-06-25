---
title: Атрибуты (PersonaAttributionType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: dc59e17e-baea-4617-8ca1-4382a89de0d7
description: Атрибуты элемента экземпляр в массиве атрибутов элемента PersonaType.
ms.openlocfilehash: 0e800c92c75bf0c475d4bffd33d6ab49f9ad9a9a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761523"
---
# <a name="attribution-personaattributiontype"></a>Атрибуты (PersonaAttributionType)

**Атрибуты** элемента экземпляр в массиве атрибутов элемента **PersonaType** . 
  
```XML
<Attribution>
    <Id></Id>
    <SourceId></SourceId>
    <DisplayName></DisplayName>
    <IsWritable></IsWritable>
    <IsQuickContact></IsQuickContact>
    <IsHidden></IsHidden>
    <FolderId></FolderId>
</Attribution>
```

 **PersonaAttributionType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Идентификатор (строка)](id-string.md) <br/> |Задает строку, которая уникально идентифицирует приложение или атрибуты в пользователя.  <br/> |
|[SourceId](sourceid.md) <br/> |Задает идентификатор получателя Active Directory или контакта.  <br/> |
|[Отображаемое имя (строка)](displayname-string.md) <br/> |Задает отображаемое имя папки, контактов, список рассылки, делегата или правило.  <br/> |
|[IsWritable](iswritable.md) <br/> |Указывает, можно ли запись базовым контакт или получателя Active Directory для.  <br/> |
|[IsQuickContact](isquickcontact.md) <br/> |Задает логическое значение, которое указывает, является ли базовый контакт или получателя Active Directory быстрого контакта.  <br/> |
|[IsHidden](ishidden.md) <br/> |Содержит логическое значение, указывающее, ли базовый контакт или получателя Active Directory необходимо скрыть или отобразить как часть пользователя.  <br/> |
|[FolderId](folderid.md) <br/> |Содержит идентификатор и ключ изменения папки.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Атрибуты (ArrayOfPersonaAttributionsType)](attributions-arrayofpersonaattributionstype.md) <br/> |Указывает массив атрибуты сведения для одной или нескольких контактов или объединить в связанного пользователя active directory (AD) получателей.  <br/> |
   
## <a name="remarks"></a>Замечания

Этот элемент появился в Exchange Server 2013.
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема типа  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> ||
   
## <a name="see-also"></a>См. также

- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

