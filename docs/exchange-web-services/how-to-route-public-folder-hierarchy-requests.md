---
title: Иерархия общедоступных папок маршрутизации запросов
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: ec35df8e-4d75-4aa1-8b9c-ae1db7e05772
description: Все запросы для общих папок, которые требуют знания по иерархии общедоступных папок, такие как перемещение, обновление, удаление или поиск общих папок, должны перенаправляться в почтовый ящик иерархии общих папок по умолчанию для определенного пользователя. Чтобы перенаправлять запросы к почтовому ящику, необходимо задать заголовки X AnchorMailbox и X-PublicFolderMailbox для определенного значения, возвращаемые службой автообнаружения.
ms.openlocfilehash: 983431864729edbb040a7206dae416d10bfb2b7a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761116"
---
# <a name="route-public-folder-hierarchy-requests"></a><span data-ttu-id="13bb2-104">Иерархия общедоступных папок маршрутизации запросов</span><span class="sxs-lookup"><span data-stu-id="13bb2-104">Route public folder hierarchy requests</span></span>

<span data-ttu-id="13bb2-105">Все запросы для общих папок, которые требуют знания по иерархии общедоступных папок, такие как перемещение, обновление, удаление или поиск общих папок, должны перенаправляться в почтовый ящик иерархии общих папок по умолчанию для определенного пользователя.</span><span class="sxs-lookup"><span data-stu-id="13bb2-105">All requests for public folder information that require knowledge of the public folder hierarchy, such as moving, updating, deleting, or finding public folders, need to be routed to the default public folder hierarchy mailbox for the given user.</span></span> <span data-ttu-id="13bb2-106">Чтобы перенаправлять запросы к почтовому ящику, необходимо задать заголовки **X AnchorMailbox** и **X-PublicFolderMailbox** для определенного значения, возвращаемые службой автообнаружения.</span><span class="sxs-lookup"><span data-stu-id="13bb2-106">To route the requests to that mailbox, you need to set the **X-AnchorMailbox** and **X-PublicFolderMailbox** headers to specific values returned by the Autodiscover service.</span></span> 
  
<span data-ttu-id="13bb2-107">**Обзор общих папок**</span><span class="sxs-lookup"><span data-stu-id="13bb2-107">**Overview of public folders**</span></span>

|<span data-ttu-id="13bb2-108">Заголовок</span><span class="sxs-lookup"><span data-stu-id="13bb2-108">Header</span></span>|<span data-ttu-id="13bb2-109">Что нужно сделать?</span><span class="sxs-lookup"><span data-stu-id="13bb2-109">What do I need?</span></span>|<span data-ttu-id="13bb2-110">Как его получить?</span><span class="sxs-lookup"><span data-stu-id="13bb2-110">How do I get it?</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="13bb2-111">**X-AnchorMailbox**</span><span class="sxs-lookup"><span data-stu-id="13bb2-111">**X-AnchorMailbox**</span></span> <br/> |<span data-ttu-id="13bb2-112">Значение [PublicFolderInformation](http://msdn.microsoft.com/en-us/library/dn751006%28v=exchg.150%29.aspx) из ответа SOAP автообнаружения [GetUserSettings](http://msdn.microsoft.com/en-us/library/office/dd877096%28v=exchg.150%29.aspx) , которое будет значение заголовка **X-AnchorMailbox** .</span><span class="sxs-lookup"><span data-stu-id="13bb2-112">The [PublicFolderInformation](http://msdn.microsoft.com/en-us/library/dn751006%28v=exchg.150%29.aspx) value from a [GetUserSettings](http://msdn.microsoft.com/en-us/library/office/dd877096%28v=exchg.150%29.aspx) Autodiscover SOAP response, which becomes the value of the **X-AnchorMailbox** header.</span></span><br/><br/> <span data-ttu-id="13bb2-113">![ЗАДАЧ](media/Ex15_PF_PFH_Anchor.png)</span><span class="sxs-lookup"><span data-stu-id="13bb2-113">![TODO](media/Ex15_PF_PFH_Anchor.png)</span></span>| <span data-ttu-id="13bb2-114">1. отправьте запрос **GetUserSetting** с SMTP-адрес почтового ящика пользователя.</span><span class="sxs-lookup"><span data-stu-id="13bb2-114">1. Send a **GetUserSetting** request with the SMTP address for the user's mailbox.</span></span><br/><br/><span data-ttu-id="13bb2-115">2. кэширование значение элемента **PublicFolderInformation** , которое возвращает службы автообнаружения.</span><span class="sxs-lookup"><span data-stu-id="13bb2-115">2. Cache the value of the **PublicFolderInformation** element that the Autodiscover service returns.</span></span> <span data-ttu-id="13bb2-116">Это может быть кэширования данных из существующей вызова службы автообнаружения в коде, или новый [звонок GetUserSettings управляемого API веб-служб Exchange](#bk_getpfinfoewsma) или [запрос GetUserSettings SOAP](#bk_getpfinfoews).</span><span class="sxs-lookup"><span data-stu-id="13bb2-116">This can be a cached from an existing Autodiscover call in your code, or a new [EWS Managed API GetUserSettings call](#bk_getpfinfoewsma) or a [GetUserSettings SOAP request](#bk_getpfinfoews).</span></span>  <br/><br/><span data-ttu-id="13bb2-117">3. Используйте элемент **PublicFolderInformation** для заполнения значение заголовка **X-AnchorMailbox** .</span><span class="sxs-lookup"><span data-stu-id="13bb2-117">3. Use the **PublicFolderInformation** element to populate the value of the **X-AnchorMailbox** header.</span></span> <span data-ttu-id="13bb2-118">Значение элемента **PublicFolderInformation** является адресом SMTP.</span><span class="sxs-lookup"><span data-stu-id="13bb2-118">The value of the **PublicFolderInformation** element is an SMTP address.</span></span>  <br/> |
|<span data-ttu-id="13bb2-119">**X-PublicFolderMailbox**</span><span class="sxs-lookup"><span data-stu-id="13bb2-119">**X-PublicFolderMailbox**</span></span> <br/> |<span data-ttu-id="13bb2-120">Значение [сервера](http://msdn.microsoft.com/en-us/library/bb204084%28v=exchg.150%29.aspx) из [ответа POX автообнаружения](http://msdn.microsoft.com/en-us/library/bb204082%28v=exchg.150%29.aspx), который становится значением заголовка **X-PublicFolderMailbox** .</span><span class="sxs-lookup"><span data-stu-id="13bb2-120">The [Server](http://msdn.microsoft.com/en-us/library/bb204084%28v=exchg.150%29.aspx) value from a [POX Autodiscover response](http://msdn.microsoft.com/en-us/library/bb204082%28v=exchg.150%29.aspx), which becomes the value of the **X-PublicFolderMailbox** header.</span></span><br/><br/> <span data-ttu-id="13bb2-121">![ЗАДАЧ](media/Ex15_PF_PFH_PFMailbox.png)</span><span class="sxs-lookup"><span data-stu-id="13bb2-121">![TODO](media/Ex15_PF_PFH_PFMailbox.png)</span></span>|<span data-ttu-id="13bb2-122">1. службы [вызова автообнаружения POX](#bk_makeautodrequest) , используя адрес электронной почты **X AnchorMailbox** .</span><span class="sxs-lookup"><span data-stu-id="13bb2-122">1. [Call the POX Autodiscover](#bk_makeautodrequest) service using the **X-AnchorMailbox** email address.</span></span>  <br/><br/><span data-ttu-id="13bb2-123">2. Используйте элемент **сервера** , возвращаемые службой автообнаружения для заполнения значение заголовка **X-PublicFolderMailbox** .</span><span class="sxs-lookup"><span data-stu-id="13bb2-123">2. Use the **Server** element returned by the Autodiscover service to populate the value of the **X-PublicFolderMailbox** header.</span></span> <span data-ttu-id="13bb2-124">Значение **X-PublicFolderMailbox** является адресом SMTP, где GUID — это имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="13bb2-124">The value of the **X-PublicFolderMailbox** is an SMTP address where the username is a GUID.</span></span>  <br/> |

<br/>

<span data-ttu-id="13bb2-125">После определения значения заголовка включайте их [во время внесения запросы иерархии общих папок](#bk_setheadervalues).</span><span class="sxs-lookup"><span data-stu-id="13bb2-125">After you have determined the header values, include them [when you make public folder hierarchy requests](#bk_setheadervalues).</span></span>
  
<span data-ttu-id="13bb2-126">Действия, описанные в этой статье относятся только к запросы иерархии общих папок.</span><span class="sxs-lookup"><span data-stu-id="13bb2-126">The steps in this article are specific to public folder hierarchy requests.</span></span> <span data-ttu-id="13bb2-127">Чтобы определить, является ли запрос иерархии общедоступных папок или содержимого запроса, обратитесь к разделу [маршрутизации запросов общих папок](public-folder-access-with-ews-in-exchange.md#bk_routing).</span><span class="sxs-lookup"><span data-stu-id="13bb2-127">To determine whether your request is a public folder hierarchy or content request, see [Routing public folder requests](public-folder-access-with-ews-in-exchange.md#bk_routing).</span></span>
  
## <a name="determine-the-value-of-the-x-anchormailbox-header-by-using-the-ews-managed-api"></a><span data-ttu-id="13bb2-128">Определите значение заголовка X-AnchorMailbox с помощью управляемого интерфейса API веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="13bb2-128">Determine the value of the X-AnchorMailbox header by using the EWS Managed API</span></span>
<span data-ttu-id="13bb2-129"><a name="bk_getpfinfoewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="13bb2-129"></span></span>

<span data-ttu-id="13bb2-130">Для получения значения [PublicFolderInformation (POX)](http://msdn.microsoft.com/library/a221aa9e-b4ac-4ec5-aa42-7e2a69e8eaa6%28Office.15%29.aspx) с помощью управляемого интерфейса API веб-служб Exchange, можно кэшировать значение элемента **PublicFolderInformation** , которое возвращает существующий вызов к службе автообнаружения или Новый звонок.</span><span class="sxs-lookup"><span data-stu-id="13bb2-130">To retrieve the [PublicFolderInformation (POX)](http://msdn.microsoft.com/library/a221aa9e-b4ac-4ec5-aa42-7e2a69e8eaa6%28Office.15%29.aspx) value by using the EWS Managed API, you can either cache the value of the **PublicFolderInformation** element that an existing call to the Autodiscover service returns, or make a new call.</span></span> 
  
<span data-ttu-id="13bb2-131">Если вы выполняете Новый звонок, можно [получить параметры пользователя с помощью управляемого интерфейса API EWS](how-to-get-user-settings-from-exchange-by-using-autodiscover.md#bk_Managed)[получить параметры пользователя с помощью управляемого интерфейса API веб-служб Exchange](how-to-get-user-settings-from-exchange-by-using-autodiscover.md#bk_Managed) для вашего кода, а затем вызвать **GetUserSettings** пример метода, используя следующий код, который извлекает только значение элемента **PublicFolderInformation** .</span><span class="sxs-lookup"><span data-stu-id="13bb2-131">If you're making a new call, you can [Get user settings by using the EWS Managed API](how-to-get-user-settings-from-exchange-by-using-autodiscover.md#bk_Managed)[Get user settings by using the EWS Managed API](how-to-get-user-settings-from-exchange-by-using-autodiscover.md#bk_Managed) to your code, and then call the **GetUserSettings** sample method by using the following code, which retrieves only the value of the **PublicFolderInformation** element.</span></span> <span data-ttu-id="13bb2-132">Включите SMTP-адрес пользователя почтового ящика в качестве входного параметра.</span><span class="sxs-lookup"><span data-stu-id="13bb2-132">Include the SMTP address of the mailbox user as an input parameter.</span></span> 
  
```cs
GetUserSettingsResponse userResponse = GetUserSettings(adservice, "sonyaf@contoso.com", 3, UserSettingName.PublicFolderInformation);
Console.WriteLine("X-AnchorMailbox value for public folder hierarchy requests: {0}", userResponse.Settings[UserSettingName.PublicFolderInformation]);
```

<span data-ttu-id="13bb2-133">После выполнения кода, в консоли отображаются следующие сведения:</span><span class="sxs-lookup"><span data-stu-id="13bb2-133">After running the code, the following information is displayed on the console:</span></span>
  
`X-AnchorMailbox for public folder hierarchy requests: SharedPublicFolder@contoso.com`

<span data-ttu-id="13bb2-134">Теперь, когда значение **PublicFolderInformation** включите его в качестве значения для заголовка X-AnchorMailbox во всех запросах иерархии общих папок.</span><span class="sxs-lookup"><span data-stu-id="13bb2-134">Now that you have the **PublicFolderInformation** value, include it as the value for the X-AnchorMailbox header in all public folder hierarchy requests.</span></span> 
  
`X-AnchorMailbox: SharedPublicFolder@contoso.com`

## <a name="determine-the-value-of-the-x-anchormailbox-header-using-soap"></a><span data-ttu-id="13bb2-135">Определите значение заголовка X-AnchorMailbox, с помощью SOAP</span><span class="sxs-lookup"><span data-stu-id="13bb2-135">Determine the value of the X-AnchorMailbox header using SOAP</span></span>
<span data-ttu-id="13bb2-136"><a name="bk_getpfinfoews"> </a></span><span class="sxs-lookup"><span data-stu-id="13bb2-136"></span></span>

<span data-ttu-id="13bb2-137">В следующем примере кода показано, как получить значение **PublicFolderInformation** с помощью операции [GetUserSettings](http://msdn.microsoft.com/en-us/library/dd877096%28v=exchg.150%29.aspx) SOAP.</span><span class="sxs-lookup"><span data-stu-id="13bb2-137">The following code example shows how to retrieve the **PublicFolderInformation** value by using the [GetUserSettings](http://msdn.microsoft.com/en-us/library/dd877096%28v=exchg.150%29.aspx) SOAP operation.</span></span> <span data-ttu-id="13bb2-138">Почтовый ящик пользователя задан в элементе [почтовых ящиков](http://msdn.microsoft.com/en-us/library/dd877076%28v=exchg.150%29.aspx) , а элемент [RequestedSettings](http://msdn.microsoft.com/en-us/library/office/dd877107%28v=exchg.150%29.aspx) ограничения в ответ на значение [PublicFolderInformation](http://msdn.microsoft.com/en-us/library/dn751006%28v=exchg.150%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="13bb2-138">The mailbox user is specified in the [Mailbox](http://msdn.microsoft.com/en-us/library/dd877076%28v=exchg.150%29.aspx) element, and the [RequestedSettings](http://msdn.microsoft.com/en-us/library/office/dd877107%28v=exchg.150%29.aspx) element limits the response to the [PublicFolderInformation](http://msdn.microsoft.com/en-us/library/dn751006%28v=exchg.150%29.aspx) value.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:a="http://schemas.microsoft.com/exchange/2010/Autodiscover"
               xmlns:wsa="http://www.w3.org/2005/08/addressing"
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <a:RequestedServerVersion>Exchange2007_SP1</a:RequestedServerVersion>
    <wsa:Action>http://schemas.microsoft.com/exchange/2010/Autodiscover/Autodiscover/GetUserSettings</wsa:Action>
    <wsa:To>https://pod51042.outlook.com/autodiscover/autodiscover.svc</wsa:To>
  </soap:Header>
  <soap:Body>
    <a:GetUserSettingsRequestMessage xmlns:a="http://schemas.microsoft.com/exchange/2010/Autodiscover">
      <a:Request>
        <a:Users>
          <a:User>
            <a:Mailbox>sonyaf@contoso.com</a:Mailbox>
          </a:User>
        </a:Users>
        <a:RequestedSettings>
          <a:Setting>PublicFolderInformation</a:Setting>
        </a:RequestedSettings>
      </a:Request>
    </a:GetUserSettingsRequestMessage>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="13bb2-139">Ответ содержит значение **PublicFolderInformation** .</span><span class="sxs-lookup"><span data-stu-id="13bb2-139">The response includes the **PublicFolderInformation** value.</span></span> 
  
```XML
<UserSetting i:type="StringSetting">
    <Name>PublicFolderInformation</Name>
    <Value>SharedPublicFolder@contoso.com</Value>
</UserSetting>
```

<span data-ttu-id="13bb2-140">Теперь, когда значение **PublicFolderInformation** включите его в качестве значения для заголовка X-AnchorMailbox во всех запросах иерархии общих папок.</span><span class="sxs-lookup"><span data-stu-id="13bb2-140">Now that you have the **PublicFolderInformation** value, include it as the value for the X-AnchorMailbox header in all public folder hierarchy requests.</span></span> 
  
`X-AnchorMailbox: SharedPublicFolder@contoso.com`

## <a name="make-an-autodiscover-request-to-determine-the-x-publicfolderinformation-value"></a><span data-ttu-id="13bb2-141">Выполнения запроса службы автообнаружения для определения значения X PublicFolderInformation</span><span class="sxs-lookup"><span data-stu-id="13bb2-141">Make an Autodiscover request to determine the X-PublicFolderInformation value</span></span>
<span data-ttu-id="13bb2-142"><a name="bk_makeautodrequest"> </a></span><span class="sxs-lookup"><span data-stu-id="13bb2-142"></span></span>

<span data-ttu-id="13bb2-143">С помощью **PublicFolderInformation** SMTP-адрес, который теперь используется как значение **X-AnchorMailbox** выполнения запроса службы автообнаружения.</span><span class="sxs-lookup"><span data-stu-id="13bb2-143">Make an Autodiscover request by using the **PublicFolderInformation** SMTP address, which is now being used as the **X-AnchorMailbox** value.</span></span> <span data-ttu-id="13bb2-144">Использование [Exchange 2013: Получение параметров пользователя с помощью службы автообнаружения](http://code.msdn.microsoft.com/exchange/Exchange-2013-Get-user-7e22c86e) пример кода для вызова службы автообнаружения, так как он оптимизирует процесса автообнаружения для вас.</span><span class="sxs-lookup"><span data-stu-id="13bb2-144">Use the [Exchange 2013: Get user settings with Autodiscover](http://code.msdn.microsoft.com/exchange/Exchange-2013-Get-user-7e22c86e) code sample to call the Autodiscover service because it streamlines the Autodiscover process for you.</span></span> <span data-ttu-id="13bb2-145">В этом примере код использует аргументы командной строки, указанные в следующей таблице для вызова службы автообнаружения POX на **PublicFolderInformation** SMTP-адрес.</span><span class="sxs-lookup"><span data-stu-id="13bb2-145">This code sample uses the command line arguments listed in the following table to call the POX Autodiscover service on the **PublicFolderInformation** SMTP address.</span></span> 
  
|<span data-ttu-id="13bb2-146">**Аргумент командной строки**</span><span class="sxs-lookup"><span data-stu-id="13bb2-146">**Command-line argument**</span></span>|<span data-ttu-id="13bb2-147">**Описание**</span><span class="sxs-lookup"><span data-stu-id="13bb2-147">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="13bb2-148">emailAddress</span><span class="sxs-lookup"><span data-stu-id="13bb2-148">emailAddress</span></span>  <br/> |<span data-ttu-id="13bb2-149">Адрес **PublicFolderInformation** SMTP.</span><span class="sxs-lookup"><span data-stu-id="13bb2-149">The **PublicFolderInformation** SMTP address.</span></span>  <br/> |
|<span data-ttu-id="13bb2-150">-skipSOAP</span><span class="sxs-lookup"><span data-stu-id="13bb2-150">-skipSOAP</span></span>  <br/> | <span data-ttu-id="13bb2-151">Использование запросов POX автообнаружения для этого сценария.</span><span class="sxs-lookup"><span data-stu-id="13bb2-151">Use POX Autodiscover requests for this scenario.</span></span>  <br/> |
|<span data-ttu-id="13bb2-152">-проверкой подлинности на основе authEmailAddress</span><span class="sxs-lookup"><span data-stu-id="13bb2-152">-auth authEmailAddress</span></span>  <br/> |<span data-ttu-id="13bb2-153">Адрес электронной почты пользователя почтового ящика, который используется для проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="13bb2-153">The mailbox user's email address, which is used for authentication.</span></span> <span data-ttu-id="13bb2-154">Будет предложено ввести пароль пользователя почтового ящика, при выполнении примера.</span><span class="sxs-lookup"><span data-stu-id="13bb2-154">You will be prompted to enter the mailbox user's password when you run the sample.</span></span>  <br/> |
   
<span data-ttu-id="13bb2-155">Например при SharedPublicFolder@contoso.com SMTP-адрес элемента, **PublicFolderInformation** и sonyaf@contoso.com — пользователь, почтовый ящик, аргументы командной строки должен выглядеть следующим образом.</span><span class="sxs-lookup"><span data-stu-id="13bb2-155">For example, when SharedPublicFolder@contoso.com is the SMTP address of the **PublicFolderInformation** element, and sonyaf@contoso.com is the mailbox user, the command-line arguments should look like this.</span></span> 
  
`SharedPublicFolder@contoso.com -skipSOAP -auth sonyaf@contoso.com`

<span data-ttu-id="13bb2-156">При выполнении **Exchange 2013: Получение параметров пользователя с помощью службы автообнаружения** образец, последний ответ автообнаружения должен быть успешные и включают все пользовательские параметры, связанные с GUID почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="13bb2-156">When you run the **Exchange 2013: Get user settings with Autodiscover** sample, the last Autodiscover response should be successful and include all the user settings associated with the mailbox GUID.</span></span> <span data-ttu-id="13bb2-157">Значение [сервера](http://msdn.microsoft.com/en-us/library/bb204084%28v=exchg.150%29.aspx) , связанные с помощью [протокола](http://msdn.microsoft.com/en-us/library/bb204278%28v=exchg.150%29.aspx)EXCH[Тип](http://msdn.microsoft.com/en-us/library/office/bb204223%28v=exchg.150%29.aspx) элемента — значение заголовка **X-PublicFolderInformation** .</span><span class="sxs-lookup"><span data-stu-id="13bb2-157">The [Server](http://msdn.microsoft.com/en-us/library/bb204084%28v=exchg.150%29.aspx) value associated with the EXCH [Protocol](http://msdn.microsoft.com/en-us/library/bb204278%28v=exchg.150%29.aspx)[Type](http://msdn.microsoft.com/en-us/library/office/bb204223%28v=exchg.150%29.aspx) element is the **X-PublicFolderInformation** header value.</span></span> 
  
```XML
<Autodiscover xmlns="http://schemas.microsoft.com/exchange/autodiscover/responseschema/2006">
  <Response xmlns="http://schemas.microsoft.com/exchange/autodiscover/outlook/responseschema/2006a">
    …
    <Account>
      <AccountType>email</AccountType>
      <Action>settings</Action>
      <Protocol>
        <Type>EXCH</Type>
        <Server>1ec2a236-ed93-4f88-b9c6-33e63fa4aa44@contoso.com</Server>

```

<span data-ttu-id="13bb2-158">Кроме того Если вы не хотите использовать **Exchange 2013: Получение параметров пользователя с помощью службы автообнаружения** образец, можно получить значение **Server** [Создание списка конечных точек службы автообнаружения](how-to-generate-a-list-of-autodiscover-endpoints.md), а затем Отправка следующие POX автообнаружения запрос для каждого URL-адреса до получения успешного ответа.</span><span class="sxs-lookup"><span data-stu-id="13bb2-158">Alternatively, if you do not want to use the **Exchange 2013: Get user settings with Autodiscover** sample, you can get the **Server** value by [generating a list of Autodiscover endpoints](how-to-generate-a-list-of-autodiscover-endpoints.md), and then sending the following POX Autodiscover request to each URL until you receive a successful response.</span></span> <span data-ttu-id="13bb2-159">SharedPublicFolder@contoso.com — это значение заголовка **X-PublicFolderMailbox** .</span><span class="sxs-lookup"><span data-stu-id="13bb2-159">SharedPublicFolder@contoso.com is the value of the **X-PublicFolderMailbox** header.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<Autodiscover xmlns="http://schemas.microsoft.com/exchange/autodiscover/outlook/requestschema/2006">
  <Request>
    <EMailAddress>SharedPublicFolder@contoso.com</EMailAddress>
    <AcceptableResponseSchema>http://schemas.microsoft.com/exchange/autodiscover/outlook/responseschema/2006a</AcceptableResponseSchema>
  </Request>
</Autodiscover>
```

<span data-ttu-id="13bb2-160">Дополнительные сведения о процессе автообнаружения можно [автообнаружения для Exchange](autodiscover-for-exchange.md), [Создать список конечных точек службы автообнаружения](how-to-generate-a-list-of-autodiscover-endpoints.md)и [получить параметры пользователя из Exchange с помощью службы автообнаружения](how-to-get-user-settings-from-exchange-by-using-autodiscover.md).</span><span class="sxs-lookup"><span data-stu-id="13bb2-160">For more information about the Autodiscover process, see [Autodiscover for Exchange](autodiscover-for-exchange.md), [Generate a list of Autodiscover endpoints](how-to-generate-a-list-of-autodiscover-endpoints.md), and [Get user settings from Exchange by using Autodiscover](how-to-get-user-settings-from-exchange-by-using-autodiscover.md).</span></span>
  
## <a name="set-the-values-of-the-x-anchormailbox-and-x-publicfoldermailbox-headers"></a><span data-ttu-id="13bb2-161">Задайте значения заголовков X AnchorMailbox и X-PublicFolderMailbox</span><span class="sxs-lookup"><span data-stu-id="13bb2-161">Set the values of the X-AnchorMailbox and X-PublicFolderMailbox headers</span></span>
<span data-ttu-id="13bb2-162"><a name="bk_setheadervalues"> </a></span><span class="sxs-lookup"><span data-stu-id="13bb2-162"></span></span>

<span data-ttu-id="13bb2-163">С использованием значения адреса **PublicFolderInformation** SMTP, полученные в [Определение значение заголовка X-AnchorMailbox с помощью управляемого интерфейса API веб-служб Exchange](#bk_getpfinfoewsma) или [Определите значение заголовка X-AnchorMailbox, с помощью SOAP](#bk_getpfinfoews) и **сервера **значение приобретенного в [выполнения запроса службы автообнаружения для определения значения X PublicFolderInformation](#bk_makeautodrequest), задайте значения **X AnchorMailbox** и **X-PublicFolderMailbox** заголовков в вашем запросе контента общей папки.</span><span class="sxs-lookup"><span data-stu-id="13bb2-163">Using the value of the **PublicFolderInformation** SMTP address acquired in [Determine the value of the X-AnchorMailbox header by using the EWS Managed API](#bk_getpfinfoewsma) or [Determine the value of the X-AnchorMailbox header using SOAP](#bk_getpfinfoews) and the **Server** value acquired in [Make an Autodiscover request to determine the X-PublicFolderInformation value](#bk_makeautodrequest), set the values of **X-AnchorMailbox** and **X-PublicFolderMailbox** headers in your public folder content request.</span></span> 
  
<span data-ttu-id="13bb2-164">Например учитывая **PublicFolderInformation** SMTP-адрес SharedPublicFolder@contoso.com и **сервера** значение 1ec2a236-ed93-4f88-b9c6-33e63fa4aa44@contoso.com, включены следующие заголовки при выполнении вызовов следующим методы или операции.</span><span class="sxs-lookup"><span data-stu-id="13bb2-164">For example, given a **PublicFolderInformation** SMTP address of SharedPublicFolder@contoso.com and a **Server** value of 1ec2a236-ed93-4f88-b9c6-33e63fa4aa44@contoso.com, include the following headers when making calls to the following methods or operations.</span></span> 
  
`X-AnchorMailbox: SharedPublicFolder@contoso.com` <br/>
`X-PublicFolderMailbox: 1ec2a236-ed93-4f88-b9c6-33e63fa4aa44@contoso.com`

<span data-ttu-id="13bb2-165">**Вызовы общих папок, которые требуют X AnchorMailbox и X-PublicFolder заголовков**</span><span class="sxs-lookup"><span data-stu-id="13bb2-165">**Public folder calls that require the X-AnchorMailbox and X-PublicFolder headers**</span></span>

|<span data-ttu-id="13bb2-166">**Методы управляемого API EWS**</span><span class="sxs-lookup"><span data-stu-id="13bb2-166">**EWS Managed API methods**</span></span>|<span data-ttu-id="13bb2-167">**Операции EWS**</span><span class="sxs-lookup"><span data-stu-id="13bb2-167">**EWS operations**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="13bb2-168">Folder.FindFolders</span><span class="sxs-lookup"><span data-stu-id="13bb2-168">Folder.FindFolders</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.findfolders%28v=exchg.80%29.aspx) <br/> [<span data-ttu-id="13bb2-169">Folder.Delete</span><span class="sxs-lookup"><span data-stu-id="13bb2-169">Folder.Delete</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.delete%28v=exchg.80%29.aspx) <br/> [<span data-ttu-id="13bb2-170">Folder.Update</span><span class="sxs-lookup"><span data-stu-id="13bb2-170">Folder.Update</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.update%28v=exchg.80%29.aspx) <br/> [<span data-ttu-id="13bb2-171">Folder.Move</span><span class="sxs-lookup"><span data-stu-id="13bb2-171">Folder.Move</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.move%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="13bb2-172">CreateFolder</span><span class="sxs-lookup"><span data-stu-id="13bb2-172">CreateFolder</span></span>](http://msdn.microsoft.com/library/6f6c334c-b190-4e55-8f0a-38f2a018d1b3%28Office.15%29.aspx) <br/> [<span data-ttu-id="13bb2-173">FindFolder</span><span class="sxs-lookup"><span data-stu-id="13bb2-173">FindFolder</span></span>](http://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx) <br/> [<span data-ttu-id="13bb2-174">DeleteFolder</span><span class="sxs-lookup"><span data-stu-id="13bb2-174">DeleteFolder</span></span>](http://msdn.microsoft.com/library/b0f92682-4895-4bcf-a4a1-e4c2e8403979%28Office.15%29.aspx) <br/> [<span data-ttu-id="13bb2-175">UpdateFolder</span><span class="sxs-lookup"><span data-stu-id="13bb2-175">UpdateFolder</span></span>](http://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx) <br/> [<span data-ttu-id="13bb2-176">MoveFolder</span><span class="sxs-lookup"><span data-stu-id="13bb2-176">MoveFolder</span></span>](http://msdn.microsoft.com/library/c7233966-6c87-4a14-8156-b1610760176d%28Office.15%29.aspx) <br/> |
   
<span data-ttu-id="13bb2-177">Чтобы добавить эти заголовки с помощью управляемого интерфейса API веб-служб Exchange, используйте метод [HttpHeaders.Add](http://msdn.microsoft.com/en-us/library/system.net.http.headers.httpheaders.add%28v=vs.118%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="13bb2-177">To add these headers by using the EWS Managed API, use the [HttpHeaders.Add](http://msdn.microsoft.com/en-us/library/system.net.http.headers.httpheaders.add%28v=vs.118%29.aspx) method.</span></span> 
  
```cs
service.HttpHeaders.Add("X-AnchorMailbox", "SharedPublicFolder@contoso.com");service.HttpHeaders.Add("X-PublicFolderMailbox", "1ec2a236-ed93-4f88-b9c6-33e63fa4aa44@contoso.com");
```

<span data-ttu-id="13bb2-178">Например в следующем коде показан запрос [FindFolder](http://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx) с заголовка **X-AnchorMailbox** и **X PublicFolderMailbox** , значения, полученные на примерах в этой статье.</span><span class="sxs-lookup"><span data-stu-id="13bb2-178">For example, the following code shows a [FindFolder](http://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx) request with the **X-AnchorMailbox** and **X-PublicFolderMailbox** header set to the values retrieved in the examples in this article.</span></span> 
  
```XML
POST https://outlook.office365.com/EWS/Exchange.asmx HTTP/1.1
Content-Type: text/xml; charset=utf-8
User-Agent: SoapSender1.0
X-AnchorMailbox: SharedPublicFolder@contoso.com
X-PublicFolderMailbox: 1ec2a236-ed93-4f88-b9c6-33e63fa4aa44@contoso.com
Host: outlook.office365.com
Content-Length: 1174
Expect: 100-continue
Connection: Keep-Alive
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2013_SP1" />
  </soap:Header>
  <soap:Body>
    <m:FindFolder Traversal="Shallow">
      <m:FolderShape>
        <t:BaseShape>AllProperties</t:BaseShape>
      </m:FolderShape>
      <m:IndexedPageFolderView MaxEntriesReturned="1" Offset="0" BasePoint="Beginning" />
      <m:Restriction>
        <t:IsEqualTo>
          <t:FieldURI FieldURI="folder:DisplayName" />
          <t:FieldURIOrConstant>
            <t:Constant Value="My Public Contacts" />
          </t:FieldURIOrConstant>
        </t:IsEqualTo>
      </m:Restriction>
      <m:ParentFolderIds>
        <t:FolderId Id="AQEuAAADy/LIWjRCp0GFb0W6aGPbwwEARg5aCLUc8k6wLfl1c0a/2AAAAwIAAAA=" ChangeKey="AQAAABYAAABGDloItRzyTrAt+XVzRr/YAABdo/XB" />
      </m:ParentFolderIds>
    </m:FindFolder>
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a><span data-ttu-id="13bb2-179">См. также</span><span class="sxs-lookup"><span data-stu-id="13bb2-179">See also</span></span>

- [<span data-ttu-id="13bb2-180">Общих папок в Exchange доступ с EWS</span><span class="sxs-lookup"><span data-stu-id="13bb2-180">Public folder access with EWS in Exchange</span></span>](public-folder-access-with-ews-in-exchange.md)    
- [<span data-ttu-id="13bb2-181">Маршрутизация запросов контента общей папки</span><span class="sxs-lookup"><span data-stu-id="13bb2-181">Route public folder content requests</span></span>](how-to-route-public-folder-content-requests.md)    
- [<span data-ttu-id="13bb2-182">Получение параметров пользователя с помощью управляемого интерфейса API веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="13bb2-182">Get user settings by using the EWS Managed API</span></span>](how-to-get-user-settings-from-exchange-by-using-autodiscover.md#bk_Managed)
    

