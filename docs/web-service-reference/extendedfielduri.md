---
title: ExtendedFieldURI
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- ExtendedFieldURI
api_type:
- schema
ms.assetid: b3c6ea3a-9ead-44b9-9d99-64ecf12bde23
description: Элемент ExtendedFieldURI определяет расширенное свойство MAPI.
ms.openlocfilehash: 0cf3926c900e1b1f35018c6706cfe99ebefbe76f
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59542318"
---
# <a name="extendedfielduri"></a>ExtendedFieldURI

Элемент **ExtendedFieldURI** определяет расширенное свойство MAPI. 
  
```xml
<ExtendedFieldURI DistinguishedPropertySetId="" PropertySetId="" PropertyTag="" PropertyName="" PropertyId="" PropertyType="" />
```

**PathToExtendedFieldType**

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|**DistinguishedPropertySetId** <br/> |Определяет известные ИД набора свойств для расширенных свойств MAPI.<br/><br/>Если этот атрибут используется, нельзя использовать **атрибуты PropertySetId** и **PropertyTag.** Этот атрибут должен использоваться как с **атрибутом PropertyId** или **PropertyName,** так и с **атрибутом PropertyType.**<br/><br/>Таблица **Атрибута DistinguishedPropertySetId,** далее в этой теме, перечисляет возможные значения для этого атрибута.<br/><br/>Этот атрибут является необязательным.  <br/> |
|**PropertySetId** <br/> |Определяет расширенный набор свойств MAPI или пространство имен по его идентификации GUID.<br/><br/>Если этот атрибут используется, нельзя использовать **атрибут DistinguishedPropertySetId** и **PropertyTag.** Этот атрибут должен использоваться как с **атрибутом PropertyId** или **PropertyName,** так и с **атрибутом PropertyType.**<br/><br/>Этот атрибут является необязательным.  <br/> |
|**PropertyTag** <br/> |Определяет тег свойства без типовой части тега. **PropertyTag** может быть представлен как hexadecimal или короткий integer.<br/><br/>Диапазон между 0x8000 и 0xFFFE представляет настраиваемый диапазон свойств. Когда база данных почтовых ящиков впервые сталкивается с настраиваемой собственностью, она назначает этому пользовательскому свойству тег свойства в пользовательском диапазоне свойств 0x8000-0xFFFE. Данный пользовательский тег свойства, скорее всего, будет отличаться между базами данных. Поэтому настраиваемый запрос свойства тегом свойств может возвращать различные свойства в различных базах данных. Использование атрибута **PropertyTag** запрещено для настраиваемого свойства. Вместо этого используйте атрибут **PropertySetId** и **атрибут PropertyName** или **PropertyId.**<br/><br/>**ВАЖНО:** Доступ к любому настраиваемом свойству между 0x8000 и 0xFFFE с помощью GUID + name/ID. Если используется **атрибут PropertyTag,** нельзя использовать **атрибуты DistinguishedPropertySetId,** **PropertySetId,** **PropertyName** и **PropertyId.**<br/><br/>Этот атрибут является необязательным.<br/><br/>**ПРИМЕЧАНИЕ.** Атрибут тега свойства нельзя использовать для свойств в настраиваемом диапазоне 0x8000-0xFFFE. В этом случае необходимо использовать имя свойства.           |
|**PropertyName** <br/> |Определяет расширенное свойство по его имени. Это свойство должно быть соедино либо **DistinguishedPropertySetId,** либо **PropertySetId.**<br/><br/>Если этот атрибут используется, нельзя использовать атрибуты **PropertyId** и **PropertyTag.**<br/><br/>Этот атрибут является необязательным.  <br/> |
|**PropertyId** <br/> |Определяет расширенное свойство по его идентификатору отправки. ID отправки можно определить в десятичных или гексадецимальных форматах. Это свойство должно быть соедино либо **DistinguishedPropertySetId,** либо **PropertySetId.**<br/><br/>Если этот атрибут используется, нельзя использовать **атрибуты PropertyName** и **PropertyTag.**<br/><br/>Этот атрибут является необязательным.  <br/> |
|**PropertyType** <br/> |Представляет тип свойства тега свойств. Это соответствует наименее значимому слову в теге свойств.<br/><br/>Таблица атрибута PropertyType, далее в этом разделе, содержит возможные значения для этого атрибута.<br/><br/>Этот атрибут является обязательным.  <br/> |
   
#### <a name="distinguishedpropertysetid-attribute"></a>Атрибут DistinguishedPropertySetId

|**Значение**|**Описание**|
|:-----|:-----|
|Адрес  <br/> |Определяет идентификатор свойства адреса по имени.  <br/> |
|Appointment  <br/> |Определяет идентификатор свойства назначения по имени.  <br/> |
|CalendarAssistant  <br/> |Определяет идентификатор набора свойств помощника календаря по имени.  <br/> |
|Распространенная  <br/> |Определяет идентификатор общего набора свойств по имени.  <br/> |
|InternetHeaders  <br/> |Определяет идентификатор свойства задатки свойств internet headers по имени.  <br/> |
|Собрание  <br/> |Определяет идентификатор свойства собрания по имени.  <br/> |
|Доступ  <br/> | <br/> |
|PublicStrings  <br/> |Определяет идентификатор свойства общедоступных строк по имени.  <br/> |
|Задача  <br/> |Определяет идентификатор свойства задачи по имени.  <br/> |
|UnifiedMessaging  <br/> |Определяет идентификатор свойства единой системы обмена сообщениями по имени.  <br/> |
   
#### <a name="propertytype-attribute"></a>Атрибут PropertyType

|**Значение**|**Описание**|
|:-----|:-----|
|ApplicationTime  <br/> |Двойное значение, которое интерпретируется как дата и время. Часть в составе — это дата, а часть — время.  <br/> |
|ApplicationTimeArray  <br/> |Массив двойных значений, интерпретируется как дата и время.  <br/> |
|В двоичном формате  <br/> |Двоичное значение с кодом Base64.  <br/> |
|BinaryArray  <br/> |Массив двоичных значений с кодом Base64.  <br/> |
|Логический  <br/> |A Boolean **true** or **false**.  <br/> |
|CLSID  <br/> |Строка GUID.  <br/> |
|CLSIDArray  <br/> |Массив строк GUID.  <br/> |
|Валюта  <br/> |64-bit integer, который интерпретируется как количество центов.  <br/> |
|CurrencyArray  <br/> |Массив из 64-битных integers, которые интерпретируются как количество центов.  <br/> |
|Двойное с плавающей точкой  <br/> |64-битное значение плавающей точки.  <br/> |
|DoubleArray  <br/> |Массив 64-битных значений плавающей точки.  <br/> |
|Error  <br/> |Значение SCODE; 32-bit unsigned integer.  <br/> Не используется для ограничений или для получения/настройки значений. Это существует только для отчетов.  <br/> |
|С плавающей запятой  <br/> |32-битное значение плавающей точки.  <br/> |
|FloatArray  <br/> |Массив 32-битных значений плавающей точки.  <br/> |
|Целое число  <br/> |Подписанный 32-битный (Int32) integer.  <br/> |
|IntegerArray  <br/> |Массив подписанных 32-битных (Int32) наборов.  <br/> |
|Длинное целое  <br/> |Подписанный или неподписаный 64-битный (Int64) integer.  <br/> |
|LongArray  <br/> |Массив подписанных или неподписаных 64-битных (Int64) наборов.  <br/> |
|Null  <br/> |Указывает отсутствие значения свойства.  <br/> Не используется для ограничений или для получения/настройки значений. Это существует только для отчетов.  <br/> |
|Объект  <br/> |Указатель на объект, реализуя интерфейс IUnknown.  <br/> Не используется для ограничений или для получения/настройки значений. Это существует только для отчетов.  <br/> |
|ObjectArray  <br/> |Массив указателей объектов, реализующих интерфейс IUnknown.  <br/> Не используется для ограничений или для получения/настройки значений. Это существует только для отчетов.  <br/> |
|Short  <br/> |Подписанный 16-битный integer.  <br/> |
|ShortArray  <br/> |Массив подписанных 16-битных наборов.  <br/> |
|SystemTime  <br/> |64-битные данные и значение времени в виде структуры FILETIME.  <br/> |
|SystemTimeArray  <br/> |Массив 64-битных данных и значений времени в виде структуры FILETIME.  <br/> |
|String  <br/> |Строка Unicode.  <br/> |
|StringArray  <br/> |Массив строк Юникод.  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[ExtendedProperty](extendedproperty.md) <br/> |Определяет расширенные свойства папок и элементов.  <br/> |
|[AdditionalProperties](additionalproperties.md) <br/> | Определяет дополнительные свойства.<br/><br/>Ниже приводится выражение XPath к этому элементу:<br/><br/>`/FindFolder/FolderShape/AdditionalProperties` <br/>  `/GetFolder/FolderShape/AdditionalProperties` <br/>  `/SyncFolderHierarchy/FolderShape/AdditionalProperties` <br/>  `/GetItem/ItemShape/AdditionalProperties` <br/>  `/FindItem/ItemShape/AdditionalProperties` <br/>  `/SyncFolderItems/ItemShape/AdditionalProperties` <br/>  `/GetAttachment/AttachmentShape/AdditionalProperties` <br/> |
|[SetItemField](setitemfield.md) <br/> |Представляет обновление одного свойства элемента в операции [UpdateItem.](updateitem-operation.md)  <br/> |
|[SetFolderField](setfolderfield.md) <br/> |Представляет обновление одного свойства в папке в операции [UpdateFolder.](updatefolder-operation.md)  <br/> |
|[DeleteItemField](deleteitemfield.md) <br/> |Представляет операцию удаления данного свойства из элемента во время операции [UpdateItem.](updateitem-operation.md)  <br/> |
|[DeleteFolderField](deletefolderfield.md) <br/> |Представляет операцию удаления для удаления заданного свойства из папки во время вызова UpdateFolder.  <br/> |
|[AppendToItemField](appendtoitemfield.md) <br/> |Определяет данные для приложения к одному свойству элемента во время операции [UpdateItem.](updateitem-operation.md)  <br/> |
|[AppendToFolderField](appendtofolderfield.md) <br/> |Указывает данные для приложения к свойству папки во время операции [UpdateFolder.](updatefolder-operation.md)  <br/> |
|[Exists](exists.md) <br/> |Представляет выражение поиска, которое возвращается **верно,** если предоставленное свойство существует на элементе.  <br/> |
|[FieldURIOrConstant](fielduriorconstant.md) <br/> |Представляет свойство или постоянное значение, используемого при сравнении с другим свойством.  <br/> |
|[IsEqualTo](isequalto.md) <br/> |Представляет выражение поиска, которое сравнивает свойство с постоянным значением или другим свойством и оценивает значение **true,** если они равны.  <br/> |
|[IsGreaterThan](isgreaterthan.md) <br/> |Представляет выражение поиска, которое сравнивает свойство с постоянным значением или другим свойством и возвращает значение **true,** если первое свойство больше.  <br/> |
|[IsGreaterThanOrEqualTo](isgreaterthanorequalto.md) <br/> |Представляет выражение поиска, которое сравнивает свойство с постоянным значением  или другим свойством и возвращает значение true, если первое свойство больше или равно второму.  <br/> |
|[IsLessThan](islessthan.md) <br/> |Представляет выражение поиска, которое сравнивает свойство с постоянным значением  или другим свойством и возвращает значение true, если первое свойство меньше второго.  <br/> |
|[IsLessThanOrEqualTo](islessthanorequalto.md) <br/> |Представляет выражение поиска, которое сравнивает свойство с постоянным значением  или другим свойством и возвращает значение true, если первое свойство меньше второго.  <br/> |
|[IsNotEqualTo](isnotequalto.md) <br/> |Представляет выражение поиска, которое сравнивает свойство с постоянным значением  или другим свойством и возвращает значение true, если значения не одинаковы.  <br/> |
|[Исключает](excludes.md) <br/> |Выполняет немного более ровную маску свойств.  <br/> |
|[Contains](contains.md) <br/> |Представляет выражение поиска, которое определяет, содержит ли заданное свойство постоянное значение строки.  <br/> |
|[FieldOrder](fieldorder.md) <br/> |Представляет одно поле для сортировки результатов и указывает направление для сортировки.  <br/> |
   
## <a name="remarks"></a>Заметки

Некоторые атрибуты нельзя использовать в сочетании с другими атрибутами. Любой запрос, который поступает с недействительным сочетанием атрибутов расширенного свойства, создает сообщение об ошибке.
  
Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.
  
> [!NOTE]
> В Microsoft .NET long — это 64-битный подписанный ряд, в то время как в MAPI и COM Long — это 32-битный ряд. Большинство разработчиков будут использовать Microsoft.NET Framework для разработки Exchange веб-служб. Поэтому вместо именования MAPI используется имя .NET.
> 
> Например, свойство PR_MESSAGE_FLAGS MAPI, 0x0E07, является типом PT \_ LONG. В .NET это считается многоугольным. Расширенное свойство для PR_MESSAGE_FLAGS определяется как `<t:ExtendedFieldURI PropertyTag="0x0E07" PropertyType="Integer"/>` . 
  
## <a name="example"></a>Пример

В следующем примере запроса создается элемент, который имеет два настраиваемого свойства. Первое настраиваемая свойство **называется IsMyHouse** с значением Boolean, заданным **значением true.** Второе пользовательское расширенное свойство **называется HousePrices**. Он содержит массив значений валюты. 
  
```XML
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <CreateItem xmlns="https://schemas.microsoft.com/exchange/services/2006/messages" 
                  xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
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
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [FieldURI](fielduri.md)
- [IndexedFieldURI](indexedfielduri.md)
- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

