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
# <a name="get-service-configuration-information-by-using-ews-in-exchange"></a>Получение сведений о конфигурации службы с помощью EWS в Exchange

Сведения о том, как получить сведения о конфигурации служб единой системы обмена сообщениями, почтовых ящиков, советах и правилах защиты от EWS в Exchange.
  
Работает ли ваше приложение EWS с единой системой обмена сообщениями, сдвигами политики, советами по электронной почте и правилами защиты? В этом случае приложению потребуется вызвать [операцию GetServiceConfiguration](https://msdn.microsoft.com/library/070cbfe5-325a-4955-8e4a-8230ea0459a7%28Office.15%29.aspx) для получения необходимых сведений о конфигурации службы. Операция **GetServiceConfiguration** возвращает сведения о конфигурации, характерные для каждой из этих функций EWS. 
  
> [!NOTE]
> Управляемый API EWS не реализует эту функцию. 
  
**Таблица 1. Сведения о конфигурации, возвращаемые операцией GetServiceConfiguration**

|Функция EWS|Операция GetServiceConfiguration возвращает...|
|:-----|:-----|
|UM  <br/> | <ul><li>Значение, указывающее, включена ли единая система обмена сообщениями.</li><li>Значение, указывающее, включено ли проигрывание на телефоне.</li><li>Строка набора номера для воспроизводимого по телефону.</li></ul> |
|Сигналы политики  <br/> | <ul><li>Сигналы политики для отображения в клиенте.</li></ul> |
|Советы по использованию электронной почты  <br/> | <ul><li>Значение, указывающее, включены ли подсказки для почты.</li><li>Максимальное количество получателей на запрос.</li><li>Максимальный размер сообщения.</li><li>Пороговое значение для большой аудитории.</li><li>Значение, указывающее, отображается ли число внешних получателей.</li><li>Список внутренних доменов.</li><li>Значение, указывающее, включены ли подсказки политики.</li><li>Пороговое значение ограничения для большой аудитории, указывающее, имеет ли ваша почта большое количество получателей.  </li></ul>|
|Правила защиты  <br/> | <ul><li>Настройка правил защиты для клиента.</li><li>Список доменов, которые являются внутренними для Организации.  </li></ul> |
   
## <a name="code-example-get-service-configuration-information-for-mail-tips-by-using-ews"></a>Пример кода: получение сведений о конфигурации службы для советов по электронной почте с помощью EWS

В следующем примере кода показано, как использовать [операцию GetServiceConfiguration](https://msdn.microsoft.com/library/070cbfe5-325a-4955-8e4a-8230ea0459a7%28Office.15%29.aspx) для запроса сведений о конфигурации службы для советов по использованию электронной почты. Вы можете запросить дополнительные сведения о конфигурации службы, добавив дополнительные элементы [configurationName](https://msdn.microsoft.com/library/3b524a2f-9c6b-4550-9f3d-f78d176b0f7b%28Office.15%29.aspx) с разными значениями. 
  
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

## <a name="next-steps"></a>Дальнейшие действия

После запроса сведений о конфигурации службы используйте [класс XmlDocument](https://msdn.microsoft.com/library/system.xml.xmldocument.aspx) для загрузки отклика XML, чтобы его можно было проанализировать. В зависимости от сценария можно выполнить одно из следующих действий: 
  
- Используйте [операцию](https://msdn.microsoft.com/library/025483ec-a9f3-4735-8a95-d26e30ea7974%28Office.15%29.aspx) по подсказке для получения советов по электронной почте для клиентских приложений, отображаемых для пользователей. 
    
- Если включена поддержка единой системы обмена сообщениями, [Узнайте, как проигрывать элементы почтового ящика](https://blogs.msdn.com/b/exchangedev/archive/2009/11/05/play-exchange-2010-mailbox-items-on-your-phone-by-using-the-ews-managed-api.aspx) по телефону. 
    
## <a name="see-also"></a>См. также

- [Настройка параметров для EWS в Exchange](configuration-options-for-ews-in-exchange.md)    
- [Настройка приложения веб-служб Exchange](setting-up-your-ews-application.md)    
- [Разработка клиентов веб-служб для Exchange](develop-web-service-clients-for-exchange.md)
    

