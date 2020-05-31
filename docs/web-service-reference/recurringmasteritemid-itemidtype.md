---
title: Рекуррингмастеритемид (Итемидтипе)
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 48d831cf-10d8-480b-86d2-f9c0b14b8167
description: Элемент Рекуррингмастеритемид (Итемидтипе) идентифицирует элемент шаблона повторения, определяя идентификаторы одного из связанных элементов вхождения.
ms.openlocfilehash: 89089067963e99ac1a6cae6ea6e1e8350d148e82
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835010"
---
# <a name="recurringmasteritemid-itemidtype"></a>Рекуррингмастеритемид (Итемидтипе)

Элемент **рекуррингмастеритемид (итемидтипе)** идентифицирует элемент шаблона повторения, определяя идентификаторы одного из связанных элементов вхождения. 
  
```XML
<RecurringMasterItemId Id="" ChangeKey=""/>
```

 **итемидтипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

****

|**Атрибут**|**Описание**|
|:-----|:-----|
|Id  <br/> |Определяет один экземпляр повторяющегося элемента шаблона. Этот атрибут является обязательным.  <br/> |
|чанжекэй  <br/> |Определяет конкретную версию одного экземпляра повторяющегося элемента шаблона. Кроме того, также идентифицируется шаблон повторяющегося элемента, так как он и один экземпляр будут содержать один и тот же ключ изменения. Этот атрибут является необязательным.  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

[Reminder](reminder.md)
  
## <a name="remarks"></a>Примечания

Этот элемент появился в Exchange Server 2013 с пакетом обновления 1 (SP1).
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |True  <br/> |
   
## <a name="see-also"></a>См. также



[Reminder](reminder.md)


- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

