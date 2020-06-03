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
ms.openlocfilehash: ab48353b0ffaf4bc3b9409f1a620d145bffc7a13
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44466936"
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

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

[ID (итемидтипе)](id-itemidtype.md)  |  [Почтовый ящик (превиевитеммаилбокстипе)](mailbox-previewitemmailboxtype.md)  |  [ParentID](parentid.md)  |  [ItemClass](itemclass.md)  |  [Уникуехаш](uniquehash.md)  |  [Сортвалуе](sortvalue.md)  |  [Овалинк](owalink.md)  |  [Sender (строка)](sender-string.md)  |  [ToRecipients (аррайофсмтпаддресстипе)](torecipients-arrayofsmtpaddresstype.md)  |  [CcRecipients](ccrecipients.md)  |  [BccRecipients](bccrecipients.md)  |  [CreatedTime](createdtime.md)  |  [ReceivedTime](receivedtime.md)  |  [Сенттиме](senttime.md)  |  [Subject (тема](subject.md)  |  ) [Размер (длинный)](size-long.md)  |  [Предварительная версия](preview-ex15websvcsotherref.md)  |  [Важно](importance.md)  |  ! [Read (чтение](read.md)  |  ) [HasAttachment](hasattachment.md)  |  [Екстендедпропертиес (нонемптяррайофекстендедпропертитипе)](extendedproperties-nonemptyarrayofextendedpropertytype.md)
  
### <a name="parent-elements"></a>Родительские элементы

[Элементы (Аррайофсеарчпревиевитемстипе)](items-arrayofsearchpreviewitemstype.md)
  
## <a name="remarks"></a>Примечания

Этот элемент появился в Exchange Server 2013.
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> ||
   

