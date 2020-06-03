---
title: Трассировка запросов и ответов на устранение неполадок приложений управляемого API EWS
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.assetid: 186c1d1d-b8dc-4914-b3cd-6fada7ecd877
description: Сведения о том, как отслеживать запросы и ответы EWS на устранение ошибок в приложении управляемого API EWS.
localization_priority: Priority
ms.openlocfilehash: dd225030d62a2e8211b7063ee78a59fd1a070263
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44455858"
---
# <a name="trace-requests-and-responses-to-troubleshoot-ews-managed-api-apps"></a>Трассировка запросов и ответов на устранение неполадок приложений управляемого API EWS

Сведения о том, как отслеживать запросы и ответы EWS на устранение ошибок в приложении управляемого API EWS.
  
Отладка приложения, основанного на веб-службе, может быть затруднительной, так как часть обработки выполняется на удаленном компьютере, к которому у вас нет доступа. Так как вы не можете пошагово пройти код на сервере, может быть полезно просмотреть запросы и ответы XML, которые передаются между клиентом и сервером, чтобы определить, какая часть приложения вызывает ошибку. 
  
Если вы используете EWS, у вас уже есть доступ к запросу и ответу XML; Вы можете поместить точку останова в код, чтобы проверить ответ сервера на ваш запрос, чтобы устранить проблему. Если вы используете управляемый API EWS, у вас нет прямого доступа к запросу и ответу EWS. Тем не менее, вы можете использовать методы трассировки для объекта [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) , чтобы захватывать запрос и ответ XML, а затем использовать XML-код, чтобы определить, почему ваш код не работает. 

Например, если свойство неправильно задано, может возникнуть непредвиденный ответ, и вы можете использовать результаты трассировки для просмотра запроса и ответа XML для идентификации ошибки. Данные трассировки из управляемого API EWS также могут помочь вручную создать XML-запрос для создания приложения EWS. Если вы используете EWS, вы можете создать небольшое приложение с помощью управляемого API EWS, проследить его, а затем использовать XML-запрос, который поможет вам создать запрос EWS. 
  
## <a name="enabling-tracing-on-the-exchangeservice-object"></a>Включение трассировки для объекта ExchangeService
<a name="bk_EnableTracing"> </a>

Чтобы включить трассировку, создайте объект [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) для приложения и задайте свойства трассировки, как показано в следующем примере. 
  
```cs
ExchangeService service = new ExchangeService(ExchangeVersion.Exchange2010);
service.TraceListener = ITraceListenerInstance;
// Optional flags to indicate the requests and responses to trace.
service.TraceFlags = TraceFlags.EwsRequest | TraceFlags.EwsResponse
service.TraceEnabled = true;

```

После установки для свойства [трацеенаблед](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservicebase.traceenabled%28v=exchg.80%29.aspx) значения **true**все запросы, которые совпадают с флагами трассировки, будут отправлены указанному прослушивателю трассировки. Можно указать один флаг трассировки или указать несколько флагов трассировки, объединив их с логическим **или**. [Перечисление трацефлагс](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.traceflags%28v=exchg.80%29.aspx) можно использовать для указания значений для EWS и запросов автообнаружения и ответов. 
  
## <a name="implementing-a-tracelistener-object"></a>Реализация объекта TraceListener
<a name="bk_traceListener"> </a>

Для свойства [трацеенаблед](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservicebase.traceenabled%28v=exchg.80%29.aspx) можно задать **значение true** , чтобы выводить запросы и ответы XML для приложения, такие как окно консоли. Если требуется управлять выходными данными трассировки и сохранять их в файл, рекомендуется реализовать объект [класса TraceListener](https://msdn.microsoft.com/library/system.diagnostics.tracelistener.aspx) . В следующем примере кода показан простой объект, который реализует интерфейс [итрацелистенер](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.itracelistener%28v=exchg.80%29.aspx) и сохраняет отслеживаемые запросы и ответы в XML-или текстовых файлах. 
  
```cs
class TraceListener : ITraceListener
{
    #region ITraceListener Members
    public void Trace(string traceType, string traceMessage)
    {
      CreateXMLTextFile(traceType, traceMessage.ToString());
    }
    #endregion
    private void CreateXMLTextFile(string fileName, string traceContent)
    {
      // Create a new XML file for the trace information.
      try
      {
        // If the trace data is valid XML, create an XmlDocument object and save.
        XmlDocument xmlDoc = new XmlDocument();
        xmlDoc.Load(traceContent);
        xmlDoc.Save(fileName + ".xml");
      }
      catch
      {
        // If the trace data is not valid XML, save it as a text document.
        System.IO.File.WriteAllText(fileName + ".txt", traceContent);
      }
    }
}

```

## <a name="see-also"></a>См. также

- [Начало работы с веб-службами Exchange](start-using-web-services-in-exchange.md)
- [Обработка сообщений об ошибках службы автообнаружения](handling-autodiscover-error-messages.md)    
- [Ссылка на сборку управляемого API EWS](how-to-reference-the-ews-managed-api-assembly.md)    
- [Взаимодействие с EWS с помощью управляемого API EWS](how-to-communicate-with-ews-by-using-the-ews-managed-api.md)
    

