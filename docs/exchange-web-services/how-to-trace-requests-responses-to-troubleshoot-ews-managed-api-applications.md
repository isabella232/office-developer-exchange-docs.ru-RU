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
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761115"
---
# <a name="trace-requests-and-responses-to-troubleshoot-ews-managed-api-apps"></a><span data-ttu-id="56ad6-103">Трассировка запросы и ответы для устранения неполадок приложений управляемый API EWS</span><span class="sxs-lookup"><span data-stu-id="56ad6-103">Trace requests and responses to troubleshoot EWS Managed API apps</span></span>

<span data-ttu-id="56ad6-104">Узнайте, как для трассировки запросов веб-служб Exchange и ответы для устранения ошибок в приложении управляемый API веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="56ad6-104">Find out how to trace EWS requests and responses to troubleshoot errors in your EWS Managed API application.</span></span>
  
<span data-ttu-id="56ad6-105">Отладка веб-приложения на основе службы могут возникнуть проблемы, так как часть обработки выполняется на удаленном компьютере, который может не иметь доступ к.</span><span class="sxs-lookup"><span data-stu-id="56ad6-105">Debugging a web service-based application can be difficult because part of the processing is performed on a remote computer that you might not have access to.</span></span> <span data-ttu-id="56ad6-106">Так как не удается пошаговое выполнение кода на сервере, могут быть полезны для просмотра XML запросы и ответы, отправленные между клиентом и сервером, чтобы определить, какие части приложения вызывает ошибку.</span><span class="sxs-lookup"><span data-stu-id="56ad6-106">Because you cannot step through the code on the server, it can be helpful to see the XML requests and responses that are sent between the client and the server to determine which part of the application is causing an error.</span></span> 
  
<span data-ttu-id="56ad6-107">При использовании веб-служб Exchange уже имеют доступ к XML запроса и ответа; можно поместить точку останова в код, чтобы просмотреть параметры сервера ответа на запрос для устранения неполадок.</span><span class="sxs-lookup"><span data-stu-id="56ad6-107">If you are using EWS, you already have access to the XML request and response; you can put a break point in your code to review the server's response to your request in order to troubleshoot an issue.</span></span> <span data-ttu-id="56ad6-108">Если вы используете управляемый API веб-служб Exchange, у вас нет прямой доступ к веб-служб Exchange запроса и ответа.</span><span class="sxs-lookup"><span data-stu-id="56ad6-108">If you're using the EWS Managed API, you don't have direct access to the EWS request and response.</span></span> <span data-ttu-id="56ad6-109">Тем не менее можно использовать методы трассировки на объекте [ExchangeService](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) для захвата XML запроса и ответа, и затем можно использовать XML-код для определения, почему код не работает.</span><span class="sxs-lookup"><span data-stu-id="56ad6-109">However, you can use tracing methods on the [ExchangeService](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object to capture the XML request and response, and you can then use the XML to determine why your code is not working.</span></span> 

<span data-ttu-id="56ad6-110">Например если свойство не были установлены правильно, можно получить непредвиденные ответа и выходных данных трассировки можно использовать для просмотра XML-запрос и ответ для определения ошибки.</span><span class="sxs-lookup"><span data-stu-id="56ad6-110">For example, if you did not set a property correctly, you might get an unexpected response, and you can use the trace output to look at the XML request and response to identify the error.</span></span> <span data-ttu-id="56ad6-111">Выходные данные трассировки из управляемого API EWS также может помочь вручную построения запроса XML для создания приложения в веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="56ad6-111">The trace output from the EWS Managed API can also help you manually build the XML request to create your EWS application.</span></span> <span data-ttu-id="56ad6-112">При использовании веб-служб Exchange можно создавать небольшие приложения с помощью управляемого интерфейса API веб-служб Exchange, отслеживать ее и затем использовать сведения о запросе XML позволяет создать запрос веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="56ad6-112">If you are using EWS, you can create a small application by using EWS Managed API, trace it, and then use the XML request information to help you build your EWS request.</span></span> 
  
## <a name="enabling-tracing-on-the-exchangeservice-object"></a><span data-ttu-id="56ad6-113">Включение трассировки для объекта ExchangeService</span><span class="sxs-lookup"><span data-stu-id="56ad6-113">Enabling tracing on the ExchangeService object</span></span>
<span data-ttu-id="56ad6-114"><a name="bk_EnableTracing"> </a></span><span class="sxs-lookup"><span data-stu-id="56ad6-114"></span></span>

<span data-ttu-id="56ad6-115">Чтобы включить трассировку, создайте объект [ExchangeService](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) для вашего приложения и задать свойства трассировки, как показано в следующем примере.</span><span class="sxs-lookup"><span data-stu-id="56ad6-115">To enable tracing, create an [ExchangeService](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object for your application, and set the tracing properties as shown in the following example.</span></span> 
  
```cs
ExchangeService service = new ExchangeService(ExchangeVersion.Exchange2010);
service.TraceListener = ITraceListenerInstance;
// Optional flags to indicate the requests and responses to trace.
service.TraceFlags = TraceFlags.EwsRequest | TraceFlags.EwsResponse
service.TraceEnabled = true;

```

<span data-ttu-id="56ad6-116">Свойство [TraceEnabled](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.exchangeservicebase.traceenabled%28v=exchg.80%29.aspx) присвоено **значение true**, все запросы, соответствующие флаги трассировки будут отправлены прослушивателю указанной трассировки.</span><span class="sxs-lookup"><span data-stu-id="56ad6-116">After you set the [TraceEnabled](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.exchangeservicebase.traceenabled%28v=exchg.80%29.aspx) property to **true**, all requests that match the trace flags will be sent to the specified trace listener.</span></span> <span data-ttu-id="56ad6-117">Можно указать флаг одного трассировки, или вы можете указать несколько флагов трассировки, их объединения с логического **или**.</span><span class="sxs-lookup"><span data-stu-id="56ad6-117">You can specify a single trace flag, or you can specify multiple trace flags by combining them with a logical **OR**.</span></span> <span data-ttu-id="56ad6-118">[Перечисление TraceFlags](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.traceflags%28v=exchg.80%29.aspx) можно использовать для указания значения для веб-служб Exchange, а также для автоматического обнаружения запросы и ответы.</span><span class="sxs-lookup"><span data-stu-id="56ad6-118">You can use the [TraceFlags enumeration](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.traceflags%28v=exchg.80%29.aspx) to specify values for EWS and for Autodiscover requests and responses.</span></span> 
  
## <a name="implementing-a-tracelistener-object"></a><span data-ttu-id="56ad6-119">Реализация объекта прослушиватель трассировки</span><span class="sxs-lookup"><span data-stu-id="56ad6-119">Implementing a TraceListener object</span></span>
<span data-ttu-id="56ad6-120"><a name="bk_traceListener"> </a></span><span class="sxs-lookup"><span data-stu-id="56ad6-120"></span></span>

<span data-ttu-id="56ad6-121">Свойства [TraceEnabled](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.exchangeservicebase.traceenabled%28v=exchg.80%29.aspx) значение **true** для вывода XML запросы и ответы для приложения, такие как окно консоли.</span><span class="sxs-lookup"><span data-stu-id="56ad6-121">You can set the [TraceEnabled](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.exchangeservicebase.traceenabled%28v=exchg.80%29.aspx) property to **true** to output the XML requests and responses to your application, such as a console window.</span></span> <span data-ttu-id="56ad6-122">Если вы хотите управлять выходные данные трассировки и сохраните его в файл, рекомендуется реализовать объект [класса прослушиватель трассировки](http://msdn.microsoft.com/ru-ru/library/system.diagnostics.tracelistener.aspx) .</span><span class="sxs-lookup"><span data-stu-id="56ad6-122">If you want to control the trace output and save it to a file, we recommend that you implement a [TraceListener class](http://msdn.microsoft.com/ru-ru/library/system.diagnostics.tracelistener.aspx) object.</span></span> <span data-ttu-id="56ad6-123">В следующем примере кода показан простой объект, реализующий интерфейс [ITraceListener](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.itracelistener%28v=exchg.80%29.aspx) и хранятся в файлах XML или текст трассировки запросов и ответов.</span><span class="sxs-lookup"><span data-stu-id="56ad6-123">The following code example shows a simple object that implements the [ITraceListener](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.itracelistener%28v=exchg.80%29.aspx) interface and stores the traced requests and responses in XML or text files.</span></span> 
  
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

## <a name="see-also"></a><span data-ttu-id="56ad6-124">См. также</span><span class="sxs-lookup"><span data-stu-id="56ad6-124">See also</span></span>

- [<span data-ttu-id="56ad6-125">Начать работу с использованием веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="56ad6-125">Start using web services in Exchange</span></span>](start-using-web-services-in-exchange.md)
- [<span data-ttu-id="56ad6-126">Обработка сообщений об ошибках службы автообнаружения</span><span class="sxs-lookup"><span data-stu-id="56ad6-126">Handling Autodiscover error messages</span></span>](handling-autodiscover-error-messages.md)    
- [<span data-ttu-id="56ad6-127">Ссылки на сборку управляемого интерфейса API веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="56ad6-127">Reference the EWS Managed API assembly</span></span>](how-to-reference-the-ews-managed-api-assembly.md)    
- [<span data-ttu-id="56ad6-128">Взаимодействие с веб-служб Exchange с помощью управляемого интерфейса API веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="56ad6-128">Communicate with EWS by using the EWS Managed API</span></span>](how-to-communicate-with-ews-by-using-the-ews-managed-api.md)
    

