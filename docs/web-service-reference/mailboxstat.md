---
title: маилбоксстат
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 5f24dc30-3ac2-4c82-9dfc-be9dbdb585be
description: Элемент Маилбоксстат указывает статистику для почтового ящика, в котором выполняется поиск обнаружения.
ms.openlocfilehash: 417f63f5e1aa34c2157b1d5ad868461113afec7b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44451434"
---
# <a name="mailboxstat"></a>маилбоксстат

Элемент **маилбоксстат** указывает статистику для почтового ящика, в котором выполняется поиск обнаружения. 
  
```XML
<MailboxStat>
   <MailboxId/>
   <DisplayName/>
   <ItemCount/>
   <Size/>
</MailboxStat>
```

**маилбоксстатистикситемтипе**

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

[MailboxId](mailboxid.md)  |  [DisplayName (строка)](displayname-string.md)  |  [ItemCount](itemcount.md)  |  [Размер (длинный)](size-long.md)
  
### <a name="parent-elements"></a>Родительские элементы

[маилбоксстатс](mailboxstats.md)
  
## <a name="remarks"></a>Примечания

Этот элемент появился в Exchange Server 2013.
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |false  <br/> |
   

