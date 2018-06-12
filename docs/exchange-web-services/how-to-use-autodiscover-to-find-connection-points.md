---
title: Использование службы автообнаружения для поиска точек подключения
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 03896542-549b-4c45-973c-98f9025ea26c
description: Узнайте, как использовать службу автообнаружения для направления клиентского приложения к правильному серверу Exchange.
ms.openlocfilehash: 653fcd1c094c23c3e89e903b7194b96720802b51
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761127"
---
# <a name="use-autodiscover-to-find-connection-points"></a>Использование службы автообнаружения для поиска точек подключения

Узнайте, как использовать службу автообнаружения для направления клиентского приложения к правильному серверу Exchange.
  
Служба автообнаружения Exchange предоставляет клиентского приложения с помощью параметров конфигурации для учетных записей электронной почты, размещенных на Exchange Online, Exchange Online в составе Office 365 или Exchange server, версия Exchange начиная с Exchange 2013. Служба автообнаружения — веб-службы, который предоставляет параметры конфигурации. Служба автообнаружения — веб-службы, который предоставляет сведения о конфигурации сервера Exchange для клиентского приложения. Клиентские приложения используйте службы автообнаружения для определения конечной точки службы автообнаружения для определенного почтового ящика. В этой статье объясняется, как выполнять ответов с сервера Exchange, чтобы найти правильный конечной точки. 
  
Сведения о том, как получить параметры конфигурации адрес электронной почты можно [получить параметры пользователя из Exchange с помощью службы автообнаружения](how-to-get-user-settings-from-exchange-by-using-autodiscover.md) и [получить параметры домена с сервера Exchange](how-to-get-domain-settings-from-an-exchange-server.md).
  
> [!NOTE]
> Процесс поиска правильный конечная точка является частью запроса для пользователя или параметры домена. Служба автообнаружения использует ряд ответы перенаправления для отправки клиентского приложения к конечной точке правильные адреса электронной почты. 
  
Можно использовать один из следующих технологиях разработки Exchange для доступа к службе автообнаружения:
  
> [!NOTE]
> Дополнительные сведения об этих технологиях разработки Exchange можно [Проводник управляемый API веб-служб Exchange, веб-служб Exchange и веб-служб Exchange](explore-the-ews-managed-api-ews-and-web-services-in-exchange.md). 
  
- Веб-служб Exchange (EWS) управляемого интерфейса API
    
- EWS
    
    При использовании веб-служб Exchange, можно использовать следующие методы для получения параметров пользователя:
    
  - Служба автообнаружения на основе SOAP
    
  - Служба автообнаружения XML (POX)
    
  - Прокси-сервер автоматически созданный, созданный из службы SOAP или автоматического обнаружения XML
    
    Дополнительные сведения об этих методов можно [автообнаружения для Exchange](autodiscover-for-exchange.md).
    
Управляемый API веб-служб Exchange предоставляет объектно ориентированный интерфейс для извлечения параметров пользователя. Если клиентское приложение использует управляемый код, мы рекомендуем использовать управляемый API веб-служб Exchange. Чем обычно автоматически созданный прокси веб-службы для простой объектной модели лучше оптимизированный интерфейс управляемый API веб-служб Exchange. 
  
При использовании веб-служб Exchange, рекомендуется использовать службы автообнаружения SOAP, поскольку она поддерживает расширенный набор функциональных возможностей, чем службы автообнаружения POX.
  
## <a name="prerequisites-for-finding-an-endpoint"></a>Необходимые условия для поиска конечную точку
<a name="bk_Prereq"> </a>

Перед созданием клиентское приложение, которое использует службу автообнаружения, необходимо иметь доступ к таким компонентам:
  
- Exchange Online или сервера, на котором выполняется версия Exchange о том, начиная с Exchange 2007 с пакетом обновления 1. При использовании службы автообнаружения на основе SOAP, Exchange Online или версии Exchange, начиная с Exchange 2010.
    
- Exchange server, который настроен на прием подключений от клиентского приложения. Сведения о настройке Exchange server в разделе [Управление доступом к клиентского приложения для веб-служб Exchange в Exchange](controlling-client-application-access-to-ews-in-exchange.md).
    
- Учетная запись, разрешенных для использования веб-служб Exchange. Сведения о настройке учетной записи в разделе [Управление доступом к клиентского приложения для веб-служб Exchange в Exchange](controlling-client-application-access-to-ews-in-exchange.md).
    
> [!NOTE]
> Если используется управляемый API веб-служб Exchange, необходимо предоставить обратного вызова проверки сертификата при определенных обстоятельствах. Может также потребоваться обратного вызова проверки сертификата с библиотеками некоторые созданного прокси-сервера, например, которые были созданы с помощью Visual Studio. Дополнительные сведения можно [Проверить сертификат сервера для управляемого интерфейса API веб-служб Exchange](how-to-validate-a-server-certificate-for-the-ews-managed-api.md). 
  
### <a name="core-concepts-for-finding-an-endpoint"></a>Основные понятия, которые поиска конечную точку
<a name="bk_Core"> </a>

Прежде чем использовать службы автообнаружения для поиска конечную точку, необходимо ознакомиться с понятиями, приведенными в следующей таблице.
  
|**Концепция**|**Описание**|
|:-----|:-----|
|[Автообнаружение для Exchange](autodiscover-for-exchange.md) <br/> |Обзор работы службы автообнаружения.  <br/> |
   
При использовании управляемого интерфейса API веб-служб Exchange, используйте класс [Microsoft.Exchange.WebServices.Data.ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) в пространстве имен [Microsoft.Exchange.WebServices.Data](http://msdn.microsoft.com/en-us/library/dd633907%28v=exchg.80%29.aspx) для управления подключением к веб-служб Exchange. Чтобы использовать управляемый API EWS примеры кода в этой статье, необходимо ссылаться на следующие пространства имен в коде: 
  
- **System.Net**
    
- **Microsoft.Exchange.WebServices.Data.ExchangeService**
    
## <a name="find-the-correct-endpoint-by-using-the-ews-managed-api"></a>Найти правильный конечных точек с помощью управляемого интерфейса API веб-служб Exchange
<a name="bk_Managed"> </a>

При использовании управляемого интерфейса API веб-служб Exchange для службы автообнаружения вызовами классом **ExchangeService** . Чтобы определить правильное конечной точки для учетной записи электронной почты, вызовите метод **AutodiscoverUrl** объекта **[ExchangeService]** . В следующем примере кода показано, как задать конечную веб-службы веб-служб Exchange для адреса электронной почты Exchange.asmx файла на правильный сервер клиентского доступа с помощью управляемого интерфейса API веб-служб Exchange. 
  
```cs
NetworkCredential credentials = new NetworkCredential(securelyStoredEmail, securelyStoredPassword);
ExchangeService service = new ExchangeService(ExchangeVersion.Exchange2013);
service.Credentials = credentials;
service.AutodiscoverUrl("User1@contoso.com");
```

## <a name="find-the-correct-endpoint-by-using-ews"></a>Найти правильный конечных точек с помощью веб-служб Exchange
<a name="bk_SOAP"> </a>

Служба автообнаружения SOAP может использовать ряд запросы и ответы для направления приложения правильные конечную точку для веб-служб Exchange. Сведения о процессе по определению правильный конечных точек для учетной записи электронной почты содержатся в разделе [службы автообнаружения для Exchange](autodiscover-for-exchange.md). В следующих примерах XML серии запросов и ответов, которые можно ожидать при выполнении запроса SOAP автообнаружения найти правильный конечную точку.
  
### <a name="soap-autodiscover-endpoint-request"></a>Запрос конечной точки службы автообнаружения SOAP

В следующем примере показано запрос XML, который отправляется найти правильный конечной точки для службы автообнаружения.
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:a="http://schemas.microsoft.com/exchange/2010/Autodiscover" 
        xmlns:wsa="http://www.w3.org/2005/08/addressing" 
        xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
        xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <a:RequestedServerVersion>Exchange2013</a:RequestedServerVersion>
    <wsa:Action>http://schemas.microsoft.com/exchange/2010/Autodiscover/Autodiscover/GetUserSettings</wsa:Action>
    <wsa:To>https://mail.microsoft.com/autodiscover/autodiscover.svc</wsa:To>
  </soap:Header>
  <soap:Body>
    <a:GetUserSettingsRequestMessage xmlns:a="http://schemas.microsoft.com/exchange/2010/Autodiscover">
      <a:Request>
        <a:Users>
          <a:User>
            <a:Mailbox>User1@Contoso.com</a:Mailbox>
          </a:User>
        </a:Users>
        <a:RequestedSettings>
          <a:Setting>InternalEwsUrl</a:Setting>
          <a:Setting>ExternalEwsUrl</a:Setting>
        </a:RequestedSettings>
      </a:Request>
    </a:GetUserSettingsRequestMessage>
  </soap:Body>
</soap:Envelope>

```

### <a name="soap-autodiscover-redirection-response"></a>Ответ SOAP автообнаружения в режиме одобрения администратором

Служба автообнаружения может отвечать на запросы с одним из двух ответы перенаправления: на перенаправление HTTP 302 или в режиме одобрения администратором ответа SOAP. Если ответ от сервера Exchange на перенаправление HTTP 302, клиентское приложение следует проверить, что адрес перенаправления является приемлемым и следуйте ответа в режиме одобрения администратором.
  
> [! Примечание по безопасности] критериев для проверки правильности ответа в режиме одобрения администратором, посвященной [автообнаружения для Exchange](autodiscover-for-exchange.md). 
  
Если служба автообнаружения возвращать ответа в режиме одобрения администратором, указанный в параметре элемент [ErrorCode](http://msdn.microsoft.com/library/0bb00cee-c66b-4f34-b99d-355458f5e83b%28Office.15%29.aspx) элемента **ответ пользователя** , клиентское приложение следует использовать элемент **RedirectTarget** для создания нового запроса параметров, то есть Отправить на сервер, указанный в ответ в режиме одобрения администратором. В следующем примере показано ответа в режиме одобрения администратором на сервере. 
  
```XML
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/" xmlns:a="http://www.w3.org/2005/08/addressing">
  <s:Header>
    <a:Action s:mustUnderstand="1">http://schemas.microsoft.com/exchange/2010/
        Autodiscover/Autodiscover/GetUserSettingsResponse</a:Action>
    <h:ServerVersionInfo xmlns:h="http://schemas.microsoft.com/exchange/2010/Autodiscover" 
        xmlns:i="http://www.w3.org/2001/XMLSchema-instance">
      <h:MajorVersion>15</h:MajorVersion>
      <h:MinorVersion>0</h:MinorVersion>
      <h:MajorBuildNumber>682</h:MajorBuildNumber>
      <h:MinorBuildNumber>1</h:MinorBuildNumber>
      <h:Version>Exchange2013</h:Version>
    </h:ServerVersionInfo>
  </s:Header>
  <s:Body>
    <GetUserSettingsResponseMessage xmlns="http://schemas.microsoft.com/exchange/2010/Autodiscover">
      <Response xmlns:i="http://www.w3.org/2001/XMLSchema-instance">
        <ErrorCode>NoError</ErrorCode>
        <ErrorMessage />
        <UserResponses>
          <UserResponse>
            <ErrorCode>RedirectAddress</ErrorCode>
            <ErrorMessage>Redirection address.</ErrorMessage>
            <RedirectTarget>User1@mail.Contoso.com</RedirectTarget>
            <UserSettingErrors />
            <UserSettings />
          </UserResponse>
        </UserResponses>
      </Response>
    </GetUserSettingsResponseMessage>
  </s:Body>
</s:Envelope>

```

После перенаправления клиент использует URL-адрес перенаправления для подготовки другой запрос. Следующий код является примером запроса, создаваемого из ответа в режиме одобрения администратором.
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:a="http://schemas.microsoft.com/exchange/2010/Autodiscover" 
        xmlns:wsa="http://www.w3.org/2005/08/addressing" 
        xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
        xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <a:RequestedServerVersion>Exchange2013</a:RequestedServerVersion>
    <wsa:Action>http://schemas.microsoft.com/exchange/2010/
        Autodiscover/Autodiscover/GetUserSettings</wsa:Action>
    <wsa:To>https://autodiscover.exchange.microsoft.com/autodiscover/autodiscover.svc</wsa:To>
  </soap:Header>
  <soap:Body>
    <a:GetUserSettingsRequestMessage xmlns:a="http://schemas.microsoft.com/exchange/2010/Autodiscover">
      <a:Request>
        <a:Users>
          <a:User>
            <a:Mailbox>User1@mail.Contoso.com</a:Mailbox>
          </a:User>
        </a:Users>
        <a:RequestedSettings>
          <a:Setting>InternalEwsUrl</a:Setting>
          <a:Setting>ExternalEwsUrl</a:Setting>
        </a:RequestedSettings>
      </a:Request>
    </a:GetUserSettingsRequestMessage>
  </soap:Body>
</soap:Envelope>

```

Если клиентское приложение были перенаправлены на правильные конечной точки для службы автообнаружения, сервер отправляет ответ, содержащий элемент [ErrorCode](http://msdn.microsoft.com/library/0bb00cee-c66b-4f34-b99d-355458f5e83b%28Office.15%29.aspx) элемента **ответ пользователя** значение **NoError** и содержащий запрашиваемый параметры пользователя. Возвращаются только запрошенный параметры пользователя, **InternalEwsUrl** и **ExternalEwsUrl**. В следующем примере показано ответ от сервера. 
  
```XML
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/" 
        xmlns:a="http://www.w3.org/2005/08/addressing">
  <s:Header>
    <a:Action s:mustUnderstand="1">http://schemas.microsoft.com/exchange/2010/
        Autodiscover/Autodiscover/GetUserSettingsResponse</a:Action>
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
    <GetUserSettingsResponseMessage xmlns="http://schemas.microsoft.com/exchange/2010/Autodiscover">
      <Response xmlns:i="http://www.w3.org/2001/XMLSchema-instance">
        <ErrorCode>NoError</ErrorCode>
        <ErrorMessage />
        <UserResponses>
          <UserResponse>
            <ErrorCode>NoError</ErrorCode>
            <ErrorMessage>No error.</ErrorMessage>
            <RedirectTarget i:nil="true" />
            <UserSettingErrors />
            <UserSettings>
              <UserSetting i:type="StringSetting">
                <Name>InternalEwsUrl</Name>
                <Value>https://server.Contoso.com/ews/exchange.asmx</Value>
              </UserSetting>
              <UserSetting i:type="StringSetting">
                <Name>ExternalEwsUrl</Name>
                <Value>https://server.Contoso.com/ews/exchange.asmx</Value>
              </UserSetting>
            </UserSettings>
          </UserResponse>
        </UserResponses>
      </Response>
    </GetUserSettingsResponseMessage>
  </s:Body>
</s:Envelope>
```

## <a name="next-steps"></a>Дальнейшие действия
<a name="bk_Next"> </a>

Поиск в конечную точку, выполнив процесса автообнаружения возвращает запрошенного домена или параметров пользователя. Сведения о выполнении запроса для определенных параметров см в следующих статьях:
  
- [Получение параметров домена с сервера Exchange](how-to-get-domain-settings-from-an-exchange-server.md)
    
- [Получить параметры пользователя из Exchange с помощью службы автообнаружения](how-to-get-user-settings-from-exchange-by-using-autodiscover.md)
    
## <a name="see-also"></a>См. также


- [Настройка приложения веб-служб Exchange](setting-up-your-ews-application.md)
    
- [Автообнаружение для Exchange](autodiscover-for-exchange.md)
    
- [Ссылки веб-службу автообнаружения для Exchange](http://msdn.microsoft.com/library/a01124a8-a8cf-4b80-8625-d7ee05690bca%28Office.15%29.aspx)
    
- [Справка по веб-служб Exchange для Exchange](http://msdn.microsoft.com/library/2a873474-1bb2-4cb1-a556-40e8c4159f4a%28Office.15%29.aspx)
    

