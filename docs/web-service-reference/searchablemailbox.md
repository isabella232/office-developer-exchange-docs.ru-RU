---
title: SearchableMailbox
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 339005cd-a3b9-47dd-bc7b-a860b699625b
description: Элемент SearchableMailbox указывает почтовый ящик, возвращаемый из запроса GetSearchableMailboxes.
ms.openlocfilehash: 75d5680de8b0776b1ecf441ff71266ee74c4aa66
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59524429"
---
# <a name="searchablemailbox"></a>SearchableMailbox

Элемент **SearchableMailbox** указывает почтовый ящик, возвращаемый из **запроса GetSearchableMailboxes.** 
  
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

 **SearchableMailboxType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

[Guid](guid-ex15websvcsotherref.md)  |  [PrimarySmtpAddress (string)](primarysmtpaddress-string.md)  |  [IsExternalMailbox](isexternalmailbox.md)  |  [ExternalEmailAddress](externalemailaddress.md)  |  [DisplayName (string)](displayname-string.md)  |  [IsMembershipGroup](ismembershipgroup.md)  |  [ReferenceId](referenceid.md)
  
### <a name="parent-elements"></a>Родительские элементы

[SearchableMailboxes](searchablemailboxes.md)
  
## <a name="remarks"></a>Заметки

Этот элемент появился в Exchange Server 2013.
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> ||
   

