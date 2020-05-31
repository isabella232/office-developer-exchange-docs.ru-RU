---
title: Маски
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
description: Элемент битовая маска представляет шестнадцатеричную или десятичную маску, используемую во время операции ограничения исключений.
ms.openlocfilehash: 86c8c61f22d8d620a9139280b2a43ed7fec4727d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761575"
---
# <a name="bitmask"></a>Маски

Элемент **Битовая** маска представляет шестнадцатеричную или десятичную маску, используемую во время операции ограничения [исключений](excludes.md) . 
  
```xml
<Bitmask Value="" />
```

**ексклудесвалуетипе**

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|**Значение** | Представляет десятичную или шестнадцатеричную битовую маску. Значение представлено следующим регулярным выражением:<br/>"((0x|0X) [0-9A-Fa-f] *)|([0-9] *) '.<br/><br/>Ниже приведены примеры шестнадцатеричных значений для этого атрибута.<br/>- 0x12AF<br/>- 0X334AE<br/><br/>Ниже приведены примеры десятичных значений для этого атрибута.<br/>– 10<br/>— 255<br/>— 4562 |
   
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Исключает](excludes.md) <br/> |Выполняет битовую маску для свойств.  <br/> |
   
## <a name="remarks"></a>Примечания

Шестнадцатеричные значения должны иметь префикс 0x или 0X. Если этот префикс не существует, предполагается, что значение равно десятичному числу.
  
Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

