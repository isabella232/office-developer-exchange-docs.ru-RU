---
title: UpdateItemInRecoverableItemsResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 2f61b038-eba0-40fc-8af2-c3db5cc5a420
description: Элемент UpdateItemInRecoverableItemsResponse указывает ответ на запрос UpdateItemInRecoverableItems.
ms.openlocfilehash: 2cb9bcb2752599a546c1391d6ea306735b3b0c78
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19840354"
---
# <a name="updateiteminrecoverableitemsresponse"></a>UpdateItemInRecoverableItemsResponse

Элемент **UpdateItemInRecoverableItemsResponse** указывает ответ на запрос **UpdateItemInRecoverableItems** . 
  
```XML
<UpdateItemInRecoverableItemsResponse>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <Items/>
   <Attachments/>
   <ConflictResults/>
</UpdateItemInRecoverableItemsResponse>
```

 **UpdateItemInRecoverableItemsResponseMessageType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

[MessageText](messagetext.md) | [ResponseCode](responsecode.md) | [DescriptiveLinkKey](descriptivelinkkey.md) | [MessageXml](messagexml.md) | [элементы](items.md) | [вложения](attachments-ex15websvcsotherref.md) | [ConflictResults](conflictresults.md)
  
### <a name="parent-elements"></a>Родительские элементы

Нет.
  
## <a name="remarks"></a>Замечания

Этот элемент появился в Exchange Server 2013.
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |Нет  <br/> |
   

