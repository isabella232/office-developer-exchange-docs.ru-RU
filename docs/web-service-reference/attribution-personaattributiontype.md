---
title: Attribution (PersonaAttributionType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: dc59e17e-baea-4617-8ca1-4382a89de0d7
description: Элемент Attribution указывает экземпляр в массиве атрибутов элемента PersonaType.
ms.openlocfilehash: eb2fe66042b6c7f52732be20195f0f4b94ab867c
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59524380"
---
# <a name="attribution-personaattributiontype"></a>Attribution (PersonaAttributionType)

Элемент **Attribution** указывает экземпляр в массиве атрибутов элемента **PersonaType.** 
  
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
|[ID (строка)](id-string.md) <br/> |Указывает строку, которая однозначно идентифицирует приложение или атрибут в персоне.  <br/> |
|[SourceId](sourceid.md) <br/> |Указывает идентификатор контакта или получателя Active Directory.  <br/> |
|[DisplayName (string)](displayname-string.md) <br/> |Определяет имя отображения папки, контакта, списка рассылки, пользователя делегирования или правила.  <br/> |
|[IsWritable](iswritable.md) <br/> |Указывает, можно ли написать для конкретного контакта или получателя Active Directory.  <br/> |
|[IsQuickContact](isquickcontact.md) <br/> |Указывает значение Boolean, которое указывает, является ли контактный контакт или получатель Active Directory быстрым.  <br/> |
|[IsHidden](ishidden.md) <br/> |Содержит значение Boolean, которое указывает, должен ли скрытый или активный получатель Каталога в качестве части персоны.  <br/> |
|[FolderId](folderid.md) <br/> |Содержит идентификатор и ключ изменения папки.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Attributions (ArrayOfPersonaAttributionsType)](attributions-arrayofpersonaattributionstype.md) <br/> |Указывает массив сведений об атрибуции для одного или более контактов или активных получателей каталога(AD), агрегированных в связанное лицо.  <br/> |
   
## <a name="remarks"></a>Заметки

Этот элемент появился в Exchange Server 2013.
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема типа  <br/> |
|Файл проверки  <br/> |types.xsd  <br/> |
|Может быть пустым  <br/> ||
   
## <a name="see-also"></a>См. также

- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

