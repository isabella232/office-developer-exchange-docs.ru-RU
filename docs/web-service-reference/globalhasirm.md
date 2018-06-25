---
title: GlobalHasIrm
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 425272b2-7a4e-4376-aea9-d9b10c1ad6ee
description: Элемент GlobalHasIrm указывает, является ли по крайней мере один сообщений в окне беседы и во всех папках сообщение защищенные IRM.
ms.openlocfilehash: ad3eafcb38829e7ea57cbc7535b0f5411ad595d2
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833717"
---
# <a name="globalhasirm"></a>GlobalHasIrm

Элемент **GlobalHasIrm** указывает, является ли по крайней мере один сообщений в окне беседы и во всех папках сообщение защищенные IRM. 
  
```XML
<GlobalHasIrm> true | false </GlobalHasIrm>
```

 **Boolean**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

[Беседы (ConversationType)](conversation-conversationtype.md)
  
## <a name="text-value"></a>Текстовое значение

Текстовое значение элемента **GlobalHasIrm** равно **true** , если хотя бы один сообщение в окне беседы и во всех папках является сообщением защищенные IRM. В противном случае — значение **false**.
  
## <a name="remarks"></a>Замечания

Этот элемент появился в Exchange Server 2013 с пакетом обновления 1 (SP1).
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |True  <br/> |
   
## <a name="see-also"></a>См. также



[Беседы (ConversationType)](conversation-conversationtype.md)


- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

