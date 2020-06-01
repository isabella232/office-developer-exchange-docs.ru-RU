---
title: Атрибуты (Персонааттрибутионтипе)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: dc59e17e-baea-4617-8ca1-4382a89de0d7
description: Элемент Attribute указывает экземпляр в массиве атрибутов для элемента Персонатипе.
ms.openlocfilehash: 05b0d41c116f2ed7b8dbb3ac44108bb879256b5c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44464177"
---
# <a name="attribution-personaattributiontype"></a>Атрибуты (Персонааттрибутионтипе)

Элемент **Attribute** указывает экземпляр в массиве атрибутов для элемента **персонатипе** . 
  
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

 **персонааттрибутионтипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[ID (строка)](id-string.md) <br/> |Указывает строку, которая уникально идентифицирует приложение или атрибуты в имени пользователя.  <br/> |
|[SourceId](sourceid.md) <br/> |Указывает идентификатор контакта или получателя Active Directory.  <br/> |
|[DisplayName (строка)](displayname-string.md) <br/> |Определяет отображаемое имя папки, контакта, списка рассылки, делегированного пользователя или правила.  <br/> |
|[Доступный для записи](iswritable.md) <br/> |Указывает, можно ли записывать базового контакта или получателя Active Directory.  <br/> |
|[искуиккконтакт](isquickcontact.md) <br/> |Задает логическое значение, указывающее, является ли основной контакт или получатель Active Directory быстрым контактом.  <br/> |
|[IsHidden](ishidden.md) <br/> |Содержит логическое значение, которое указывает, следует ли скрывать или показывать базовый контакт или получатель Active Directory в составе персонажа.  <br/> |
|[FolderId](folderid.md) <br/> |Содержит идентификатор и ключ изменения папки.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Атрибуты (Аррайофперсонааттрибутионстипе)](attributions-arrayofpersonaattributionstype.md) <br/> |Задает массив сведений о сопоставлении для одного или нескольких получателей контактов или Active Directory (AD), собранных в сопоставленный с ним пользователь.  <br/> |
   
## <a name="remarks"></a>Примечания

Этот элемент появился в Exchange Server 2013.
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема типа  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> ||
   
## <a name="see-also"></a>См. также

- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

