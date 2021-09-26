---
title: AdditionalInfo
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 50bebbab-2fef-4a27-a5a9-32d7200820b6
description: Элемент AdditionalInfo указывает дополнительные сведения о состоянии удержания почтового ящика.
ms.openlocfilehash: d8b707fb04ffe91d5c7aa793c6b56c8bb048f160
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59544320"
---
# <a name="additionalinfo"></a>AdditionalInfo

Элемент **AdditionalInfo** указывает дополнительные сведения о состоянии удержания почтового ящика. 
  
```XML
<AdditionalInfo></AdditionalInfo>
```

 **xs:string**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[MailboxHoldStatus](mailboxholdstatus.md) <br/> |Указывает состояние удержания почтового ящика.  <br/> |
|[NonIndexableItemDetail](nonindexableitemdetail.md) <br/> |Указывает подробности для элемента, который не может быть проиндексировать.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение элемента AdditionalInfo — это дополнительные сведения о состоянии удержания почтового ящика.
  
## <a name="remarks"></a>Заметки

Этот элемент является необязательным.
  
Этот элемент появился в Exchange Server 2013.
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема типа  <br/> |
|Файл проверки  <br/> |types.xsd  <br/> |
|Может быть пустым  <br/> ||
   
## <a name="see-also"></a>См. также

- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

