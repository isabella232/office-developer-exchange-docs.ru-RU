---
title: аддбланктаржеттолинкс
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 30180298-2501-4369-9b8f-2f7663f02336
description: Элемент Аддбланктаржеттолинкс указывает, что целевой атрибут в HTML-ссылках имеет значение открыть новое окно.
ms.openlocfilehash: 1d4d36c1f4b98ebee96baea683c40527d2a9ec27
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465045"
---
# <a name="addblanktargettolinks"></a>аддбланктаржеттолинкс

Элемент **аддбланктаржеттолинкс** указывает, что целевой атрибут в HTML-ссылках имеет значение открыть новое окно. 
  
```XML
<AddBlankTargetToLinks> true | false </AddBlankTargetToLinks>
```

**xs: Boolean**

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

Отсутствуют.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[итемшапе](itemshape.md) <br/> | Определяет свойства и контент элемента, включаемые в ответ **GetItem**, **FindItem**, **GetConversationItems** или **SyncFolderItems** .<br/><br/>  Ниже приведены выражения XPath для этого элемента.<br/><br/>  `/GetItem/ItemShape` <br/>  `/FindItem/ItemShape` <br/>  `/SyncFolderItems/ItemShape` <br/>  `/GetConversationItems/ItemShape` <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение **true** для элемента **аддбланктаржеттолинкс** указывает на то, что все HTML-ссылки будут настроены на открытие нового окна. Значение **false** указывает, что HTML-ссылки будут открываться в текущем окне. 
  
## <a name="remarks"></a>Примечания

Этот элемент является необязательным.
  
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

