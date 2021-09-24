---
title: Получите сведения о конфигурации службы с помощью EWS в Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.localizationpriority: medium
ms.assetid: 9379740a-96e1-490d-a229-0f9937c548d2
description: Сведения о том, как получить сведения о конфигурации службы для системы электронной почты, подсказки политики, советы по почте и правила защиты от EWS в Exchange.
ms.openlocfilehash: 30d4058104726c79f473a88a09398689675b988d
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59513173"
---
# <a name="get-service-configuration-information-by-using-ews-in-exchange"></a>Получите сведения о конфигурации службы с помощью EWS в Exchange

Сведения о том, как получить сведения о конфигурации службы для системы электронной почты, подсказки политики, советы по почте и правила защиты от EWS в Exchange.
  
Работает ли ваше приложение EWS с единой системы обмена сообщениями(единой системы обмена сообщениями), подгонами политики, советами по почте или правилами защиты? Если это так, вашему приложению потребуется вызвать [операцию GetServiceConfiguration,](https://msdn.microsoft.com/library/070cbfe5-325a-4955-8e4a-8230ea0459a7%28Office.15%29.aspx) чтобы получить необходимые ему сведения о конфигурации службы. Операция **GetServiceConfiguration** возвращает сведения о конфигурации, специфические для каждой из этих функций EWS. 
  
> [!NOTE]
> Управляемый API EWS не реализует эту функцию. 
  
**Таблица 1. Сведения о конфигурации, возвращаемой операцией GetServiceConfiguration**

|Функция EWS|Операция GetServiceConfiguration возвращается...|
|:-----|:-----|
|Um  <br/> | <ul><li>Значение, которое указывает, включена ли ОМ.</li><li>Значение, которое указывает, включена ли игра на телефоне.</li><li>Игра на телефонной строке набора.</li></ul> |
|Подталкивает к политике  <br/> | <ul><li>Политика подталкивает для отображения в клиенте.</li></ul> |
|Советы по использованию электронной почты  <br/> | <ul><li>Значение, которое указывает, включены ли советы почты.</li><li>Максимальное число получателей по запросу.</li><li>Максимальный размер сообщения.</li><li>Порог большой аудитории.</li><li>Значение, которое указывает, отображается ли число внешних получателей.</li><li>Список внутренних доменов.</li><li>Значение, которое указывает, включены ли советы политики.</li><li>Порог большой аудитории для указания того, считается ли ваша почта большим числом получателей.  </li></ul>|
|Правила защиты  <br/> | <ul><li>Настройка правил защиты для клиента.</li><li>Список доменов, которые являются внутренними для организации.  </li></ul> |
   
## <a name="code-example-get-service-configuration-information-for-mail-tips-by-using-ews"></a>Пример кода. Сведения о конфигурации службы для советов по почте с помощью EWS

В следующем примере кода операция [GetServiceConfiguration](https://msdn.microsoft.com/library/070cbfe5-325a-4955-8e4a-8230ea0459a7%28Office.15%29.aspx) используется для запроса сведений о конфигурации служб для подсказок почты. Вы можете запросить дополнительные сведения о конфигурации службы, добавив дополнительные элементы [ConfigurationName](https://msdn.microsoft.com/library/3b524a2f-9c6b-4550-9f3d-f78d176b0f7b%28Office.15%29.aspx) с различными значениями. 
  
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

## <a name="next-steps"></a>Дальнейшие действия

После запроса сведений о конфигурации службы используйте [класс XmlDocument](https://msdn.microsoft.com/library/system.xml.xmldocument.aspx) для загрузки XML отклика, чтобы можно было его разбереть. Затем в зависимости от сценария можно сделать один из следующих вариантов: 
  
- Используйте операцию [GetMailTips,](https://msdn.microsoft.com/library/025483ec-a9f3-4735-8a95-d26e30ea7974%28Office.15%29.aspx) чтобы получить советы по почте для отображения пользователям клиентских приложений. 
    
- Если включена электронная почта, [узнайте, как играть в](https://blogs.msdn.com/b/exchangedev/archive/2009/11/05/play-exchange-2010-mailbox-items-on-your-phone-by-using-the-ews-managed-api.aspx) элементы почтовых ящиков по телефону. 
    
## <a name="see-also"></a>См. также

- [Настройка параметров для EWS в Exchange](configuration-options-for-ews-in-exchange.md)    
- [Настройка приложения веб-служб Exchange](setting-up-your-ews-application.md)    
- [Разработка клиентов веб-служб для Exchange](develop-web-service-clients-for-exchange.md)
    

