---
title: Обработка сообщений об ошибках службы автообнаружения
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.assetid: e5939ec2-1100-4174-8a88-5a6e09b60b23
description: Узнайте о различных типах ошибок автообнаружения и действиях, которые необходимо выполнить.
localization_priority: Priority
ms.openlocfilehash: 0cba7e54cb251a9775e0971826560e277dcd9d2d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44455963"
---
# <a name="handling-autodiscover-error-messages"></a>Обработка сообщений об ошибках службы автообнаружения

Узнайте о различных типах ошибок автообнаружения и действиях, которые необходимо выполнить.
  
Служба автообнаружения позволяет приложениям автоматически получать сведения о конфигурации и прекрасно работает. Тем не менее, они не всегда переходят в соответствии с планом. Рассмотрим распространенные ошибки и их обработку, чтобы свести к минимуму необходимость запрашивать пользователя вручную для настройки клиента.
  
## <a name="http-status-errors"></a>Ошибки состояния HTTP
<a name="bk_HttpErrors"> </a>

Первый тип ошибки, которая может возникнуть при отправке запросов автообнаружения — это состояние HTTP. Если состояние HTTP в отклике отлично от 200 (ОК), полезные данные отклика не содержат ответ автообнаружения, который вы искали. Для простоты мы можем группировать коды состояния, не относящиеся к 200, в три категории.
  
**Таблица 1. Коды состояния HTTP**

|**Код состояния**|**Тип ошибки**|**Обработка...**|
|:-----|:-----|:-----|
|301 или 302  <br/> |Ошибка перенаправления  <br/> |Отправьте запрос в URI, содержащийся в заголовке HTTP-ответа "Location". Дополнительные сведения см в разделе [Обработка ошибок перенаправления](#bk_HandlingRedirects).  <br/> |
|401  <br/> |Несанкционированная ошибка  <br/> |Так как [процесс автообнаружения](autodiscover-for-exchange.md) включает несколько возможных URL-адресов, вы можете получить их по одному URL-адресу, чтобы только следующий пользователь принимал свои учетные данные. По этой причине не следует учитывать одну ошибку 401, указывающую на недопустимые учетные данные. Однако при получении сообщений об ошибках 401 из нескольких URL-адресов может потребоваться, чтобы пользователь повторно вводил свой пароль (если это возможно).  <br/> |
|Любое другое состояние, отличное от 200  <br/> |Недопустимая ошибка конечной точки автообнаружения  <br/> |Рассмотрим URL-адрес, который возвращает любой другой код состояния, не относящийся к 200, и продолжайте пытаться использовать следующий URL-адрес в списке.  <br/> |
   
## <a name="autodiscover-errors"></a>Ошибки автообнаружения
<a name="bk_AutodiscoverErrors"> </a>

Даже если вы получаете код состояния 200 (OK) после отправки запроса на обнаружение, это не означает, что сервер отправил необходимые сведения. Состояние 200 означает, что у вас есть ответ автообнаружения, и ответ может содержать ошибку в полезных данных. Расположение сведений об ошибке зависит от того, является ли формат SOAP или POX.
  
### <a name="soap-autodiscover-errors"></a>Ошибки автообнаружения SOAP

Для автообнаружения SOAP ответ может содержать один или несколько элементов [ErrorCode (SOAP)](https://msdn.microsoft.com/library/5e5ec861-0191-4ecb-a906-47ce8ed96381%28Office.15%29.aspx) в разных местах. Как правило, вы можете ожидать один дочерний элемент элемента [Response (SOAP)](https://msdn.microsoft.com/library/4c2bcdeb-95ce-4ffa-bd83-118af53b534f%28Office.15%29.aspx) , а другой в качестве дочернего для каждого элемента [усерреспонсе (SOAP)](https://msdn.microsoft.com/library/5007b1ba-bfcc-40d7-b1cb-e32fbaf54ffd%28Office.15%29.aspx) в ответе. Кроме того, вы также можете столкнуться с одним дочерним элементом элемента [усерсеттинжеррор (SOAP)](https://msdn.microsoft.com/library/abb175c5-4f38-4dcc-81e3-b511686862eb%28Office.15%29.aspx) , если он присутствует. Контекст ошибки зависит от того, где находится элемент **ErrorCode** , как показано ниже. 
  
- В качестве дочернего элемента элемента **Response** элемент **ErrorCode** представляет ошибку, которая применяется ко всему запросу. 
    
- В качестве дочернего элемента для элемента **усерреспонсе** представляет ошибку, которая применяется только к определенному пользователю. 
    
- В качестве дочернего элемента для элемента **усерсеттинжеррор** представляет ошибку, которая применяется к определенному запрошенному параметру. 
    
Давайте рассмотрим пример ответа. В этом примере элемент **ErrorCode** в элементе **Response** имеет значение "No Error", которое указывает на общее успешное выполнение. Однако элемент **ErrorCode** в элементе **усерреспонсе** имеет значение "RedirectAddress", которое указывает на то, что для конкретного пользователя возникла ошибка. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/" 
    xmlns:a="http://www.w3.org/2005/08/addressing">
  <s:Header>
    <a:Action s:mustUnderstand="1">https://schemas.microsoft.com/exchange/2010/Autodiscover/Autodiscover/GetUserSettingsResponse</a:Action>
    <h:ServerVersionInfo xmlns:h="https://schemas.microsoft.com/exchange/2010/Autodiscover" 
        xmlns:i="http://www.w3.org/2001/XMLSchema-instance">
      <h:MajorVersion>14</h:MajorVersion>
      <h:MinorVersion>3</h:MinorVersion>
      <h:MajorBuildNumber>136</h:MajorBuildNumber>
      <h:MinorBuildNumber>1</h:MinorBuildNumber>
      <h:Version>Exchange2010_SP2</h:Version>
    </h:ServerVersionInfo>
  </s:Header>
  <s:Body>
    <GetUserSettingsResponseMessage xmlns="https://schemas.microsoft.com/exchange/2010/Autodiscover">
      <Response xmlns:i="http://www.w3.org/2001/XMLSchema-instance">
        <ErrorCode>NoError</ErrorCode>
        <ErrorMessage />
        <UserResponses>
          <UserResponse>
            <ErrorCode>RedirectAddress</ErrorCode>
            <ErrorMessage>Redirection address.</ErrorMessage>
            <RedirectTarget>elvin@mail.contoso.com</RedirectTarget>
            <UserSettingErrors />
            <UserSettings />
          </UserResponse>
        </UserResponses>
      </Response>
    </GetUserSettingsResponseMessage>
  </s:Body>
</s:Envelope>
```

В статье [ErrorCode (SOAP)](https://msdn.microsoft.com/library/5e5ec861-0191-4ecb-a906-47ce8ed96381%28Office.15%29.aspx) содержится полный список возможных ошибок. Большинство из них указывают на неустранимую ошибку, но не требует особой обработки. 
  
**Таблица 2. Значения ErrorCode обнаружение autodisover SOAP**

|**Значение ErrorCode**|**Обработка...**|
|:-----|:-----|
|RedirectAddress  <br/> |[Перезапуск службы автообнаружения с новым адресом электронной почты](#bk_RestartAutodiscover) с адресом электронной почты в элементе [редиректтаржет (SOAP)](https://msdn.microsoft.com/library/f8162724-cf9a-4543-a1ad-5846c8b10bfa%28Office.15%29.aspx) .  <br/> |
|RedirectUrl адресом  <br/> |[Повторно отправит запрос на новый URL](#bk_ResendRequest) -адрес в URL-адрес в элементе **редиректтаржет** .  <br/> |
|ServerBusy  <br/> |Повторите этот URL-адрес после небольшой задержки. Вы можете подождать заданный URL-адрес или просто переместить его в конец списка URL-адресов, чтобы попробовать. Если вы получаете эту ошибку несколько раз с URL-адреса, необходимо учитывать, что URL-адрес является недопустимым.  <br/> |
   
### <a name="pox-autodiscover-errors"></a>Ошибки автообнаружения POX

Служба автообнаружения POX зачитывает ошибки немного по-другому. Ошибки, которые не могут быть восстановлены, хранятся в элементе [Error (POX)](https://msdn.microsoft.com/library/91c63b62-ab68-4c32-a2f7-5a87c188335b%28Office.15%29.aspx) . В статье [ErrorCode (POX)](https://msdn.microsoft.com/library/064d73e4-45b7-4797-828e-9df590830db8%28Office.15%29.aspx) содержится полный список возможных кодов ошибок. 
  
Ошибки перенаправления находятся в элементе [Action (POX)](https://msdn.microsoft.com/library/a3462c6b-453c-462a-830d-f29ee4a2babb%28Office.15%29.aspx) . Любое значение элемента **Action** , кроме "Settings", указывает на ошибку перенаправления. 
  
**Таблица 3. POX обнаружение autodisover значения ErrorCode**

|**Значение действия**|**Обработка...**|
|:-----|:-----|
|редиректаддр  <br/> |[Перезапуск службы автообнаружения с новым адресом электронной почты](#bk_RestartAutodiscover) с адресом электронной почты в элементе [редиректаддр (POX)](https://msdn.microsoft.com/library/0e9fa6b6-7991-4dc1-a59a-48e5f8e041e4%28Office.15%29.aspx) .  <br/> |
|redirectUrl  <br/> |[Повторно отправит запрос на новый URL](#bk_ResendRequest) -адрес в URL-адрес в элементе [redirectUrl адресом (POX)](https://msdn.microsoft.com/library/c54f310f-8c99-4c37-8e73-ac87722b6229%28Office.15%29.aspx) .  <br/> |
   
В этом примере элемент **Action** имеет значение "редиректаддр", которое указывает, что новый запрос должен отправляться с новым адресом электронной почты, который хранится в элементе **редиректаддр** . 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<Autodiscover xmlns="https://schemas.microsoft.com/exchange/autodiscover/responseschema/2006">
  <Response xmlns="https://schemas.microsoft.com/exchange/autodiscover/outlook/responseschema/2006a">
    <Account>
      <Action>redirectAddr</Action>
      <RedirectAddr>elvin@mail.contoso.com</RedirectAddr>
    </Account>
  </Response>
</Autodiscover>
```

## <a name="handling-redirect-errors"></a>Обработка ошибок перенаправления
<a name="bk_HandlingRedirects"> </a>

Сценарии ошибок перенаправления можно обрабатывать двумя способами:
  
- Путем перезапуска автообнаружения с новым адресом электронной почты.
    
- Повторно отправляя запрос на новый URL-адрес.
    
В обоих сценариях требуется проверка перед продолжением.
  
### <a name="restarting-autodiscover-with-a-new-email-address"></a>Перезапуск автообнаружения с новым адресом электронной почты
<a name="bk_RestartAutodiscover"> </a>

При получении нового адреса электронной почты в ответе на перенаправление автообнаружения сначала убедитесь, что новый адрес электронной почты, указанный в ответе на сообщение об ошибке перенаправления, отличается от адреса, отправленного в запросе, который привел к ошибке. Если это так, не следует перезапускать службу автообнаружения, а вместо этого считать недопустимым URL-адрес, который выдал ответ.
  
Если новый адрес электронной почты отличается, удалите существующий список возможных URL-адресов конечных точек автообнаружения и создайте новый список на основе нового адреса электронной почты.
  
### <a name="resending-your-request-to-a-new-url"></a>Повторная отправка запроса на новый URL-адрес
<a name="bk_ResendRequest"> </a>

При получении нового URL-адреса в ответе на перенаправление автообнаружения сначала необходимо проверить URL-адрес следующим образом:
  
- Убедитесь, что URL-адрес является URL-адресом HTTPS.
    
- Убедитесь, что вы не получали ошибку от этого URL-адреса с текущим адресом электронной почты, прежде чем.
    
- Если это применимо к приложению, сообщите пользователю о перенаправлении и получите разрешение на отслеживание перенаправления.
    
- Отправьте запрос на URL-адрес и [Убедитесь, что сертификат SSL, предоставленный сервером, является допустимым](how-to-validate-a-server-certificate-for-the-ews-managed-api.md).
    
Если URL-адрес проходит проверку, отправьте запрос на этот новый URL-адрес.
  
## <a name="see-also"></a>См. также


- [Автообнаружение в Exchange](autodiscover-for-exchange.md)
    
- [Обнаружение конечных точек автообнаружения с помощью поиска SCP в Exchange](how-to-find-autodiscover-endpoints-by-using-scp-lookup-in-exchange.md)
    
- [ErrorCode (SOAP)](https://msdn.microsoft.com/library/5e5ec861-0191-4ecb-a906-47ce8ed96381%28Office.15%29.aspx)
    
- [ErrorCode (POX)](https://msdn.microsoft.com/library/064d73e4-45b7-4797-828e-9df590830db8%28Office.15%29.aspx)
    

