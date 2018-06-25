---
title: Транспорта агента пространства имен в Exchange 2013
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 5c40788e-c182-4502-9202-206e6aaa53f8
description: Узнайте о классов .NET Framework и элементы, которые можно использовать для создания настраиваемых транспортных агентов для Exchange 2013.
ms.openlocfilehash: a8189ca9915312b64fefda3091f8f81e51271ad6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761320"
---
# <a name="transport-agent-namespaces-in-exchange-2013"></a>Транспорта агента пространства имен в Exchange 2013

Узнайте о классов .NET Framework и элементы, которые можно использовать для создания настраиваемых транспортных агентов для Exchange 2013.
  
**Применимо к:** Exchange Server 2013 
  
В этой статье представлены сведения о пространства имен, содержащие сведения, которые можно использовать для создания агенты транспорта для Exchange Server 2013. Этот параметр также описывает классы, которые транспортных агентов можно использовать для чтения и изменения сообщений электронной почты, проходящих через транспортный конвейер.
  
## <a name="transport-agent-class-library"></a>Библиотека классов агента транспорта

Следующие пространства имен содержат типы, которые можно использовать для создания и расширения агенты транспорта.

**В таблице 1. Пространства имен .NET framework**

|**Пространство имен**|**Описание**|
|:-----|:-----|
|[Microsoft.Exchange.Data](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.aspx) <br/> |Содержит типы, которые задают исключения данных и конфигурации.  <br/> |
|[Microsoft.Exchange.Data.Common](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Common.aspx) <br/> |Содержит типы, которые поддерживают локализации и обработка ошибок.  <br/> |
|[Microsoft.Exchange.Data.ContentTypes.iCalendar](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.ContentTypes.iCalendar.aspx) <br/> |Содержит типы, которые позволяют читать и записывать данные iCalendar.  <br/> |
|[Microsoft.Exchange.Data.ContentTypes.Tnef](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.ContentTypes.Tnef.aspx) <br/> |Содержит типы, которые позволяют читать и записывать данные TNEF.  <br/> |
|[Microsoft.Exchange.Data.ContentTypes.vCard](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.ContentTypes.vCard.aspx) <br/> |Содержит типы, которые позволяют читать и записывать данные визитной карточки.  <br/> |
|[Microsoft.Exchange.Data.Globalization](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Globalization.aspx) <br/> |Содержит типы, которые позволяют знаков наборов данных, подлежащих необходимо создать локализованное содержимое и работа с языки и региональные параметры.  <br/> |
|[Microsoft.Exchange.Data.Mime](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.aspx) <br/> |Содержит типы, которые позволяют читать и записывать данные MIME.  <br/> |
|[Microsoft.Exchange.Data.Mime.Encoders](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.Encoders.aspx) <br/> |Содержит типы, которые позволяют вам для кодирования и декодирования данных MIME.  <br/> |
|[Microsoft.Exchange.Data.TextConverters](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.TextConverters.aspx) <br/> |Содержит типы, которые позволяют читать и записывать данные в разных форматах и преобразования данных и в этих форматах.  <br/> |
|[Microsoft.Exchange.Data.Transport](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.aspx) <br/> |Содержит типы, которые позволяют получить доступ к маршрутизации, узел и домена сведения о транспортный конвейер.  <br/> |
|[Имен Microsoft.Exchange.Data.Transport](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Delivery.aspx) <br/> |Содержит типы, которые поддерживают расширение агентов доставки Exchange 2013.  <br/> |
|[Microsoft.Exchange.Data.Transport.Email](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Email.aspx) <br/> |Содержит типы, поддерживающие создание, чтение, запись и изменение сообщений электронной почты.  <br/> |
|[Microsoft.Exchange.Data.Transport.Routing](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.aspx) <br/> |Содержит типы, которые поддерживают расширение поведения Маршрутизация транспорта Exchange 2013.  <br/> |
|[Microsoft.Exchange.Data.Transport.Smtp](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.aspx) <br/> |Содержит типы, которые поддерживают расширение поведения SMTP транспорта Exchange 2013.  <br/> |
   
## <a name="see-also"></a>См. также

- [Агенты транспорта в Exchange](transport-agents-in-exchange-2013.md)   
- [Транспорта концепции агентов в Exchange 2013](transport-agent-concepts-in-exchange-2013.md) 
- [Справочник по API сервера для Exchange](http://msdn.microsoft.com/library/6eddd052-f59f-45b4-b846-7e53d4d7eb16%28Office.15%29.aspx)
- [Элементы файла конфигурации агентов для Exchange 2013](agents-configuration-file-elements-for-exchange-2013.md)
    

