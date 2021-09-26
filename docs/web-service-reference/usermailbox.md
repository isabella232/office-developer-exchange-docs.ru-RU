---
title: UserMailbox
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 1d47141c-3c3f-45b8-90c5-33a44adb34b2
description: Элемент UserMailbox идентифицирует почтовый ящик пользователя.
ms.openlocfilehash: c2a66b23de5e4b312f60019f0b4ecfb4088b3da2
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59542619"
---
# <a name="usermailbox"></a>UserMailbox

Элемент **UserMailbox** идентифицирует почтовый ящик пользователя. 
  
```XML
<UserMailbox Id="" IsArchive=""/>
```

 **UserMailboxType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|Id  <br/> |Текстовое значение атрибута **Id** — идентификатор почтового ящика.  <br/> |
|IsArchive  <br/> |Текстовое значение **атрибута IsArchive** указывает, является ли почтовый ящик архивным. Значение текста, **истинное для** **атрибута IsArchive,** указывает на то, что почтовый ящик — это архивный почтовый ящик. Значение false **для** **атрибута IsArchive** указывает, что почтовый ящик является основным почтовым ящиком.  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

[Почтовые ящики (ArrayOfUserMailboxesType)](mailboxes-arrayofusermailboxestype.md)  |  [MailboxStatisticsSearchResult](mailboxstatisticssearchresult.md)
  
## <a name="remarks"></a>Заметки

Этот элемент появился в Exchange Server 2013.
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |true  <br/> |
   

