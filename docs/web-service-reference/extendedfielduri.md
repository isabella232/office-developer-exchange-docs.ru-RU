---
title: ExtendedFieldURI
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ExtendedFieldURI
api_type:
- schema
ms.assetid: b3c6ea3a-9ead-44b9-9d99-64ecf12bde23
description: Элемент ExtendedFieldURI определяет расширенных свойств MAPI.
ms.openlocfilehash: 50ce46652863b0c534d09d58d4b9f7c8095deef2
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/28/2018
ms.locfileid: "21353793"
---
# <a name="extendedfielduri"></a>ExtendedFieldURI

Элемент **ExtendedFieldURI** определяет расширенных свойств MAPI. 
  
```xml
<ExtendedFieldURI DistinguishedPropertySetId="" PropertySetId="" PropertyTag="" PropertyName="" PropertyId="" PropertyType="" />
```

**PathToExtendedFieldType**

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|**DistinguishedPropertySetId** <br/> |Определяет хорошо известных свойство значение идентификаторов для расширенных свойств MAPI.<br/><br/>Если используется этот атрибут не может использоваться атрибуты **PropertySetId** и **PropertyTag** . Этот атрибут должен использоваться с **PropertyId** , либо **PropertyName** атрибутов и **PropertyType** .<br/><br/>В таблице атрибут **DistinguishedPropertySetId** далее в этом разделе приведены возможные значения этого атрибута.<br/><br/>Этот атрибут является необязательным.  <br/> |
|**PropertySetId** <br/> |Идентифицирует расширенных набор свойств или пространство имен по их идентификатору GUID MAPI.<br/><br/>Если используется этот атрибут не может использоваться атрибут **DistinguishedPropertySetId** и **PropertyTag** . Этот атрибут должен использоваться с **PropertyId** , либо **PropertyName** атрибутов и **PropertyType** .<br/><br/>Этот атрибут является необязательным.  <br/> |
|**PropertyTag** <br/> |Определяет свойство tag без введите часть тега. **PropertyTag** может быть представлена как шестнадцатеричного или короткое целое число.<br/><br/>Диапазон от 0x8000 до 0xFFFE представляет собой настраиваемый диапазон свойств. База данных почтовых ящиков обнаруживает настраиваемого свойства в первый раз, назначает, настраиваемые свойства, тег свойства в диапазоне настраиваемое свойство 0x8000 0xFFFE. Тег указанного настраиваемого свойства вероятнее всего будут отличаться между базами данных. Таким образом запрос настраиваемого свойства, свойство tag можно вернуть различных свойств в разных базах данных. Использование атрибута **PropertyTag** запрещен для настраиваемых свойств. Используйте атрибут **PropertySetId** и атрибута **PropertyName** или **PropertyId** .<br/><br/>**Важно**: доступ к любого настраиваемого свойства от 0x8000 до 0xFFFE с помощью идентификатора GUID + имя или идентификатор. Если используется атрибут **PropertyTag** , не может использоваться атрибуты **DistinguishedPropertySetId**, **PropertySetId**, **PropertyName**и **PropertyId** .<br/><br/>Этот атрибут является необязательным.<br/><br/>**Примечание**: нельзя использовать атрибут тега свойства для свойств настраиваемых диапазона 0x8000 0xFFFE. В этом случае необходимо использовать именованные свойства.           |
|**PropertyName** <br/> |Определяет расширенное свойство по его имени. Это свойство должен быть связан с **DistinguishedPropertySetId** или **PropertySetId**.<br/><br/>Если используется этот атрибут не может использоваться атрибуты **PropertyId** и **PropertyTag** .<br/><br/>Этот атрибут является необязательным.  <br/> |
|**PropertyId** <br/> |Идентифицирует расширенное свойство с идентификатором его отправки. Можно определить идентификатор диспетчеризации в десятичном или шестнадцатеричном форматах. Это свойство должен быть связан с **DistinguishedPropertySetId** или **PropertySetId**.<br/><br/>Если используется этот атрибут не может использоваться атрибуты **PropertyName** и **PropertyTag** .<br/><br/>Этот атрибут является необязательным.  <br/> |
|**PropertyType** <br/> |Представляет тип свойства тега свойства. Это соответствует бы значительные word в теге свойства.<br/><br/>В таблице атрибут PropertyType далее в этом разделе приведены возможные значения этого атрибута.<br/><br/>Этот атрибут является обязательным.  <br/> |
   
#### <a name="distinguishedpropertysetid-attribute"></a>Атрибут DistinguishedPropertySetId

|**Значение**|**Описание**|
|:-----|:-----|
|Собрание  <br/> |Идентифицирует собрания ИД по имени, набора свойств.  <br/> |
|Appointment  <br/> |Определяет идентификатор набора свойств встречи по имени.  <br/> |
|Common  <br/> |Определяет общие идентификатор набора свойств по имени.  <br/> |
|PublicStrings  <br/> |Определяет идентификатор набора свойств общих строк по имени.  <br/> |
|Address  <br/> |Определяет идентификатор набора свойств адреса по имени.  <br/> |
|InternetHeaders  <br/> |Определяет идентификатор set свойства заголовки Интернета по имени.  <br/> |
|CalendarAssistant  <br/> |Определяет идентификатор набора свойств помощник по календаря по имени.  <br/> |
|Единой системы обмена сообщениями  <br/> |Определяет единой системы обмена сообщениями идентификатора набора свойств по имени.  <br/> |
   
#### <a name="propertytype-attribute"></a>Атрибут PropertyType

|**Значение**|**Описание**|
|:-----|:-----|
|ApplicationTime  <br/> |Значение типа double, интерпретируется как дата и время. Целая часть — это дата, а дробная часть — время.  <br/> |
|ApplicationTimeArray  <br/> |Массив значений типа double, которые интерпретируются как дата и время.  <br/> |
|Binary  <br/> |Двоичное значение кодировки Base64.  <br/> |
|BinaryArray  <br/> |Массив двоичных значений в кодировке Base64.  <br/> |
|Логический  <br/> |Логическое **значение true** или **false**.  <br/> |
|CLSID  <br/> |Строка идентификатора GUID.  <br/> |
|CLSIDArray  <br/> |Массив строк GUID.  <br/> |
|Денежный  <br/> |64-разрядное целое число, обрабатывается как количество сотен.  <br/> |
|CurrencyArray  <br/> |Массив 64-разрядных целых чисел, которые интерпретируются как количество сотен.  <br/> |
|Double  <br/> |64-разрядное значение с плавающей запятой.  <br/> |
|DoubleArray  <br/> |Массив значений с плавающей запятой 64-разрядная версия.  <br/> |
|Error  <br/> |Значение SCODE; 32-разрядное целое число без знака.  <br/> Не используется для ограничения или начало параметр значения. Это существует только для создания отчетов.  <br/> |
|Float  <br/> |32-разрядное значение с плавающей запятой.  <br/> |
|FloatArray  <br/> |Массив значений с плавающей запятой 32-разрядная версия.  <br/> |
|Целое число  <br/> |32-разрядная версия (Int32) целого числа со знаком.  <br/> |
|IntegerArray  <br/> |Массив целых 32-разрядная версия (Int32).  <br/> |
|Long  <br/> |Подписанные или неподписанные 64-разрядная версия (Int64) целое число.  <br/> |
|LongArray  <br/> |Массив целых чисел (Int64) 64-разрядная версия знаком или без знака.  <br/> |
|Null  <br/> |Указывает на отсутствие значения свойства.  <br/> Не используется для ограничения или начало параметр значения. Это существует только для создания отчетов.  <br/> |
|Объект  <br/> |Указатель на объект, реализующий интерфейс IUnknown.  <br/> Не используется для ограничения или начало параметр значения. Это существует только для создания отчетов.  <br/> |
|ObjectArray  <br/> |Массив ссылок на объекты, реализующие интерфейс IUnknown.  <br/> Не используется для ограничения или начало параметр значения. Это существует только для создания отчетов.  <br/> |
|Короткие  <br/> |16-разрядного целого числа со знаком.  <br/> |
|ShortArray  <br/> |Массив из 16-разрядной целые числа со знаком.  <br/> |
|SystemTime  <br/> |64-разрядное целое число данных значения и времени в виде структуру FILETIME.  <br/> |
|SystemTimeArray  <br/> |Массив значений 64-разрядное целое число дату и время в формате структуру FILETIME.  <br/> |
|Строка  <br/> |Строка Юникода.  <br/> |
|StringArray  <br/> |Массив строк в кодировке Юникод.  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[ExtendedProperty](extendedproperty.md) <br/> |Определяет расширенные свойства для папок и элементов.  <br/> |
|[AdditionalProperties](additionalproperties.md) <br/> | Определяет дополнительные свойства.<br/><br/>Ниже приведены выражения XPath для этого элемента.<br/><br/>`/FindFolder/FolderShape/AdditionalProperties` <br/>  `/GetFolder/FolderShape/AdditionalProperties` <br/>  `/SyncFolderHierarchy/FolderShape/AdditionalProperties` <br/>  `/GetItem/ItemShape/AdditionalProperties` <br/>  `/FindItem/ItemShape/AdditionalProperties` <br/>  `/SyncFolderItems/ItemShape/AdditionalProperties` <br/>  `/GetAttachment/AttachmentShape/AdditionalProperties` <br/> |
|[SetItemField](setitemfield.md) <br/> |Представляет отдельное свойство элемента в [UpdateItem операции](updateitem-operation.md)обновления.  <br/> |
|[SetFolderField](setfolderfield.md) <br/> |Представляет обновление для одного свойства папки в рамках одной [операции UpdateFolder](updatefolder-operation.md).  <br/> |
|[DeleteItemField](deleteitemfield.md) <br/> |Представляет операцию удаления для удаления заданного свойства из элемента во время [операции UpdateItem](updateitem-operation.md).  <br/> |
|[DeleteFolderField](deletefolderfield.md) <br/> |Представляет операцию удаления для удаления заданного свойства из папки во время вызова UpdateFolder.  <br/> |
|[AppendToItemField](appendtoitemfield.md) <br/> |Указывает данные для добавления к отдельное свойство элемента во время [операции UpdateItem](updateitem-operation.md).  <br/> |
|[AppendToFolderField](appendtofolderfield.md) <br/> |Указывает данные для добавления к папке свойство во время [операции UpdateFolder](updatefolder-operation.md).  <br/> |
|[Exists](exists.md) <br/> |Представляет выражение поиска, которое возвращает **значение true, если существует указанное свойство элемента** .  <br/> |
|[FieldURIOrConstant](fielduriorconstant.md) <br/> |Представляет свойство или постоянное значение для использования при сравнении с другого свойства.  <br/> |
|[IsEqualTo](isequalto.md) <br/> |Представляет выражение поиска, которое сравнивает свойство с постоянным значением или другим свойством и имеет значение **true** , если они равны.  <br/> |
|[IsGreaterThan](isgreaterthan.md) <br/> |Представляет выражение поиска, которое сравнивает свойство с постоянным значением или другим свойством и возвращает **значение true,** Если первое свойство больше.  <br/> |
|[IsGreaterThanOrEqualTo](isgreaterthanorequalto.md) <br/> |Представляет выражение поиска, которое сравнивает свойство с постоянным значением или другим свойством и возвращает **значение true,** Если первое свойство больше или равен ему.  <br/> |
|[IsLessThan](islessthan.md) <br/> |Представляет выражение поиска, которое сравнивает свойство с постоянным значением или другим свойством и возвращает **значение true,** Если первое свойство меньше, чем второй.  <br/> |
|[IsLessThanOrEqualTo](islessthanorequalto.md) <br/> |Представляет выражение поиска, которое сравнивает свойство с постоянным значением или другим свойством и возвращает **значение true,** Если первое свойство меньше, чем второй.  <br/> |
|[IsNotEqualTo](isnotequalto.md) <br/> |Представляет выражение поиска, которое сравнивает свойство с постоянным значением или другим свойством и возвращает **значение true,** Если значения не совпадают.  <br/> |
|[Excludes](excludes.md) <br/> |Выполняет битовую маску свойства.  <br/> |
|[Contains](contains.md) <br/> |Представляет выражение поиска, которое определяет, содержит ли данное свойство указанную константу строчного типа.  <br/> |
|[FieldOrder](fieldorder.md) <br/> |Представляет одно поле, по которому будут отсортированы результаты и задает направление сортировки.  <br/> |
   
## <a name="remarks"></a>Замечания

Некоторые атрибуты нельзя использовать в сочетании с помощью других атрибутов. Все запросы, которая приходит с Недопустимое сочетание атрибутов расширенного свойства создаст сообщение об ошибке.
  
Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.
  
> [!NOTE]
> В Microsoft .NET значение типа Long находится 64-разрядное целое число со знаком, а в MAPI и COM, значение типа Long — это 32-разрядное целое число. Большинство разработчиков будет использовать.NET Framework для разработки веб-служб Exchange клиентских приложений. Таким образом, именование .NET используется вместо MAPI именования.
> 
> Например, свойство PR_MESSAGE_FLAGS MAPI, 0x0E07, будет PT\_ДОЛГО введите. В .NET это считается целое число. Расширенные свойства для PR_MESSAGE_FLAGS определяется как `<t:ExtendedFieldURI PropertyTag="0x0E07" PropertyType="Integer"/>`. 
  
## <a name="example"></a>Пример

В следующем примере запрос создается элемент, который имеет две настраиваемые свойства. Первый настраиваемого свойства с именем **IsMyHouse** со значением логическое значение **true**. Второй дополнительное пользовательское свойство называется **HousePrices**. Он содержит массив значений валюты. 
  
```XML
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <CreateItem xmlns="http://schemas.microsoft.com/exchange/services/2006/messages" 
                  xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
    MessageDisposition="SaveOnly">
      <SavedItemFolderId>
        <t:DistinguishedFolderId Id="inbox"/>
      </SavedItemFolderId>
      <Items>
        <t:Item>
          <t:ItemClass>IPM.Note</t:ItemClass>
          <t:Subject>Create an extended property</t:Subject>
          <t:Body BodyType="Text">Added info to extended props</t:Body>
          <t:ExtendedProperty>
            <t:ExtendedFieldURI DistinguishedPropertySetId="PublicStrings" 
                                PropertyName="IsMyHouse" 
                                PropertyType="Boolean"/>
            <t:Value>true</t:Value>
          </t:ExtendedProperty>
          <t:ExtendedProperty>
            <t:ExtendedFieldURI DistinguishedPropertySetId="PublicStrings" 
                                PropertyName="HousePrices" 
                                PropertyType="CurrencyArray"/>
            <t:Values>
              <t:Value>30000000</t:Value>
              <t:Value>40000000</t:Value>
              <t:Value>50000000</t:Value>
            </t:Values>
          </t:ExtendedProperty>
        </t:Item>
      </Items>
    </CreateItem>
  </soap:Body>
</soap:Envelope>
```

## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [FieldURI](fielduri.md)
- [IndexedFieldURI](indexedfielduri.md)
- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

