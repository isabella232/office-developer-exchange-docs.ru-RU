---
title: Bitmask
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Bitmask
api_type:
- schema
ms.assetid: fc7eeac2-555f-4cbc-8b48-26d9ed67748a
description: Элемент Bitmask представляет гексадецимальную или десятичной маску, которая будет использоваться во время операции ограничений Excludes.
ms.openlocfilehash: 83307fc7f5ba328c5d6f7574a8b3be1ea25595f3
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59543592"
---
# <a name="bitmask"></a>Bitmask

Элемент **Bitmask представляет** гексадецимальную или десятичной маску, которая будет использоваться во время операции ограничений [Excludes.](excludes.md) 
  
```xml
<Bitmask Value="" />
```

**ExcludesValueType**

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|**Значение** | Представляет десятичной или hexadecimal bitmask. Значение представлено следующим регулярным выражением:<br/>`((0x|0X)[0-9A-Fa-f]*)|([0-9]*)`.<br/><br/>Ниже приводится пример гексадецимальных значений для этого атрибута:<br/>- 0x12AF<br/>- 0X334AE<br/><br/>Ниже приводится пример десятичных значений для этого атрибута:<br/>- 10<br/>- 255<br/>- 4562 |
   
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Исключает](excludes.md) <br/> |Выполняет немного более ровную маску свойств.  <br/> |
   
## <a name="remarks"></a>Заметки

Hexadecimal values must have a prefix of either 0x or 0X. Если этого префикса не существует, предполагается, что это значение является десятичной.
  
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

