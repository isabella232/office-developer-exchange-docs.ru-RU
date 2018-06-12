---
title: Битовая маска
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Bitmask
api_type:
- schema
ms.assetid: fc7eeac2-555f-4cbc-8b48-26d9ed67748a
description: Элемент Битовая маска представляет шестнадцатеричном или десятичном маска для использования во время операции ограничения Excludes.
ms.openlocfilehash: 86c8c61f22d8d620a9139280b2a43ed7fec4727d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761575"
---
# <a name="bitmask"></a>Битовая маска

Элемент **Битовая маска** представляет шестнадцатеричном или десятичном маска для использования во время операции ограничения [Excludes](excludes.md) . 
  
```xml
<Bitmask Value="" />
```

**ExcludesValueType**

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|**Значение** | Представляет decimal или шестнадцатеричную битовую маску. Значение, представленное следующее регулярное выражение:<br/>"((0 x|0x)[0-9A-Fa-f]*)|([0-9] *) ".<br/><br/>Ниже приведены примеры шестнадцатеричные значения этого атрибута.<br/>-0x12AF<br/>-0X334AE<br/><br/>Ниже приведены примеры decimal значения этого атрибута.<br/>-10<br/>-255<br/>-4562 |
   
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Исключает](excludes.md) <br/> |Выполняет битовую маску свойства.  <br/> |
   
## <a name="remarks"></a>Замечания

Шестнадцатеричные значения должны иметь префикс 0 x или 0 X. Если этот префикс не существует, значение считается десятичного числа.
  
Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

