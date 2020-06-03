---
title: Получение сведений о конфигурации службы с помощью EWS в Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 9379740a-96e1-490d-a229-0f9937c548d2
description: Сведения о том, как получить сведения о конфигурации служб единой системы обмена сообщениями, почтовых ящиков, советах и правилах защиты от EWS в Exchange.
ms.openlocfilehash: 7546d9524f1e004eda2bdc55687fb44beafa44af
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44528008"
---
# <a name="get-service-configuration-information-by-using-ews-in-exchange"></a><span data-ttu-id="a16e1-103">Получение сведений о конфигурации службы с помощью EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="a16e1-103">Get service configuration information by using EWS in Exchange</span></span>

<span data-ttu-id="a16e1-104">Сведения о том, как получить сведения о конфигурации служб единой системы обмена сообщениями, почтовых ящиков, советах и правилах защиты от EWS в Exchange.</span><span class="sxs-lookup"><span data-stu-id="a16e1-104">Find out how to get service configuration information for UM, policy nudges, mail tips, and protection rules from EWS in Exchange.</span></span>
  
<span data-ttu-id="a16e1-105">Работает ли ваше приложение EWS с единой системой обмена сообщениями, сдвигами политики, советами по электронной почте и правилами защиты?</span><span class="sxs-lookup"><span data-stu-id="a16e1-105">Does your EWS application work with Unified Messaging (UM), policy nudges, mail tips, or protection rules?</span></span> <span data-ttu-id="a16e1-106">В этом случае приложению потребуется вызвать [операцию GetServiceConfiguration](https://msdn.microsoft.com/library/070cbfe5-325a-4955-8e4a-8230ea0459a7%28Office.15%29.aspx) для получения необходимых сведений о конфигурации службы.</span><span class="sxs-lookup"><span data-stu-id="a16e1-106">If so, your application will need to call the [GetServiceConfiguration operation](https://msdn.microsoft.com/library/070cbfe5-325a-4955-8e4a-8230ea0459a7%28Office.15%29.aspx) to get the service configuration information that it needs.</span></span> <span data-ttu-id="a16e1-107">Операция **GetServiceConfiguration** возвращает сведения о конфигурации, характерные для каждой из этих функций EWS.</span><span class="sxs-lookup"><span data-stu-id="a16e1-107">The **GetServiceConfiguration** operation returns configuration information that is specific to each of these EWS features.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="a16e1-108">Управляемый API EWS не реализует эту функцию.</span><span class="sxs-lookup"><span data-stu-id="a16e1-108">The EWS Managed API does not implement this functionality.</span></span> 
  
<span data-ttu-id="a16e1-109">**Таблица 1. Сведения о конфигурации, возвращаемые операцией GetServiceConfiguration**</span><span class="sxs-lookup"><span data-stu-id="a16e1-109">**Table 1. Configuration information that the GetServiceConfiguration operation returns**</span></span>

|<span data-ttu-id="a16e1-110">Функция EWS</span><span class="sxs-lookup"><span data-stu-id="a16e1-110">EWS feature</span></span>|<span data-ttu-id="a16e1-111">Операция GetServiceConfiguration возвращает...</span><span class="sxs-lookup"><span data-stu-id="a16e1-111">GetServiceConfiguration operation returns…</span></span>|
|:-----|:-----|
|<span data-ttu-id="a16e1-112">UM</span><span class="sxs-lookup"><span data-stu-id="a16e1-112">UM</span></span>  <br/> | <ul><li><span data-ttu-id="a16e1-113">Значение, указывающее, включена ли единая система обмена сообщениями.</span><span class="sxs-lookup"><span data-stu-id="a16e1-113">A value that indicates whether UM is enabled.</span></span></li><li><span data-ttu-id="a16e1-114">Значение, указывающее, включено ли проигрывание на телефоне.</span><span class="sxs-lookup"><span data-stu-id="a16e1-114">A value that indicates whether play on phone is enabled.</span></span></li><li><span data-ttu-id="a16e1-115">Строка набора номера для воспроизводимого по телефону.</span><span class="sxs-lookup"><span data-stu-id="a16e1-115">The play on phone dial string.</span></span></li></ul> |
|<span data-ttu-id="a16e1-116">Сигналы политики</span><span class="sxs-lookup"><span data-stu-id="a16e1-116">Policy nudges</span></span>  <br/> | <ul><li><span data-ttu-id="a16e1-117">Сигналы политики для отображения в клиенте.</span><span class="sxs-lookup"><span data-stu-id="a16e1-117">Policy nudges for display in your client.</span></span></li></ul> |
|<span data-ttu-id="a16e1-118">Советы по использованию электронной почты</span><span class="sxs-lookup"><span data-stu-id="a16e1-118">Mail tips</span></span>  <br/> | <ul><li><span data-ttu-id="a16e1-119">Значение, указывающее, включены ли подсказки для почты.</span><span class="sxs-lookup"><span data-stu-id="a16e1-119">A value that indicates whether mail tips are enabled.</span></span></li><li><span data-ttu-id="a16e1-120">Максимальное количество получателей на запрос.</span><span class="sxs-lookup"><span data-stu-id="a16e1-120">The maximum number of recipients per request.</span></span></li><li><span data-ttu-id="a16e1-121">Максимальный размер сообщения.</span><span class="sxs-lookup"><span data-stu-id="a16e1-121">The maximum message size.</span></span></li><li><span data-ttu-id="a16e1-122">Пороговое значение для большой аудитории.</span><span class="sxs-lookup"><span data-stu-id="a16e1-122">The large audience threshold.</span></span></li><li><span data-ttu-id="a16e1-123">Значение, указывающее, отображается ли число внешних получателей.</span><span class="sxs-lookup"><span data-stu-id="a16e1-123">A value that indicates whether the number of external recipients is shown.</span></span></li><li><span data-ttu-id="a16e1-124">Список внутренних доменов.</span><span class="sxs-lookup"><span data-stu-id="a16e1-124">A list of internal domains.</span></span></li><li><span data-ttu-id="a16e1-125">Значение, указывающее, включены ли подсказки политики.</span><span class="sxs-lookup"><span data-stu-id="a16e1-125">A value that indicates whether policy tips are enabled.</span></span></li><li><span data-ttu-id="a16e1-126">Пороговое значение ограничения для большой аудитории, указывающее, имеет ли ваша почта большое количество получателей.</span><span class="sxs-lookup"><span data-stu-id="a16e1-126">The large audience cap threshold for indicating whether your mail is considered to have a large number of recipients.</span></span>  </li></ul>|
|<span data-ttu-id="a16e1-127">Правила защиты</span><span class="sxs-lookup"><span data-stu-id="a16e1-127">Protection rules</span></span>  <br/> | <ul><li><span data-ttu-id="a16e1-128">Настройка правил защиты для клиента.</span><span class="sxs-lookup"><span data-stu-id="a16e1-128">Protection rules setup for your client.</span></span></li><li><span data-ttu-id="a16e1-129">Список доменов, которые являются внутренними для Организации.</span><span class="sxs-lookup"><span data-stu-id="a16e1-129">A list of domains that are internal to your organization.</span></span>  </li></ul> |
   
## <a name="code-example-get-service-configuration-information-for-mail-tips-by-using-ews"></a><span data-ttu-id="a16e1-130">Пример кода: получение сведений о конфигурации службы для советов по электронной почте с помощью EWS</span><span class="sxs-lookup"><span data-stu-id="a16e1-130">Code example: Get service configuration information for mail tips by using EWS</span></span>

<span data-ttu-id="a16e1-131">В следующем примере кода показано, как использовать [операцию GetServiceConfiguration](https://msdn.microsoft.com/library/070cbfe5-325a-4955-8e4a-8230ea0459a7%28Office.15%29.aspx) для запроса сведений о конфигурации службы для советов по использованию электронной почты.</span><span class="sxs-lookup"><span data-stu-id="a16e1-131">The following code example uses the [GetServiceConfiguration operation](https://msdn.microsoft.com/library/070cbfe5-325a-4955-8e4a-8230ea0459a7%28Office.15%29.aspx) to request service configuration information for mail tips.</span></span> <span data-ttu-id="a16e1-132">Вы можете запросить дополнительные сведения о конфигурации службы, добавив дополнительные элементы [configurationName](https://msdn.microsoft.com/library/3b524a2f-9c6b-4550-9f3d-f78d176b0f7b%28Office.15%29.aspx) с разными значениями.</span><span class="sxs-lookup"><span data-stu-id="a16e1-132">You can request additional service configuration information by adding more [ConfigurationName](https://msdn.microsoft.com/library/3b524a2f-9c6b-4550-9f3d-f78d176b0f7b%28Office.15%29.aspx) elements with different values.</span></span> 
  
```cs
private static void GetServiceConfiguration(ExchangeService service, NetworkCredential creds)
{ 
  // XML for the GetServiceConfiguration request SOAP envelope for mail tips configuration information.
  const string getServiceConfigurationRequest = 
    "<?xml version=\"1.0\" encoding=\"utf-8\"?>\n" +
    "<soap:Envelope xmlns:xsi=\"http://www.w3.org/2001/XMLSchema-instance\"\n" +
    "               xmlns:m=\"https://schemas.microsoft.com/exchange/services/2006/messages\"\n" +
    "               xmlns:t=\"https://schemas.microsoft.com/exchange/services/2006/types\" \n" +
    "               xmlns:soap=\"https://schemas.xmlsoap.org/soap/envelope/\"\n" +
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

## <a name="next-steps"></a><span data-ttu-id="a16e1-133">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="a16e1-133">Next steps</span></span>

<span data-ttu-id="a16e1-134">После запроса сведений о конфигурации службы используйте [класс XmlDocument](https://msdn.microsoft.com/library/system.xml.xmldocument.aspx) для загрузки отклика XML, чтобы его можно было проанализировать.</span><span class="sxs-lookup"><span data-stu-id="a16e1-134">After you request service configuration information, use the [XmlDocument class](https://msdn.microsoft.com/library/system.xml.xmldocument.aspx) to load the response XML so that you can parse it.</span></span> <span data-ttu-id="a16e1-135">В зависимости от сценария можно выполнить одно из следующих действий:</span><span class="sxs-lookup"><span data-stu-id="a16e1-135">Then, depending on your scenario, you can do one of the following:</span></span> 
  
- <span data-ttu-id="a16e1-136">Используйте [операцию](https://msdn.microsoft.com/library/025483ec-a9f3-4735-8a95-d26e30ea7974%28Office.15%29.aspx) по подсказке для получения советов по электронной почте для клиентских приложений, отображаемых для пользователей.</span><span class="sxs-lookup"><span data-stu-id="a16e1-136">Use the [GetMailTips operation](https://msdn.microsoft.com/library/025483ec-a9f3-4735-8a95-d26e30ea7974%28Office.15%29.aspx) to get mail tips for client applications to display to users.</span></span> 
    
- <span data-ttu-id="a16e1-137">Если включена поддержка единой системы обмена сообщениями, [Узнайте, как проигрывать элементы почтового ящика](https://blogs.msdn.com/b/exchangedev/archive/2009/11/05/play-exchange-2010-mailbox-items-on-your-phone-by-using-the-ews-managed-api.aspx) по телефону.</span><span class="sxs-lookup"><span data-stu-id="a16e1-137">If UM is enabled, [learn about how to play mailbox items](https://blogs.msdn.com/b/exchangedev/archive/2009/11/05/play-exchange-2010-mailbox-items-on-your-phone-by-using-the-ews-managed-api.aspx) over your phone.</span></span> 
    
## <a name="see-also"></a><span data-ttu-id="a16e1-138">См. также</span><span class="sxs-lookup"><span data-stu-id="a16e1-138">See also</span></span>

- [<span data-ttu-id="a16e1-139">Настройка параметров для EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="a16e1-139">Configuration options for EWS in Exchange</span></span>](configuration-options-for-ews-in-exchange.md)    
- [<span data-ttu-id="a16e1-140">Настройка приложения веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="a16e1-140">Setting up your EWS application</span></span>](setting-up-your-ews-application.md)    
- [<span data-ttu-id="a16e1-141">Разработка клиентов веб-служб для Exchange</span><span class="sxs-lookup"><span data-stu-id="a16e1-141">Develop web service clients for Exchange</span></span>](develop-web-service-clients-for-exchange.md)
    

