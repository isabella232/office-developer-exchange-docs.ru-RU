---
title: Получение параметров домена с сервера Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 2f9acb81-5135-4f72-94e8-65c235d725e6
description: Узнайте, как получить параметры домена с сервера Exchange Server с помощью службы автообнаружения.
ms.openlocfilehash: 0dd990cc82762936e7827115685ce0178eafb5ae
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761012"
---
# <a name="get-domain-settings-from-an-exchange-server"></a>Получение параметров домена с сервера Exchange

Узнайте, как получить параметры домена с сервера Exchange Server с помощью службы автообнаружения.
  
Сведения о конфигурации для домена электронной почты можно получить с помощью службы автообнаружения. Служба автообнаружения предоставляет приложению процесс для подключения к правильной конечной точке службы для определенного домена.
  
Для доступа к службе автообнаружения можно использовать одну из следующих технологий разработки:
  
- Управляемый API веб-служб Exchange (EWS)
    
- EWS
    
    Если вы используете EWS, вы можете использовать следующие методы для получения параметров пользователя:
    
  - Служба автообнаружения на основе SOAP
    
  - Служба автообнаружения XML (POX)
    
  - Автоматически созданный прокси-сервер, созданный службой автообнаружения SOAP или XML
    
    Дополнительные сведения об этих методах см. в разделе [автообнаружения для Exchange](autodiscover-for-exchange.md).
    
Управляемый API EWS предоставляет интерфейс на основе объектов для получения параметров пользователя. Если клиентское приложение использует управляемый код, мы рекомендуем использовать управляемый API EWS. Интерфейс управляемого API EWS лучше оптимизирован для простой объектной модели по сравнению с обычным автоматически созданным прокси-сервером веб-службы. 
  
Если вы используете EWS, мы рекомендуем использовать службу автообнаружения SOAP, так как она поддерживает более широкий набор функций, чем служба автообнаружения POX.
  
Служба автообнаружения возвращает только запрошенные параметры конфигурации. В следующей таблице перечислены параметры конфигурации домена, которые может возвращать служба автообнаружения.
  
**Таблица 1: параметры конфигурации домена**

|**Параметр конфигурации**|**Описание**|
|:-----|:-----|
|екстерналевсурл  <br/> |Внешний URL-адрес для EWS.  <br/> |
|екстерналевсверсион  <br/> |Версия сервера Exchange Server, на котором размещается URL-адрес EWS.  <br/> |
   
## <a name="prerequisites-for-getting-domain-settings"></a>Необходимые условия для настройки параметров домена
<a name="bk_Prereq"> </a>

Перед созданием приложения, которое подключается к службе автообнаружения для получения параметров домена, убедитесь, что у вас есть доступ к следующим:
  
- Exchange Online, Exchange Online в составе Office 365, или сервер с версией Exchange, начинающейся с Exchange 2007. Если вы используете службу автообнаружения на основе SOAP для EWS, сервер, на котором работает версия Exchange, начиная с Exchange 2010.
    
- Сервер Exchange, настроенный для приема подключений из клиентского приложения. Сведения о настройке сервера Exchange Server можно найти [в статье Управление доступом клиентского приложения к EWS в Exchange](controlling-client-application-access-to-ews-in-exchange.md).
    
- Учетная запись, которая авторизована для использования EWS. Сведения о настройке учетной записи см [в разделе Управление доступом клиентского приложения к EWS в Exchange](controlling-client-application-access-to-ews-in-exchange.md).
    
> [!NOTE]
> Если вы используете управляемый API EWS, в некоторых обстоятельствах необходимо предоставить обратный вызов проверки сертификата. Кроме того, вам может потребоваться обратный вызов проверки сертификата со всеми созданными библиотеками прокси, например, созданными Visual Studio. Дополнительные сведения см. [в статье Проверка сертификата сервера для управляемого API EWS](how-to-validate-a-server-certificate-for-the-ews-managed-api.md). 
  
### <a name="core-concepts-for-getting-domain-settings"></a>Основные понятия, связанные с извлечением параметров домена
<a name="bk_Core"> </a>

Прежде чем использовать службу автообнаружения для получения параметров домена, необходимо ознакомиться с концепциями, приведенными в следующей таблице.
  
|**Концепция**|**Описание**|
|:-----|:-----|
|[Автообнаружение для Exchange](autodiscover-for-exchange.md) <br/> |Предоставляет общие сведения о работе службы автообнаружения.  <br/> |
|[Поиск точек соединения с помощью службы автообнаружения](how-to-use-autodiscover-to-find-connection-points.md) <br/> |Описывает процесс, используемый службой автообнаружения для перенаправления клиентского приложения в правильную конечную точку службы.  <br/> |
   
Если вы используете управляемый API EWS, вы используете класс [Microsoft. Exchange. WebServices. Data. ExchangeService](http://msdn.microsoft.com/en-us/library/exchange/dd635811%28v=exchg.80%29.aspx) в пространстве имен [Microsoft. Exchange. WebServices. Data](http://msdn.microsoft.com/en-us/library/exchange/dd633907%28v=exchg.80%29.aspx) для управления подключением к EWS. В примерах кода, приведенных в этом разделе, предполагается, что вы ссылаетесь на следующие пространства имен в коде: 
  
- **System.Net**
    
- **Microsoft. Exchange. WebServices. Data. ExchangeService**
    
## <a name="get-domain-settings-by-using-the-ews-managed-api"></a>Получение параметров домена с помощью управляемого API EWS
<a name="bk_Managed"> </a>

Если вы используете управляемый API EWS, вы можете использовать метод [Microsoft. Exchange. WebServices. Data. аутодисковерсеттингс. GetUserSettings](http://msdn.microsoft.com/en-us/library/exchange/microsoft.exchange.webservices.autodiscover.autodiscoverservice.getusersettings%28v=exchg.80%29.aspx) объекта [Microsoft. Exchange. WebServices. AutodiscoverService](http://msdn.microsoft.com/en-us/library/exchange/dd634321%28v=exchg.80%29.aspx) , чтобы создать запрос, который получает сведения о конфигурации для домена, как показано в следующем примере. В этом примере запрашиваются только некоторые из возможных параметров домена, а с сервера возвращаются только запрошенные параметры. 
  
```cs
AutodiscoverService autodiscoverService = new AutodiscoverService("domain.contoso.com");
autodiscoverService.Credentials = new NetworkCredential("User1", "password", "domain.contoso.com");
// Submit a request and get the settings. The response contains only the
// settings that are requested, if they exist.
GetDomainSettingsResponse domainresponse = autodiscoverService.GetDomainSettings(
    "domain",
    ExchangeVersion.Exchang2013,
    DomainSettingName.ExternalEwsUrl,
    DomainSettingName.ExternalEwsVersion);
```

Вы можете проанализировать коллекцию, возвращаемую для доступа к каждой из этих ключей и значений. В приведенном ниже примере показано, как выполнить анализ каждого возвращаемого элемента и отобразить имя и значение каждой из этих ключей и значений.
  
```cs
// Display each retrieved value. The settings are part of a key/value pair.
foreach (KeyValuePair<DomainSettingName, Object> domainsetting in domainresponse.Settings)
{
    Console.WriteLine(domainsetting.Key.ToString() + ": " + domainsetting.Value.ToString());
}
```

Кроме того, вы можете получить значение определенного параметра. В следующем примере отображается параметр **екстерналевсурл** . 
  
```cs
// Display a specific setting, such as ExternalEwsUrl.
Console.WriteLine(domainresponse.Settings[DomainSettingName.ExternalEwsUrl]);
```

## <a name="get-user-settings-by-using-ews-soap-autodiscover"></a>Получение параметров пользователя с помощью автообнаружения SOAP для службы EWS
<a name="bk_SOAP"> </a>

В следующем примере показан SOAP-запрос SOAP для получения параметров домена из службы автообнаружения.
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:a="http://schemas.microsoft.com/exchange/2010/Autodiscover" 
        xmlns:wsa="http://www.w3.org/2005/08/addressing" 
        xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
        xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <a:RequestedServerVersion>Exchange2013</a:RequestedServerVersion>
    <wsa:Action>http://schemas.microsoft.com/exchange/2010/Autodiscover/Autodiscover/GetDomainSettings</wsa:Action>
    <wsa:To>https://autodiscover.exchange.microsoft.com/autodiscover/autodiscover.svc</wsa:To>
  </soap:Header>
  <soap:Body>
    <a:GetDomainSettingsRequestMessage xmlns:a="http://schemas.microsoft.com/exchange/2010/Autodiscover">
      <a:Request>
        <a:Domains>
          <a:Domain>domain</a:Domain>
        </a:Domains>
        <a:RequestedSettings>
          <a:Setting>ExternalEwsUrl</a:Setting>
          <a:Setting>ExternalEwsVersion</a:Setting>
        </a:RequestedSettings>
        <a:RequestedVersion>Exchange2013</a:RequestedVersion>
      </a:Request>
    </a:GetDomainSettingsRequestMessage>
  </soap:Body>
</soap:Envelope>
```

В следующем примере показан ответ XML, возвращенный сервером после синтаксического анализа запроса от клиента.
  
```XML
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/" 
        xmlns:a="http://www.w3.org/2005/08/addressing">
  <s:Header>
    <a:Action s:mustUnderstand="1">http://schemas.microsoft.com/exchange/2010/
          Autodiscover/Autodiscover/GetDomainSettingsResponse</a:Action>
    <h:ServerVersionInfo xmlns:h="http://schemas.microsoft.com/exchange/2010/Autodiscover" 
          xmlns:i="http://www.w3.org/2001/XMLSchema-instance">
      <h:MajorVersion>15</h:MajorVersion>
      <h:MinorVersion>0</h:MinorVersion>
      <h:MajorBuildNumber>160</h:MajorBuildNumber>
      <h:MinorBuildNumber>4</h:MinorBuildNumber>
      <h:Version>Exchange2013</h:Version>
    </h:ServerVersionInfo>
  </s:Header>
  <s:Body>
    <GetDomainSettingsResponseMessage xmlns="http://schemas.microsoft.com/exchange/2010/Autodiscover">
      <Response xmlns:i="http://www.w3.org/2001/XMLSchema-instance">
        <ErrorCode>NoError</ErrorCode>
        <ErrorMessage />
        <DomainResponses>
          <DomainResponse>
            <ErrorCode>NoError</ErrorCode>
            <ErrorMessage>No error.</ErrorMessage>
            <DomainSettingErrors />
            <DomainSettings>
              <DomainSetting i:type="DomainStringSetting">
                <Name>ExternalEwsUrl</Name>
                <Value>https://failover.exchange.microsoft.com/ews/exchange.asmx</Value>
              </DomainSetting>
              <DomainSetting i:type="DomainStringSetting">
                <Name>ExternalEwsVersion</Name>
                <Value>15.00.0085.000</Value>
              </DomainSetting>
            </DomainSettings>
            <RedirectTarget i:nil="true" />
          </DomainResponse>
        </DomainResponses>
      </Response>
    </GetDomainSettingsResponseMessage>
  </s:Body>
</s:Envelope>
```

## <a name="next-steps"></a>Дальнейшие действия
<a name="bk_Next"> </a>

Параметры домена предоставляют основные сведения, необходимые вашему клиенту для подключения к службам EWS. Эти сведения можно использовать для подключения к EWS, а также для получения дополнительных параметров конфигурации для учетной записи электронной почты с сервера. Более подробную информацию можно найти в следующей статье:
  
- [Получение параметров пользователя из Exchange с помощью службы автообнаружения](how-to-get-user-settings-from-exchange-by-using-autodiscover.md)
    
## <a name="see-also"></a>См. также


- [Настройка приложения веб-служб Exchange](setting-up-your-ews-application.md)
    
- [Справочные материалы по веб-службе автообнаружения для Exchange](http://msdn.microsoft.com/library/a01124a8-a8cf-4b80-8625-d7ee05690bca%28Office.15%29.aspx)
    
- [Справка по веб-служб Exchange для Exchange](http://msdn.microsoft.com/library/2a873474-1bb2-4cb1-a556-40e8c4159f4a%28Office.15%29.aspx)
    

