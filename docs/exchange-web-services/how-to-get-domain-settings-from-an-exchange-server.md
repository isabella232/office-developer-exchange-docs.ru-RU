---
title: Получение параметров домена с сервера Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 2f9acb81-5135-4f72-94e8-65c235d725e6
description: Узнайте, как получить параметры домена с сервера Exchange с помощью службы автообнаружения.
ms.openlocfilehash: 0dd990cc82762936e7827115685ce0178eafb5ae
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761012"
---
# <a name="get-domain-settings-from-an-exchange-server"></a>Получение параметров домена с сервера Exchange

Узнайте, как получить параметры домена с сервера Exchange с помощью службы автообнаружения.
  
Сведения о конфигурации для домен электронной почты можно извлечь с помощью службы автообнаружения. Служба автообнаружения обеспечивает приложение процесс для подключения к конечной точке службы правильный для определенного домена.
  
Можно использовать один из следующих технологиями разработки для доступа к службе автообнаружения:
  
- Веб-служб Exchange (EWS) управляемого интерфейса API
    
- EWS
    
    При использовании веб-служб Exchange, можно использовать следующие методы для получения параметров пользователя:
    
  - Служба автообнаружения на основе SOAP
    
  - Служба автообнаружения XML (POX)
    
  - Прокси-сервер автоматически созданный, созданный из службы SOAP или автоматического обнаружения XML
    
    Дополнительные сведения об этих методов можно [автообнаружения для Exchange](autodiscover-for-exchange.md).
    
Управляемый API веб-служб Exchange предоставляет объектно ориентированный интерфейс для извлечения параметров пользователя. Если клиентское приложение использует управляемый код, мы рекомендуем использовать управляемый API веб-служб Exchange. Чем обычно автоматически созданный прокси веб-службы для простой объектной модели лучше оптимизированный интерфейс управляемый API веб-служб Exchange. 
  
При использовании веб-служб Exchange, рекомендуется использовать службы автообнаружения SOAP, поскольку она поддерживает расширенный набор функциональных возможностей, чем службы автообнаружения POX.
  
Служба автообнаружения возвращать только параметры конфигурации запрошенного. В следующей таблице перечислены параметры конфигурации домена, которые можно вернуть службы автообнаружения.
  
**В таблице 1: Параметры конфигурации домена**

|**Параметр конфигурации**|**Описание**|
|:-----|:-----|
|ExternalEwsUrl  <br/> |Внешний URL-адрес для веб-служб Exchange.  <br/> |
|ExternalEwsVersion  <br/> |Версия Exchange server, на котором размещается URL-адрес веб-служб Exchange.  <br/> |
   
## <a name="prerequisites-for-getting-domain-settings"></a>Необходимые условия для получения параметров домена
<a name="bk_Prereq"> </a>

Перед созданием приложения, которое подключается к службе автообнаружения для получения параметров домена, убедитесь, что у вас есть доступ к следующее:
  
- Exchange Online, Exchange Online в составе Office 365 или на сервере под управлением версии Exchange, начиная с Exchange 2007. При использовании службы автообнаружения на основе SOAP веб-служб Exchange, сервере под управлением версии Exchange, начиная с Exchange 2010.
    
- Exchange server, который настроен на прием подключений от клиентского приложения. Сведения о настройке Exchange server в разделе [Управление доступом к клиентского приложения для веб-служб Exchange в Exchange](controlling-client-application-access-to-ews-in-exchange.md).
    
- Учетная запись, разрешенных для использования веб-служб Exchange. Сведения о настройке учетной записи в разделе [Управление доступом к клиентского приложения для веб-служб Exchange в Exchange](controlling-client-application-access-to-ews-in-exchange.md).
    
> [!NOTE]
> Если используется управляемый API веб-служб Exchange, необходимо предоставить обратного вызова проверки сертификата при определенных обстоятельствах. Может также потребоваться обратного вызова проверки сертификата с библиотеками некоторые созданного прокси-сервера, например, которые были созданы с помощью Visual Studio. Дополнительные сведения можно [Проверить сертификат сервера для управляемого интерфейса API веб-служб Exchange](how-to-validate-a-server-certificate-for-the-ews-managed-api.md). 
  
### <a name="core-concepts-for-getting-domain-settings"></a>Основные понятия, которые для получения параметров домена
<a name="bk_Core"> </a>

Прежде чем использовать службы автообнаружения для получения параметров домена, необходимо ознакомиться с понятиями, приведенными в следующей таблице.
  
|**Концепция**|**Описание**|
|:-----|:-----|
|[Автообнаружение для Exchange](autodiscover-for-exchange.md) <br/> |Обзор работы службы автообнаружения.  <br/> |
|[Использование службы автообнаружения для поиска точек подключения](how-to-use-autodiscover-to-find-connection-points.md) <br/> |Описывает процесс, используемый службой автообнаружения для перенаправления клиентского приложения к конечной точке службы правильное.  <br/> |
   
При использовании управляемого интерфейса API веб-служб Exchange, используйте класс [Microsoft.Exchange.WebServices.Data.ExchangeService](http://msdn.microsoft.com/en-us/library/exchange/dd635811%28v=exchg.80%29.aspx) в пространстве имен [Microsoft.Exchange.WebServices.Data](http://msdn.microsoft.com/en-us/library/exchange/dd633907%28v=exchg.80%29.aspx) для управления подключением к веб-служб Exchange. В примерах кода в этом разделе предполагается ссылаются следующие пространства имен в коде: 
  
- **System.Net**
    
- **Microsoft.Exchange.WebServices.Data.ExchangeService**
    
## <a name="get-domain-settings-by-using-the-ews-managed-api"></a>Получение параметров домена с помощью управляемого интерфейса API веб-служб Exchange
<a name="bk_Managed"> </a>

Если вы используете управляемый API веб-служб Exchange, можно использовать метод [Microsoft.Exchange.WebServices.Data.AutodiscoverSettings.GetUserSettings](http://msdn.microsoft.com/en-us/library/exchange/microsoft.exchange.webservices.autodiscover.autodiscoverservice.getusersettings%28v=exchg.80%29.aspx) объекта [Microsoft.Exchange.WebServices.Data.AutodiscoverService](http://msdn.microsoft.com/en-us/library/exchange/dd634321%28v=exchg.80%29.aspx) для создания запроса который извлекает данные конфигурации для домена, как показано в следующем примере. В этом примере запрашиваются только некоторые возможные домена параметры и возвращаются только те параметры, запрашиваемый с сервера. 
  
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

Может выполнять синтаксический анализ коллекции, возвращаемой для доступа к каждой пары ключ значение. Следующем примере показано, как анализировать каждого возвращаемого элемента и отображать имя и значение каждой пары "ключ значение".
  
```cs
// Display each retrieved value. The settings are part of a key/value pair.
foreach (KeyValuePair<DomainSettingName, Object> domainsetting in domainresponse.Settings)
{
    Console.WriteLine(domainsetting.Key.ToString() + ": " + domainsetting.Value.ToString());
}
```

Кроме того можно получить значение определенного параметра. В следующем примере значение **ExternalEwsUrl** — для отображения. 
  
```cs
// Display a specific setting, such as ExternalEwsUrl.
Console.WriteLine(domainresponse.Settings[DomainSettingName.ExternalEwsUrl]);
```

## <a name="get-user-settings-by-using-ews-soap-autodiscover"></a>Получение параметров пользователя с помощью службы автообнаружения SOAP веб-служб Exchange
<a name="bk_SOAP"> </a>

В следующем примере показано запрос SOAP XML для получения параметров оба домена с службы автообнаружения.
  
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

В следующем примере показано XML-ответ, возвращенный сервером после анализирует запрос от клиента.
  
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

Настройка домена предоставляют сведения, которую клиент необходимо подключение к веб-служб Exchange. Эти сведения можно использовать для подключения к веб-служб Exchange, или можно получить дополнительные параметры настройки для учетной записи электронной почты с сервера. Для получения дополнительных сведений в следующей статье:
  
- [Получить параметры пользователя из Exchange с помощью службы автообнаружения](how-to-get-user-settings-from-exchange-by-using-autodiscover.md)
    
## <a name="see-also"></a>См. также


- [Настройка приложения веб-служб Exchange](setting-up-your-ews-application.md)
    
- [Ссылки веб-службу автообнаружения для Exchange](http://msdn.microsoft.com/library/a01124a8-a8cf-4b80-8625-d7ee05690bca%28Office.15%29.aspx)
    
- [Справка по веб-служб Exchange для Exchange](http://msdn.microsoft.com/library/2a873474-1bb2-4cb1-a556-40e8c4159f4a%28Office.15%29.aspx)
    

