---
title: AddBlankTargetToLinks
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 30180298-2501-4369-9b8f-2f7663f02336
description: Элемент AddBlankTargetToLinks указывает, что целевой атрибут в HTML-ссылках задан для открытия нового окна.
ms.openlocfilehash: c8d7a5973e60e43638472b0da29842ce1caacc98
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59543830"
---
# <a name="addblanktargettolinks"></a>AddBlankTargetToLinks

Элемент **AddBlankTargetToLinks** указывает, что целевой атрибут в HTML-ссылках задан для открытия нового окна. 
  
```XML
<AddBlankTargetToLinks> true | false </AddBlankTargetToLinks>
```

**xs:Boolean**

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[ItemShape](itemshape.md) <br/> | Определяет свойства и содержимое элемента, которые необходимо включить в **ответ GetItem,** **FindItem,** **GetConversationItems** или **SyncFolderItems.**<br/><br/>  Ниже приводится выражение XPath к этому элементу:<br/><br/>  `/GetItem/ItemShape` <br/>  `/FindItem/ItemShape` <br/>  `/SyncFolderItems/ItemShape` <br/>  `/GetConversationItems/ItemShape` <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое **значение, истинное** для **элемента AddBlankTargetToLinks,** указывает на то, что все HTML-ссылки будут настроены на открытие нового окна. Значение false **указывает,** что HTML-ссылки будут открываться в текущем окне. 
  
## <a name="remarks"></a>Заметки

Этот элемент является необязательным.
  
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

