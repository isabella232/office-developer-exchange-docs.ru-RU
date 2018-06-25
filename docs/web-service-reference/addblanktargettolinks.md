---
title: AddBlankTargetToLinks
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 30180298-2501-4369-9b8f-2f7663f02336
description: Элемент AddBlankTargetToLinks указывает, что атрибут target в HTML-ссылки откройте новое окно.
ms.openlocfilehash: 8a47e44d89bcc84bc0e8b61d45f18ff3182f7870
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761332"
---
# <a name="addblanktargettolinks"></a>AddBlankTargetToLinks

Элемент **AddBlankTargetToLinks** указывает, что атрибут target в HTML-ссылки откройте новое окно. 
  
```XML
<AddBlankTargetToLinks> true | false </AddBlankTargetToLinks>
```

**xs: Boolean**

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[ItemShape](itemshape.md) <br/> | Определяет свойства элемента и содержимого для включения в **GetItem**, **FindItem**, **GetConversationItems** или **SyncFolderItems** ответа.<br/><br/>  Ниже приведены выражения XPath для этого элемента.<br/><br/>  `/GetItem/ItemShape` <br/>  `/FindItem/ItemShape` <br/>  `/SyncFolderItems/ItemShape` <br/>  `/GetConversationItems/ItemShape` <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение **true** для элемента **AddBlankTargetToLinks** указывает, что все ссылки HTML-код будет иметь значение откройте новое окно. Значение **false** указывает, что HTML-ссылки будут открываться в текущем окне. 
  
## <a name="remarks"></a>Замечания

Этот элемент является необязательным.
  
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

