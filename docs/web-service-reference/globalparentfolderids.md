---
title: GlobalParentFolderIds
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 8f5fcbcb-05ed-462a-99cf-a6b112a4aef6
description: Элемент GlobalParentFolderIds указывает идентификаторы глобального родительских папок.
ms.openlocfilehash: b0ff9ab00f3e46351b5a2db9bc4b6282fa4385cd
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833747"
---
# <a name="globalparentfolderids"></a>GlobalParentFolderIds

Элемент **GlobalParentFolderIds** указывает идентификаторы глобального родительских папок. 
  
```XML
<GlobalParentFolderIds>
    <FolderId/>
    <DistinguishedFolderId/>
</GlobalParentFolderIds>
```

 **NonEmptyArrayOfBaseFolderIdsType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[FolderId](folderid.md) <br/> |Содержит идентификатор и ключ изменения папки.  <br/> |
|[DistinguishedFolderId](distinguishedfolderid.md) <br/> |Идентифицирует папки, которые можно ссылаться по имени.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Беседы (ConversationType)](conversation-conversationtype.md) <br/> |Представляет одну беседу.  <br/> |
   
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

