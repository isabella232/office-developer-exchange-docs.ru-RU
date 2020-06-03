---
title: сеарчаблемаилбокс
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 339005cd-a3b9-47dd-bc7b-a860b699625b
description: Элемент Сеарчаблемаилбокс указывает почтовый ящик, возвращенный из запроса GetSearchableMailboxes.
ms.openlocfilehash: f790d9a707f10f64a776b2fc35255c233ad854b6
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467454"
---
# <a name="searchablemailbox"></a>сеарчаблемаилбокс

Элемент **сеарчаблемаилбокс** указывает почтовый ящик, возвращенный из запроса **GetSearchableMailboxes** . 
  
```XML
<SearchableMailbox>
   <Guid/>
   <PrimarySmtpAddress/>
   <IsExternalMailbox/>
   <ExternalEmailAddress/>
   <DisplayName/>
   <IsMembershipGroup/>
   <ReferenceId/>
</SearchableMailbox>
```

 **сеарчаблемаилбокстипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

[Идентификатор GUID](guid-ex15websvcsotherref.md)  |  [PrimarySmtpAddress (строка)](primarysmtpaddress-string.md)  |  [Исекстерналмаилбокс](isexternalmailbox.md)  |  [ExternalEmailAddress](externalemailaddress.md)  |  [DisplayName (строка)](displayname-string.md)  |  [Исмембершипграуп](ismembershipgroup.md)  |  [Референцеид](referenceid.md)
  
### <a name="parent-elements"></a>Родительские элементы

[сеарчаблемаилбоксес](searchablemailboxes.md)
  
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
   

