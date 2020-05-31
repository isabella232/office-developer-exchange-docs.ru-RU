---
title: Поиск точек соединения с помощью службы автообнаружения
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 03896542-549b-4c45-973c-98f9025ea26c
description: Узнайте, как использовать службу автообнаружения для направления клиентского приложения на соответствующий сервер Exchange.
ms.openlocfilehash: eb3fb3664e5789638c097a43cf48f757bb0713ae
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/28/2018
ms.locfileid: "21353982"
---
# <a name="use-autodiscover-to-find-connection-points"></a>Поиск точек соединения с помощью службы автообнаружения

Узнайте, как использовать службу автообнаружения для направления клиентского приложения на соответствующий сервер Exchange.
  
Служба автообнаружения Exchange предоставляет клиентским приложениям параметры конфигурации для учетных записей электронной почты, размещенных в Exchange Online, Exchange Online в составе Office 365, или на сервере Exchange Server с Exchange 2013. Служба автообнаружения — это веб-служба, предоставляющая параметры конфигурации. Служба автообнаружения — это веб-служба, которая предоставляет клиентским приложениям сведения о конфигурации Exchange Server. Клиентские приложения используют службу автообнаружения для определения конечной точки службы автообнаружения для определенного почтового ящика. В этой статье объясняется, как выполнять ответы от сервера Exchange Server, чтобы найти правильную конечную точку. 
  
Сведения о получении параметров конфигурации адресов электронной почты приведены в статье [Получение параметров пользователя из Exchange с помощью автообнаружения](how-to-get-user-settings-from-exchange-by-using-autodiscover.md) и [Получение параметров домена с сервера Exchange](how-to-get-domain-settings-from-an-exchange-server.md).
  
> [!NOTE]
> Процесс поиска правильной конечной точки является частью запроса параметров пользователя или домена. Служба автообнаружения использует серию ответов перенаправления для отправки клиентского приложения в правильную конечную точку для адреса электронной почты. 
  
Для доступа к службе автообнаружения можно использовать одну из следующих технологий разработки Exchange:

- Управляемый API веб-служб Exchange (EWS)
    
- EWS
    
Если вы используете EWS, вы можете использовать следующие методы для получения параметров пользователя:
    
- Служба автообнаружения на основе SOAP
    
- Служба автообнаружения XML (POX)
    
- Автоматически созданный прокси-сервер, созданный службой автообнаружения SOAP или XML
    
Дополнительные сведения об этих методах см. в разделе [автообнаружения для Exchange](autodiscover-for-exchange.md).

Дополнительные сведения об этих технологиях разработки Exchange можно найти [в статье Обзор управляемого API EWS, EWS и веб-служб в Exchange](explore-the-ews-managed-api-ews-and-web-services-in-exchange.md). 

Управляемый API EWS предоставляет интерфейс на основе объектов для получения параметров пользователя. Если клиентское приложение использует управляемый код, мы рекомендуем использовать управляемый API EWS. Интерфейс управляемого API EWS лучше оптимизирован для простой объектной модели по сравнению с обычным автоматически созданным прокси-сервером веб-службы. 
  
Если вы используете EWS, мы рекомендуем использовать службу автообнаружения SOAP, так как она поддерживает более широкий набор функций, чем служба автообнаружения POX.
  
## <a name="prerequisites-for-finding-an-endpoint"></a>Необходимые условия для поиска конечной точки
<a name="bk_Prereq"> </a>

Прежде чем можно будет создать клиентское приложение, использующее службу автообнаружения, необходимо иметь доступ к следующим параметрам:
  
- Exchange Online или сервер, на котором работает версия Exchange начиная с Exchange 2007 с пакетом обновления 1 (SP1). Если вы используете службу автообнаружения на основе SOAP, Exchange Online или версию Exchange, начиная с Exchange 2010.
    
- Сервер Exchange, настроенный для приема подключений из клиентского приложения. Сведения о настройке сервера Exchange Server можно найти [в статье Управление доступом клиентского приложения к EWS в Exchange](controlling-client-application-access-to-ews-in-exchange.md).
    
- Учетная запись, которая авторизована для использования EWS. Сведения о настройке учетной записи см [в разделе Управление доступом клиентского приложения к EWS в Exchange](controlling-client-application-access-to-ews-in-exchange.md).
    
> [!NOTE]
> Если вы используете управляемый API EWS, в некоторых обстоятельствах необходимо предоставить обратный вызов проверки сертификата. Кроме того, вам может потребоваться обратный вызов проверки сертификата со всеми созданными библиотеками прокси, например, созданными Visual Studio. Дополнительные сведения см. [в статье Проверка сертификата сервера для управляемого API EWS](how-to-validate-a-server-certificate-for-the-ews-managed-api.md). 
  
### <a name="core-concepts-for-finding-an-endpoint"></a>Основные понятия, связанные с поиском конечной точки
<a name="bk_Core"> </a>

Прежде чем использовать службу автообнаружения для поиска конечной точки, необходимо ознакомиться с концепциями, приведенными в следующей таблице.
  
|**Концепция**|**Описание**|
|:-----|:-----|
|[Автообнаружение для Exchange](autodiscover-for-exchange.md) <br/> |Предоставляет общие сведения о работе службы автообнаружения.  <br/> |
   
Если вы используете управляемый API EWS, вы используете класс [Microsoft. Exchange. WebServices. Data. ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) в пространстве имен [Microsoft. Exchange. WebServices. Data](http://msdn.microsoft.com/en-us/library/dd633907%28v=exchg.80%29.aspx) для управления подключением к EWS. Чтобы использовать примеры кода управляемого API EWS, приведенные в этой статье, необходимо сослаться на следующие пространства имен в коде: 
  
- **System.Net**
    
- **Microsoft. Exchange. WebServices. Data. ExchangeService**
    
## <a name="find-the-correct-endpoint-by-using-the-ews-managed-api"></a>Поиск правильной конечной точки с помощью управляемого API EWS
<a name="bk_Managed"> </a>

Если вы используете управляемый API EWS, вызовы службы автообнаружения обрабатываются классом **ExchangeService** . Чтобы определить правильную конечную точку для учетной записи электронной почты, необходимо вызвать метод **AutodiscoverUrl** для объекта **[ExchangeService]** . В следующем примере кода показано, как установить конечную точку веб-службы EWS для адреса электронной почты в файл Exchange. asmx на правильном сервере клиентского доступа с помощью управляемого API EWS. 
  
```cs
NetworkCredential credentials = new NetworkCredential(securelyStoredEmail, securelyStoredPassword);
ExchangeService service = new ExchangeService(ExchangeVersion.Exchange2013);
service.Credentials = credentials;
service.AutodiscoverUrl("User1@contoso.com");
```

## <a name="find-the-correct-endpoint-by-using-ews"></a>Поиск правильной конечной точки с помощью EWS
<a name="bk_SOAP"> </a>

Служба автообнаружения SOAP может использовать серию запросов и ответов для направления приложения в правильную конечную точку для EWS. Сведения о том, как определить правильную конечную точку для учетной записи электронной почты, можно найти в разделе Служба [автообнаружения для Exchange](autodiscover-for-exchange.md). В следующих примерах XML-кода показан ряд запросов и ответов, которые можно ожидать при выполнении запроса автообнаружения SOAP для поиска нужной конечной точки.
  
### <a name="soap-autodiscover-endpoint-request"></a>Запрос конечной точки автообнаружения SOAP

В следующем примере показан XML-запрос, который отправляется в службу автообнаружения, чтобы найти правильную конечную точку.
  
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

### <a name="soap-autodiscover-redirection-response"></a>Ответ на перенаправление автообнаружения SOAP

Служба автообнаружения может отвечать на один из двух ответов перенаправления: HTTP 302 Redirect или ответ на перенаправление SOAP. Если ответ сервера Exchange Server является перенаправлением HTTP 302, клиентское приложение должно проверить, является ли адрес перенаправления допустимым, а затем следовать ответу перенаправления.
  
> [!IMPORTANT]
> Условия проверки отклика перенаправления содержатся в разделе Служба [автообнаружения для Exchange](autodiscover-for-exchange.md). 
  
Если служба автообнаружения возвращает ответ на перенаправление, который указывается элементом [ErrorCode](http://msdn.microsoft.com/library/0bb00cee-c66b-4f34-b99d-355458f5e83b%28Office.15%29.aspx) элемента **усерреспонсе** , клиентское приложение должно использовать элемент **редиректтаржет** для создания нового запроса на параметры, который отправляется на сервер, указанный в ответе на перенаправление. В следующем примере показан ответ перенаправления от сервера. 
  
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

После перенаправления клиент использует URL-адрес перенаправления, чтобы подготовить еще один запрос. В приведенном ниже коде показан пример запроса, созданного на основе ответа на перенаправление.
  
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

Когда клиентское приложение направляется в правильную конечную точку для службы автообнаружения, сервер отправит ответ с элементом [ErrorCode](http://msdn.microsoft.com/library/0bb00cee-c66b-4f34-b99d-355458f5e83b%28Office.15%29.aspx) элемента **усерреспонсе** , установленным в значение " **Ошибка** ", и содержащий запрошенные параметры пользователя. Возвращаются только запрошенные параметры пользователя, **интерналевсурл** и **екстерналевсурл**. В следующем примере показан ответ от сервера. 
  
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

Поиск конечной точки с помощью процесса автообнаружения возвращает запрошенный домен или параметры пользователя. Сведения о том, как сделать запрос на определенные параметры, можно найти в следующих статьях:
  
- [Получение параметров домена с сервера Exchange](how-to-get-domain-settings-from-an-exchange-server.md)    
- [Получение параметров пользователя из Exchange с помощью службы автообнаружения](how-to-get-user-settings-from-exchange-by-using-autodiscover.md)
    
## <a name="see-also"></a>См. также

- [Настройка приложения веб-служб Exchange](setting-up-your-ews-application.md)   
- [Автообнаружение для Exchange](autodiscover-for-exchange.md)    
- [Справочные материалы по веб-службе автообнаружения для Exchange](http://msdn.microsoft.com/library/a01124a8-a8cf-4b80-8625-d7ee05690bca%28Office.15%29.aspx)    
- [Справка по веб-служб Exchange для Exchange](http://msdn.microsoft.com/library/2a873474-1bb2-4cb1-a556-40e8c4159f4a%28Office.15%29.aspx)
    

