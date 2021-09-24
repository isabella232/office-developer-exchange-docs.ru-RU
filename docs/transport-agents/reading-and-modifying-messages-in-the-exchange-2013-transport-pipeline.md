---
title: Чтение и изменение сообщений в конвейере Exchange 2013 г.
manager: sethgros
ms.date: 09/17/2021
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: b53ed47a-3d01-4c4e-ad32-fb0532872aad
description: Узнайте о классах платформа .NET Framework, которые можно использовать в транспортных агентах Exchange 2013 г. для чтения, записи и изменения сообщений.
ms.openlocfilehash: 5bf4406f7ca82512bb55388e0865e0d343cae66e
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59537238"
---
# <a name="reading-and-modifying-messages-in-the-exchange-2013-transport-pipeline"></a>Чтение и изменение сообщений в конвейере Exchange 2013 г.

Узнайте о классах платформа .NET Framework, которые можно использовать в транспортных агентах Exchange 2013 г. для чтения, записи и изменения сообщений.
  
**Применяется к:** Exchange Server 2013 г.
  
- Классы, используемые для чтения, записи или изменения сообщений
- Пространство имен кодаторов
- пространство имен iCalendar
- Пространство имен MIME
- Пространство имен TextConverters
- Пространство имен Tnef
- пространство имен vCard
  
По мере передачи сообщений по транспортному конвейеру транспортный агент может читать, записывать и преобразовывать содержимое сообщений в различных форматах данных. Например, можно читать и записывать данные MIME, определять входящие сообщения, которые находятся в формате Uuencoded или Quoted-printable (qp), а затем преобразовать их в стандарт, используемый вашей организацией, или прочитать, а затем сохранить календарь или контактные данные, связанные с входящие сообщения. 
  
Вы также можете определить содержимое, представляю которое представляет угрозу безопасности, и переместить или удалить содержимое или сообщения, содержащие их; например, путем удаления ссылок в HTML-сообщении.
  
В этой статье приводится информация платформа .NET Framework классов, которые можно использовать для чтения, записи и изменения сообщений.
  
> [!CAUTION]
> Многие свойства и параметры API преобразования контента позволяют иметь достаточно большие значения, чтобы вызвать проблемы с производительностью, включая отказ в обслуживании. При использовании API преобразования контента в транспортном агенте необходимо реализовать ограничения на размеры свойств и параметров, поддерживаемые при чтении или записи, чтобы ограничить потребление ресурсов агентом. 

<a name="Namespaces"> </a>

## <a name="classes-used-to-read-write-or-modify-messages"></a>Классы, используемые для чтения, записи или изменения сообщений

В следующей таблице перечислены платформа .NET Framework классы, которые можно использовать для чтения, записи и изменения сообщений электронной почты.
  
**платформа .NET Framework области имен обработки сообщений**

|**платформа .NET Framework пространства имен**|**занятия**;|
|:-----|:-----|
|[Microsoft. Exchange. Data.Mime.Encoders](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.Encoders.aspx) <br/> |Содержит классы для кодирования и декодирования в памяти, класс потока кодирования, который принимает один из классов кодера или декодера, содержащихся в связанном переумеществе, и базовый класс [ByteEncoder](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.Encoders.ByteEncoder.aspx) и класс исключения [ByteEncoderException](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.Encoders.ByteEncoderException.aspx) для кодеров и декодеров.  <br/> |
|[Microsoft. Exchange. Data.ContentTypes.iCalendar](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.ContentTypes.iCalendar.aspx) <br/> |Содержит типы, позволяющие читать и записывать потоки данных, содержащие сведения о календаре. Включает в себя считыватель календаря и писатель, объект исключения, объект повторяемости, а также структуры и список, которые помогают возвращать сведения о свойствах элементов календаря.  <br/> |
|[Microsoft. Exchange. Data.Mime](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.aspx) <br/> |Содержит классы, структуры, переумывания и делегаты, которые можно использовать для создания, чтения, записи, обхода, кодирования и декодирования данных MIME. Включает в себя потоковый читатель и писатель, который предоставляет доступ к потокам данных MIME только для чтения и записи, а также методы и классы на основе DOM, которые можно использовать в документах MIME.  <br/> |
|[Microsoft. Exchange. Data.TextConverters](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.TextConverters.aspx) <br/> |Содержит классы, структуры, переучеты и делегаты, которые позволяют читать и записывать поток данных и выполнять преобразования между определенными типами данных; например, HTML-формат с богатым текстом (RTF). Текстовые преобразователи позволяют изменять формат потока документов из одной формы в другую, а также выборочно удалять элементы документа, которые могут представлять угрозу безопасности.  <br/> |
|[Microsoft. Exchange. Data.ContentTypes.Tnef](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.ContentTypes.Tnef.aspx) <br/> |Содержит только считыватель и писатель потокового потока, класс исключений, а также структуры и перемеры, которые облегчают чтение и написание данных формата инкапсуляции транспортного нейтрального формата (TNEF).  <br/> |
|[Microsoft. Exchange. Data.ContentTypes.vCard](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.ContentTypes.vCard.aspx) <br/> |Содержит только считыватель и писатель потокового потока, класс исключений, а также структуры и перемеры, облегчающие чтение и написание контактных данных в формате vCard.  <br/> |
   
## <a name="encoders-namespace"></a>Пространство имен кодаторов
<a name="Encoders"> </a>

Пространство имен кодаторов содержит классы для кодирования и декодирования в памяти. Они наследуются базовым классом [ByteEncoder.](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.Encoders.ByteEncoder.aspx) Классы кодируют и декодируют для Base64, BinHex, Quoted-printable (qp) и Unix-to-Unix (Uu). Для кодирования и декодирования в памяти используются следующие классы: 
  
- [Base64Encoder](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.Encoders.Base64Encoder.aspx)
    
- [Base64Decoder](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.Encoders.Base64Decoder.aspx)
    
- [BinHexEncoder](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.Encoders.BinHexEncoder.aspx)
    
- [BinHexDecoder](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.Encoders.BinHexDecoder.aspx)
    
- [QPEncoder](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.Encoders.QPEncoder.aspx)
    
- [QPDecoder](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.Encoders.QPDecoder.aspx)
    
- [UUEncoder](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.Encoders.UUEncoder.aspx)
    
- [UUDecoder](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.Encoders.UUDecoder.aspx)
    
Кодаторы и декодеры наследуют базовый класс [ByteEncoder](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.Encoders.ByteEncoder.aspx) и используют класс исключения [ByteEncoderException](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.Encoders.ByteEncoderException.aspx) для обработки ошибок. 
  
Кроме того, пространство имен содержит класс [MacBinaryHeader,](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.Encoders.MacBinaryHeader.aspx) который идентифицирует закодированные файлы MacBinary и читает связанные с ними заголовок файлов. 
  
Наконец, [класс EncoderStream](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.Encoders.EncoderStream.aspx) выполняет преобразование в потоке данных вместо объекта в памяти. Этот класс принимает один из классов коддера или декодера и читает или пишет согласно связанному переучету [EncoderStreamAccess.](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.Encoders.EncoderStreamAccess.aspx) 
  
## <a name="icalendar-namespace"></a>пространство имен iCalendar
<a name="iCalendar"> </a>

Пространство имен iCalendar предоставляет только для чтения и записи данных iCalendar, а также поддерживает структуры и классы для создания, доступа и изменения потоков iCalendar.
  
Классы [CalendarReader](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.ContentTypes.iCalendar.CalendarReader.aspx) и [CalendarWriter](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.ContentTypes.iCalendar.CalendarWriter.aspx) используются для чтения и записи данных потока iCalendar. 
  
CalendarReader принимает читаемый [поток](https://msdn.microsoft.com/library/System.IO.Stream.aspx) в качестве аргумента для своих конструкторов. Затем можно использовать методы [ReadFirstChildComponent,](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.ContentTypes.iCalendar.CalendarReader.ReadFirstChildComponent.aspx) [ReadNextSiblingComponent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.ContentTypes.iCalendar.CalendarReader.ReadNextSiblingComponent.aspx)и [ReadNextComponent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.ContentTypes.iCalendar.CalendarReader.ReadNextComponent.aspx) для последовательного доступа к компонентам iCalendar в потоке данных. В зависимости от значения, заданного для свойства [ComplianceMode,](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.ContentTypes.iCalendar.CalendarReader.ComplianceMode.aspx) ошибки в потоке iCalendar могут привести к тому, что будет выброшено исключение или свойство [ComplianceStatus](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.ContentTypes.iCalendar.CalendarReader.ComplianceStatus.aspx) будет задано значение, не комплаенсирующее . [](https://msdn.microsoft.com/library/microsoft.exchange.data.contenttypes.icalendar.calendarcompliancestatus.aspx) Вы можете проверить это свойство, чтобы обнаружить любые проблемы с входящие данные iCalendar. 
  
Класс [CalendarWriter](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.ContentTypes.iCalendar.CalendarWriter.aspx) принимает writable [Stream](https://msdn.microsoft.com/library/System.IO.Stream.aspx) в качестве аргумента для своих конструкторов. 
  
## <a name="mime-namespace"></a>Пространство имен MIME
<a name="MIME"> </a>

Пространство имен MIME предоставляет классы, позволяющие создавать, получать доступ и изменять документы MIME. Вы можете работать с документами MIME с помощью метода на основе потока или на основе DOM.
  
### <a name="mimedocument-class-and-the-mime-dom"></a>Класс MimeDocument и DOM MIME

Класс [MimeDocument](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.MimeDocument.aspx) позволяет DOM-доступ к документу MIME. Используйте объекты этого типа, если у вас есть доступная память для загрузки всего DOM, и вы должны иметь случайный доступ к загонам и содержимому сообщения. 
  
Данные загружаются в [объект MimeDocument](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.MimeDocument.aspx) с помощью методов [GetLoadStream](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.MimeDocument.GetLoadStream.aspx) или [Load.](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.MimeDocument.Load.aspx) Затем можно ходить по иерархии DOM и создавать, изменять или удалять данные MIME. После изменения данных MIME их можно записать в поток с помощью одного из методов [WriteTo.](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.MimeNode.WriteTo.aspx) 
  
На следующем рисунке показана структура данных в [объекте MimeDocument.](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.MimeDocument.aspx) 
  
**Рис. 1. Структура объектов MimeDocument**

![Архитектура модели DOM MIME](media/MimeDomArchitecture.gif)
  
### <a name="mimereader-and-mimewriter-classes-and-stream-based-mime-parsing"></a>Классы MimeReader и MimeWriter и разметка MIME на основе потоковой передачи

Классы [MimeReader и](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.MimeReader.aspx) [MimeWriter](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.MimeWriter.aspx) позволяют получать доступ только к потокам MIME. Используйте эти классы, если вам не нужно менять данные MIME, которые требуют данных, которые уже прочитано или записано. Например, если вы хотите распечатать сообщения, подходящие предварительному формату, класс [MimeWriter](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.MimeWriter.aspx) может быть идеальным. 
  
Класс [MimeDocument](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.MimeDocument.aspx) инкапсулирует DOM. Классы [MimeReader и](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.MimeReader.aspx) [MimeWriter](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.MimeWriter.aspx) представляют государственные компьютеры. Их состояния изменяются в зависимости от полученных входных данных и используемых методов. Рисунки от 2 до 5 — это упрощенные схемы перехода состояния, которые показывают объект [MimeReader,](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.MimeReader.aspx) методы которого допустимы для вызова из каждого состояния и состояния, которое приведет к этому. 
  
Чтобы использовать эти схемы, следуйте стрелкам из одного состояния в следующее, заметь, что метод вызывает или возвращает значения, которые вызывают изменение состояния. Например, на первой схеме предположим, что вы находитесь в начале потока, который принадлежит созданному MimeReader. Чтобы добраться до состояния Главы части, в этом порядке вызовите один из [readNextPart](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.MimeReader.ReadNextPart.aspx) или [ReadFirstChildPart.](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.MimeReader.ReadFirstChildPart.aspx) Если есть загонщики (то есть, если MIME хорошо сформирован), введите состояние Заглавные части. В противном случае будет отброшено исключение. 
  
**Рис. 2. Упрощенная схема перехода состояния для объектов MimeReader**

![Схема состояния MimeReader](media/MimeReader_StateDiagram_01.gif)
  
> [!NOTE]
> Цифры 3, 4 и 5 расширяют состояния, показанные на каждой из предыдущих схем. 
  
**Рис. 3. Расширение состояния заглавных окантовок части с рисунка 2**

![Расширенное представление состояния "Заголовки части"](media/MimeReader_StateDiagram_02.gif)
  
**Рис. 4. Расширение состояния Header с рисунка 3 при столкновении параметра в загонах**

![Расширение состояния "Заглавные части" при столкновении параметра в загонах](media/MimeReader_StateDiagram_03.gif)
  
> [!NOTE]
> Состояние, представленное рис. 5, является рекурсивным, так как при столкновении с адресной группой можно использовать свойство [GroupRecipientReader](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.MimeAddressReader.GroupRecipientReader.aspx) для чтения адресов в группе. 
  
**Рис. 5. Расширение состояния Header с рисунка 3 при столкновении с адресом или группой адресов**

![Расширенное представление состояния "Заголовок" для адреса группы](media/MimeReader_StateDiagram_04.gif)
  
На рисунках 6 и 7 покажут упрощенные схемы перехода состояния для [объекта MimeWriter.](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.MimeWriter.aspx) 
  
> [!NOTE]
> На рисунке 7 расширяется состояние заглавов части, показанное на рисунке 6. 
  
**Рис. 6. Упрощенная схема перехода состояния для объектов MimeWriter**

![Схема смены состояния для MimeWriter](media/MimeWriter_TopLevel.gif)
  
**Рис. 7. Расширение состояния заглавных окантовок части с рисунка 6**

![Расширенная схема смены состояния для MimeWriter](media/MimeWriter_Diagram_Expansion.gif)
  
## <a name="textconverters-namespace"></a>Пространство имен TextConverters
<a name="TextConverters"> </a>

Пространство имен TextConverters содержит типы, поддерживают преобразование содержимого сообщений электронной почты. Эти типы могут выполнять преобразование страницы кода, удалять не защищенный HTML и выполнять другие преобразования в органах сообщений электронной почты. [Microsoft.Exchange. Пространство имен Data.TextConverters](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.TextConverters.aspx) включает следующие классы, которые вытекают из абстрактного класса [TextConverter:](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.TextConverters.TextConverter.aspx) 
  
- [EnrichedToHtml](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.TextConverters.EnrichedToHtml.aspx)
    
- [EnrichedToText](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.TextConverters.EnrichedToText.aspx)
    
- [HtmlToEnriched](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.TextConverters.HtmlToEnriched.aspx)
    
- [HtmlToHtml](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.TextConverters.HtmlToHtml.aspx)
    
- [HtmlToRtf](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.TextConverters.HtmlToRtf.aspx)
    
- [HtmlToText](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.TextConverters.HtmlToText.aspx)
    
- [RtfCompressedToRtf](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.TextConverters.RtfCompressedToRtf.aspx)
    
- [RtfToHtml](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.TextConverters.RtfToHtml.aspx)
    
- [RtfToRtf](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.TextConverters.RtfToRtf.aspx)
    
- [RtfToRtfCompressed](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.TextConverters.RtfToRtfCompressed.aspx)
    
- [RtfToText](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.TextConverters.RtfToText.aspx)
    
- [TextToHtml](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.TextConverters.TextToHtml.aspx)
    
- [TextToRtf](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.TextConverters.TextToRtf.aspx)
    
- [TextToText](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.TextConverters.TextToText.aspx)
    
Эти текстовые преобразователи позволяют изменить формат потока документов или удалить элементы, которые не защищены из HTML-документа. Эти классы можно использовать самостоятельно для преобразования, используя один вызов в один из методов Преобразования в базовом классе [TextConverter,](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.TextConverters.TextConverter.aspx) или они могут быть переданы конструктору конвертера, который использует его для выполнения преобразованных считывателя или записей. 
  
Функциональные возможности, унаследованные от базового класса, полезны для выполнения преобразований, если у вас достаточно места для хранения исходного документа и его преобразованного вывода или для хранения результатов преобразования. Метод **Convert** принимает потоки ввода и вывода, считыватели текста или текстовые сочинители и преобразует содержимое ввода в связанные выходные данные. 
  
Кроме того, в пространство имен включены следующие классы чтения текста, записи и потоковой передачи:
  
- [ConverterReader](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.TextConverters.ConverterReader.aspx) — производный от **System.IO.TextReader**. 
    
- [ConverterWriter](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.TextConverters.ConverterWriter.aspx) — производный **от System.IO.TextWriter**. 
    
- [ConverterStream](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.TextConverters.ConverterStream.aspx) — производный **от System.IO.Stream**. 
    
Они используются для выполнения преобразований, когда у вас нет места для хранения исходного или преобразованного вывода, при поступлении ввода или отправке вывода в поток или когда вы хотите получить выход только для индексации или поиска и поэтому не хотите хранить результат преобразования.
  
## <a name="tnef-namespace"></a>Пространство имен Tnef
<a name="TNEF"> </a>

Пространство имен Tnef содержит классы и типы, которые позволяют читать и писать данные TNEF только на основе потоков. TNEF — это формат данных, используемый для инкапсулации свойств MAPI для клиентов, которые не могут интерпретировать MAPI.
  
Классы [TnefReader](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.ContentTypes.Tnef.TnefReader.aspx) и [TnefWriter](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.ContentTypes.Tnef.TnefWriter.aspx) предоставляют основные функции в [Microsoft.Exchange. Пространство имен Data.ContentTypes.Tnef.](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.ContentTypes.Tnef.aspx) 
  
Класс [TnefReader](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.ContentTypes.Tnef.TnefReader.aspx) принимает читаемый поток в качестве аргумента для своих конструкторов. Затем метод [ReadNextAttribute](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.ContentTypes.Tnef.TnefReader.ReadNextAttribute.aspx) используется для последовательного чтения атрибутов в потоке TNEF. После прочтенного атрибута можно получить доступ к сведениям о атрибуте с помощью любого свойства только для чтения на объекте [TnefReader,](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.ContentTypes.Tnef.TnefReader.aspx) а также получить доступ к [TnefPropertyReader](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.ContentTypes.Tnef.TnefPropertyReader.aspx) для чтения текущего свойства. Вы также можете напрямую получить доступ к текущему атрибуту с помощью метода [ReadAttributeRawValue.](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.ContentTypes.Tnef.TnefReader.ReadAttributeRawValue.aspx) 
  
Класс [TnefWriter](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.ContentTypes.Tnef.TnefWriter.aspx) принимает writable [Stream](https://msdn.microsoft.com/library/System.IO.Stream.aspx) в качестве аргумента для своих конструкторов. Класс [TnefWriter](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.ContentTypes.Tnef.TnefWriter.aspx) предоставляет несколько способов записи данных в этот поток. 
  
## <a name="vcard-namespace"></a>пространство имен vCard
<a name="vCard"> </a>

Пространство имен vCard содержит классы, структуры и переумерия, используемые для чтения и записи контактных данных, содержащихся в сообщении электронной почты, которое находится в формате данных vCard. Пространство имен содержит считыватель контактов и писатель, класс исключений, считыватель свойств, считыватель параметров и поддерживающие перемеры, которые позволяют читать данные vCard, связанные с сообщением электронной почты.
  
## <a name="see-also"></a>См. также

- [Агенты транспорта в Exchange](transport-agents-in-exchange-2013.md)  
- [Концепции транспортного агента в Exchange 2013 г.](transport-agent-concepts-in-exchange-2013.md) 
- [Ссылка агента транспорта на Exchange 2013 г.](transport-agent-reference-for-exchange-2013.md)
- [Типы мультимедиа MIME](http://www.iana.org/assignments/media-types)
    

