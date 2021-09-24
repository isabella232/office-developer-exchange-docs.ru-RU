---
title: ExtendedProperty (PathToExtendedFieldType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: fa620b48-2ce3-437d-b51e-541247eea1d9
description: Элемент ExtendedProperty указывает расширенное свойство для единого магазина контактов.
ms.openlocfilehash: 5cb320e15d3a01c542907048357d1ef0cc78f96a
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59530761"
---
# <a name="extendedproperty-pathtoextendedfieldtype"></a>ExtendedProperty (PathToExtendedFieldType)

Элемент **ExtendedProperty** указывает расширенное свойство для единого магазина контактов. 
  
```xml
<ExtendedProperty DistinguishedPropertySetId="" PropertySetId="" PropertyTag="" PropertyName="" PropertyId="" PropertyType="" FieldURI="">
</ExtendedProperty>
```

**PathToExtendedFieldType**

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|DistinguishedPropertySetId  <br/> |Указывает идентификатор набора свойств. Этот атрибут является необязательным.  <br/> |
|PropertySetId  <br/> |Указывает идентификатор набора свойств GUID. Этот атрибут является необязательным.  <br/> |
|PropertyTag  <br/> | Представляет тег свойства минус часть типа.<br/><br/>Существует два варианта представления:  <br/><br/>- Hexadecimal: 0x3fa4  <br/>- Десятичной: 0-65535<br/><br/>  Этот атрибут является необязательным.  <br/> |
|PropertyName  <br/> |Строка, которая указывает имя свойства. Этот атрибут является необязательным.  <br/> |
|PropertyId  <br/> |Integer, который указывает идентификатор свойства. Этот атрибут является необязательным.  <br/> |
|PropertyType  <br/> |Указывает тип свойства. Этот атрибут является обязательным.  <br/> |
|FieldURI  <br/> |Указывает поле Единообразный идентификатор ресурса (URI). Этот атрибут является обязательным. Возможные значения см. в [элементе FieldURI.](fielduri.md)  <br/> |
   
#### <a name="distinguishedpropertysetid"></a>DistinguishedPropertySetId

|**Значение**|**Описание**|
|:-----|:-----|
|Собрание  <br/> |Указывает собрание.  <br/> |
|Appointment  <br/> |Указывает встречу.  <br/> |
|Распространенная  <br/> |Указывает общий набор свойств.  <br/> |
|PublicStrings  <br/> |Указывает общедоступные строки.  <br/> |
|Address  <br/> |Указывает адрес.  <br/> |
|InternetHeaders  <br/> |Указывает заглавные данные в Интернете.  <br/> |
|CalendarAssistant  <br/> |Указывает помощник календаря.  <br/> |
|UnifiedMessaging  <br/> |Указывает единую систему обмена сообщениями.  <br/> |
|Задача  <br/> |Указывает задачу.  <br/> |
   
#### <a name="propertytype"></a>PropertyType

|**Значение**|**Описание**|
|:-----|:-----|
|ApplicationTime  <br/> |Указывает время приложения.  <br/> |
|ApplicationTimeArray  <br/> |Указывает массив времени приложения.  <br/> |
|В двоичном формате  <br/> |Указывает двоичное значение.  <br/> |
|BinaryArray  <br/> |Указывает массив двоичных значений.  <br/> |
|Логический  <br/> |Указывает значение Boolean.  <br/> |
|CLSID  <br/> |Указывает CLSID.  <br/> |
|CLSIDArray  <br/> |Указывает массив CLSIDs.  <br/> |
|Валюта  <br/> |Указывает значение валюты.  <br/> |
|CurrencyArray  <br/> |Указывает массив значений валюты.  <br/> |
|Двойное с плавающей точкой  <br/> |Указывает двойной **.**  <br/> |
|DoubleArray  <br/> |Указывает массив **двойных** значений.  <br/> |
|Error  <br/> |Указывает на ошибку. Это предназначено для отчетности об ошибках. Он не может использоваться в ограничениях или для получения или настройки значений.  <br/> |
|С плавающей запятой  <br/> |Указывает **поплавок**.  <br/> |
|FloatArray  <br/> |Указывает массив значений **float.**  <br/> |
|Целое число  <br/> |Указывает на многоугольник.  <br/> |
|IntegerArray  <br/> |Указывает массив наборов.  <br/> |
|Длинное целое  <br/> |Указывает **длинную**.  <br/> |
|LongArray  <br/> |Указывает массив **длинных** значений.  <br/> |
|Null  <br/> |Указывает значение null. Это предназначено для отчетности об ошибках. Он не может использоваться в ограничениях или для получения или настройки значений.  <br/> |
|Объект  <br/> |Указывает объект. Это предназначено для отчетности об ошибках. Он не может использоваться в ограничениях или для получения или настройки значений.  <br/> |
|ObjectArray  <br/> |Указывает массив объектов. Это предназначено для отчетности об ошибках. Он не может использоваться в ограничениях или для получения или настройки значений.  <br/> |
|Short  <br/> |Указывает **краткое**.  <br/> |
|ShortArray  <br/> |Указывает массив **коротких** значений.  <br/> |
|SystemTime  <br/> |Указывает значение времени системы.  <br/> |
|SystemTimeArray  <br/> |Указывает массив значений времени системы.  <br/> |
|String  <br/> |Указывает строку.  <br/> |
|StringArray  <br/> |Указывает массив строк.  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[ExtendedFieldURI](extendedfielduri.md) <br/> |Определяет расширенное свойство MAPI.  <br/> |
   
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

