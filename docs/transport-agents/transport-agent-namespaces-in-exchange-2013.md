---
title: Пространства имен агента транспорта в Exchange 2013
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 5c40788e-c182-4502-9202-206e6aaa53f8
description: Сведения о классах и членах .NET Framework, которые можно использовать для создания настраиваемых агентов транспорта для Exchange 2013.
ms.openlocfilehash: fc2d9108c910a730bb48c5be028797f0f15ad4ad
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461795"
---
# <a name="transport-agent-namespaces-in-exchange-2013"></a>Пространства имен агента транспорта в Exchange 2013

Сведения о классах и членах .NET Framework, которые можно использовать для создания настраиваемых агентов транспорта для Exchange 2013.
  
**Применимо к:** Exchange Server 2013 
  
В этой статье представлены сведения о пространствах имен, содержащие справочные сведения, которые можно использовать для создания агентов транспорта для Exchange Server 2013. Здесь также описываются классы, которые агенты транспорта могут использовать для чтения и изменения сообщений электронной почты, которые проходят через транспортный конвейер.
  
## <a name="transport-agent-class-library"></a>Библиотека классов агентов транспорта

Следующие пространства имен содержат типы, которые можно использовать для создания и расширения агентов транспорта.

**Таблица 1. Пространства имен .NET Framework**

|**Namespace**|**Описание**|
|:-----|:-----|
|[Microsoft. Exchange. Data](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.aspx) <br/> |Содержит типы, указывающие исключения данных и конфигурации.  <br/> |
|[Microsoft. Exchange. Data. Common](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Common.aspx) <br/> |Содержит типы, поддерживающие локализацию и обработку ошибок.  <br/> |
|[Microsoft. Exchange. Data. ContentTypes. iCalendar](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.ContentTypes.iCalendar.aspx) <br/> |Содержит типы, которые позволяют считывать и записывать данные iCalendar.  <br/> |
|[Microsoft. Exchange. Data. ContentTypes. TNEF](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.ContentTypes.Tnef.aspx) <br/> |Содержит типы, которые позволяют считывать и записывать данные в формате TNEF.  <br/> |
|[Microsoft. Exchange. Data. ContentTypes. vCard](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.ContentTypes.vCard.aspx) <br/> |Содержит типы, которые позволяют считывать и записывать данные vCard.  <br/> |
|[Microsoft. Exchange. Data. Globalization](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Globalization.aspx) <br/> |Содержит типы, которые позволяют работать с культурами и наборами символов для получения локализованного содержимого.  <br/> |
|[Microsoft. Exchange. Data. MIME](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.aspx) <br/> |Содержит типы, которые позволяют считывать и записывать данные MIME.  <br/> |
|[Microsoft. Exchange. Data. MIME. Encoders](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.Encoders.aspx) <br/> |Содержит типы, позволяющие кодировать и декодировать данные MIME.  <br/> |
|[Microsoft. Exchange. Data. Текстконвертерс](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.TextConverters.aspx) <br/> |Содержит типы, которые позволяют считывать и записывать данные с помощью разных текстовых форматов, а также преобразовывать данные в эти форматы и из этих форматов.  <br/> |
|[Microsoft. Exchange. Data. Transport](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.aspx) <br/> |Содержит типы, которые позволяют получить доступ к маршрутизации, ведущему приложению и сведениям о домене о транспортном конвейере.  <br/> |
|[Microsoft. Exchange. Data. Transport. Delivery](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Delivery.aspx) <br/> |Содержит типы, поддерживающие расширение агентов доставки Exchange 2013.  <br/> |
|[Microsoft. Exchange. Data. Transport. email](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Email.aspx) <br/> |Содержит типы, которые поддерживают создание, чтение, запись и изменение сообщений электронной почты.  <br/> |
|[Microsoft. Exchange. Data. Transport. Routing](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.aspx) <br/> |Содержит типы, которые поддерживают расширение режима маршрутизации транспорта Exchange 2013.  <br/> |
|[Microsoft. Exchange. Data. Transport. SMTP](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.aspx) <br/> |Содержит типы, поддерживающие расширение SMTP-поведения транспорта Exchange 2013.  <br/> |
   
## <a name="see-also"></a>См. также

- [Агенты транспорта в Exchange](transport-agents-in-exchange-2013.md)   
- [Основные понятия, связанные с агентами транспорта в Exchange 2013](transport-agent-concepts-in-exchange-2013.md) 
- 
  [Справочные материалы по серверному API для Exchange](https://msdn.microsoft.com/library/6eddd052-f59f-45b4-b846-7e53d4d7eb16%28Office.15%29.aspx)
- [Элементы файла конфигурации агентов для Exchange 2013](agents-configuration-file-elements-for-exchange-2013.md)
    

