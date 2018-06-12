---
title: Трассировка запросы и ответы для устранения неполадок приложений управляемый API EWS
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 186c1d1d-b8dc-4914-b3cd-6fada7ecd877
description: Узнайте, как для трассировки запросов веб-служб Exchange и ответы для устранения ошибок в приложении управляемый API веб-служб Exchange.
ms.openlocfilehash: 056a1f84c4172b0404975d6fc35f9ecd7395ecdb
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761115"
---
# <a name="trace-requests-and-responses-to-troubleshoot-ews-managed-api-apps"></a>Трассировка запросы и ответы для устранения неполадок приложений управляемый API EWS

Узнайте, как для трассировки запросов веб-служб Exchange и ответы для устранения ошибок в приложении управляемый API веб-служб Exchange.
  
Отладка веб-приложения на основе службы могут возникнуть проблемы, так как часть обработки выполняется на удаленном компьютере, который может не иметь доступ к. Так как не удается пошаговое выполнение кода на сервере, могут быть полезны для просмотра XML запросы и ответы, отправленные между клиентом и сервером, чтобы определить, какие части приложения вызывает ошибку. 
  
При использовании веб-служб Exchange уже имеют доступ к XML запроса и ответа; можно поместить точку останова в код, чтобы просмотреть параметры сервера ответа на запрос для устранения неполадок. Если вы используете управляемый API веб-служб Exchange, у вас нет прямой доступ к веб-служб Exchange запроса и ответа. Тем не менее можно использовать методы трассировки на объекте [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) для захвата XML запроса и ответа, и затем можно использовать XML-код для определения, почему код не работает. 

Например если свойство не были установлены правильно, можно получить непредвиденные ответа и выходных данных трассировки можно использовать для просмотра XML-запрос и ответ для определения ошибки. Выходные данные трассировки из управляемого API EWS также может помочь вручную построения запроса XML для создания приложения в веб-служб Exchange. При использовании веб-служб Exchange можно создавать небольшие приложения с помощью управляемого интерфейса API веб-служб Exchange, отслеживать ее и затем использовать сведения о запросе XML позволяет создать запрос веб-служб Exchange. 
  
## <a name="enabling-tracing-on-the-exchangeservice-object"></a>Включение трассировки для объекта ExchangeService
<a name="bk_EnableTracing"> </a>

Чтобы включить трассировку, создайте объект [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) для вашего приложения и задать свойства трассировки, как показано в следующем примере. 
  
```cs
ExchangeService service = new ExchangeService(ExchangeVersion.Exchange2010);
service.TraceListener = ITraceListenerInstance;
// Optional flags to indicate the requests and responses to trace.
service.TraceFlags = TraceFlags.EwsRequest | TraceFlags.EwsResponse
service.TraceEnabled = true;

```

Свойство [TraceEnabled](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservicebase.traceenabled%28v=exchg.80%29.aspx) присвоено **значение true**, все запросы, соответствующие флаги трассировки будут отправлены прослушивателю указанной трассировки. Можно указать флаг одного трассировки, или вы можете указать несколько флагов трассировки, их объединения с логического **или**. [Перечисление TraceFlags](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.traceflags%28v=exchg.80%29.aspx) можно использовать для указания значения для веб-служб Exchange, а также для автоматического обнаружения запросы и ответы. 
  
## <a name="implementing-a-tracelistener-object"></a>Реализация объекта прослушиватель трассировки
<a name="bk_traceListener"> </a>

Свойства [TraceEnabled](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservicebase.traceenabled%28v=exchg.80%29.aspx) значение **true** для вывода XML запросы и ответы для приложения, такие как окно консоли. Если вы хотите управлять выходные данные трассировки и сохраните его в файл, рекомендуется реализовать объект [класса прослушиватель трассировки](http://msdn.microsoft.com/en-us/library/system.diagnostics.tracelistener.aspx) . В следующем примере кода показан простой объект, реализующий интерфейс [ITraceListener](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.itracelistener%28v=exchg.80%29.aspx) и хранятся в файлах XML или текст трассировки запросов и ответов. 
  
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

- [Начать работу с использованием веб-служб Exchange](start-using-web-services-in-exchange.md)
- [Обработка сообщений об ошибках службы автообнаружения](handling-autodiscover-error-messages.md)    
- [Ссылки на сборку управляемого интерфейса API веб-служб Exchange](how-to-reference-the-ews-managed-api-assembly.md)    
- [Взаимодействие с веб-служб Exchange с помощью управляемого интерфейса API веб-служб Exchange](how-to-communicate-with-ews-by-using-the-ews-managed-api.md)
    

