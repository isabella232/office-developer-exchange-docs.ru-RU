---
title: RetentionPolicyTag
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: f46679d0-9236-41e2-8624-72300079c67c
description: Элемент RetentionPolicyTag указывает политику хранения элемента почтового ящика.
ms.openlocfilehash: 58ca3016bed0be625b213a57e5ead1b38a301bfa
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59524548"
---
# <a name="retentionpolicytag"></a>RetentionPolicyTag

Элемент **RetentionPolicyTag** указывает политику хранения элемента почтового ящика. 
  
```XML
<RetentionPolicyTag>
   <DisplayName/>
   <RetentionId/>
   <RetentionPeriod/>
   <Type/>
   <RetentionAction/>
   <Description/>
   <IsVisible/>
   <OptedInto/>
   <IsArchive/>
</RetentionPolicyTag>
```

 **RetentionPolicyTagType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

[DisplayName (string)](displayname-string.md)  |  [RetentionId](retentionid.md)  |  [RetentionPeriod](retentionperiod.md)  |  [Тип (ElcFolderType)](type-elcfoldertype.md)  |  [RetentionAction](retentionaction.md)  |  [Описание](description.md)  |  [IsVisible](isvisible.md)  |  [OptedInto](optedinto.md)  |  [IsArchive](isarchive.md)
  
### <a name="parent-elements"></a>Родительские элементы

[RetentionPolicyTags](retentionpolicytags.md)
  
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
   

