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
ms.openlocfilehash: 0d0981d050fa388e83eaa8408b60d305296c1f36
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835284"
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

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

[GUID](guid-ex15websvcsotherref.md) | [PrimarySmtpAddress (String)](primarysmtpaddress-string.md) | [исекстерналмаилбокс](isexternalmailbox.md) | [ExternalEmailAddress](externalemailaddress.md) | [DisplayName (строка)](displayname-string.md) | [исмембершипграуп](ismembershipgroup.md) | [референцеид](referenceid.md)
  
### <a name="parent-elements"></a>Родительские элементы

[сеарчаблемаилбоксес](searchablemailboxes.md)
  
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
   

