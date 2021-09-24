---
title: Значение
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Value
api_type:
- schema
ms.assetid: 9a30cadd-909e-41b1-b4e9-291643dd89c6
description: Элемент Value содержит значение расширенного свойства.
ms.openlocfilehash: dc9d81a17896e730a5140a097574faa7619576d1
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59513950"
---
# <a name="value"></a>Значение

Элемент **Value** содержит значение расширенного свойства. 
  
```xml
<Value/>
```

**String**

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Значения](values.md) <br/> |Содержит коллекцию значений для расширенного свойства.  <br/> |
|[ExtendedProperty](extendedproperty.md) <br/> |Определяет расширенные свойства папок и элементов.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение должно быть совместимо с типом, указанным атрибутом PropertyType extendedFieldURI.
  
## <a name="remarks"></a>Заметки

Элемент **Value** может возникать как в одиночных, так и в многооценных экземплярах расширенного свойства. Для одноприемных экземпляров он существует как прямой ребенок элемента [ExtendedProperty.](extendedproperty.md) Для многоценного экземпляра он существует как прямой ребенок коллекции **Значений.** 
  
Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

