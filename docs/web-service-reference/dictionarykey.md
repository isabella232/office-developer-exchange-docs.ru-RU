---
title: диктионарикэй
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DictionaryKey
api_type:
- schema
ms.assetid: f331c8ac-f1c7-4248-a570-97701969d5bf
description: Элемент Диктионарикэй указывает ключ словаря для свойства Dictionary.
ms.openlocfilehash: 8d9d897c86eb5048068936433c6c0d77917ff777
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462152"
---
# <a name="dictionarykey"></a>диктионарикэй

Элемент **диктионарикэй** указывает ключ словаря для свойства Dictionary. 
  
```xml
<DictionaryKey>
   <Type/>
   <Value/>
</DictionaryKey>
```

 **усерконфигуратиондиктионарйобжекттипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Тип (Усерконфигуратион)](type-userconfiguration.md) <br/> | Указывает тип объекта Dictionary.<br/><br/>Типом может быть одно из следующих строковых значений:<br/><br/>– DateTime  <br/>— Логическое значение  <br/>– Byte  <br/>— Строка  <br/>- Integer32  <br/>- UnsignedInteger32  <br/>- Integer64  <br/>- UnsignedInteger64  <br/>— Стрингаррай  <br/>— Битеаррай  <br/> |
|[Значение (Усерконфигуратион)](value-userconfiguration.md) <br/> |Задает значение объекта Dictionary в виде строки.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[диктионарентри](dictionaryentry.md) <br/> |Задает содержимое одного свойства записи словаря.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Нет.
  
## <a name="remarks"></a>Примечания

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

