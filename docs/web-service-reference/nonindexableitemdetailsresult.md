---
title: NonIndexableItemDetailsResult
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 7cbdbc21-5405-4cbc-8ca0-d7b0257927aa
description: Элемент NonIndexableItemDetailsResult указывает результаты операции GetNonIndexableItemDetails WSDL.
ms.openlocfilehash: 16f3c8a74f635fdd8204fe207777b4b30bc4d2ed
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59539284"
---
# <a name="nonindexableitemdetailsresult"></a>NonIndexableItemDetailsResult

Элемент **NonIndexableItemDetailsResult** указывает результаты операции **GetNonIndexableItemDetails** WSDL. 
  
```XML
<NonIndexableItemDetailsResult>
   <Items/>
   <FailedMailboxes/>
</NonIndexableItemDetailsResult>
```

 **NonIndexableItemDetailResultType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

[Элементы (ArrayOfNonIndexableItemDetailsType),](items-arrayofnonindexableitemdetailstype.md) [failedMailboxes](failedmailboxes.md)
  
### <a name="parent-elements"></a>Родительские элементы

[GetNonIndexableItemDetailsResponse,](getnonindexableitemdetailsresponse.md) [GetNonIndexableItemDetailsResponseMessage](getnonindexableitemdetailsresponsemessage.md)
  
## <a name="remarks"></a>Заметки

Этот элемент появился в Exchange Server 2013.
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция GetNonIndexableItemDetails](getnonindexableitemdetails-operation.md)


- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

