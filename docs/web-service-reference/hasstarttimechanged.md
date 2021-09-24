---
title: HasStartTimeChanged
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 04a6968d-7fb5-47ee-b66e-dc99c35dbb63
description: Элемент HasStartTimeChanged указывает, изменилось ли время начала собрания.
ms.openlocfilehash: 7f04c4d34a081b91adbb0796019e93bc50bfb8ab
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59539649"
---
# <a name="hasstarttimechanged"></a>HasStartTimeChanged

Элемент **HasStartTimeChanged** указывает, изменилось ли время начала собрания. 
  
```XML
<HasStartTimeChanged> true | false </HasStartTimeChanged>
```

 **Boolean**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[ChangeHighlights](changehighlights.md) <br/> |Указывает, что изменилось между двумя версиями сообщения о запросе на собрание.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Значение **текста, истинное** для **элемента HasStartTimeChanged,** указывает на то, что время начала собрания изменилось. Значение false **указывает,** что время начала не изменилось. 
  
## <a name="remarks"></a>Заметки

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

