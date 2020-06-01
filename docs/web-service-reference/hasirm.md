---
title: хасирм
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: fedc04e0-cfd2-4652-a2a8-51de859ae847
description: Элемент Хасирм указывает, является ли по крайней мере одно сообщение в беседе и в текущей папке защищенным сообщением управления правами на доступ к данным.
ms.openlocfilehash: 1596610ed5f6b2bac353900624fbec9140aaa693
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462782"
---
# <a name="hasirm"></a>хасирм

Элемент **хасирм** указывает, является ли по крайней мере одно сообщение в беседе и в текущей папке защищенным сообщением управления правами на доступ к данным. 
  
```XML
<HasIrm> true | false </HasIrm>
```

 **Boolean**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

Отсутствуют.
  
### <a name="parent-elements"></a>Родительские элементы

[Беседы (ConversationType)](conversation-conversationtype.md)
  
## <a name="text-value"></a>Текстовое значение

Текстовое значение элемента **хасирм** имеет значение **true** , если по крайней мере одно сообщение в беседе и текущая папка имеют IRM. В противном случае — значение **false**.
  
## <a name="remarks"></a>Примечания

Этот элемент появился в Exchange Server 2013 с пакетом обновления 1 (SP1).
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |True  <br/> |
   
## <a name="see-also"></a>См. также



[Беседы (ConversationType)](conversation-conversationtype.md)


- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

