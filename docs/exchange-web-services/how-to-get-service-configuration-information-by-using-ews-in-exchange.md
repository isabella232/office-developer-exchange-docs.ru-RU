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
# <a name="get-service-configuration-information-by-using-ews-in-exchange"></a>Получение сведений о конфигурации службы с помощью веб-служб Exchange в Exchange

Узнайте, как получить сведения о конфигурации службы для единой системы обмена СООБЩЕНИЯМИ, будильника политики, почтовые подсказки и правила защиты от веб-служб Exchange в Exchange.
  
Работает ли приложение веб-служб Exchange с единой системы обмена сообщениями (UM), политики будильника, почтовые подсказки или правила защиты? Если это так, приложения необходимо вызвать [GetServiceConfiguration операции](http://msdn.microsoft.com/library/070cbfe5-325a-4955-8e4a-8230ea0459a7%28Office.15%29.aspx) для получения сведений о конфигурации службы, необходимые. Операция **GetServiceConfiguration** возвращает сведения о конфигурации, характерные для каждой из этих функций веб-служб Exchange. 
  
> [!NOTE]
> Управляемый API EWS не реализует эту функцию. 
  
**В таблице 1. Сведения о конфигурации, операция GetServiceConfiguration возвращает**

|Компонент веб-служб Exchange|Возвращает операции GetServiceConfiguration...|
|:-----|:-----|
|ЕДИНАЯ СИСТЕМА ОБМЕНА СООБЩЕНИЯМИ  <br/> | <ul><li>Значение, указывающее, включено ли единой системы обмена СООБЩЕНИЯМИ.</li><li>Значение, указывающее, включено ли воспроизвести на телефоне.</li><li>Воспроизвести на строку номера телефона.</li></ul> |
|Политика будильника  <br/> | <ul><li>Политика сдвиг для отображения в клиенте.</li></ul> |
|Почтовые подсказки  <br/> | <ul><li>Значение, указывающее, включены ли почтовые подсказки.</li><li>Максимальное количество получателей каждого запроса.</li><li>Максимальный размер сообщения.</li><li>Большая аудитория пороговое значение.</li><li>Значение, указывающее, отображается ли число внешних получателей.</li><li>Список внутренних доменов.</li><li>Значение, указывающее, включены ли подсказки политики.</li><li>Порога ограничения большие аудитории, указывающие считается большое количество получателей почты.  </li></ul>|
|Правила защиты  <br/> | <ul><li>Настройка правил защиты для вашего клиента.</li><li>Список доменов, которые являются внутренними для вашей организации.  </li></ul> |
   
## <a name="code-example-get-service-configuration-information-for-mail-tips-by-using-ews"></a>Пример кода: получение сведений о конфигурации службы для подсказки электронной почты с помощью веб-служб Exchange

В следующем примере кода используется [операция GetServiceConfiguration](http://msdn.microsoft.com/library/070cbfe5-325a-4955-8e4a-8230ea0459a7%28Office.15%29.aspx) для запроса сведений о конфигурации службы для подсказки. Можно запросить дополнительные сведения о конфигурации, добавив дополнительные элементы [имя_конфигурации](http://msdn.microsoft.com/library/3b524a2f-9c6b-4550-9f3d-f78d176b0f7b%28Office.15%29.aspx) на разные значения. 
  
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

После запроса сведений о конфигурации службы, используйте [класс XmlDocument](http://msdn.microsoft.com/en-us/library/system.xml.xmldocument.aspx) для загрузки ответа XML, поэтому может выполнять синтаксический анализ его. Затем, в зависимости от используемого сценария выполните одно из следующих действий. 
  
- Чтобы получить почтовые подсказки для клиентских приложений, в котором отображается для пользователей с помощью [GetMailTips операции](http://msdn.microsoft.com/library/025483ec-a9f3-4735-8a95-d26e30ea7974%28Office.15%29.aspx) . 
    
- Если этот параметр включен единой системы обмена СООБЩЕНИЯМИ, [Узнайте, как для воспроизведения элементы почтовых ящиков](http://blogs.msdn.com/b/exchangedev/archive/2009/11/05/play-exchange-2010-mailbox-items-on-your-phone-by-using-the-ews-managed-api.aspx) через телефон. 
    
## <a name="see-also"></a>См. также

- [Параметры конфигурации для веб-службах Exchange](configuration-options-for-ews-in-exchange.md)    
- [Настройка приложения веб-служб Exchange](setting-up-your-ews-application.md)    
- [Разработка клиентов веб-служб для Exchange](develop-web-service-clients-for-exchange.md)
    

