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
# <a name="handling-autodiscover-error-messages"></a><span data-ttu-id="648c9-103">Обработка сообщений об ошибках службы автообнаружения</span><span class="sxs-lookup"><span data-stu-id="648c9-103">Handling Autodiscover error messages</span></span>

<span data-ttu-id="648c9-104">Узнайте о различных типах ошибок автообнаружения и действиях, которые необходимо выполнить.</span><span class="sxs-lookup"><span data-stu-id="648c9-104">Learn about the different types of Autodiscover errors and what to do with them.</span></span>
  
<span data-ttu-id="648c9-105">Служба автообнаружения позволяет приложениям автоматически получать сведения о конфигурации и прекрасно работает.</span><span class="sxs-lookup"><span data-stu-id="648c9-105">Autodiscover enables your applications to retrieve configuration information automatically, and it works great.</span></span> <span data-ttu-id="648c9-106">Тем не менее, они не всегда переходят в соответствии с планом.</span><span class="sxs-lookup"><span data-stu-id="648c9-106">However, things don't always go according to plan.</span></span> <span data-ttu-id="648c9-107">Рассмотрим распространенные ошибки и их обработку, чтобы свести к минимуму необходимость запрашивать пользователя вручную для настройки клиента.</span><span class="sxs-lookup"><span data-stu-id="648c9-107">Let's look at the common errors that might occur and how you can handle them to minimize the need to prompt your user to manually configure your client.</span></span>
  
## <a name="http-status-errors"></a><span data-ttu-id="648c9-108">Ошибки состояния HTTP</span><span class="sxs-lookup"><span data-stu-id="648c9-108">HTTP status errors</span></span>
<span data-ttu-id="648c9-109"><a name="bk_HttpErrors"> </a></span><span class="sxs-lookup"><span data-stu-id="648c9-109"><a name="bk_HttpErrors"> </a></span></span>

<span data-ttu-id="648c9-110">Первый тип ошибки, которая может возникнуть при отправке запросов автообнаружения — это состояние HTTP.</span><span class="sxs-lookup"><span data-stu-id="648c9-110">The first type of error you might encounter when sending Autodiscover requests is the HTTP status.</span></span> <span data-ttu-id="648c9-111">Если состояние HTTP в отклике отлично от 200 (ОК), полезные данные отклика не содержат ответ автообнаружения, который вы искали.</span><span class="sxs-lookup"><span data-stu-id="648c9-111">If the HTTP status in your response is anything other than 200 (OK), the response payload doesn't contain the Autodiscover response you were looking for.</span></span> <span data-ttu-id="648c9-112">Для простоты мы можем группировать коды состояния, не относящиеся к 200, в три категории.</span><span class="sxs-lookup"><span data-stu-id="648c9-112">For simplicity, we can group non-200 status codes into three categories.</span></span>
  
<span data-ttu-id="648c9-113">**Таблица 1. Коды состояния HTTP**</span><span class="sxs-lookup"><span data-stu-id="648c9-113">**Table 1. HTTP status codes**</span></span>

|<span data-ttu-id="648c9-114">**Код состояния**</span><span class="sxs-lookup"><span data-stu-id="648c9-114">**Status code**</span></span>|<span data-ttu-id="648c9-115">**Тип ошибки**</span><span class="sxs-lookup"><span data-stu-id="648c9-115">**Type of error**</span></span>|<span data-ttu-id="648c9-116">**Обработка...**</span><span class="sxs-lookup"><span data-stu-id="648c9-116">**To handle…**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="648c9-117">301 или 302</span><span class="sxs-lookup"><span data-stu-id="648c9-117">301 or 302</span></span>  <br/> |<span data-ttu-id="648c9-118">Ошибка перенаправления</span><span class="sxs-lookup"><span data-stu-id="648c9-118">Redirect error</span></span>  <br/> |<span data-ttu-id="648c9-119">Отправьте запрос в URI, содержащийся в заголовке HTTP-ответа "Location".</span><span class="sxs-lookup"><span data-stu-id="648c9-119">Resend your request to the URI contained in the "Location" HTTP response header.</span></span> <span data-ttu-id="648c9-120">Дополнительные сведения см в разделе [Обработка ошибок перенаправления](#bk_HandlingRedirects).</span><span class="sxs-lookup"><span data-stu-id="648c9-120">For details, see [Handling redirect errors](#bk_HandlingRedirects).</span></span>  <br/> |
|<span data-ttu-id="648c9-121">401</span><span class="sxs-lookup"><span data-stu-id="648c9-121">401</span></span>  <br/> |<span data-ttu-id="648c9-122">Несанкционированная ошибка</span><span class="sxs-lookup"><span data-stu-id="648c9-122">Unauthorized error</span></span>  <br/> |<span data-ttu-id="648c9-123">Так как [процесс автообнаружения](autodiscover-for-exchange.md) включает несколько возможных URL-адресов, вы можете получить их по одному URL-адресу, чтобы только следующий пользователь принимал свои учетные данные.</span><span class="sxs-lookup"><span data-stu-id="648c9-123">Because the [Autodiscover process](autodiscover-for-exchange.md) involves trying multiple potential URLs, you could get this on one URL only to have the next one accept your credentials.</span></span> <span data-ttu-id="648c9-124">По этой причине не следует учитывать одну ошибку 401, указывающую на недопустимые учетные данные.</span><span class="sxs-lookup"><span data-stu-id="648c9-124">For this reason, you shouldn't consider a single 401 error to indicate that the credentials are invalid.</span></span> <span data-ttu-id="648c9-125">Однако при получении сообщений об ошибках 401 из нескольких URL-адресов может потребоваться, чтобы пользователь повторно вводил свой пароль (если это возможно).</span><span class="sxs-lookup"><span data-stu-id="648c9-125">However, if you receive 401 errors from multiple URLs, you might want to prompt the user to reenter their password (if possible).</span></span>  <br/> |
|<span data-ttu-id="648c9-126">Любое другое состояние, отличное от 200</span><span class="sxs-lookup"><span data-stu-id="648c9-126">Any other non-200 status</span></span>  <br/> |<span data-ttu-id="648c9-127">Недопустимая ошибка конечной точки автообнаружения</span><span class="sxs-lookup"><span data-stu-id="648c9-127">Invalid Autodiscover endpoint error</span></span>  <br/> |<span data-ttu-id="648c9-128">Рассмотрим URL-адрес, который возвращает любой другой код состояния, не относящийся к 200, и продолжайте пытаться использовать следующий URL-адрес в списке.</span><span class="sxs-lookup"><span data-stu-id="648c9-128">Consider the URL that returns any other non-200 status code to be invalid, and continue trying the next URL in your list.</span></span>  <br/> |
   
## <a name="autodiscover-errors"></a><span data-ttu-id="648c9-129">Ошибки автообнаружения</span><span class="sxs-lookup"><span data-stu-id="648c9-129">Autodiscover errors</span></span>
<span data-ttu-id="648c9-130"><a name="bk_AutodiscoverErrors"> </a></span><span class="sxs-lookup"><span data-stu-id="648c9-130"><a name="bk_AutodiscoverErrors"> </a></span></span>

<span data-ttu-id="648c9-131">Даже если вы получаете код состояния 200 (OK) после отправки запроса на обнаружение, это не означает, что сервер отправил необходимые сведения.</span><span class="sxs-lookup"><span data-stu-id="648c9-131">Even if you get a 200 (OK) status code after sending an Autodiscover request, that doesn't mean that the server sent the information you need.</span></span> <span data-ttu-id="648c9-132">Состояние 200 означает, что у вас есть ответ автообнаружения, и ответ может содержать ошибку в полезных данных.</span><span class="sxs-lookup"><span data-stu-id="648c9-132">The 200 status only means that you have an Autodiscover response, and that response might contain an error within the payload.</span></span> <span data-ttu-id="648c9-133">Расположение сведений об ошибке зависит от того, является ли формат SOAP или POX.</span><span class="sxs-lookup"><span data-stu-id="648c9-133">The location of the error information differs depending on whether the format is SOAP or POX.</span></span>
  
### <a name="soap-autodiscover-errors"></a><span data-ttu-id="648c9-134">Ошибки автообнаружения SOAP</span><span class="sxs-lookup"><span data-stu-id="648c9-134">SOAP Autodiscover errors</span></span>

<span data-ttu-id="648c9-135">Для автообнаружения SOAP ответ может содержать один или несколько элементов [ErrorCode (SOAP)](https://msdn.microsoft.com/library/5e5ec861-0191-4ecb-a906-47ce8ed96381%28Office.15%29.aspx) в разных местах.</span><span class="sxs-lookup"><span data-stu-id="648c9-135">For SOAP Autodiscover, the response can contain one or more [ErrorCode (SOAP)](https://msdn.microsoft.com/library/5e5ec861-0191-4ecb-a906-47ce8ed96381%28Office.15%29.aspx) elements, in different places.</span></span> <span data-ttu-id="648c9-136">Как правило, вы можете ожидать один дочерний элемент элемента [Response (SOAP)](https://msdn.microsoft.com/library/4c2bcdeb-95ce-4ffa-bd83-118af53b534f%28Office.15%29.aspx) , а другой в качестве дочернего для каждого элемента [усерреспонсе (SOAP)](https://msdn.microsoft.com/library/5007b1ba-bfcc-40d7-b1cb-e32fbaf54ffd%28Office.15%29.aspx) в ответе.</span><span class="sxs-lookup"><span data-stu-id="648c9-136">Typically you can expect one as a child element of the [Response (SOAP)](https://msdn.microsoft.com/library/4c2bcdeb-95ce-4ffa-bd83-118af53b534f%28Office.15%29.aspx) element, and one as a child of each [UserResponse (SOAP)](https://msdn.microsoft.com/library/5007b1ba-bfcc-40d7-b1cb-e32fbaf54ffd%28Office.15%29.aspx) element in the response.</span></span> <span data-ttu-id="648c9-137">Кроме того, вы также можете столкнуться с одним дочерним элементом элемента [усерсеттинжеррор (SOAP)](https://msdn.microsoft.com/library/abb175c5-4f38-4dcc-81e3-b511686862eb%28Office.15%29.aspx) , если он присутствует.</span><span class="sxs-lookup"><span data-stu-id="648c9-137">You might also encounter one as a child of a [UserSettingError (SOAP)](https://msdn.microsoft.com/library/abb175c5-4f38-4dcc-81e3-b511686862eb%28Office.15%29.aspx) element, if one is present.</span></span> <span data-ttu-id="648c9-138">Контекст ошибки зависит от того, где находится элемент **ErrorCode** , как показано ниже.</span><span class="sxs-lookup"><span data-stu-id="648c9-138">The context of the error depends on where the **ErrorCode** element is located, as follows:</span></span> 
  
- <span data-ttu-id="648c9-139">В качестве дочернего элемента элемента **Response** элемент **ErrorCode** представляет ошибку, которая применяется ко всему запросу.</span><span class="sxs-lookup"><span data-stu-id="648c9-139">As a child element of the **Response** element, the **ErrorCode** element represents an error that applies to the entire request.</span></span> 
    
- <span data-ttu-id="648c9-140">В качестве дочернего элемента для элемента **усерреспонсе** представляет ошибку, которая применяется только к определенному пользователю.</span><span class="sxs-lookup"><span data-stu-id="648c9-140">As a child of the **UserResponse** element, it represents an error that applies just to that specific user.</span></span> 
    
- <span data-ttu-id="648c9-141">В качестве дочернего элемента для элемента **усерсеттинжеррор** представляет ошибку, которая применяется к определенному запрошенному параметру.</span><span class="sxs-lookup"><span data-stu-id="648c9-141">As a child of a **UserSettingError** element, it represents an error that applies to a specific setting that was requested.</span></span> 
    
<span data-ttu-id="648c9-142">Давайте рассмотрим пример ответа.</span><span class="sxs-lookup"><span data-stu-id="648c9-142">Let's take a look at an example of a response.</span></span> <span data-ttu-id="648c9-143">В этом примере элемент **ErrorCode** в элементе **Response** имеет значение "No Error", которое указывает на общее успешное выполнение.</span><span class="sxs-lookup"><span data-stu-id="648c9-143">In this example, the **ErrorCode** element under the **Response** element has a value of "NoError", which indicates overall success.</span></span> <span data-ttu-id="648c9-144">Однако элемент **ErrorCode** в элементе **усерреспонсе** имеет значение "RedirectAddress", которое указывает на то, что для конкретного пользователя возникла ошибка.</span><span class="sxs-lookup"><span data-stu-id="648c9-144">However, the **ErrorCode** element under the **UserResponse** element has a value of "RedirectAddress", which indicates that an error occurred for that particular user.</span></span> 
  
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

<span data-ttu-id="648c9-145">В статье [ErrorCode (SOAP)](https://msdn.microsoft.com/library/5e5ec861-0191-4ecb-a906-47ce8ed96381%28Office.15%29.aspx) содержится полный список возможных ошибок.</span><span class="sxs-lookup"><span data-stu-id="648c9-145">The [ErrorCode (SOAP)](https://msdn.microsoft.com/library/5e5ec861-0191-4ecb-a906-47ce8ed96381%28Office.15%29.aspx) article contains a full list of possible errors.</span></span> <span data-ttu-id="648c9-146">Большинство из них указывают на неустранимую ошибку, но не требует особой обработки.</span><span class="sxs-lookup"><span data-stu-id="648c9-146">Most of these indicate an unrecoverable error, but a few warrant special handling.</span></span> 
  
<span data-ttu-id="648c9-147">**Таблица 2. Значения ErrorCode обнаружение autodisover SOAP**</span><span class="sxs-lookup"><span data-stu-id="648c9-147">**Table 2. SOAP Autodisover ErrorCode values**</span></span>

|<span data-ttu-id="648c9-148">**Значение ErrorCode**</span><span class="sxs-lookup"><span data-stu-id="648c9-148">**ErrorCode value**</span></span>|<span data-ttu-id="648c9-149">**Обработка...**</span><span class="sxs-lookup"><span data-stu-id="648c9-149">**To handle…**</span></span>|
|:-----|:-----|
|<span data-ttu-id="648c9-150">RedirectAddress</span><span class="sxs-lookup"><span data-stu-id="648c9-150">RedirectAddress</span></span>  <br/> |<span data-ttu-id="648c9-151">[Перезапуск службы автообнаружения с новым адресом электронной почты](#bk_RestartAutodiscover) с адресом электронной почты в элементе [редиректтаржет (SOAP)](https://msdn.microsoft.com/library/f8162724-cf9a-4543-a1ad-5846c8b10bfa%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="648c9-151">[Restarting Autodiscover with a new email address](#bk_RestartAutodiscover) with the email address in the [RedirectTarget (SOAP)](https://msdn.microsoft.com/library/f8162724-cf9a-4543-a1ad-5846c8b10bfa%28Office.15%29.aspx) element.</span></span>  <br/> |
|<span data-ttu-id="648c9-152">RedirectUrl адресом</span><span class="sxs-lookup"><span data-stu-id="648c9-152">RedirectUrl</span></span>  <br/> |<span data-ttu-id="648c9-153">[Повторно отправит запрос на новый URL](#bk_ResendRequest) -адрес в URL-адрес в элементе **редиректтаржет** .</span><span class="sxs-lookup"><span data-stu-id="648c9-153">[Resending your request to a new URL](#bk_ResendRequest) to the URL in the **RedirectTarget** element.</span></span>  <br/> |
|<span data-ttu-id="648c9-154">ServerBusy</span><span class="sxs-lookup"><span data-stu-id="648c9-154">ServerBusy</span></span>  <br/> |<span data-ttu-id="648c9-155">Повторите этот URL-адрес после небольшой задержки.</span><span class="sxs-lookup"><span data-stu-id="648c9-155">Retry this URL after a small delay.</span></span> <span data-ttu-id="648c9-156">Вы можете подождать заданный URL-адрес или просто переместить его в конец списка URL-адресов, чтобы попробовать.</span><span class="sxs-lookup"><span data-stu-id="648c9-156">You might wait a set amount of time or simply move this URL to the end of your list of URLs to try.</span></span> <span data-ttu-id="648c9-157">Если вы получаете эту ошибку несколько раз с URL-адреса, необходимо учитывать, что URL-адрес является недопустимым.</span><span class="sxs-lookup"><span data-stu-id="648c9-157">If you receive this error multiple times from a URL, you should consider the URL to be invalid.</span></span>  <br/> |
   
### <a name="pox-autodiscover-errors"></a><span data-ttu-id="648c9-158">Ошибки автообнаружения POX</span><span class="sxs-lookup"><span data-stu-id="648c9-158">POX Autodiscover errors</span></span>

<span data-ttu-id="648c9-159">Служба автообнаружения POX зачитывает ошибки немного по-другому.</span><span class="sxs-lookup"><span data-stu-id="648c9-159">The POX Autodiscover service reports errors a little differently.</span></span> <span data-ttu-id="648c9-160">Ошибки, которые не могут быть восстановлены, хранятся в элементе [Error (POX)](https://msdn.microsoft.com/library/91c63b62-ab68-4c32-a2f7-5a87c188335b%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="648c9-160">Non-recoverable errors are contained in the [Error (POX)](https://msdn.microsoft.com/library/91c63b62-ab68-4c32-a2f7-5a87c188335b%28Office.15%29.aspx) element.</span></span> <span data-ttu-id="648c9-161">В статье [ErrorCode (POX)](https://msdn.microsoft.com/library/064d73e4-45b7-4797-828e-9df590830db8%28Office.15%29.aspx) содержится полный список возможных кодов ошибок.</span><span class="sxs-lookup"><span data-stu-id="648c9-161">The [ErrorCode (POX)](https://msdn.microsoft.com/library/064d73e4-45b7-4797-828e-9df590830db8%28Office.15%29.aspx) article contains a full list of possible error codes.</span></span> 
  
<span data-ttu-id="648c9-162">Ошибки перенаправления находятся в элементе [Action (POX)](https://msdn.microsoft.com/library/a3462c6b-453c-462a-830d-f29ee4a2babb%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="648c9-162">Redirect errors are contained in the [Action (POX)](https://msdn.microsoft.com/library/a3462c6b-453c-462a-830d-f29ee4a2babb%28Office.15%29.aspx) element.</span></span> <span data-ttu-id="648c9-163">Любое значение элемента **Action** , кроме "Settings", указывает на ошибку перенаправления.</span><span class="sxs-lookup"><span data-stu-id="648c9-163">Any value of the **Action** element other than "settings" indicates a redirect error.</span></span> 
  
<span data-ttu-id="648c9-164">**Таблица 3. POX обнаружение autodisover значения ErrorCode**</span><span class="sxs-lookup"><span data-stu-id="648c9-164">**Table 3. POX Autodisover ErrorCode values**</span></span>

|<span data-ttu-id="648c9-165">**Значение действия**</span><span class="sxs-lookup"><span data-stu-id="648c9-165">**Action value**</span></span>|<span data-ttu-id="648c9-166">**Обработка...**</span><span class="sxs-lookup"><span data-stu-id="648c9-166">**To handle…**</span></span>|
|:-----|:-----|
|<span data-ttu-id="648c9-167">редиректаддр</span><span class="sxs-lookup"><span data-stu-id="648c9-167">redirectAddr</span></span>  <br/> |<span data-ttu-id="648c9-168">[Перезапуск службы автообнаружения с новым адресом электронной почты](#bk_RestartAutodiscover) с адресом электронной почты в элементе [редиректаддр (POX)](https://msdn.microsoft.com/library/0e9fa6b6-7991-4dc1-a59a-48e5f8e041e4%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="648c9-168">[Restarting Autodiscover with a new email address](#bk_RestartAutodiscover) with the email address in the [RedirectAddr (POX)](https://msdn.microsoft.com/library/0e9fa6b6-7991-4dc1-a59a-48e5f8e041e4%28Office.15%29.aspx) element.</span></span>  <br/> |
|<span data-ttu-id="648c9-169">redirectUrl</span><span class="sxs-lookup"><span data-stu-id="648c9-169">redirectUrl</span></span>  <br/> |<span data-ttu-id="648c9-170">[Повторно отправит запрос на новый URL](#bk_ResendRequest) -адрес в URL-адрес в элементе [redirectUrl адресом (POX)](https://msdn.microsoft.com/library/c54f310f-8c99-4c37-8e73-ac87722b6229%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="648c9-170">[Resending your request to a new URL](#bk_ResendRequest) to the URL in the [RedirectUrl (POX)](https://msdn.microsoft.com/library/c54f310f-8c99-4c37-8e73-ac87722b6229%28Office.15%29.aspx) element.</span></span>  <br/> |
   
<span data-ttu-id="648c9-171">В этом примере элемент **Action** имеет значение "редиректаддр", которое указывает, что новый запрос должен отправляться с новым адресом электронной почты, который хранится в элементе **редиректаддр** .</span><span class="sxs-lookup"><span data-stu-id="648c9-171">In this example, the **Action** element has a value of "redirectAddr", which indicates that a new request should be sent with the new email address contained in the **RedirectAddr** element.</span></span> 
  
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

## <a name="handling-redirect-errors"></a><span data-ttu-id="648c9-172">Обработка ошибок перенаправления</span><span class="sxs-lookup"><span data-stu-id="648c9-172">Handling redirect errors</span></span>
<span data-ttu-id="648c9-173"><a name="bk_HandlingRedirects"> </a></span><span class="sxs-lookup"><span data-stu-id="648c9-173"><a name="bk_HandlingRedirects"> </a></span></span>

<span data-ttu-id="648c9-174">Сценарии ошибок перенаправления можно обрабатывать двумя способами:</span><span class="sxs-lookup"><span data-stu-id="648c9-174">You can handle redirect error scenarios in two ways:</span></span>
  
- <span data-ttu-id="648c9-175">Путем перезапуска автообнаружения с новым адресом электронной почты.</span><span class="sxs-lookup"><span data-stu-id="648c9-175">By restarting Autodiscover with a new email address.</span></span>
    
- <span data-ttu-id="648c9-176">Повторно отправляя запрос на новый URL-адрес.</span><span class="sxs-lookup"><span data-stu-id="648c9-176">By resending your request to a new URL.</span></span>
    
<span data-ttu-id="648c9-177">В обоих сценариях требуется проверка перед продолжением.</span><span class="sxs-lookup"><span data-stu-id="648c9-177">Both scenarios require some validation before proceeding.</span></span>
  
### <a name="restarting-autodiscover-with-a-new-email-address"></a><span data-ttu-id="648c9-178">Перезапуск автообнаружения с новым адресом электронной почты</span><span class="sxs-lookup"><span data-stu-id="648c9-178">Restarting Autodiscover with a new email address</span></span>
<span data-ttu-id="648c9-179"><a name="bk_RestartAutodiscover"> </a></span><span class="sxs-lookup"><span data-stu-id="648c9-179"><a name="bk_RestartAutodiscover"> </a></span></span>

<span data-ttu-id="648c9-180">При получении нового адреса электронной почты в ответе на перенаправление автообнаружения сначала убедитесь, что новый адрес электронной почты, указанный в ответе на сообщение об ошибке перенаправления, отличается от адреса, отправленного в запросе, который привел к ошибке.</span><span class="sxs-lookup"><span data-stu-id="648c9-180">When you get a new email address in an Autodiscover redirect response, first verify that the new email address that was provided in the redirect error response is not the same address that you sent in the request that resulted in the error.</span></span> <span data-ttu-id="648c9-181">Если это так, не следует перезапускать службу автообнаружения, а вместо этого считать недопустимым URL-адрес, который выдал ответ.</span><span class="sxs-lookup"><span data-stu-id="648c9-181">If it is, you should not restart Autodiscover and instead consider the URL that generated the response to be invalid.</span></span>
  
<span data-ttu-id="648c9-182">Если новый адрес электронной почты отличается, удалите существующий список возможных URL-адресов конечных точек автообнаружения и создайте новый список на основе нового адреса электронной почты.</span><span class="sxs-lookup"><span data-stu-id="648c9-182">If the new email address is different, discard your existing list of potential Autodiscover endpoint URLs and generate a new list based on the new email address.</span></span>
  
### <a name="resending-your-request-to-a-new-url"></a><span data-ttu-id="648c9-183">Повторная отправка запроса на новый URL-адрес</span><span class="sxs-lookup"><span data-stu-id="648c9-183">Resending your request to a new URL</span></span>
<span data-ttu-id="648c9-184"><a name="bk_ResendRequest"> </a></span><span class="sxs-lookup"><span data-stu-id="648c9-184"><a name="bk_ResendRequest"> </a></span></span>

<span data-ttu-id="648c9-185">При получении нового URL-адреса в ответе на перенаправление автообнаружения сначала необходимо проверить URL-адрес следующим образом:</span><span class="sxs-lookup"><span data-stu-id="648c9-185">When you get a new URL in an Autodiscover redirect response, you should first validate the URL as follows:</span></span>
  
- <span data-ttu-id="648c9-186">Убедитесь, что URL-адрес является URL-адресом HTTPS.</span><span class="sxs-lookup"><span data-stu-id="648c9-186">Verify that the URL is an HTTPS URL.</span></span>
    
- <span data-ttu-id="648c9-187">Убедитесь, что вы не получали ошибку от этого URL-адреса с текущим адресом электронной почты, прежде чем.</span><span class="sxs-lookup"><span data-stu-id="648c9-187">Verify that you have not received an error from this URL with the current email address before.</span></span>
    
- <span data-ttu-id="648c9-188">Если это применимо к приложению, сообщите пользователю о перенаправлении и получите разрешение на отслеживание перенаправления.</span><span class="sxs-lookup"><span data-stu-id="648c9-188">If applicable to your application, inform the user of the redirection and get their permission to follow the redirect.</span></span>
    
- <span data-ttu-id="648c9-189">Отправьте запрос на URL-адрес и [Убедитесь, что сертификат SSL, предоставленный сервером, является допустимым](how-to-validate-a-server-certificate-for-the-ews-managed-api.md).</span><span class="sxs-lookup"><span data-stu-id="648c9-189">Send a request to the URL and [verify that the SSL certificate presented by the server is valid](how-to-validate-a-server-certificate-for-the-ews-managed-api.md).</span></span>
    
<span data-ttu-id="648c9-190">Если URL-адрес проходит проверку, отправьте запрос на этот новый URL-адрес.</span><span class="sxs-lookup"><span data-stu-id="648c9-190">If the URL passes validation, resend the request to this new URL.</span></span>
  
## <a name="see-also"></a><span data-ttu-id="648c9-191">См. также</span><span class="sxs-lookup"><span data-stu-id="648c9-191">See also</span></span>


- [<span data-ttu-id="648c9-192">Автообнаружение в Exchange</span><span class="sxs-lookup"><span data-stu-id="648c9-192">Autodiscover for Exchange</span></span>](autodiscover-for-exchange.md)
    
- [<span data-ttu-id="648c9-193">Обнаружение конечных точек автообнаружения с помощью поиска SCP в Exchange</span><span class="sxs-lookup"><span data-stu-id="648c9-193">Find Autodiscover endpoints by using SCP lookup in Exchange</span></span>](how-to-find-autodiscover-endpoints-by-using-scp-lookup-in-exchange.md)
    
- [<span data-ttu-id="648c9-194">ErrorCode (SOAP)</span><span class="sxs-lookup"><span data-stu-id="648c9-194">ErrorCode (SOAP)</span></span>](https://msdn.microsoft.com/library/5e5ec861-0191-4ecb-a906-47ce8ed96381%28Office.15%29.aspx)
    
- [<span data-ttu-id="648c9-195">ErrorCode (POX)</span><span class="sxs-lookup"><span data-stu-id="648c9-195">ErrorCode (POX)</span></span>](https://msdn.microsoft.com/library/064d73e4-45b7-4797-828e-9df590830db8%28Office.15%29.aspx)
    

