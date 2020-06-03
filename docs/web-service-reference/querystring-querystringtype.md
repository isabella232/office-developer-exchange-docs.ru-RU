---
title: Строка запроса (Куеристрингтипе)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
api_name:
- QueryString
api_type:
- schema
ms.assetid: cadbf9a5-b87e-4d7f-b488-b76fb0ee7150
description: Элемент QueryString содержит строку запроса к почтовому ящику на основе расширенного синтаксиса запросов (AQS).
localization_priority: Priority
ms.openlocfilehash: eafbbab6de8d191197fb4b80e2b8e3cea80ab800
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459190"
---
# <a name="querystring-querystringtype"></a>Строка запроса (Куеристрингтипе)

Элемент **QueryString** содержит строку запроса к почтовому ящику на основе расширенного синтаксиса запросов (AQS). 
  
```XML
<QueryString/>
```

 **куеристрингтипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|ресеткаче  <br/> |Указывает, что необходимо сбросить кэш.  <br/> |
|ретурнделетедитемс  <br/> |Указывает, что необходимо возвратить удаленные элементы.  <br/> |
|ретурнхигхлигхттермс  <br/> |Указывает, что выделенные термины должны быть возвращены.  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

Отсутствуют.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[FindItem](finditem.md) <br/> |Определяет запрос на поиск элементов в почтовом ящике.  <br/> Ниже приведено выражение XPath для этого элемента:/Финдитем.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение элемента **QueryString** представляет запрос к почтовому ящику, который выполняется с помощью подмножества [расширенного синтаксиса запросов (AQS)](https://msdn.microsoft.com/library/aa965711%28VS.85%29.aspx). В разделе "Примечания" представлены сведения о поддерживаемых параметрах синтаксиса для строк запросов.
  
## <a name="remarks"></a>Примечания

В Exchange Server 2010 этот элемент относится к типу string схемы XML. В версиях Exchange, начиная с Exchange Server 2013, включая Exchange Online, типом для этого элемента является **куеристрингтипе**. Это изменение не нарушает существующие клиенты, так как добавляет три новых дополнительных атрибута. 
  
Элемент **QueryString** исключает использование ограничений EWS. AQS в EWS поддерживает три типа ограничений: ограничение этапа Word, ограничение диапазона дат и ограничение типов сообщений. В следующих таблицах перечислены поддерживаемые свойства поиска для каждого типа ограничения. 
  
**Ограничение для этапов Word**

|**Свойство**|**Пример**|**Function**|
|:-----|:-----|:-----|
|from  <br/> |От: Деан  <br/> From: "Деан Халстеад"  <br/> |Поиск элементов, отправленных из Деан.  <br/> Элементы поиска, отправленные из Деан Халстеад. Отправитель должен быть в точности "Деан Халстеад".  <br/> |
|на  <br/> |Кому: Деан  <br/> |Поиск элементов, отправленных в Деан.  <br/> |
|копия;  <br/> |CC: Деан  <br/> |Поиск элементов с Деан в строке "копия".  <br/> |
|СК.  <br/> |СК: Деан  <br/> |Поиск элементов с Деан в строке "Скрытая копия".  <br/> |
|Participants  <br/> |Участники: Деан  <br/> |Поиск элементов с Деан в полях "Кому", "копия" или "Скрытая копия".  <br/> |
|Subject  <br/> |Тема: Product  <br/> Тема: (разработка продукта)  <br/> Тема: "Разработка продуктов"  <br/> |Поиск элементов с товаром в теме.  <br/> Поиск элементов с продуктом и разработкой в теме.  <br/> |
|Основной текст  <br/> Контент  <br/> |Основной текст: ход выполнения  <br/> Контент: ход выполнения  <br/> |Поиск элементов с ходом выполнения в теле.  <br/> |
|Вложение  <br/> |Вложение: отчет  <br/> |Поиск элементов с отчетом в имени файла вложения или в его тексте.  <br/> |
|(свойство не задано)  <br/> |Разработка продукта  <br/> |Поиск элементов, которые содержат как продукты, так и разработку во всех свойствах этапа слов.  <br/> |
   
Сравнение ограничений для этапа Word всегда не учитывает регистр. Ограничение на этап Word поддерживает два типа совпадений: совпадение префиксов или точное совпадение. Префикс "ПОИСКПОЗ" является поведением по умолчанию. Если требуется точное совпадение, используйте двойные кавычки. Например, Subject: "продукт" соответствует "продукту", но не "производству" в теме. Несколько слов в двойных кавычках ограничивают оба этапа и порядок слов. Например, "Win Product" соответствует только "Win Product", а не "Win95 Product" или "Product of Win". Можно использовать звездочку ( \* ), чтобы определить префикс с ограничением порядка. Например, "Win Product" \* соответствует "Win95 Product", "Windows Production Line", но не "Windows New Product" или "Product of Win". Можно выполнять поиск по всем сообщениям, отправляемым с домена или в домен. Например, from: "@hotmail. com" возвращает все сообщения, отправленные из hotmail.com.
  
В следующей таблице описываются ограничения диапазона дат.
  
**Ограничение диапазона дат**

|**Свойство**|**Пример**|**Function**|
|:-----|:-----|:-----|
|Sent  <br/> |Отправлено: на прошлой неделе  <br/> Отправлено: 01/01/2001  <br/> Отправлено: 01/01/2001.. 01/15/2001  <br/> |Поиск элементов, отправленных за последнюю неделю.  <br/> Поиск элементов, отправленных на 1 января 2001.  <br/> Поиск элементов, отправленных между 1 января по 2001 и 15 января 2001.  <br/> |
|ПОЛУЧЕНО  <br/> |Получено: сегодня  <br/> Получено: 01/01/2001  <br/> |Элементы поиска, полученные сегодня.  <br/> Элементы поиска, полученные 1 января 2001 г.  <br/> |
   
Две точки (..) — это оператор диапазона. Его можно использовать для определения диапазона с начальной и конечной датами. Чтобы указать дату, можно использовать относительные даты. Поддерживаются следующие относительные даты:
  
- Относительные даты: сегодня, завтра, вчера
    
- Относительные даты для нескольких слов: Эта неделя, следующий месяц, последняя неделя, последний месяц или следующий год
    
- Дни: воскресенье, понедельник, вторник, среда, четверг, пятница, Суббота
    
- Январь, Февраль, Март, Апрель, Май, Июнь, Июль, Август, Сентябрь, Октябрь, Ноябрь, Декабрь
    
В следующей таблице описываются ограничения на типы сообщений. 
  
**Ограничение на тип сообщения**

|**Свойство**|**Пример**|**Function**|
|:-----|:-----|:-----|
|Kind  <br/> |Вид: задачи  <br/> |Поиск во всех элементах задач.  <br/> |
   
AQS в EWS использует свойство **Kind** , чтобы указать тип сообщения. Свойство Kind можно использовать со следующими типами элементов: 
  
- email
    
- meetings
    
- tasks
    
- notes
    
- docs
    
- journals
    
- contacts
    
- im
    
В следующей таблице описываются логические соединители группировки.
  
**Группировка логических соединителей**

|**Connector**|**Пример**|**Function**|
|:-----|:-----|:-----|
|И  <br/> |Тема: продукт и Тема: Разработка  <br/> Тема: (продукт и разработка)  <br/> Тема: (разработка продукта)  <br/> |Поиск элементов в теме с помощью продукта и разработки.  <br/> |
|OR  <br/> |Текст: проект или текст: предложение  <br/> Основной текст: (проект или предложение)  <br/> |Поиск элементов с помощью продукта или разработки в теле.  <br/> |
|NOT  <br/> |НЕТ текста: предложение  <br/> Основной текст: (нет предложения)  <br/> |Поиск в сообщениях без предложения в теле.  <br/> |
   
И всегда является соединителем по умолчанию. Например, Subject: Subject: Project и Body: предложение равно "subject": "Body": предложение. Логические соединители чувствительны к регистру. Например, body: (проект или предложение) выполняет поиск в сообщениях с помощью "проект", "или" и "предложение" в тексте, а не "проект" или "предложение". Символ "плюс" (+) эквивалентен и. Символ дефиса (-) эквивалентен параметру NOT. Например, body: (проект-предложение) выполняет поиск в сообщениях с "Project", но без предложения "предложение" в теле. 
  
Строка запроса также может содержать неиндексированные свойства для поиска. Если строка запроса содержит неиндексированные свойства, поиск может выполнить поиск Exchange по индексированным свойствам и поиск хранилища для неиндексированных свойств. 
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="example"></a>Пример

В приведенном ниже примере показан запрос на поиск сообщений в папке "Входящие" с автообнаружением в теме.
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
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

В следующем примере показан успешный ответ на запрос.
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="14" 
                         MinorVersion="0" 
                         MajorBuildNumber="639" 
                         MinorBuildNumber="20" 
                         Version="Exchange2010" 
                         xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:FindItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                        xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
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
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция FindItem](finditem-operation.md)
  
[Операция FindConversation](findconversation-operation.md)


- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

