---
title: Обработка сообщений об ошибках службы автообнаружения
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: e5939ec2-1100-4174-8a88-5a6e09b60b23
description: Узнайте о различных типах автоматического обнаружения ошибок и что делать с ними.
ms.openlocfilehash: fcafc799f4d35e92159d2913845474ecf7bc5657
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760956"
---
# <a name="handling-autodiscover-error-messages"></a>Обработка сообщений об ошибках службы автообнаружения

Узнайте о различных типах автоматического обнаружения ошибок и что делать с ними.
  
Автообнаружение включает приложения, чтобы автоматически извлечь сведения о конфигурации и прекрасно работает. Тем не менее что не всегда переход согласно плану. Давайте взглянем на распространенные ошибки, которые могут возникать и как их для сведения к минимуму необходимость запрашивать вручную настроить клиент обработки.
  
## <a name="http-status-errors"></a>Состояние ошибки HTTP
<a name="bk_HttpErrors"> </a>

Первый тип ошибки, которые могут возникать при отправке запросов автообнаружения — состояние HTTP. Если отображается состояние HTTP в свой ответ отличное от 200 (ОК), полезных данных ответа не содержит ответа службы автообнаружения, который вы искали. Для простоты выполняется группировка кодов состояния не 200 на три категории.
  
**В таблице 1. Коды состояния HTTP**

|**Код состояния**|**Тип ошибки**|**Обработка...**|
|:-----|:-----|:-----|
|301 или 302  <br/> |Перенаправление ошибок  <br/> |Повторно отправьте запрос к URI, содержащихся в заголовке ответа «Расположение» HTTP. Дополнительные сведения см [Перенаправление обработки ошибок](#bk_HandlingRedirects).  <br/> |
|401  <br/> |Сообщение об ошибке авторизации  <br/> |Так как [процесс автообнаружения](autodiscover-for-exchange.md) состоит из ознакомления с несколько возможных URL-адресов, получения это на один URL-адрес, только чтобы следующим принять свои учетные данные. По этой причине не следует учитывать одной 401 об ошибке, указывающее, что учетные данные являются недопустимыми. Тем не менее в случае 401 ошибок из несколько URL-адресов, можно запрашивать повторно введите пароль (если это возможно).  <br/> |
|Другие состояния не 200  <br/> |Недопустимый ошибка конечной точки службы автообнаружения  <br/> |Попробуйте URL-адрес, который возвращает другой код состояния не 200 недействительной и повторить попытку следующий URL-адрес в списке.  <br/> |
   
## <a name="autodiscover-errors"></a>Ошибки службы автообнаружения
<a name="bk_AutodiscoverErrors"> </a>

Даже если код состояния 200 (ОК) после отправки запроса службы автообнаружения, это не означает, что сервер отправляться информацию, необходимую. 200 состояние только означает, что у вас есть ответа службы автообнаружения и этого ответа может содержать ошибки внутри полезных данных. Расположение сведения об ошибке отличается в зависимости от того, является ли формат SOAP или POX.
  
### <a name="soap-autodiscover-errors"></a>Ошибки автообнаружения SOAP

Для службы автообнаружения SOAP ответ может содержать один или несколько элементов [ErrorCode (SOAP)](http://msdn.microsoft.com/library/5e5ec861-0191-4ecb-a906-47ce8ed96381%28Office.15%29.aspx) в различных местах. Обычно можно ожидать один дочерний элемент элемента [Ответа SOAP](http://msdn.microsoft.com/library/4c2bcdeb-95ce-4ffa-bd83-118af53b534f%28Office.15%29.aspx) и качестве дочернего для каждого элемента [Ответ пользователя (SOAP)](http://msdn.microsoft.com/library/5007b1ba-bfcc-40d7-b1cb-e32fbaf54ffd%28Office.15%29.aspx) в ответе. В качестве дочернего для элемента [UserSettingError (SOAP)](http://msdn.microsoft.com/library/abb175c5-4f38-4dcc-81e3-b511686862eb%28Office.15%29.aspx) , также могут возникать при его наличии. Контекст ошибки зависит от того, где элемент **ErrorCode** расположена, как показано ниже: 
  
- Дочерний элемент элемент **ответа** **код ошибки** элемент представляет ошибку, которое применяется ко всему запросу. 
    
- Как дочерний элемент **ответ пользователя** он представляет ошибку, которая применяется только для определенных пользователей. 
    
- Как дочерний элемент **UserSettingError** он представляет ошибку, которая применяется к определенному параметру, который был запрошен. 
    
Давайте рассмотрим пример ответа. В этом примере **код ошибки** элемента под элементом **ответа** имеет значение «NoError», это означает успех проекта. Тем не менее **код ошибки** элемента под элементом **ответ пользователя** имеет значение «RedirectAddress», это означает, что произошла ошибка для данного пользователя. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/" 
    xmlns:a="http://www.w3.org/2005/08/addressing">
  <s:Header>
    <a:Action s:mustUnderstand="1">http://schemas.microsoft.com/exchange/2010/Autodiscover/Autodiscover/GetUserSettingsResponse</a:Action>
    <h:ServerVersionInfo xmlns:h="http://schemas.microsoft.com/exchange/2010/Autodiscover" 
        xmlns:i="http://www.w3.org/2001/XMLSchema-instance">
      <h:MajorVersion>14</h:MajorVersion>
      <h:MinorVersion>3</h:MinorVersion>
      <h:MajorBuildNumber>136</h:MajorBuildNumber>
      <h:MinorBuildNumber>1</h:MinorBuildNumber>
      <h:Version>Exchange2010_SP2</h:Version>
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

[Код ошибки (SOAP)](http://msdn.microsoft.com/library/5e5ec861-0191-4ecb-a906-47ce8ed96381%28Office.15%29.aspx) статья содержит полный список возможных ошибок. Большинство из их показывает Неустранимая ошибка, но некоторые гарантируете специальная обработка. 
  
**В таблице 2. Код ошибки Autodisover значения SOAP**

|**Код ошибки значение**|**Обработка...**|
|:-----|:-----|
|RedirectAddress  <br/> |[Перезапуск службы автообнаружения с новый адрес электронной почты](#bk_RestartAutodiscover) с адресом электронной почты в элементе [RedirectTarget (SOAP)](http://msdn.microsoft.com/library/f8162724-cf9a-4543-a1ad-5846c8b10bfa%28Office.15%29.aspx) .  <br/> |
|RedirectUrl  <br/> |[Повторная отправка запроса на новый URL-адрес](#bk_ResendRequest) в URL-адрес в элементе **RedirectTarget** .  <br/> |
|ServerBusy  <br/> |Повторите этот URL-адрес с небольшой задержкой. Может ждать установленного периода времени или просто перейти в конец списка URL-адресов для пробного этот URL-адрес. При получении данной ошибки несколько раз с URL-адреса, следует учитывать URL-адрес недопустим.  <br/> |
   
### <a name="pox-autodiscover-errors"></a>POX автоматического обнаружения ошибок

Служба автообнаружения POX немного по-разному сообщает об ошибках. Неустранимая ошибки содержащиеся в элементе [Ошибки (POX)](http://msdn.microsoft.com/library/91c63b62-ab68-4c32-a2f7-5a87c188335b%28Office.15%29.aspx) . [Код ошибки (POX)](http://msdn.microsoft.com/library/064d73e4-45b7-4797-828e-9df590830db8%28Office.15%29.aspx) статья содержит полный список кодов ошибок. 
  
Перенаправление ошибок, содержатся в элемент [Action (POX)](http://msdn.microsoft.com/library/a3462c6b-453c-462a-830d-f29ee4a2babb%28Office.15%29.aspx) . Любое значение элемент **Action** , отличный от «параметры» указывает на ошибки перенаправления. 
  
**В таблице 3. Код ошибки Autodisover POX значения**

|**Значение действия**|**Обработка...**|
|:-----|:-----|
|redirectAddr  <br/> |[Перезапуск службы автообнаружения с новый адрес электронной почты](#bk_RestartAutodiscover) с адресом электронной почты в элементе [RedirectAddr (POX)](http://msdn.microsoft.com/library/0e9fa6b6-7991-4dc1-a59a-48e5f8e041e4%28Office.15%29.aspx) .  <br/> |
|redirectUrl  <br/> |[Повторная отправка запроса на новый URL-адрес](#bk_ResendRequest) в URL-адрес в элемент [RedirectUrl (POX)](http://msdn.microsoft.com/library/c54f310f-8c99-4c37-8e73-ac87722b6229%28Office.15%29.aspx) .  <br/> |
   
В следующем примере элемент **Action** имеет значение «redirectAddr», который указывает отправку новый запрос с новый адрес электронной почты, содержащихся в элементе **RedirectAddr** . 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<Autodiscover xmlns="http://schemas.microsoft.com/exchange/autodiscover/responseschema/2006">
  <Response xmlns="http://schemas.microsoft.com/exchange/autodiscover/outlook/responseschema/2006a">
    <Account>
      <Action>redirectAddr</Action>
      <RedirectAddr>elvin@mail.contoso.com</RedirectAddr>
    </Account>
  </Response>
</Autodiscover>
```

## <a name="handling-redirect-errors"></a>Обработка ошибок перенаправления
<a name="bk_HandlingRedirects"> </a>

Может обрабатывать сценарии ошибка перенаправления двумя способами:
  
- Можно перезапустить службы автообнаружения с новый адрес электронной почты.
    
- С повторной отправки запроса на новый URL-адрес.
    
Оба сценария требуются некоторые проверки перед тем как перейти.
  
### <a name="restarting-autodiscover-with-a-new-email-address"></a>Перезапуск службы автообнаружения с новый адрес электронной почты
<a name="bk_RestartAutodiscover"> </a>

Когда вы получаете новый адрес электронной почты в автообнаружения перенаправление ответа, сначала убедитесь, что адрес электронной почты, которое было указано в ответ ошибка перенаправления не тот же адрес, отправляемых в запросе, который вызвал ошибку. Если он установлен, следует не перезапустите службы автообнаружения и URL-адрес, создавшее ответа недопустим в качестве альтернативы.
  
Если отличается новый адрес электронной почты, отменить существующий список возможных URL-адреса конечной точки службы автообнаружения и создать новый список на основе нового адреса электронной почты.
  
### <a name="resending-your-request-to-a-new-url"></a>Повторная отправка запроса на новый URL-адрес
<a name="bk_ResendRequest"> </a>

Получить новый URL-адрес в ответ перенаправить автообнаружения, сначала следует проверить URL-адрес следующим образом:
  
- Убедитесь, что URL-адрес, URL-адрес HTTPS.
    
- Убедитесь, что ошибка не получено из этот URL-адрес с текущей адрес электронной почты, прежде чем.
    
- Если это допустимо для приложения, оповещения пользователя в режиме одобрения администратором и получать их разрешение для выполнения перенаправления.
    
- Отправляет запрос на URL-адрес и [Убедитесь, что сертификат SSL на сервере является допустимым](how-to-validate-a-server-certificate-for-the-ews-managed-api.md).
    
Если URL-адрес проходит проверку, повторно отправьте запрос этот новый URL-адрес.
  
## <a name="see-also"></a>См. также


- [Автообнаружение для Exchange](autodiscover-for-exchange.md)
    
- [Найдите конечных точек службы автообнаружения с помощью поиска SCP в Exchange](how-to-find-autodiscover-endpoints-by-using-scp-lookup-in-exchange.md)
    
- [Код ошибки (SOAP)](http://msdn.microsoft.com/library/5e5ec861-0191-4ecb-a906-47ce8ed96381%28Office.15%29.aspx)
    
- [Код ошибки (POX)](http://msdn.microsoft.com/library/064d73e4-45b7-4797-828e-9df590830db8%28Office.15%29.aspx)
    

