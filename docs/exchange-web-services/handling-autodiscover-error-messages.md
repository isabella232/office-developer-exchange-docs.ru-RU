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
# <a name="handling-autodiscover-error-messages"></a><span data-ttu-id="80efb-103">Обработка сообщений об ошибках службы автообнаружения</span><span class="sxs-lookup"><span data-stu-id="80efb-103">Handling Autodiscover error messages</span></span>

<span data-ttu-id="80efb-104">Узнайте о различных типах автоматического обнаружения ошибок и что делать с ними.</span><span class="sxs-lookup"><span data-stu-id="80efb-104">Learn about the different types of Autodiscover errors and what to do with them.</span></span>
  
<span data-ttu-id="80efb-105">Автообнаружение включает приложения, чтобы автоматически извлечь сведения о конфигурации и прекрасно работает.</span><span class="sxs-lookup"><span data-stu-id="80efb-105">Autodiscover enables your applications to retrieve configuration information automatically, and it works great.</span></span> <span data-ttu-id="80efb-106">Тем не менее что не всегда переход согласно плану.</span><span class="sxs-lookup"><span data-stu-id="80efb-106">However, things don't always go according to plan.</span></span> <span data-ttu-id="80efb-107">Давайте взглянем на распространенные ошибки, которые могут возникать и как их для сведения к минимуму необходимость запрашивать вручную настроить клиент обработки.</span><span class="sxs-lookup"><span data-stu-id="80efb-107">Let's look at the common errors that might occur and how you can handle them to minimize the need to prompt your user to manually configure your client.</span></span>
  
## <a name="http-status-errors"></a><span data-ttu-id="80efb-108">Состояние ошибки HTTP</span><span class="sxs-lookup"><span data-stu-id="80efb-108">HTTP status errors</span></span>
<span data-ttu-id="80efb-109"><a name="bk_HttpErrors"> </a></span><span class="sxs-lookup"><span data-stu-id="80efb-109"></span></span>

<span data-ttu-id="80efb-110">Первый тип ошибки, которые могут возникать при отправке запросов автообнаружения — состояние HTTP.</span><span class="sxs-lookup"><span data-stu-id="80efb-110">The first type of error you might encounter when sending Autodiscover requests is the HTTP status.</span></span> <span data-ttu-id="80efb-111">Если отображается состояние HTTP в свой ответ отличное от 200 (ОК), полезных данных ответа не содержит ответа службы автообнаружения, который вы искали.</span><span class="sxs-lookup"><span data-stu-id="80efb-111">If the HTTP status in your response is anything other than 200 (OK), the response payload doesn't contain the Autodiscover response you were looking for.</span></span> <span data-ttu-id="80efb-112">Для простоты выполняется группировка кодов состояния не 200 на три категории.</span><span class="sxs-lookup"><span data-stu-id="80efb-112">For simplicity, we can group non-200 status codes into three categories.</span></span>
  
<span data-ttu-id="80efb-113">**В таблице 1. Коды состояния HTTP**</span><span class="sxs-lookup"><span data-stu-id="80efb-113">**Table 1. HTTP status codes**</span></span>

|<span data-ttu-id="80efb-114">**Код состояния**</span><span class="sxs-lookup"><span data-stu-id="80efb-114">**Status code**</span></span>|<span data-ttu-id="80efb-115">**Тип ошибки**</span><span class="sxs-lookup"><span data-stu-id="80efb-115">**Type of error**</span></span>|<span data-ttu-id="80efb-116">**Обработка...**</span><span class="sxs-lookup"><span data-stu-id="80efb-116">**To handle…**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="80efb-117">301 или 302</span><span class="sxs-lookup"><span data-stu-id="80efb-117">301 or 302</span></span>  <br/> |<span data-ttu-id="80efb-118">Перенаправление ошибок</span><span class="sxs-lookup"><span data-stu-id="80efb-118">Redirect error</span></span>  <br/> |<span data-ttu-id="80efb-119">Повторно отправьте запрос к URI, содержащихся в заголовке ответа «Расположение» HTTP.</span><span class="sxs-lookup"><span data-stu-id="80efb-119">Resend your request to the URI contained in the "Location" HTTP response header.</span></span> <span data-ttu-id="80efb-120">Дополнительные сведения см [Перенаправление обработки ошибок](#bk_HandlingRedirects).</span><span class="sxs-lookup"><span data-stu-id="80efb-120">For details, see [Handling redirect errors](#bk_HandlingRedirects).</span></span>  <br/> |
|<span data-ttu-id="80efb-121">401</span><span class="sxs-lookup"><span data-stu-id="80efb-121">401</span></span>  <br/> |<span data-ttu-id="80efb-122">Сообщение об ошибке авторизации</span><span class="sxs-lookup"><span data-stu-id="80efb-122">Unauthorized error</span></span>  <br/> |<span data-ttu-id="80efb-123">Так как [процесс автообнаружения](autodiscover-for-exchange.md) состоит из ознакомления с несколько возможных URL-адресов, получения это на один URL-адрес, только чтобы следующим принять свои учетные данные.</span><span class="sxs-lookup"><span data-stu-id="80efb-123">Because the [Autodiscover process](autodiscover-for-exchange.md) involves trying multiple potential URLs, you could get this on one URL only to have the next one accept your credentials.</span></span> <span data-ttu-id="80efb-124">По этой причине не следует учитывать одной 401 об ошибке, указывающее, что учетные данные являются недопустимыми.</span><span class="sxs-lookup"><span data-stu-id="80efb-124">For this reason, you shouldn't consider a single 401 error to indicate that the credentials are invalid.</span></span> <span data-ttu-id="80efb-125">Тем не менее в случае 401 ошибок из несколько URL-адресов, можно запрашивать повторно введите пароль (если это возможно).</span><span class="sxs-lookup"><span data-stu-id="80efb-125">However, if you receive 401 errors from multiple URLs, you might want to prompt the user to reenter their password (if possible).</span></span>  <br/> |
|<span data-ttu-id="80efb-126">Другие состояния не 200</span><span class="sxs-lookup"><span data-stu-id="80efb-126">Any other non-200 status</span></span>  <br/> |<span data-ttu-id="80efb-127">Недопустимый ошибка конечной точки службы автообнаружения</span><span class="sxs-lookup"><span data-stu-id="80efb-127">Invalid Autodiscover endpoint error</span></span>  <br/> |<span data-ttu-id="80efb-128">Попробуйте URL-адрес, который возвращает другой код состояния не 200 недействительной и повторить попытку следующий URL-адрес в списке.</span><span class="sxs-lookup"><span data-stu-id="80efb-128">Consider the URL that returns any other non-200 status code to be invalid, and continue trying the next URL in your list.</span></span>  <br/> |
   
## <a name="autodiscover-errors"></a><span data-ttu-id="80efb-129">Ошибки службы автообнаружения</span><span class="sxs-lookup"><span data-stu-id="80efb-129">Autodiscover errors</span></span>
<span data-ttu-id="80efb-130"><a name="bk_AutodiscoverErrors"> </a></span><span class="sxs-lookup"><span data-stu-id="80efb-130"></span></span>

<span data-ttu-id="80efb-131">Даже если код состояния 200 (ОК) после отправки запроса службы автообнаружения, это не означает, что сервер отправляться информацию, необходимую.</span><span class="sxs-lookup"><span data-stu-id="80efb-131">Even if you get a 200 (OK) status code after sending an Autodiscover request, that doesn't mean that the server sent the information you need.</span></span> <span data-ttu-id="80efb-132">200 состояние только означает, что у вас есть ответа службы автообнаружения и этого ответа может содержать ошибки внутри полезных данных.</span><span class="sxs-lookup"><span data-stu-id="80efb-132">The 200 status only means that you have an Autodiscover response, and that response might contain an error within the payload.</span></span> <span data-ttu-id="80efb-133">Расположение сведения об ошибке отличается в зависимости от того, является ли формат SOAP или POX.</span><span class="sxs-lookup"><span data-stu-id="80efb-133">The location of the error information differs depending on whether the format is SOAP or POX.</span></span>
  
### <a name="soap-autodiscover-errors"></a><span data-ttu-id="80efb-134">Ошибки автообнаружения SOAP</span><span class="sxs-lookup"><span data-stu-id="80efb-134">SOAP Autodiscover errors</span></span>

<span data-ttu-id="80efb-135">Для службы автообнаружения SOAP ответ может содержать один или несколько элементов [ErrorCode (SOAP)](http://msdn.microsoft.com/library/5e5ec861-0191-4ecb-a906-47ce8ed96381%28Office.15%29.aspx) в различных местах.</span><span class="sxs-lookup"><span data-stu-id="80efb-135">For SOAP Autodiscover, the response can contain one or more [ErrorCode (SOAP)](http://msdn.microsoft.com/library/5e5ec861-0191-4ecb-a906-47ce8ed96381%28Office.15%29.aspx) elements, in different places.</span></span> <span data-ttu-id="80efb-136">Обычно можно ожидать один дочерний элемент элемента [Ответа SOAP](http://msdn.microsoft.com/library/4c2bcdeb-95ce-4ffa-bd83-118af53b534f%28Office.15%29.aspx) и качестве дочернего для каждого элемента [Ответ пользователя (SOAP)](http://msdn.microsoft.com/library/5007b1ba-bfcc-40d7-b1cb-e32fbaf54ffd%28Office.15%29.aspx) в ответе.</span><span class="sxs-lookup"><span data-stu-id="80efb-136">Typically you can expect one as a child element of the [Response (SOAP)](http://msdn.microsoft.com/library/4c2bcdeb-95ce-4ffa-bd83-118af53b534f%28Office.15%29.aspx) element, and one as a child of each [UserResponse (SOAP)](http://msdn.microsoft.com/library/5007b1ba-bfcc-40d7-b1cb-e32fbaf54ffd%28Office.15%29.aspx) element in the response.</span></span> <span data-ttu-id="80efb-137">В качестве дочернего для элемента [UserSettingError (SOAP)](http://msdn.microsoft.com/library/abb175c5-4f38-4dcc-81e3-b511686862eb%28Office.15%29.aspx) , также могут возникать при его наличии.</span><span class="sxs-lookup"><span data-stu-id="80efb-137">You might also encounter one as a child of a [UserSettingError (SOAP)](http://msdn.microsoft.com/library/abb175c5-4f38-4dcc-81e3-b511686862eb%28Office.15%29.aspx) element, if one is present.</span></span> <span data-ttu-id="80efb-138">Контекст ошибки зависит от того, где элемент **ErrorCode** расположена, как показано ниже:</span><span class="sxs-lookup"><span data-stu-id="80efb-138">The context of the error depends on where the **ErrorCode** element is located, as follows:</span></span> 
  
- <span data-ttu-id="80efb-139">Дочерний элемент элемент **ответа** **код ошибки** элемент представляет ошибку, которое применяется ко всему запросу.</span><span class="sxs-lookup"><span data-stu-id="80efb-139">As a child element of the **Response** element, the **ErrorCode** element represents an error that applies to the entire request.</span></span> 
    
- <span data-ttu-id="80efb-140">Как дочерний элемент **ответ пользователя** он представляет ошибку, которая применяется только для определенных пользователей.</span><span class="sxs-lookup"><span data-stu-id="80efb-140">As a child of the **UserResponse** element, it represents an error that applies just to that specific user.</span></span> 
    
- <span data-ttu-id="80efb-141">Как дочерний элемент **UserSettingError** он представляет ошибку, которая применяется к определенному параметру, который был запрошен.</span><span class="sxs-lookup"><span data-stu-id="80efb-141">As a child of a **UserSettingError** element, it represents an error that applies to a specific setting that was requested.</span></span> 
    
<span data-ttu-id="80efb-142">Давайте рассмотрим пример ответа.</span><span class="sxs-lookup"><span data-stu-id="80efb-142">Let's take a look at an example of a response.</span></span> <span data-ttu-id="80efb-143">В этом примере **код ошибки** элемента под элементом **ответа** имеет значение «NoError», это означает успех проекта.</span><span class="sxs-lookup"><span data-stu-id="80efb-143">In this example, the **ErrorCode** element under the **Response** element has a value of "NoError", which indicates overall success.</span></span> <span data-ttu-id="80efb-144">Тем не менее **код ошибки** элемента под элементом **ответ пользователя** имеет значение «RedirectAddress», это означает, что произошла ошибка для данного пользователя.</span><span class="sxs-lookup"><span data-stu-id="80efb-144">However, the **ErrorCode** element under the **UserResponse** element has a value of "RedirectAddress", which indicates that an error occurred for that particular user.</span></span> 
  
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

<span data-ttu-id="80efb-145">[Код ошибки (SOAP)](http://msdn.microsoft.com/library/5e5ec861-0191-4ecb-a906-47ce8ed96381%28Office.15%29.aspx) статья содержит полный список возможных ошибок.</span><span class="sxs-lookup"><span data-stu-id="80efb-145">The [ErrorCode (SOAP)](http://msdn.microsoft.com/library/5e5ec861-0191-4ecb-a906-47ce8ed96381%28Office.15%29.aspx) article contains a full list of possible errors.</span></span> <span data-ttu-id="80efb-146">Большинство из их показывает Неустранимая ошибка, но некоторые гарантируете специальная обработка.</span><span class="sxs-lookup"><span data-stu-id="80efb-146">Most of these indicate an unrecoverable error, but a few warrant special handling.</span></span> 
  
<span data-ttu-id="80efb-147">**В таблице 2. Код ошибки Autodisover значения SOAP**</span><span class="sxs-lookup"><span data-stu-id="80efb-147">**Table 2. SOAP Autodisover ErrorCode values**</span></span>

|<span data-ttu-id="80efb-148">**Код ошибки значение**</span><span class="sxs-lookup"><span data-stu-id="80efb-148">**ErrorCode value**</span></span>|<span data-ttu-id="80efb-149">**Обработка...**</span><span class="sxs-lookup"><span data-stu-id="80efb-149">**To handle…**</span></span>|
|:-----|:-----|
|<span data-ttu-id="80efb-150">RedirectAddress</span><span class="sxs-lookup"><span data-stu-id="80efb-150">RedirectAddress</span></span>  <br/> |<span data-ttu-id="80efb-151">[Перезапуск службы автообнаружения с новый адрес электронной почты](#bk_RestartAutodiscover) с адресом электронной почты в элементе [RedirectTarget (SOAP)](http://msdn.microsoft.com/library/f8162724-cf9a-4543-a1ad-5846c8b10bfa%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="80efb-151">[Restarting Autodiscover with a new email address](#bk_RestartAutodiscover) with the email address in the [RedirectTarget (SOAP)](http://msdn.microsoft.com/library/f8162724-cf9a-4543-a1ad-5846c8b10bfa%28Office.15%29.aspx) element.</span></span>  <br/> |
|<span data-ttu-id="80efb-152">RedirectUrl</span><span class="sxs-lookup"><span data-stu-id="80efb-152">RedirectUrl</span></span>  <br/> |<span data-ttu-id="80efb-153">[Повторная отправка запроса на новый URL-адрес](#bk_ResendRequest) в URL-адрес в элементе **RedirectTarget** .</span><span class="sxs-lookup"><span data-stu-id="80efb-153">[Resending your request to a new URL](#bk_ResendRequest) to the URL in the **RedirectTarget** element.</span></span>  <br/> |
|<span data-ttu-id="80efb-154">ServerBusy</span><span class="sxs-lookup"><span data-stu-id="80efb-154">ServerBusy</span></span>  <br/> |<span data-ttu-id="80efb-155">Повторите этот URL-адрес с небольшой задержкой.</span><span class="sxs-lookup"><span data-stu-id="80efb-155">Retry this URL after a small delay.</span></span> <span data-ttu-id="80efb-156">Может ждать установленного периода времени или просто перейти в конец списка URL-адресов для пробного этот URL-адрес.</span><span class="sxs-lookup"><span data-stu-id="80efb-156">You might wait a set amount of time or simply move this URL to the end of your list of URLs to try.</span></span> <span data-ttu-id="80efb-157">При получении данной ошибки несколько раз с URL-адреса, следует учитывать URL-адрес недопустим.</span><span class="sxs-lookup"><span data-stu-id="80efb-157">If you receive this error multiple times from a URL, you should consider the URL to be invalid.</span></span>  <br/> |
   
### <a name="pox-autodiscover-errors"></a><span data-ttu-id="80efb-158">POX автоматического обнаружения ошибок</span><span class="sxs-lookup"><span data-stu-id="80efb-158">POX Autodiscover errors</span></span>

<span data-ttu-id="80efb-159">Служба автообнаружения POX немного по-разному сообщает об ошибках.</span><span class="sxs-lookup"><span data-stu-id="80efb-159">The POX Autodiscover service reports errors a little differently.</span></span> <span data-ttu-id="80efb-160">Неустранимая ошибки содержащиеся в элементе [Ошибки (POX)](http://msdn.microsoft.com/library/91c63b62-ab68-4c32-a2f7-5a87c188335b%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="80efb-160">Non-recoverable errors are contained in the [Error (POX)](http://msdn.microsoft.com/library/91c63b62-ab68-4c32-a2f7-5a87c188335b%28Office.15%29.aspx) element.</span></span> <span data-ttu-id="80efb-161">[Код ошибки (POX)](http://msdn.microsoft.com/library/064d73e4-45b7-4797-828e-9df590830db8%28Office.15%29.aspx) статья содержит полный список кодов ошибок.</span><span class="sxs-lookup"><span data-stu-id="80efb-161">The [ErrorCode (POX)](http://msdn.microsoft.com/library/064d73e4-45b7-4797-828e-9df590830db8%28Office.15%29.aspx) article contains a full list of possible error codes.</span></span> 
  
<span data-ttu-id="80efb-162">Перенаправление ошибок, содержатся в элемент [Action (POX)](http://msdn.microsoft.com/library/a3462c6b-453c-462a-830d-f29ee4a2babb%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="80efb-162">Redirect errors are contained in the [Action (POX)](http://msdn.microsoft.com/library/a3462c6b-453c-462a-830d-f29ee4a2babb%28Office.15%29.aspx) element.</span></span> <span data-ttu-id="80efb-163">Любое значение элемент **Action** , отличный от «параметры» указывает на ошибки перенаправления.</span><span class="sxs-lookup"><span data-stu-id="80efb-163">Any value of the **Action** element other than "settings" indicates a redirect error.</span></span> 
  
<span data-ttu-id="80efb-164">**В таблице 3. Код ошибки Autodisover POX значения**</span><span class="sxs-lookup"><span data-stu-id="80efb-164">**Table 3. POX Autodisover ErrorCode values**</span></span>

|<span data-ttu-id="80efb-165">**Значение действия**</span><span class="sxs-lookup"><span data-stu-id="80efb-165">**Action value**</span></span>|<span data-ttu-id="80efb-166">**Обработка...**</span><span class="sxs-lookup"><span data-stu-id="80efb-166">**To handle…**</span></span>|
|:-----|:-----|
|<span data-ttu-id="80efb-167">redirectAddr</span><span class="sxs-lookup"><span data-stu-id="80efb-167">redirectAddr</span></span>  <br/> |<span data-ttu-id="80efb-168">[Перезапуск службы автообнаружения с новый адрес электронной почты](#bk_RestartAutodiscover) с адресом электронной почты в элементе [RedirectAddr (POX)](http://msdn.microsoft.com/library/0e9fa6b6-7991-4dc1-a59a-48e5f8e041e4%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="80efb-168">[Restarting Autodiscover with a new email address](#bk_RestartAutodiscover) with the email address in the [RedirectAddr (POX)](http://msdn.microsoft.com/library/0e9fa6b6-7991-4dc1-a59a-48e5f8e041e4%28Office.15%29.aspx) element.</span></span>  <br/> |
|<span data-ttu-id="80efb-169">redirectUrl</span><span class="sxs-lookup"><span data-stu-id="80efb-169">redirectUrl</span></span>  <br/> |<span data-ttu-id="80efb-170">[Повторная отправка запроса на новый URL-адрес](#bk_ResendRequest) в URL-адрес в элемент [RedirectUrl (POX)](http://msdn.microsoft.com/library/c54f310f-8c99-4c37-8e73-ac87722b6229%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="80efb-170">[Resending your request to a new URL](#bk_ResendRequest) to the URL in the [RedirectUrl (POX)](http://msdn.microsoft.com/library/c54f310f-8c99-4c37-8e73-ac87722b6229%28Office.15%29.aspx) element.</span></span>  <br/> |
   
<span data-ttu-id="80efb-171">В следующем примере элемент **Action** имеет значение «redirectAddr», который указывает отправку новый запрос с новый адрес электронной почты, содержащихся в элементе **RedirectAddr** .</span><span class="sxs-lookup"><span data-stu-id="80efb-171">In this example, the **Action** element has a value of "redirectAddr", which indicates that a new request should be sent with the new email address contained in the **RedirectAddr** element.</span></span> 
  
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

## <a name="handling-redirect-errors"></a><span data-ttu-id="80efb-172">Обработка ошибок перенаправления</span><span class="sxs-lookup"><span data-stu-id="80efb-172">Handling redirect errors</span></span>
<span data-ttu-id="80efb-173"><a name="bk_HandlingRedirects"> </a></span><span class="sxs-lookup"><span data-stu-id="80efb-173"></span></span>

<span data-ttu-id="80efb-174">Может обрабатывать сценарии ошибка перенаправления двумя способами:</span><span class="sxs-lookup"><span data-stu-id="80efb-174">You can handle redirect error scenarios in two ways:</span></span>
  
- <span data-ttu-id="80efb-175">Можно перезапустить службы автообнаружения с новый адрес электронной почты.</span><span class="sxs-lookup"><span data-stu-id="80efb-175">By restarting Autodiscover with a new email address.</span></span>
    
- <span data-ttu-id="80efb-176">С повторной отправки запроса на новый URL-адрес.</span><span class="sxs-lookup"><span data-stu-id="80efb-176">By resending your request to a new URL.</span></span>
    
<span data-ttu-id="80efb-177">Оба сценария требуются некоторые проверки перед тем как перейти.</span><span class="sxs-lookup"><span data-stu-id="80efb-177">Both scenarios require some validation before proceeding.</span></span>
  
### <a name="restarting-autodiscover-with-a-new-email-address"></a><span data-ttu-id="80efb-178">Перезапуск службы автообнаружения с новый адрес электронной почты</span><span class="sxs-lookup"><span data-stu-id="80efb-178">Restarting Autodiscover with a new email address</span></span>
<span data-ttu-id="80efb-179"><a name="bk_RestartAutodiscover"> </a></span><span class="sxs-lookup"><span data-stu-id="80efb-179"></span></span>

<span data-ttu-id="80efb-180">Когда вы получаете новый адрес электронной почты в автообнаружения перенаправление ответа, сначала убедитесь, что адрес электронной почты, которое было указано в ответ ошибка перенаправления не тот же адрес, отправляемых в запросе, который вызвал ошибку.</span><span class="sxs-lookup"><span data-stu-id="80efb-180">When you get a new email address in an Autodiscover redirect response, first verify that the new email address that was provided in the redirect error response is not the same address that you sent in the request that resulted in the error.</span></span> <span data-ttu-id="80efb-181">Если он установлен, следует не перезапустите службы автообнаружения и URL-адрес, создавшее ответа недопустим в качестве альтернативы.</span><span class="sxs-lookup"><span data-stu-id="80efb-181">If it is, you should not restart Autodiscover and instead consider the URL that generated the response to be invalid.</span></span>
  
<span data-ttu-id="80efb-182">Если отличается новый адрес электронной почты, отменить существующий список возможных URL-адреса конечной точки службы автообнаружения и создать новый список на основе нового адреса электронной почты.</span><span class="sxs-lookup"><span data-stu-id="80efb-182">If the new email address is different, discard your existing list of potential Autodiscover endpoint URLs and generate a new list based on the new email address.</span></span>
  
### <a name="resending-your-request-to-a-new-url"></a><span data-ttu-id="80efb-183">Повторная отправка запроса на новый URL-адрес</span><span class="sxs-lookup"><span data-stu-id="80efb-183">Resending your request to a new URL</span></span>
<span data-ttu-id="80efb-184"><a name="bk_ResendRequest"> </a></span><span class="sxs-lookup"><span data-stu-id="80efb-184"></span></span>

<span data-ttu-id="80efb-185">Получить новый URL-адрес в ответ перенаправить автообнаружения, сначала следует проверить URL-адрес следующим образом:</span><span class="sxs-lookup"><span data-stu-id="80efb-185">When you get a new URL in an Autodiscover redirect response, you should first validate the URL as follows:</span></span>
  
- <span data-ttu-id="80efb-186">Убедитесь, что URL-адрес, URL-адрес HTTPS.</span><span class="sxs-lookup"><span data-stu-id="80efb-186">Verify that the URL is an HTTPS URL.</span></span>
    
- <span data-ttu-id="80efb-187">Убедитесь, что ошибка не получено из этот URL-адрес с текущей адрес электронной почты, прежде чем.</span><span class="sxs-lookup"><span data-stu-id="80efb-187">Verify that you have not received an error from this URL with the current email address before.</span></span>
    
- <span data-ttu-id="80efb-188">Если это допустимо для приложения, оповещения пользователя в режиме одобрения администратором и получать их разрешение для выполнения перенаправления.</span><span class="sxs-lookup"><span data-stu-id="80efb-188">If applicable to your application, inform the user of the redirection and get their permission to follow the redirect.</span></span>
    
- <span data-ttu-id="80efb-189">Отправляет запрос на URL-адрес и [Убедитесь, что сертификат SSL на сервере является допустимым](how-to-validate-a-server-certificate-for-the-ews-managed-api.md).</span><span class="sxs-lookup"><span data-stu-id="80efb-189">Send a request to the URL and [verify that the SSL certificate presented by the server is valid](how-to-validate-a-server-certificate-for-the-ews-managed-api.md).</span></span>
    
<span data-ttu-id="80efb-190">Если URL-адрес проходит проверку, повторно отправьте запрос этот новый URL-адрес.</span><span class="sxs-lookup"><span data-stu-id="80efb-190">If the URL passes validation, resend the request to this new URL.</span></span>
  
## <a name="see-also"></a><span data-ttu-id="80efb-191">См. также</span><span class="sxs-lookup"><span data-stu-id="80efb-191">See also</span></span>


- [<span data-ttu-id="80efb-192">Автообнаружение для Exchange</span><span class="sxs-lookup"><span data-stu-id="80efb-192">Autodiscover for Exchange</span></span>](autodiscover-for-exchange.md)
    
- [<span data-ttu-id="80efb-193">Найдите конечных точек службы автообнаружения с помощью поиска SCP в Exchange</span><span class="sxs-lookup"><span data-stu-id="80efb-193">Find Autodiscover endpoints by using SCP lookup in Exchange</span></span>](how-to-find-autodiscover-endpoints-by-using-scp-lookup-in-exchange.md)
    
- [<span data-ttu-id="80efb-194">Код ошибки (SOAP)</span><span class="sxs-lookup"><span data-stu-id="80efb-194">ErrorCode (SOAP)</span></span>](http://msdn.microsoft.com/library/5e5ec861-0191-4ecb-a906-47ce8ed96381%28Office.15%29.aspx)
    
- [<span data-ttu-id="80efb-195">Код ошибки (POX)</span><span class="sxs-lookup"><span data-stu-id="80efb-195">ErrorCode (POX)</span></span>](http://msdn.microsoft.com/library/064d73e4-45b7-4797-828e-9df590830db8%28Office.15%29.aspx)
    

