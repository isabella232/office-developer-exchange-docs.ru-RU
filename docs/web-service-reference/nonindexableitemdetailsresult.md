---
title: нониндексаблеитемдетаилсресулт
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 7cbdbc21-5405-4cbc-8ca0-d7b0257927aa
description: Элемент Нониндексаблеитемдетаилсресулт указывает результаты операции WSDL GetNonIndexableItemDetails.
ms.openlocfilehash: 6e271f2cf0e37f26b945332c94167b6a42354115
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834535"
---
# <a name="nonindexableitemdetailsresult"></a>нониндексаблеитемдетаилсресулт

Элемент **нониндексаблеитемдетаилсресулт** указывает результаты операции WSDL **GetNonIndexableItemDetails** . 
  
```XML
<NonIndexableItemDetailsResult>
   <Items/>
   <FailedMailboxes/>
</NonIndexableItemDetailsResult>
```

 **нониндексаблеитемдетаилресулттипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

[Items (аррайофнониндексаблеитемдетаилстипе)](items-arrayofnonindexableitemdetailstype.md) , [фаиледмаилбоксес](failedmailboxes.md)
  
### <a name="parent-elements"></a>Родительские элементы

[Жетнониндексаблеитемдетаилсреспонсе](getnonindexableitemdetailsresponse.md) , [жетнониндексаблеитемдетаилсреспонсемессаже](getnonindexableitemdetailsresponsemessage.md)
  
## <a name="remarks"></a>Примечания

Этот элемент появился в Exchange Server 2013.
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция GetNonIndexableItemDetails](getnonindexableitemdetails-operation.md)


- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

