---
title: ExtendedProperty (PathToExtendedFieldType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: fa620b48-2ce3-437d-b51e-541247eea1d9
description: Элемент ExtendedProperty указывает расширенные свойства для единого хранилища контактов.
ms.openlocfilehash: 7541fa6330ee96f7791febfabc672dbcf0e95b54
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762477"
---
# <a name="extendedproperty-pathtoextendedfieldtype"></a>ExtendedProperty (PathToExtendedFieldType)

Элемент **ExtendedProperty** указывает расширенные свойства для единого хранилища контактов. 
  
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
|DistinguishedPropertySetId  <br/> |Указывает идентификатор набора свойств различающееся. Этот атрибут является необязательным.  <br/> |
|PropertySetId  <br/> |Указывает идентификатор GUID набора свойств. Этот атрибут является необязательным.  <br/> |
|PropertyTag  <br/> | Представляет свойство tag минус введите часть.<br/><br/>Существует два варианта для представления.  <br/><br/>-Шестнадцатеричный: 0x3fa4  <br/>-Знаков после запятой: 0-65535<br/><br/>  Этот атрибут является необязательным.  <br/> |
|PropertyName  <br/> |Строка, указывающая имя свойства. Этот атрибут является необязательным.  <br/> |
|PropertyId  <br/> |Целое число, указывающее идентификатор свойства. Этот атрибут является необязательным.  <br/> |
|PropertyType  <br/> |Указывает тип свойства. Этот атрибут является обязательным.  <br/> |
|FieldURI  <br/> |Указывает поля универсальный код ресурса (URI). Этот атрибут является обязательным. Возможные значения [FieldURI](fielduri.md) см.  <br/> |
   
#### <a name="distinguishedpropertysetid"></a>DistinguishedPropertySetId

|**Значение**|**Описание**|
|:-----|:-----|
|Собрание  <br/> |Указывает собрания.  <br/> |
|Appointment  <br/> |Указывает встречи.  <br/> |
|Common  <br/> |Указывает общий набор свойств.  <br/> |
|PublicStrings  <br/> |Указывает общих строк.  <br/> |
|Address  <br/> |Указывает адрес.  <br/> |
|InternetHeaders  <br/> |Указывает заголовках Интернета.  <br/> |
|CalendarAssistant  <br/> |Указывает, помощник по календарей.  <br/> |
|Единой системы обмена сообщениями  <br/> |Указывает, единой системы обмена сообщениями.  <br/> |
|Задача  <br/> |Означает, что задачи.  <br/> |
   
#### <a name="propertytype"></a>PropertyType

|**Значение**|**Описание**|
|:-----|:-----|
|ApplicationTime  <br/> |Указывает время приложения.  <br/> |
|ApplicationTimeArray  <br/> |Указывает массив времени приложения.  <br/> |
|Binary  <br/> |Указывает двоичное значение.  <br/> |
|BinaryArray  <br/> |Указывает массив двоичных значений.  <br/> |
|Логический  <br/> |Указывает значение типа Boolean.  <br/> |
|CLSID  <br/> |Указывает CLSID.  <br/> |
|CLSIDArray  <br/> |Указывает массив идентификаторов CLSID.  <br/> |
|Денежный  <br/> |Указывает значение типа currency.  <br/> |
|CurrencyArray  <br/> |Указывает массив значений валюты.  <br/> |
|Double  <br/> |Указывает значение **типа double**.  <br/> |
|DoubleArray  <br/> |Указывает массив значений **двойной точности** .  <br/> |
|Ошибка  <br/> |Отображается сообщение об ошибке. Это исключительно в целях создания отчетов об ошибках. Он не может использоваться в ограничения или для получения и установки значений.  <br/> |
|Float  <br/> |Указывает **число с плавающей запятой**.  <br/> |
|FloatArray  <br/> |Указывает массив значений **с плавающей запятой** .  <br/> |
|Целое число  <br/> |Указывает целое число.  <br/> |
|IntegerArray  <br/> |Указывает массив целых чисел.  <br/> |
|Длинный  <br/> |Указывает значение типа **long**.  <br/> |
|LongArray  <br/> |Указывает массив значений **времени** .  <br/> |
|Null  <br/> |Указывает значение null. Это исключительно в целях создания отчетов об ошибках. Он не может использоваться в ограничения или для получения и установки значений.  <br/> |
|Объект  <br/> |Указывает объект. Это исключительно в целях создания отчетов об ошибках. Он не может использоваться в ограничения или для получения и установки значений.  <br/> |
|ObjectArray  <br/> |Указывает массив объектов. Это исключительно в целях создания отчетов об ошибках. Он не может использоваться в ограничения или для получения и установки значений.  <br/> |
|Короткие  <br/> |Указывает, **короткий**.  <br/> |
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
|[ExtendedFieldURI](extendedfielduri.md) <br/> |Идентифицирует расширенных свойств MAPI.  <br/> |
   
## <a name="remarks"></a>Замечания

Этот элемент появился в Exchange Server 2013.
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема типа  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> ||
   
## <a name="see-also"></a>См. также

- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

