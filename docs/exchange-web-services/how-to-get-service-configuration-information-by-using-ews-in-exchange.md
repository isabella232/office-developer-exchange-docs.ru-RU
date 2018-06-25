---
title: Получение сведений о конфигурации службы с помощью веб-служб Exchange в Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 9379740a-96e1-490d-a229-0f9937c548d2
description: Узнайте, как получить сведения о конфигурации службы для единой системы обмена СООБЩЕНИЯМИ, будильника политики, почтовые подсказки и правила защиты от веб-служб Exchange в Exchange.
ms.openlocfilehash: e84a563bb094a2fe03e08f8e1a81b2b054d45850
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761009"
---
# <a name="get-service-configuration-information-by-using-ews-in-exchange"></a><span data-ttu-id="2c03e-103">Получение сведений о конфигурации службы с помощью веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="2c03e-103">Get service configuration information by using EWS in Exchange</span></span>

<span data-ttu-id="2c03e-104">Узнайте, как получить сведения о конфигурации службы для единой системы обмена СООБЩЕНИЯМИ, будильника политики, почтовые подсказки и правила защиты от веб-служб Exchange в Exchange.</span><span class="sxs-lookup"><span data-stu-id="2c03e-104">Find out how to get service configuration information for UM, policy nudges, mail tips, and protection rules from EWS in Exchange.</span></span>
  
<span data-ttu-id="2c03e-105">Работает ли приложение веб-служб Exchange с единой системы обмена сообщениями (UM), политики будильника, почтовые подсказки или правила защиты?</span><span class="sxs-lookup"><span data-stu-id="2c03e-105">Does your EWS application work with Unified Messaging (UM), policy nudges, mail tips, or protection rules?</span></span> <span data-ttu-id="2c03e-106">Если это так, приложения необходимо вызвать [GetServiceConfiguration операции](http://msdn.microsoft.com/library/070cbfe5-325a-4955-8e4a-8230ea0459a7%28Office.15%29.aspx) для получения сведений о конфигурации службы, необходимые.</span><span class="sxs-lookup"><span data-stu-id="2c03e-106">If so, your application will need to call the [GetServiceConfiguration operation](http://msdn.microsoft.com/library/070cbfe5-325a-4955-8e4a-8230ea0459a7%28Office.15%29.aspx) to get the service configuration information that it needs.</span></span> <span data-ttu-id="2c03e-107">Операция **GetServiceConfiguration** возвращает сведения о конфигурации, характерные для каждой из этих функций веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="2c03e-107">The **GetServiceConfiguration** operation returns configuration information that is specific to each of these EWS features.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="2c03e-108">Управляемый API EWS не реализует эту функцию.</span><span class="sxs-lookup"><span data-stu-id="2c03e-108">The EWS Managed API does not implement this functionality.</span></span> 
  
<span data-ttu-id="2c03e-109">**В таблице 1. Сведения о конфигурации, операция GetServiceConfiguration возвращает**</span><span class="sxs-lookup"><span data-stu-id="2c03e-109">**Table 1. Configuration information that the GetServiceConfiguration operation returns**</span></span>

|<span data-ttu-id="2c03e-110">Компонент веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="2c03e-110">EWS feature</span></span>|<span data-ttu-id="2c03e-111">Возвращает операции GetServiceConfiguration...</span><span class="sxs-lookup"><span data-stu-id="2c03e-111">GetServiceConfiguration operation returns…</span></span>|
|:-----|:-----|
|<span data-ttu-id="2c03e-112">ЕДИНАЯ СИСТЕМА ОБМЕНА СООБЩЕНИЯМИ</span><span class="sxs-lookup"><span data-stu-id="2c03e-112">UM</span></span>  <br/> | <ul><li><span data-ttu-id="2c03e-113">Значение, указывающее, включено ли единой системы обмена СООБЩЕНИЯМИ.</span><span class="sxs-lookup"><span data-stu-id="2c03e-113">A value that indicates whether UM is enabled.</span></span></li><li><span data-ttu-id="2c03e-114">Значение, указывающее, включено ли воспроизвести на телефоне.</span><span class="sxs-lookup"><span data-stu-id="2c03e-114">A value that indicates whether play on phone is enabled.</span></span></li><li><span data-ttu-id="2c03e-115">Воспроизвести на строку номера телефона.</span><span class="sxs-lookup"><span data-stu-id="2c03e-115">The play on phone dial string.</span></span></li></ul> |
|<span data-ttu-id="2c03e-116">Политика будильника</span><span class="sxs-lookup"><span data-stu-id="2c03e-116">Policy nudges</span></span>  <br/> | <ul><li><span data-ttu-id="2c03e-117">Политика сдвиг для отображения в клиенте.</span><span class="sxs-lookup"><span data-stu-id="2c03e-117">Policy nudges for display in your client.</span></span></li></ul> |
|<span data-ttu-id="2c03e-118">Почтовые подсказки</span><span class="sxs-lookup"><span data-stu-id="2c03e-118">Mail tips</span></span>  <br/> | <ul><li><span data-ttu-id="2c03e-119">Значение, указывающее, включены ли почтовые подсказки.</span><span class="sxs-lookup"><span data-stu-id="2c03e-119">A value that indicates whether mail tips are enabled.</span></span></li><li><span data-ttu-id="2c03e-120">Максимальное количество получателей каждого запроса.</span><span class="sxs-lookup"><span data-stu-id="2c03e-120">The maximum number of recipients per request.</span></span></li><li><span data-ttu-id="2c03e-121">Максимальный размер сообщения.</span><span class="sxs-lookup"><span data-stu-id="2c03e-121">The maximum message size.</span></span></li><li><span data-ttu-id="2c03e-122">Большая аудитория пороговое значение.</span><span class="sxs-lookup"><span data-stu-id="2c03e-122">The large audience threshold.</span></span></li><li><span data-ttu-id="2c03e-123">Значение, указывающее, отображается ли число внешних получателей.</span><span class="sxs-lookup"><span data-stu-id="2c03e-123">A value that indicates whether the number of external recipients is shown.</span></span></li><li><span data-ttu-id="2c03e-124">Список внутренних доменов.</span><span class="sxs-lookup"><span data-stu-id="2c03e-124">A list of internal domains.</span></span></li><li><span data-ttu-id="2c03e-125">Значение, указывающее, включены ли подсказки политики.</span><span class="sxs-lookup"><span data-stu-id="2c03e-125">A value that indicates whether policy tips are enabled.</span></span></li><li><span data-ttu-id="2c03e-126">Порога ограничения большие аудитории, указывающие считается большое количество получателей почты.</span><span class="sxs-lookup"><span data-stu-id="2c03e-126">The large audience cap threshold for indicating whether your mail is considered to have a large number of recipients.</span></span>  </li></ul>|
|<span data-ttu-id="2c03e-127">Правила защиты</span><span class="sxs-lookup"><span data-stu-id="2c03e-127">Protection rules</span></span>  <br/> | <ul><li><span data-ttu-id="2c03e-128">Настройка правил защиты для вашего клиента.</span><span class="sxs-lookup"><span data-stu-id="2c03e-128">Protection rules setup for your client.</span></span></li><li><span data-ttu-id="2c03e-129">Список доменов, которые являются внутренними для вашей организации.</span><span class="sxs-lookup"><span data-stu-id="2c03e-129">A list of domains that are internal to your organization.</span></span>  </li></ul> |
   
## <a name="code-example-get-service-configuration-information-for-mail-tips-by-using-ews"></a><span data-ttu-id="2c03e-130">Пример кода: получение сведений о конфигурации службы для подсказки электронной почты с помощью веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="2c03e-130">Code example: Get service configuration information for mail tips by using EWS</span></span>

<span data-ttu-id="2c03e-131">В следующем примере кода используется [операция GetServiceConfiguration](http://msdn.microsoft.com/library/070cbfe5-325a-4955-8e4a-8230ea0459a7%28Office.15%29.aspx) для запроса сведений о конфигурации службы для подсказки.</span><span class="sxs-lookup"><span data-stu-id="2c03e-131">The following code example uses the [GetServiceConfiguration operation](http://msdn.microsoft.com/library/070cbfe5-325a-4955-8e4a-8230ea0459a7%28Office.15%29.aspx) to request service configuration information for mail tips.</span></span> <span data-ttu-id="2c03e-132">Можно запросить дополнительные сведения о конфигурации, добавив дополнительные элементы [имя_конфигурации](http://msdn.microsoft.com/library/3b524a2f-9c6b-4550-9f3d-f78d176b0f7b%28Office.15%29.aspx) на разные значения.</span><span class="sxs-lookup"><span data-stu-id="2c03e-132">You can request additional service configuration information by adding more [ConfigurationName](http://msdn.microsoft.com/library/3b524a2f-9c6b-4550-9f3d-f78d176b0f7b%28Office.15%29.aspx) elements with different values.</span></span> 
  
```cs
private static void GetServiceConfiguration(ExchangeService service, NetworkCredential creds)
{ 
  // XML for the GetServiceConfiguration request SOAP envelope for mail tips configuration information.
  const string getServiceConfigurationRequest = 
    "<?xml version=\"1.0\" encoding=\"utf-8\"?>\n" +
    "<soap:Envelope xmlns:xsi=\"http://www.w3.org/2001/XMLSchema-instance\"\n" +
    "               xmlns:m=\"http://schemas.microsoft.com/exchange/services/2006/messages\"\n" +
    "               xmlns:t=\"http://schemas.microsoft.com/exchange/services/2006/types\" \n" +
    "               xmlns:soap=\"http://schemas.xmlsoap.org/soap/envelope/\"\n" +
    "               xmlns:xs=\"http://www.w3.org/2001/XMLSchema\">\n" +
    "  <soap:Header>\n" +
    "    <t:RequestServerVersion Version=\"Exchange2013\" />\n" +
    "  </soap:Header>\n" +
    "  <soap:Body>\n" +
    "    <m:GetServiceConfiguration>\n" +
    "      <m:ActingAs>\n" +
    "        <t:EmailAddress>user1@contoso.com</t:EmailAddress>\n" +
    "        <t:RoutingType>SMTP</t:RoutingType>\n" +
    "      </m:ActingAs>\n" +
    "      <m:RequestedConfiguration>\n" +
    "        <m:ConfigurationName>MailTips</m:ConfigurationName>\n" +
    "      </m:RequestedConfiguration>\n" +
    "    </m:GetServiceConfiguration>\n" +
    "  </soap:Body>\n" +
    "</soap:Envelope>";
  // Encoded GetServiceConfiguration operation request.
  byte[] payload = System.Text.Encoding.UTF8.GetBytes(getServiceConfigurationRequest);
  try
  {
    HttpWebRequest request = (HttpWebRequest)WebRequest.Create(service.Url);
    request.AllowAutoRedirect = false;
    request.Credentials = creds;
    request.Method = "POST";
    request.ContentType = "text/xml";
    Stream requestStream = request.GetRequestStream();
    requestStream.Write(payload, 0, payload.Length);
    requestStream.Close();
    HttpWebResponse response = (HttpWebResponse)request.GetResponse();
    if (response.StatusCode == HttpStatusCode.OK)
    {
      Stream responseStream = response.GetResponseStream();
      StreamReader reader = new StreamReader(responseStream);
      string responseFromServer = reader.ReadToEnd();
      Console.WriteLine("You will need to parse this response to get the configuration information:\n\n" + responseFromServer);
      reader.Close();
      responseStream.Close();
    }
    else
      throw new WebException(response.StatusDescription);
          
  }
  catch (WebException e)
  {
    Console.WriteLine(e.Message);
  }
}

```

## <a name="next-steps"></a><span data-ttu-id="2c03e-133">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="2c03e-133">Next steps</span></span>

<span data-ttu-id="2c03e-134">После запроса сведений о конфигурации службы, используйте [класс XmlDocument](http://msdn.microsoft.com/en-us/library/system.xml.xmldocument.aspx) для загрузки ответа XML, поэтому может выполнять синтаксический анализ его.</span><span class="sxs-lookup"><span data-stu-id="2c03e-134">After you request service configuration information, use the [XmlDocument class](http://msdn.microsoft.com/en-us/library/system.xml.xmldocument.aspx) to load the response XML so that you can parse it.</span></span> <span data-ttu-id="2c03e-135">Затем, в зависимости от используемого сценария выполните одно из следующих действий.</span><span class="sxs-lookup"><span data-stu-id="2c03e-135">Then, depending on your scenario, you can do one of the following:</span></span> 
  
- <span data-ttu-id="2c03e-136">Чтобы получить почтовые подсказки для клиентских приложений, в котором отображается для пользователей с помощью [GetMailTips операции](http://msdn.microsoft.com/library/025483ec-a9f3-4735-8a95-d26e30ea7974%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="2c03e-136">Use the [GetMailTips operation](http://msdn.microsoft.com/library/025483ec-a9f3-4735-8a95-d26e30ea7974%28Office.15%29.aspx) to get mail tips for client applications to display to users.</span></span> 
    
- <span data-ttu-id="2c03e-137">Если этот параметр включен единой системы обмена СООБЩЕНИЯМИ, [Узнайте, как для воспроизведения элементы почтовых ящиков](http://blogs.msdn.com/b/exchangedev/archive/2009/11/05/play-exchange-2010-mailbox-items-on-your-phone-by-using-the-ews-managed-api.aspx) через телефон.</span><span class="sxs-lookup"><span data-stu-id="2c03e-137">If UM is enabled, [learn about how to play mailbox items](http://blogs.msdn.com/b/exchangedev/archive/2009/11/05/play-exchange-2010-mailbox-items-on-your-phone-by-using-the-ews-managed-api.aspx) over your phone.</span></span> 
    
## <a name="see-also"></a><span data-ttu-id="2c03e-138">См. также</span><span class="sxs-lookup"><span data-stu-id="2c03e-138">See also</span></span>

- [<span data-ttu-id="2c03e-139">Параметры конфигурации для веб-службах Exchange</span><span class="sxs-lookup"><span data-stu-id="2c03e-139">Configuration options for EWS in Exchange</span></span>](configuration-options-for-ews-in-exchange.md)    
- [<span data-ttu-id="2c03e-140">Настройка приложения веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="2c03e-140">Setting up your EWS application</span></span>](setting-up-your-ews-application.md)    
- [<span data-ttu-id="2c03e-141">Разработка клиентов веб-служб для Exchange</span><span class="sxs-lookup"><span data-stu-id="2c03e-141">Develop web service clients for Exchange</span></span>](develop-web-service-clients-for-exchange.md)
    

