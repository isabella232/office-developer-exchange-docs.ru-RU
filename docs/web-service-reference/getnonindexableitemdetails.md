---
title: GetNonIndexableItemDetails
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: ce3994c1-3bb4-4571-b026-34a6c5705410
description: Элемент GetNonIndexableItemDetails указывает запрос на получение сведений о неиндексируемых элементах.
ms.openlocfilehash: 1c04b4cd7a86183210be869973c9779188fa0adf
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458602"
---
# <a name="getnonindexableitemdetails"></a>GetNonIndexableItemDetails

Элемент **GetNonIndexableItemDetails** указывает запрос на получение сведений о неиндексируемых элементах. 
  
```XML
<GetNonIndexableItemDetails>
    <Mailboxes/>
    <PageSize/>
    <PageItemReference/>
    <PageDirection/>
</GetNonIndexableItemDetails>
```

 **жетнониндексаблеитемдетаилстипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Почтовые ящики (Нонемптяррайофлегациднстипе)](mailboxes-nonemptyarrayoflegacydnstype.md) <br/> |Указывает массив элементов **почтового ящика** .  <br/> |
|[PageSize](pagesize.md) <br/> |Содержит количество элементов, возвращаемых на одной странице для результатов поиска.  <br/> |
|[пажеитемреференце](pageitemreference.md) <br/> |Указывает ссылку на элемент страницы.  <br/> |
|[пажедиректион](pagedirection.md) <br/> |Содержит направление разбивки в результатах поиска.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

Нет.
  
## <a name="remarks"></a>Примечания

Этот элемент появился в Exchange Server 2013.
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема сообщения  <br/> |
|Файл проверки  <br/> |messages. xsd  <br/> |
|Может быть пустым  <br/> ||
   
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

