---
title: Строка запроса (QueryStringType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- QueryString
api_type:
- schema
ms.assetid: cadbf9a5-b87e-4d7f-b488-b76fb0ee7150
description: Элемент строки запроса содержит строку запроса почтовых ящиков на основе на расширенный синтаксис запроса (AQS).
ms.openlocfilehash: 410405638b3f8628dc589049873cfea1f153310c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19834943"
---
# <a name="querystring-querystringtype"></a>Строка запроса (QueryStringType)

Элемент **строки запроса** содержит строку запроса почтовых ящиков на основе на расширенный синтаксис запроса (AQS). 
  
```XML
<QueryString/>
```

 **QueryStringType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|ResetCache  <br/> |Указывает, что необходимо очистить кэш.  <br/> |
|ReturnDeletedItems  <br/> |Указывает, что должны быть возвращены "Удаленные".  <br/> |
|ReturnHighlightTerms  <br/> |Указывает, что выделенный терминов должны быть возвращены.  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[FindItem](finditem.md) <br/> |Определяет запрос для поиска элементов в почтовом ящике.  <br/> Ниже приведен выражение XPath для этого элемента: /FindItem.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение **строки запроса** элемент представляет почтового ящика запросы, выполненные с помощью подмножество [Расширенного синтаксиса запроса (AQS)](http://msdn.microsoft.com/en-us/library/aa965711%28VS.85%29.aspx). Сведения о поддерживаемых синтаксис параметров строки запроса см.
  
## <a name="remarks"></a>Замечания

В Exchange Server 2010 этот элемент относится к типу string схемы XML. В версиях Exchange, начиная с Exchange Server 2013 включая Exchange Online тип для этого элемента — **QueryStringType**. Это изменение не нарушает все существующие клиенты, так как трех новых необязательные атрибуты. 
  
Элемент **строки запроса** исключает использование ограничения веб-служб Exchange. AQS в веб-служб Exchange поддерживает три типа ограничений: этап ограничения, ограничение диапазон даты и ограничения типа сообщения word. В следующей таблице перечислены поддерживаемые поиска свойств для каждого типа ограничений. 
  
**Ограничение этап Word**

|**Свойство**|**Пример**|**�������**|
|:-----|:-----|:-----|
|from  <br/> |От: Дин  <br/> От: «Дин Halstead»  <br/> |Поиск элементов, отправляемых с Дин.  <br/> Поиск элементов, отправляемых с Halstead Дин. Отправитель должен быть точно «Дин Halstead».  <br/> |
|to  <br/> |Чтобы: Дин  <br/> |Поиск элементов, отправленных Дин.  <br/> |
|cc  <br/> |Cc:Dean  <br/> |Поиск элементов с Дин в строке копия.  <br/> |
|bcc  <br/> |BCC:Dean  <br/> |Поиск элементов с Дин строки Скрытая копия.  <br/> |
|Участники  <br/> |Участники: Дин  <br/> |Поиск элементов с Дин Кому, копия или Скрытая копия поля.  <br/> |
|Subject  <br/> |Тема: продукта  <br/> Тема:(product development)  <br/> Тема: «разработка продукта»  <br/> |Поиск элементов с продукта в теме сообщения.  <br/> Поиск элементов с помощью продуктов и разработки в теме сообщения.  <br/> |
|Body  <br/> Контент  <br/> |BODY: хода выполнения  <br/> Содержимое: хода выполнения  <br/> |Поиск элементов с о ходе выполнения в тексте запроса.  <br/> |
|Attachment  <br/> |Вложения: отчет  <br/> |Поиск элементов с отчета в теле имя или файл файл вложения.  <br/> |
|(свойство не указан)  <br/> |Разработка продукта  <br/> |Поиск элементов, которые содержат продукта и разработки решений в все свойства этап word.  <br/> |
   
Этап ограничение соответствие всегда без учета регистра. Ограничение этап Word поддерживает два типа соответствия: префикс или точное соответствие. Соответствие префикса — это поведение по умолчанию совпадение. Если вы хотите точное совпадение, используйте двойные кавычки. Например, тема: «продукт» соответствует «продукт», но не «производственной» в теме сообщения. Несколько слов в двойные кавычки ограничить этапов word и их порядок. Для примера «win продукта» соответствует только «win продукт», не «win95 продукт» или «продукт win». Можно использовать символ звездочки (\*) для определения соответствие префикса с порядком ограниченного доступа. Например, «win продукта»\* соответствует «win95 продукт», «строка рабочей windows», но не «новый продукт windows» или «продукт win». Можно выполнить поиск всех сообщений, отправляемых из или в домен. Например, from:"@hotmail.com» возвращает все сообщения, отправляемые hotmail.com.
  
В следующей таблице описаны ограничения диапазона дат.
  
**Ограничение диапазона дат**

|**Свойство**|**Пример**|**�������**|
|:-----|:-----|:-----|
|Sent  <br/> |Отправлено: прошлую неделю  <br/> Отправлено: 01/01/2001 г.  <br/> Sent:01/01/2001..01/15/2001  <br/> |Поиск элементов, отправленных прошлую неделю.  <br/> Поиск элементов, переданного по 1-го января 2001 года.  <br/> Поиск элементов, передаваемых между 1 января 2001 года и 15 января 2001 года.  <br/> |
|Получено  <br/> |Получено: сегодня  <br/> Получено: 01/01/2001 г.  <br/> |Поиск элементов, полученных сегодня.  <br/> Поиск элементов, полученного по 1-го января 2001 года.  <br/> |
   
Две точки (.) — это оператор диапазона. Используется для определения диапазона с начала и Дата окончания. Чтобы указать дату, можно использовать относительные даты. Поддерживаются следующие относительные даты:
  
- Относительные даты: сегодня, завтра, за вчерашний день
    
- Multiword относительные даты: этой неделе следующего месяца, последнюю неделю за месяц или следующий год
    
- Дней: Воскресенье, понедельник, Вторник, среда, четверг, пятница, суббота
    
- Январь, февраль, март, апрель, возможно, июня, июля, августа, сентябрь, октябрь, ноябрь, декабрь
    
В следующей таблице описаны ограничения типов сообщений. 
  
**Ограничение типа сообщения**

|**Свойство**|**Пример**|**�������**|
|:-----|:-----|:-----|
|Тип  <br/> |Тип: задачи  <br/> |Поиск во всех элементах задач.  <br/> |
   
AQS в веб-свойство **типа** используется для указания типа сообщения. Тип свойства можно с помощью следующих типов элементов: 
  
- email
    
- собрания
    
- tasks
    
- notes
    
- документы
    
- журналы.
    
- contacts
    
- обмен мгновенными сообщениями
    
В следующей таблице описываются группировки логической соединители.
  
**Соединители логической группировки**

|**Соединитель**|**Пример**|**�������**|
|:-----|:-----|:-----|
|AND  <br/> |Тема: продукта и Тема: Разработка  <br/> Тема:(product AND development)  <br/> Тема:(product development)  <br/> |Поиск элементов с помощью продуктов и разработки в теме сообщения.  <br/> |
|OR  <br/> |BODY: проекта или тело: предложения  <br/> BODY:(project OR proposal)  <br/> |Поиск элементов с продуктом или разработки в тексте запроса.  <br/> |
|NOT  <br/> |Body: предложения  <br/> :(NOT proposal) текста  <br/> |Поиск в тексте сообщения без предложения.  <br/> |
   
Всегда и соединитель по умолчанию. Тема: проекта и тело: предложения совпадает с body: предложения Тема: проекта. Логическая соединители чувствительны к регистру. Например, body:(project Or proposal) выполняет поиск сообщений с «project», «или» и «предложения» в теле вместо «project» или «предложения». Знак плюса (+) является эквивалентом AND. НЕ эквивалентно символ дефиса (-). Например, body:(project-proposal) выполняет поиск сообщений с «project», но без «предложения» в тексте запроса. 
  
Строка запроса также может содержать неиндексируемых свойств для поиска. Если строка запроса содержит неиндексируемых свойств, поиска может выполнить поиск Exchange на индексированные свойства и поиска хранилища на неиндексируемых свойств. 
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="example"></a>Пример

В следующем примере показано запрос на поиск сообщений в папке "Входящие" с помощью службы автообнаружения в теме сообщения.
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2010" />
  </soap:Header>
  <soap:Body>
    <m:FindItem Traversal="Shallow">
      <m:ItemShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="item:Subject" />
        </t:AdditionalProperties>
      </m:ItemShape>
      <m:IndexedPageItemView MaxEntriesReturned="1" Offset="0" BasePoint="Beginning" />
      <m:ParentFolderIds>
        <t:DistinguishedFolderId Id="inbox" />
      </m:ParentFolderIds>
      <m:QueryString>subject:Autodiscover</m:QueryString>
    </m:FindItem>
  </soap:Body>
</soap:Envelope>
```

В следующем примере показано успешного ответа на запрос.
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="14" 
                         MinorVersion="0" 
                         MajorBuildNumber="639" 
                         MinorBuildNumber="20" 
                         Version="Exchange2010" 
                         xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:FindItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                        xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:FindItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:RootFolder IndexedPagingOffset="1" 
                        TotalItemsInView="5" 
                        IncludesLastItemInRange="false">
            <t:Items>
              <t:Message>
                <t:ItemId Id="AAMkADEzOTExYjJkLTYx" ChangeKey="CQAAABY" />
                <t:Subject>How to use Autodiscover</t:Subject>
              </t:Message>
            </t:Items>
          </m:RootFolder>
        </m:FindItemResponseMessage>
      </m:ResponseMessages>
    </m:FindItemResponse>
  </s:Body>
</s:Envelope>

```

## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[FindItem Operation](finditem-operation.md)
  
[FindConversation Operation](findconversation-operation.md)


- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

