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
ms.lasthandoff: 06/03/2020
ms.locfileid: "44455858"
---
# <a name="trace-requests-and-responses-to-troubleshoot-ews-managed-api-apps"></a><span data-ttu-id="b4398-103">Трассировка запросов и ответов на устранение неполадок приложений управляемого API EWS</span><span class="sxs-lookup"><span data-stu-id="b4398-103">Trace requests and responses to troubleshoot EWS Managed API apps</span></span>

<span data-ttu-id="b4398-104">Сведения о том, как отслеживать запросы и ответы EWS на устранение ошибок в приложении управляемого API EWS.</span><span class="sxs-lookup"><span data-stu-id="b4398-104">Find out how to trace EWS requests and responses to troubleshoot errors in your EWS Managed API application.</span></span>
  
<span data-ttu-id="b4398-105">Отладка приложения, основанного на веб-службе, может быть затруднительной, так как часть обработки выполняется на удаленном компьютере, к которому у вас нет доступа.</span><span class="sxs-lookup"><span data-stu-id="b4398-105">Debugging a web service-based application can be difficult because part of the processing is performed on a remote computer that you might not have access to.</span></span> <span data-ttu-id="b4398-106">Так как вы не можете пошагово пройти код на сервере, может быть полезно просмотреть запросы и ответы XML, которые передаются между клиентом и сервером, чтобы определить, какая часть приложения вызывает ошибку.</span><span class="sxs-lookup"><span data-stu-id="b4398-106">Because you cannot step through the code on the server, it can be helpful to see the XML requests and responses that are sent between the client and the server to determine which part of the application is causing an error.</span></span> 
  
<span data-ttu-id="b4398-107">Если вы используете EWS, у вас уже есть доступ к запросу и ответу XML; Вы можете поместить точку останова в код, чтобы проверить ответ сервера на ваш запрос, чтобы устранить проблему.</span><span class="sxs-lookup"><span data-stu-id="b4398-107">If you are using EWS, you already have access to the XML request and response; you can put a break point in your code to review the server's response to your request in order to troubleshoot an issue.</span></span> <span data-ttu-id="b4398-108">Если вы используете управляемый API EWS, у вас нет прямого доступа к запросу и ответу EWS.</span><span class="sxs-lookup"><span data-stu-id="b4398-108">If you're using the EWS Managed API, you don't have direct access to the EWS request and response.</span></span> <span data-ttu-id="b4398-109">Тем не менее, вы можете использовать методы трассировки для объекта [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) , чтобы захватывать запрос и ответ XML, а затем использовать XML-код, чтобы определить, почему ваш код не работает.</span><span class="sxs-lookup"><span data-stu-id="b4398-109">However, you can use tracing methods on the [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object to capture the XML request and response, and you can then use the XML to determine why your code is not working.</span></span> 

<span data-ttu-id="b4398-110">Например, если свойство неправильно задано, может возникнуть непредвиденный ответ, и вы можете использовать результаты трассировки для просмотра запроса и ответа XML для идентификации ошибки.</span><span class="sxs-lookup"><span data-stu-id="b4398-110">For example, if you did not set a property correctly, you might get an unexpected response, and you can use the trace output to look at the XML request and response to identify the error.</span></span> <span data-ttu-id="b4398-111">Данные трассировки из управляемого API EWS также могут помочь вручную создать XML-запрос для создания приложения EWS.</span><span class="sxs-lookup"><span data-stu-id="b4398-111">The trace output from the EWS Managed API can also help you manually build the XML request to create your EWS application.</span></span> <span data-ttu-id="b4398-112">Если вы используете EWS, вы можете создать небольшое приложение с помощью управляемого API EWS, проследить его, а затем использовать XML-запрос, который поможет вам создать запрос EWS.</span><span class="sxs-lookup"><span data-stu-id="b4398-112">If you are using EWS, you can create a small application by using EWS Managed API, trace it, and then use the XML request information to help you build your EWS request.</span></span> 
  
## <a name="enabling-tracing-on-the-exchangeservice-object"></a><span data-ttu-id="b4398-113">Включение трассировки для объекта ExchangeService</span><span class="sxs-lookup"><span data-stu-id="b4398-113">Enabling tracing on the ExchangeService object</span></span>
<span data-ttu-id="b4398-114"><a name="bk_EnableTracing"> </a></span><span class="sxs-lookup"><span data-stu-id="b4398-114"><a name="bk_EnableTracing"> </a></span></span>

<span data-ttu-id="b4398-115">Чтобы включить трассировку, создайте объект [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) для приложения и задайте свойства трассировки, как показано в следующем примере.</span><span class="sxs-lookup"><span data-stu-id="b4398-115">To enable tracing, create an [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object for your application, and set the tracing properties as shown in the following example.</span></span> 
  
```cs
ExchangeService service = new ExchangeService(ExchangeVersion.Exchange2010);
service.TraceListener = ITraceListenerInstance;
// Optional flags to indicate the requests and responses to trace.
service.TraceFlags = TraceFlags.EwsRequest | TraceFlags.EwsResponse
service.TraceEnabled = true;

```

<span data-ttu-id="b4398-116">После установки для свойства [трацеенаблед](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservicebase.traceenabled%28v=exchg.80%29.aspx) значения **true**все запросы, которые совпадают с флагами трассировки, будут отправлены указанному прослушивателю трассировки.</span><span class="sxs-lookup"><span data-stu-id="b4398-116">After you set the [TraceEnabled](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservicebase.traceenabled%28v=exchg.80%29.aspx) property to **true**, all requests that match the trace flags will be sent to the specified trace listener.</span></span> <span data-ttu-id="b4398-117">Можно указать один флаг трассировки или указать несколько флагов трассировки, объединив их с логическим **или**.</span><span class="sxs-lookup"><span data-stu-id="b4398-117">You can specify a single trace flag, or you can specify multiple trace flags by combining them with a logical **OR**.</span></span> <span data-ttu-id="b4398-118">[Перечисление трацефлагс](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.traceflags%28v=exchg.80%29.aspx) можно использовать для указания значений для EWS и запросов автообнаружения и ответов.</span><span class="sxs-lookup"><span data-stu-id="b4398-118">You can use the [TraceFlags enumeration](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.traceflags%28v=exchg.80%29.aspx) to specify values for EWS and for Autodiscover requests and responses.</span></span> 
  
## <a name="implementing-a-tracelistener-object"></a><span data-ttu-id="b4398-119">Реализация объекта TraceListener</span><span class="sxs-lookup"><span data-stu-id="b4398-119">Implementing a TraceListener object</span></span>
<span data-ttu-id="b4398-120"><a name="bk_traceListener"> </a></span><span class="sxs-lookup"><span data-stu-id="b4398-120"><a name="bk_traceListener"> </a></span></span>

<span data-ttu-id="b4398-121">Для свойства [трацеенаблед](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservicebase.traceenabled%28v=exchg.80%29.aspx) можно задать **значение true** , чтобы выводить запросы и ответы XML для приложения, такие как окно консоли.</span><span class="sxs-lookup"><span data-stu-id="b4398-121">You can set the [TraceEnabled](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservicebase.traceenabled%28v=exchg.80%29.aspx) property to **true** to output the XML requests and responses to your application, such as a console window.</span></span> <span data-ttu-id="b4398-122">Если требуется управлять выходными данными трассировки и сохранять их в файл, рекомендуется реализовать объект [класса TraceListener](https://msdn.microsoft.com/library/system.diagnostics.tracelistener.aspx) .</span><span class="sxs-lookup"><span data-stu-id="b4398-122">If you want to control the trace output and save it to a file, we recommend that you implement a [TraceListener class](https://msdn.microsoft.com/library/system.diagnostics.tracelistener.aspx) object.</span></span> <span data-ttu-id="b4398-123">В следующем примере кода показан простой объект, который реализует интерфейс [итрацелистенер](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.itracelistener%28v=exchg.80%29.aspx) и сохраняет отслеживаемые запросы и ответы в XML-или текстовых файлах.</span><span class="sxs-lookup"><span data-stu-id="b4398-123">The following code example shows a simple object that implements the [ITraceListener](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.itracelistener%28v=exchg.80%29.aspx) interface and stores the traced requests and responses in XML or text files.</span></span> 
  
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

## <a name="see-also"></a><span data-ttu-id="b4398-124">См. также</span><span class="sxs-lookup"><span data-stu-id="b4398-124">See also</span></span>

- [<span data-ttu-id="b4398-125">Начало работы с веб-службами Exchange</span><span class="sxs-lookup"><span data-stu-id="b4398-125">Start using web services in Exchange</span></span>](start-using-web-services-in-exchange.md)
- [<span data-ttu-id="b4398-126">Обработка сообщений об ошибках службы автообнаружения</span><span class="sxs-lookup"><span data-stu-id="b4398-126">Handling Autodiscover error messages</span></span>](handling-autodiscover-error-messages.md)    
- [<span data-ttu-id="b4398-127">Ссылка на сборку управляемого API EWS</span><span class="sxs-lookup"><span data-stu-id="b4398-127">Reference the EWS Managed API assembly</span></span>](how-to-reference-the-ews-managed-api-assembly.md)    
- [<span data-ttu-id="b4398-128">Взаимодействие с EWS с помощью управляемого API EWS</span><span class="sxs-lookup"><span data-stu-id="b4398-128">Communicate with EWS by using the EWS Managed API</span></span>](how-to-communicate-with-ews-by-using-the-ews-managed-api.md)
    

