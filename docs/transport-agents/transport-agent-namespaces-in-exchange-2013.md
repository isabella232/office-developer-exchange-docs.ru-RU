---
title: Пространства имен транспортного агента в Exchange 2013 г.
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 5c40788e-c182-4502-9202-206e6aaa53f8
description: Узнайте о платформа .NET Framework классах и членах, которые можно использовать для создания настраиваемой службы транспорта для Exchange 2013 г.
ms.openlocfilehash: 076ddb8e2ccbdfa195a68aca6b296337a2876b55
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59537132"
---
# <a name="transport-agent-namespaces-in-exchange-2013"></a>Пространства имен транспортного агента в Exchange 2013 г.

Узнайте о платформа .NET Framework классах и членах, которые можно использовать для создания настраиваемой службы транспорта для Exchange 2013 г.
  
**Применяется к:** Exchange Server 2013 г. 
  
В этой статье содержатся сведения о пространствах имен, содержащих справочные сведения, которые можно использовать для создания транспортных агентов для Exchange Server 2013 г. В нем также описываются классы, которые транспортные агенты могут использовать для чтения и изменения сообщений электронной почты, которые проходят через транспортный конвейер.
  
## <a name="transport-agent-class-library"></a>Библиотека классов транспортных агентов

В следующих пространствах имен содержатся типы, которые можно использовать для создания и расширения транспортных агентов.

**Таблица 1. платформа .NET Framework пространства имен**

|**Namespace**|**Описание**|
|:-----|:-----|
|[Microsoft. Exchange. Данные](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.aspx) <br/> |Содержит типы, которые указывают исключения данных и конфигурации.  <br/> |
|[Microsoft. Exchange.Data.Common](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Common.aspx) <br/> |Содержит типы, поддерживаюющие локализацию и обработку ошибок.  <br/> |
|[Microsoft. Exchange. Data.ContentTypes.iCalendar](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.ContentTypes.iCalendar.aspx) <br/> |Содержит типы, позволяющие читать и записывать данные iCalendar.  <br/> |
|[Microsoft. Exchange. Data.ContentTypes.Tnef](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.ContentTypes.Tnef.aspx) <br/> |Содержит типы, позволяющие читать и записывать данные TNEF.  <br/> |
|[Microsoft. Exchange. Data.ContentTypes.vCard](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.ContentTypes.vCard.aspx) <br/> |Содержит типы, позволяющие читать и записывать данные vCard.  <br/> |
|[Microsoft. Exchange. Data.Globalization](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Globalization.aspx) <br/> |Содержит типы, которые позволяют работать с культурами и наборами символов для создания локализованного контента.  <br/> |
|[Microsoft. Exchange. Data.Mime](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.aspx) <br/> |Содержит типы, позволяющие читать и записывать данные MIME.  <br/> |
|[Microsoft. Exchange. Data.Mime.Encoders](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.Encoders.aspx) <br/> |Содержит типы, позволяющие кодировать и декодировать данные MIME.  <br/> |
|[Microsoft. Exchange. Data.TextConverters](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.TextConverters.aspx) <br/> |Содержит типы, которые позволяют читать и записывать данные в различных текстовых форматах, а также преобразовывать данные в эти форматы и из них.  <br/> |
|[Microsoft. Exchange. Data.Transport](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.aspx) <br/> |Содержит типы, позволяющие получать доступ к сведениям о маршрутике, хост-сайте и домене о транспортном конвейере.  <br/> |
|[Microsoft. Exchange. Data.Transport.Delivery](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Delivery.aspx) <br/> |Содержит типы, поддерживают расширение агентов Exchange 2013 года.  <br/> |
|[Microsoft. Exchange. Data.Transport.Email](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Email.aspx) <br/> |Содержит типы, поддерживающих создание, чтение, написание и изменение сообщений электронной почты.  <br/> |
|[Microsoft. Exchange. Data.Transport.Routing](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.aspx) <br/> |Содержит типы, поддерживаюющие расширение Exchange 2013 года.  <br/> |
|[Microsoft. Exchange. Data.Transport.Smtp](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.aspx) <br/> |Содержит типы, поддерживают расширение Exchange smTP 2013.  <br/> |
   
## <a name="see-also"></a>См. также

- [Агенты транспорта в Exchange](transport-agents-in-exchange-2013.md)   
- [Концепции транспортного агента в Exchange 2013 г.](transport-agent-concepts-in-exchange-2013.md) 
- 
  [Справочные материалы по серверному API для Exchange](https://msdn.microsoft.com/library/6eddd052-f59f-45b4-b846-7e53d4d7eb16%28Office.15%29.aspx)
- [Элементы конфигурации файлов агентов для Exchange 2013 г.](agents-configuration-file-elements-for-exchange-2013.md)
    

