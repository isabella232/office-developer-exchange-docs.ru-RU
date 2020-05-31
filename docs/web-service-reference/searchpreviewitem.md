---
title: сеарчпревиевитем
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 59b0b2db-a0ae-4162-a2cb-5f37f42fe872
description: Элемент Сеарчпревиевитем указывает предварительный просмотр элемента для поиска обнаружения.
ms.openlocfilehash: 46b9d6049f856ce6e93b9e49e07516ec4b52d932
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835308"
---
# <a name="searchpreviewitem"></a>сеарчпревиевитем

Элемент **сеарчпревиевитем** указывает предварительный просмотр элемента для поиска обнаружения. 
  
```XML
<SearchPreviewItem>
   <Id/>
   <Mailbox/>
   <ParentId/>
   <ItemClass/>
   <UniqueHash/>
   <SortValue/>
   <OwaLink/>
   <Sender/>
   <ToRecipients/>
   <CcRecipients/>
   <BccRecipients/>
   <CreatedTime/>
   <ReceivedTime/>
   <SentTime/>
   <Subject/>
   <Size/>
   <Preview/>
   <Importance/>
   <Read/>
   <HasAttachment/>
   <ExtendedProperties/>
</SearchPreviewItem>
```

 **сеарчпревиевитемтипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

[Идентификатор](id-itemidtype.md) | [почтового ящика (итемидтипе) (превиевитеммаилбокстипе)](mailbox-previewitemmailboxtype.md) | [ParentID](parentid.md) | [ItemClass](itemclass.md) | [уникуехаш](uniquehash.md) | [сортвалуе](sortvalue.md) | [овалинк](owalink.md) | [sender (строка)](sender-string.md) | [ToRecipients (аррайофсмтпаддресстипе)](torecipients-arrayofsmtpaddresstype.md) | [CcRecipients](ccrecipients.md) | [BccRecipients](bccrecipients.md) | [CreatedTime](createdtime.md) | [ReceivedTime](receivedtime.md) | [SentTime](senttime.md) | [subject](subject.md) | [size (Long)](size-long.md) | [Preview](preview-ex15websvcsotherref.md) | [важно](importance.md) | [читать](read.md) | [HasAttachment](hasattachment.md)HasAttachment | ExtendedProperties[(NonEmptyArrayOfExtendedPropertyType)](extendedproperties-nonemptyarrayofextendedpropertytype.md)
  
### <a name="parent-elements"></a>Родительские элементы

[Элементы (Аррайофсеарчпревиевитемстипе)](items-arrayofsearchpreviewitemstype.md)
  
## <a name="remarks"></a>Примечания

Этот элемент появился в Exchange Server 2013.
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> ||
   

