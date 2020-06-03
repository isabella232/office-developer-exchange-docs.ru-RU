---
title: филтерхтмлконтент
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FilterHtmlContent
api_type:
- schema
ms.assetid: 2f9358a0-de1d-4544-9aa0-d9f6519f3b5f
description: Элемент Филтерхтмлконтент указывает, фильтруется ли потенциально небезопасное HTML-содержимое из элемента или вложения.
ms.openlocfilehash: 28e3be86b550c3f330fbb6846b64732b5674304d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462677"
---
# <a name="filterhtmlcontent"></a>филтерхтмлконтент

Элемент **филтерхтмлконтент** указывает, фильтруется ли потенциально небезопасное HTML-содержимое из элемента или вложения. 
  
```xml
<FilterHtmlContent>true or false</FilterHtmlContent>
```

 **boolean**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

Отсутствуют.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[аттачментшапе](attachmentshape.md) <br/> | Определяет дополнительные свойства, возвращаемые в ответе на запрос [GetAttachment](getattachment.md) .  <br/><br/>  Ниже приведено выражение XPath для этого элемента: <br/> <br/>  `/GetAttachment/AttachmentShape` <br/> |
|[итемшапе](itemshape.md) <br/> | Определяет свойства и контент элемента, включаемые в ответ GetItem, FindItem или SyncFolderItems.  <br/> <br/> Ниже приведены выражения XPath для этого элемента. <br/> <br/>  `/GetItem/ItemShape`<br/> <br/>  `/FindItem/ItemShape`<br/> <br/>  `/SyncFolderItems/ItemShape` <br/> |
   
## <a name="text-value"></a>Текстовое значение

Этот элемент может иметь **значение true** или **false**. Значение по умолчанию — **false**. Это логический тип данных.
  
## <a name="remarks"></a>Примечания

Этот элемент является необязательным.
  
Схема, описывающая этот элемент, находится в виртуальном каталоге EWS компьютера, на котором установлен сервер Exchange Server с установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

