---
title: Поддержание сходства между группой подписок и сервером почтовых ящиков в Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.assetid: 1bda4094-88c3-4f61-9219-6ee70f6e81cf
description: Сведения о поддержке сходства между группой подписок и сервером почтовых ящиков.
localization_priority: Priority
ms.openlocfilehash: 1618216cf69e08b2ae774264e0910856a59851af
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/02/2020
ms.locfileid: "44455772"
---
# <a name="maintain-affinity-between-a-group-of-subscriptions-and-the-mailbox-server-in-exchange"></a><span data-ttu-id="6cea1-103">Поддержание сходства между группой подписок и сервером почтовых ящиков в Exchange</span><span class="sxs-lookup"><span data-stu-id="6cea1-103">Maintain affinity between a group of subscriptions and the Mailbox server in Exchange</span></span>

<span data-ttu-id="6cea1-104">Сведения о поддержке сходства между группой подписок и сервером почтовых ящиков.</span><span class="sxs-lookup"><span data-stu-id="6cea1-104">Find out about maintaining the affinity between a group of subscriptions and the Mailbox server.</span></span>
  
<span data-ttu-id="6cea1-105">Сходство это ассоциация последовательности запросов и ответных сообщений с определенным сервером почтовых ящиков.</span><span class="sxs-lookup"><span data-stu-id="6cea1-105">Affinity is the association of a sequence of request and response messages with a particular Mailbox server.</span></span> <span data-ttu-id="6cea1-106">Для большинства функциональных возможностей Exchange сервер обрабатывает сходство.</span><span class="sxs-lookup"><span data-stu-id="6cea1-106">For most functionality in Exchange, affinity is handled by the server.</span></span> <span data-ttu-id="6cea1-107">Однако уведомления являются исключением.</span><span class="sxs-lookup"><span data-stu-id="6cea1-107">Notifications, however, are an exception.</span></span> <span data-ttu-id="6cea1-108">Клиент отвечает за поддержание сходства с сервером почтовых ящиков для подписок на уведомления.</span><span class="sxs-lookup"><span data-stu-id="6cea1-108">The client is responsible for maintaining the affinity with the Mailbox server for notification subscriptions.</span></span> <span data-ttu-id="6cea1-109">Это сходство позволяет серверам подсистемы балансировки нагрузки и клиентского доступа между клиентом и сервером маршрутизировать подписки на уведомления и связанные запросы на сервер почтовых ящиков, который обслуживает подписку.</span><span class="sxs-lookup"><span data-stu-id="6cea1-109">This affinity enables the load balancer and Client Access servers between the client and the server to route notification subscriptions and related requests to the Mailbox server that maintains the subscription.</span></span> <span data-ttu-id="6cea1-110">Без сходства запрос может направляться на другой сервер почтовых ящиков, который не включает подписки клиента, что может привести к возвращению ошибки [еррорсубскриптионнотфаунд](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="6cea1-110">Without affinity, the request might get routed to a different Mailbox server that does not include the client's subscriptions, which can cause an [ErrorSubscriptionNotFound](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) error to be returned.</span></span> 
  
## <a name="how-is-affinity-maintained"></a><span data-ttu-id="6cea1-111">Как поддерживается сходство?</span><span class="sxs-lookup"><span data-stu-id="6cea1-111">How is affinity maintained?</span></span>
<span data-ttu-id="6cea1-112"><a name="bk_howmaintained"> </a></span><span class="sxs-lookup"><span data-stu-id="6cea1-112"><a name="bk_howmaintained"> </a></span></span>

<span data-ttu-id="6cea1-113">Сходство в Exchange — на основе файлов cookie.</span><span class="sxs-lookup"><span data-stu-id="6cea1-113">Affinity in Exchange is cookie based.</span></span> <span data-ttu-id="6cea1-114">Клиент запускает создание файла cookie, включая определенные заголовки в запросе на подписку, а затем ответ на подписку содержит файл cookie.</span><span class="sxs-lookup"><span data-stu-id="6cea1-114">The client triggers the creation of the cookie by including specific headers in the subscription request, and then the subscription response contains the cookie.</span></span> <span data-ttu-id="6cea1-115">Затем клиент отправляет этот файл cookie в последующих запросах, чтобы убедиться, что запрос перенаправляется на подходящий сервер почтовых ящиков.</span><span class="sxs-lookup"><span data-stu-id="6cea1-115">The client then sends that cookie in subsequent requests to ensure that the request is routed to the right Mailbox server.</span></span>
  
<span data-ttu-id="6cea1-116">Точнее, сходство в Exchange обрабатывается следующим образом:</span><span class="sxs-lookup"><span data-stu-id="6cea1-116">More specifically, affinity in Exchange is handled by the following:</span></span> 
  
- <span data-ttu-id="6cea1-117">X-AnchorMailbox — HTTP-заголовок, включенный в начальный запрос на подписку.</span><span class="sxs-lookup"><span data-stu-id="6cea1-117">X-AnchorMailbox — An HTTP header that is included in the initial subscription request.</span></span> <span data-ttu-id="6cea1-118">Он определяет первый почтовый ящик в группе почтовых ящиков, которые совместно используют сходство с одним и тем же сервером почтовых ящиков.</span><span class="sxs-lookup"><span data-stu-id="6cea1-118">It identifies the first mailbox in a group of mailboxes that share affinity with the same Mailbox server.</span></span>
    
- <span data-ttu-id="6cea1-119">X-Преферсервераффинити — HTTP-заголовок, который включается в начальный запрос подписки с помощью заголовка X-AnchorMailbox и имеет значение true, чтобы указать, что клиент запрашивает сопоставление соответствия с сервером почтовых ящиков.</span><span class="sxs-lookup"><span data-stu-id="6cea1-119">X-PreferServerAffinity — An HTTP header that is included in the initial subscription request with the X-AnchorMailbox header and is set to true to indicate that the client is requesting that affinity be maintained with the Mailbox server.</span></span>
    
- <span data-ttu-id="6cea1-120">X-Баккендоверридекукие — файл cookie, который включен в первоначальный ответ подписки и содержит файл cookie, используемый сервером балансировки нагрузки и сервером клиентского доступа для маршрутизации последующих запросов на один сервер почтовых ящиков.</span><span class="sxs-lookup"><span data-stu-id="6cea1-120">X-BackEndOverrideCookie — A cookie that is included in the initial subscription response and contains a cookie that the load balancer and Client Access server use to route subsequent requests to the same Mailbox server.</span></span>
    
## <a name="how-do-i-maintain-affinity-by-using-the-ews-managed-api-or-ews"></a><span data-ttu-id="6cea1-121">Как сохранить сходство с помощью управляемого API EWS или EWS?</span><span class="sxs-lookup"><span data-stu-id="6cea1-121">How do I maintain affinity by using the EWS Managed API or EWS?</span></span>
<span data-ttu-id="6cea1-122"><a name="bk_howdoimaintain"> </a></span><span class="sxs-lookup"><span data-stu-id="6cea1-122"><a name="bk_howdoimaintain"> </a></span></span>

<span data-ttu-id="6cea1-123">Вы можете использовать одни и те же действия для сохранения сходства для нескольких подписок почтовых ящиков и их серверов почтовых ящиков независимо от того, используете ли вы уведомления о потоках, опрашивающей или Push-связи, независимо от того, используете ли вы локальный сервер Exchange или Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="6cea1-123">You can use the same steps to maintain affinity for multiple mailbox subscriptions and their Mailbox servers, regardless of whether you are using streaming, pull, or push notifications, and regardless of whether you're targeting an Exchange on-premises server or Exchange Online.</span></span>
  
1. <span data-ttu-id="6cea1-124">Для каждого почтового ящика [вызовите службу автообнаружения](how-to-get-user-settings-from-exchange-by-using-autodiscover.md) и получите параметры Граупингинформатион и екстерналевсурл пользователя.</span><span class="sxs-lookup"><span data-stu-id="6cea1-124">For each mailbox, [call Autodiscover](how-to-get-user-settings-from-exchange-by-using-autodiscover.md) and get the GroupingInformation and ExternalEwsUrl user settings.</span></span> <span data-ttu-id="6cea1-125">Для автообнаружения SOAP вы используете элемент [Setting](https://msdn.microsoft.com/library/43db26e1-f7be-49fd-b26b-fc1b10bd3458%28Office.15%29.aspx) , а для службы автообнаружения POX — элемент [граупингинформатион](https://msdn.microsoft.com/library/2d8a007f-d79c-43c8-90e3-2c6d883f3a7c%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="6cea1-125">For SOAP Autodiscover, you use the [Setting](https://msdn.microsoft.com/library/43db26e1-f7be-49fd-b26b-fc1b10bd3458%28Office.15%29.aspx) element, and for POX Autodiscover, you use the [GroupingInformation](https://msdn.microsoft.com/library/2d8a007f-d79c-43c8-90e3-2c6d883f3a7c%28Office.15%29.aspx) element.</span></span> 
    
2. <span data-ttu-id="6cea1-126">С помощью параметров Граупингинформатион и Екстерналевсурл из откликов автообнаружения помещайте почтовые ящики с одинаковым значением Екстерналевсурл и Граупингинформатион сцепления в одну группу.</span><span class="sxs-lookup"><span data-stu-id="6cea1-126">Using the GroupingInformation and ExternalEwsUrl settings from the Autodiscover responses, place mailboxes with the same ExternalEwsUrl and GroupingInformation concatenated value in the same group.</span></span> <span data-ttu-id="6cea1-127">Если в одной из групп больше 200 почтовых ящиков, разделите их, чтобы в каждой группе было не более 200 почтовых ящиков.</span><span class="sxs-lookup"><span data-stu-id="6cea1-127">If any groups have more than 200 mailboxes, break the groups down further so that each group has no more than 200 mailboxes.</span></span>
    
3. <span data-ttu-id="6cea1-128">Создайте и используйте один объект [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=EXCHG.80%29.aspx) для оставшейся части процедуры.</span><span class="sxs-lookup"><span data-stu-id="6cea1-128">Create and use one [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=EXCHG.80%29.aspx) object for the rest of the procedure.</span></span> <span data-ttu-id="6cea1-129">При использовании одного и того же объекта **ExchangeService** файлы cookie и заголовки (при их задании) автоматически сохраняются.</span><span class="sxs-lookup"><span data-stu-id="6cea1-129">When you use the same **ExchangeService** object, cookies and headers (when they are set) are automatically maintained.</span></span> <span data-ttu-id="6cea1-130">Обратите внимание, что если вы не планируете группировать почтовые подписки в единое подключение, вы можете создать отдельный объект **ExchangeService** для каждого олицетворенного пользователя.</span><span class="sxs-lookup"><span data-stu-id="6cea1-130">Note that if you do not intend to group streaming subscriptions into a single connection, you are free to create a different **ExchangeService** object for each impersonated user.</span></span> 
    
4. <span data-ttu-id="6cea1-131">[Отправьте запрос на подписку](notification-subscriptions-mailbox-events-and-ews-in-exchange.md) для пользователя, имя которого отображается в алфавитном порядке, когда все пользователи в группе сортируются в алфавитном порядке (этот пользователь будет называться пользователь почтовых ящиков привязки).</span><span class="sxs-lookup"><span data-stu-id="6cea1-131">[Send a subscription](notification-subscriptions-mailbox-events-and-ews-in-exchange.md) request for the user whose user name appears first when all users in the group are sorted alphabetically (we'll refer to this user as the anchor mailbox user).</span></span> <span data-ttu-id="6cea1-132">Выполните указанные ниже действия.</span><span class="sxs-lookup"><span data-stu-id="6cea1-132">Do the following:</span></span> 
    
  - <span data-ttu-id="6cea1-133">Включите заголовок X-AnchorMailbox со значением, равным SMTP-адресу пользователя закрепленного почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="6cea1-133">Include the X-AnchorMailbox header with a value set to the SMTP address of the anchor mailbox user.</span></span>
    
  - <span data-ttu-id="6cea1-134">Включите заголовок X – Преферсервераффинити со значением true.</span><span class="sxs-lookup"><span data-stu-id="6cea1-134">Include the X-PreferServerAffinity header with a value set to true.</span></span>
    
  - <span data-ttu-id="6cea1-135">Используйте роль [ApplicationImpersonation](https://technet.microsoft.com/library/dd776119%28v=exchg.150%29.aspx) (тип [ексчанжеимперсонатион](https://msdn.microsoft.com/library/d8cbac49-47d0-4745-a2a7-545d33f8da93%28Office.15%29.aspx) ).</span><span class="sxs-lookup"><span data-stu-id="6cea1-135">Use the [ApplicationImpersonation](https://technet.microsoft.com/library/dd776119%28v=exchg.150%29.aspx) role (the [ExchangeImpersonation](https://msdn.microsoft.com/library/d8cbac49-47d0-4745-a2a7-545d33f8da93%28Office.15%29.aspx) type).</span></span> 
    
5. <span data-ttu-id="6cea1-136">В ответе на подписку получите значение X – Баккендоверридекукие.</span><span class="sxs-lookup"><span data-stu-id="6cea1-136">In the subscription response, get the X-BackEndOverrideCookie value.</span></span> <span data-ttu-id="6cea1-137">Включите это значение в каждую из последующих запросов подписки для пользователей в этой группе.</span><span class="sxs-lookup"><span data-stu-id="6cea1-137">Include this value in each of the subsequent subscription requests for users in this group.</span></span>
    
6. <span data-ttu-id="6cea1-138">Для каждого дополнительного пользователя в группе отправьте запрос на подписку и выполните следующие действия:</span><span class="sxs-lookup"><span data-stu-id="6cea1-138">For each additional user in the group, send a subscription request and do the following:</span></span>
    
  - <span data-ttu-id="6cea1-139">Включите заголовок X-AnchorMailbox со значением, равным SMTP-адресу пользователя закрепленного почтового ящика пользователя для группы.</span><span class="sxs-lookup"><span data-stu-id="6cea1-139">Include the X-AnchorMailbox header with a value set to the SMTP address of the anchor mailbox user for the group.</span></span>
    
  - <span data-ttu-id="6cea1-140">Включите заголовок X – Преферсервераффинити со значением true.</span><span class="sxs-lookup"><span data-stu-id="6cea1-140">Include the X-PreferServerAffinity header with a value set to true.</span></span>
    
  - <span data-ttu-id="6cea1-141">Включите X – Баккендоверридекукие, возвращенный в ответе на подписку пользователя привязанного почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="6cea1-141">Include the X-BackEndOverrideCookie that was returned in the anchor mailbox user's subscription response.</span></span>
    
  - <span data-ttu-id="6cea1-142">Используйте роль [ApplicationImpersonation](https://technet.microsoft.com/library/dd776119%28v=exchg.150%29.aspx) (тип [ексчанжеимперсонатион](https://msdn.microsoft.com/library/d8cbac49-47d0-4745-a2a7-545d33f8da93%28Office.15%29.aspx) ).</span><span class="sxs-lookup"><span data-stu-id="6cea1-142">Use the [ApplicationImpersonation](https://technet.microsoft.com/library/dd776119%28v=exchg.150%29.aspx) role (the [ExchangeImpersonation](https://msdn.microsoft.com/library/d8cbac49-47d0-4745-a2a7-545d33f8da93%28Office.15%29.aspx) type).</span></span> 
    
    <span data-ttu-id="6cea1-143">Обратите внимание, что сервер использует значения X – Преферсервераффинити и X Баккендоверридекукие для выполнения маршрутизации на сервер почтовых ящиков.</span><span class="sxs-lookup"><span data-stu-id="6cea1-143">Note that the server uses the X-PreferServerAffinity and X-BackendOverrideCookie values together to perform the routing to the mailbox server.</span></span> <span data-ttu-id="6cea1-144">Заголовок X-AnchorMailbox также необходим, но он игнорируется сервером, если остальные два значения являются допустимыми.</span><span class="sxs-lookup"><span data-stu-id="6cea1-144">The X-AnchorMailbox header is also required, but is ignored by the server if the other two values are valid.</span></span> <span data-ttu-id="6cea1-145">Если X-AnchorMailbox и X-Преферсервераффинити находятся в запросе, а X-Баккендоверридекукие не включено, то для маршрутизации запросов используется значение X-AnchorMailbox.</span><span class="sxs-lookup"><span data-stu-id="6cea1-145">If X-AnchorMailbox and X-PreferServerAffinity are in a request and X-BackendOverrideCookie is not included, the X-AnchorMailbox value is used to route the requests.</span></span>
    
    <span data-ttu-id="6cea1-146">Так как значения X-Преферсервераффинити и X-Баккендоверридекукие выполняют маршрутизацию, если почтовый ящик привязки когда-либо перемещается в другую группу или на другой сервер, то логика не изменяется, так как X-Баккендоверридекукие направляет запрос на правильный сервер для группы.</span><span class="sxs-lookup"><span data-stu-id="6cea1-146">Because the X-PreferServerAffinity and X-BackendOverrideCookie values perform the routing, if the anchor mailbox ever moves to another group or server, the logic does not change because the X-BackendOverrideCookie will route the request to the correct server for the group.</span></span>
    
7. <span data-ttu-id="6cea1-147">Отправьте отдельные запросы [GetStreamingEvents](https://msdn.microsoft.com/library/dbe83857-c4f8-4d98-813f-e03c289697a1%28Office.15%29.aspx) или [Events](https://msdn.microsoft.com/library/22d4da6b-d8a8-484f-82c4-3e4b8f5431cd%28Office.15%29.aspx) для группы и выполните следующие действия:</span><span class="sxs-lookup"><span data-stu-id="6cea1-147">Send a single [GetStreamingEvents](https://msdn.microsoft.com/library/dbe83857-c4f8-4d98-813f-e03c289697a1%28Office.15%29.aspx) or [GetEvents](https://msdn.microsoft.com/library/22d4da6b-d8a8-484f-82c4-3e4b8f5431cd%28Office.15%29.aspx) requests for the group, and do the following:</span></span> 
    
  - <span data-ttu-id="6cea1-148">Включите значения [SubscriptionId](https://msdn.microsoft.com/library/3f86c178-2311-4844-82db-c2a0e469d116%28Office.15%29.aspx) , возвращенные в каждом из ответов на отдельные подписки для почтовых ящиков в группе.</span><span class="sxs-lookup"><span data-stu-id="6cea1-148">Include the [SubscriptionId](https://msdn.microsoft.com/library/3f86c178-2311-4844-82db-c2a0e469d116%28Office.15%29.aspx) values returned in each of the individual subscription responses for mailboxes in the group.</span></span> 
    
  - <span data-ttu-id="6cea1-149">Если для группы существует более 200 подписок, создайте несколько запросов.</span><span class="sxs-lookup"><span data-stu-id="6cea1-149">If more than 200 subscriptions exist for the group, create multiple requests.</span></span> <span data-ttu-id="6cea1-150">Максимальное число значений [SubscriptionId](https://msdn.microsoft.com/library/3f86c178-2311-4844-82db-c2a0e469d116%28Office.15%29.aspx) , включаемых в запрос: 200.</span><span class="sxs-lookup"><span data-stu-id="6cea1-150">The maximum number of [SubscriptionId](https://msdn.microsoft.com/library/3f86c178-2311-4844-82db-c2a0e469d116%28Office.15%29.aspx) values to include in a request is 200.</span></span> 
    
  - <span data-ttu-id="6cea1-151">Если требуется больше подключений, чем доступно для целевого почтового ящика, используйте учетную запись службы для олицетворения почтового ящика привязки для группы; в противном случае не используйте олицетворение.</span><span class="sxs-lookup"><span data-stu-id="6cea1-151">If you need more connections than are available to the target mailbox, use the service account to impersonate the anchor mailbox for the group; otherwise, do not use impersonation.</span></span> <span data-ttu-id="6cea1-152">В идеале необходимо олицетворять уникальный почтовый ящик на запрос [GetStreamingEvents](https://msdn.microsoft.com/library/dbe83857-c4f8-4d98-813f-e03c289697a1%28Office.15%29.aspx) или [Events](https://msdn.microsoft.com/library/22d4da6b-d8a8-484f-82c4-3e4b8f5431cd%28Office.15%29.aspx) , чтобы никогда не применялись ограничения на регулирование.</span><span class="sxs-lookup"><span data-stu-id="6cea1-152">Ideally, you want to impersonate a unique mailbox per [GetStreamingEvents](https://msdn.microsoft.com/library/dbe83857-c4f8-4d98-813f-e03c289697a1%28Office.15%29.aspx) or [GetEvents](https://msdn.microsoft.com/library/22d4da6b-d8a8-484f-82c4-3e4b8f5431cd%28Office.15%29.aspx) request so that you never encounter throttling limits.</span></span> 
    
  - <span data-ttu-id="6cea1-153">Используйте ApplicationImpersonation, если вам требуется [больше подключений, чем доступно для целевого почтового ящика](how-to-maintain-affinity-between-group-of-subscriptions-and-mailbox-server.md#bk_throttling); в противном случае не используйте ApplicationImpersonation.</span><span class="sxs-lookup"><span data-stu-id="6cea1-153">Use ApplicationImpersonation if you need [more connections than are available to the target mailbox](how-to-maintain-affinity-between-group-of-subscriptions-and-mailbox-server.md#bk_throttling); otherwise, do not use ApplicationImpersonation.</span></span>
    
  - <span data-ttu-id="6cea1-154">Включите заголовок X – Преферсервераффинити и задайте для него значение true.</span><span class="sxs-lookup"><span data-stu-id="6cea1-154">Include the X-PreferServerAffinity header and set it to true.</span></span> <span data-ttu-id="6cea1-155">Это значение автоматически включается при использовании объекта **ExchangeService** , созданного на шаге 2.</span><span class="sxs-lookup"><span data-stu-id="6cea1-155">This value is automatically included if you are using the **ExchangeService** object that you created in step 2.</span></span> 
    
  - <span data-ttu-id="6cea1-156">Включите X-Баккендоверридекукие для группы (X-Баккендоверридекукие, которая была возвращена в ответе на подписку пользователя привязанного почтового ящика).</span><span class="sxs-lookup"><span data-stu-id="6cea1-156">Include the X-BackEndOverrideCookie for the group (the X-BackEndOverrideCookie that was returned in the anchor mailbox user's subscription response).</span></span> <span data-ttu-id="6cea1-157">Это значение автоматически включается при использовании объекта **ExchangeService** , созданного на шаге 2.</span><span class="sxs-lookup"><span data-stu-id="6cea1-157">This value is automatically included if you are using the **ExchangeService** object that you created in step 2.</span></span> 
    
8. <span data-ttu-id="6cea1-158">Передайте возвращенные события в отдельный поток для обработки.</span><span class="sxs-lookup"><span data-stu-id="6cea1-158">Pass the returned events to a separate thread for processing.</span></span>
    
## <a name="what-throttling-values-do-i-need-to-take-into-consideration"></a><span data-ttu-id="6cea1-159">Какие значения регулирования необходимо учитывать?</span><span class="sxs-lookup"><span data-stu-id="6cea1-159">What throttling values do I need to take into consideration?</span></span>
<span data-ttu-id="6cea1-160"><a name="bk_throttling"> </a></span><span class="sxs-lookup"><span data-stu-id="6cea1-160"><a name="bk_throttling"> </a></span></span>

<span data-ttu-id="6cea1-161">При планировании реализации уведомлений необходимо учитывать два значения: количество подключений и число подписок.</span><span class="sxs-lookup"><span data-stu-id="6cea1-161">As you plan your notification implementation, you'll want to take two values into consideration: the number of connections, and the number of subscriptions.</span></span> <span data-ttu-id="6cea1-162">В следующей таблице приведены значения по умолчанию для каждого параметра [регулирования](ews-throttling-in-exchange.md) и способов использования этих параметров.</span><span class="sxs-lookup"><span data-stu-id="6cea1-162">The following table lists the default values for each [throttling](ews-throttling-in-exchange.md) setting and how the settings are used.</span></span> <span data-ttu-id="6cea1-163">Для каждого значения бюджет размещается в целевом почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="6cea1-163">For each value, the budget is allocated to the target mailbox.</span></span> <span data-ttu-id="6cea1-164">По этой причине использование олицетворения для получения дополнительных подключений является обязательным шагом во многих сценариях.</span><span class="sxs-lookup"><span data-stu-id="6cea1-164">For this reason, using impersonation to gain additional connections is a required step in many scenarios.</span></span> 
  
<span data-ttu-id="6cea1-165">**Таблица 1. Значения регулирования по умолчанию**</span><span class="sxs-lookup"><span data-stu-id="6cea1-165">**Table 1. Default throttling values**</span></span>

|<span data-ttu-id="6cea1-166">**Область рассмотрения**</span><span class="sxs-lookup"><span data-stu-id="6cea1-166">**Area of consideration**</span></span>|<span data-ttu-id="6cea1-167">**Параметр регулирования**</span><span class="sxs-lookup"><span data-stu-id="6cea1-167">**Throttling setting**</span></span>|<span data-ttu-id="6cea1-168">**Значение по умолчанию**</span><span class="sxs-lookup"><span data-stu-id="6cea1-168">**Default value**</span></span>|<span data-ttu-id="6cea1-169">**Описание**</span><span class="sxs-lookup"><span data-stu-id="6cea1-169">**Description**</span></span>|
|:-----|:-----|:-----|:-----|
|<span data-ttu-id="6cea1-170">Потоковое подключение</span><span class="sxs-lookup"><span data-stu-id="6cea1-170">Streaming connections</span></span>  <br/> |<span data-ttu-id="6cea1-171">Предельное число подключений по умолчанию</span><span class="sxs-lookup"><span data-stu-id="6cea1-171">Default hanging connection limit</span></span>  <br/> |<span data-ttu-id="6cea1-172">10 для Exchange Online</span><span class="sxs-lookup"><span data-stu-id="6cea1-172">10 for Exchange Online</span></span>  <br/> <span data-ttu-id="6cea1-173">3 для Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="6cea1-173">3 for Exchange 2013</span></span>  <br/> |<span data-ttu-id="6cea1-174">Максимальное число одновременных потоков подключений, которые могут быть открыты учетной записью на сервере в один момент времени.</span><span class="sxs-lookup"><span data-stu-id="6cea1-174">The maximum number of concurrent streaming connections that an account can have open on the server at one time.</span></span> <span data-ttu-id="6cea1-175">Для работы с этим пределом используйте учетную запись службы с ролью ApplicationImpersonation, назначенной для целевых почтовых ящиков, и олицетворяет первого пользователя в каждой группе ИДЕНТИФИКАТОРов подписки, когда вы получаете потоковые события.</span><span class="sxs-lookup"><span data-stu-id="6cea1-175">To work within this limit, use a service account with the ApplicationImpersonation role assigned for the target mailboxes, and impersonate the first user in each subscription ID group when getting streamed events.</span></span>  <br/> |
|<span data-ttu-id="6cea1-176">Опрашивающие или Push-подключения</span><span class="sxs-lookup"><span data-stu-id="6cea1-176">Pull or push connections</span></span>  <br/> |<span data-ttu-id="6cea1-177">евсмаксконкурренци</span><span class="sxs-lookup"><span data-stu-id="6cea1-177">EWSMaxConcurrency</span></span>  <br/> |<span data-ttu-id="6cea1-178">27</span><span class="sxs-lookup"><span data-stu-id="6cea1-178">27</span></span>  <br/> |<span data-ttu-id="6cea1-179">Максимальное количество одновременных запросов на получение или принудительной передачи (запросов, которые еще не ответили), которые учетная запись может открыть на сервере в один момент времени.</span><span class="sxs-lookup"><span data-stu-id="6cea1-179">The maximum number of concurrent pull or push connections (requests that have been received but not yet responded to) that an account can have open on the server at one time.</span></span>  <br/> |
|<span data-ttu-id="6cea1-180">Подписки</span><span class="sxs-lookup"><span data-stu-id="6cea1-180">Subscriptions</span></span>  <br/> |<span data-ttu-id="6cea1-181">евсмакссубскриптионс</span><span class="sxs-lookup"><span data-stu-id="6cea1-181">EWSMaxSubscriptions</span></span>  <br/> |<span data-ttu-id="6cea1-182">20 для Exchange Online</span><span class="sxs-lookup"><span data-stu-id="6cea1-182">20 for Exchange Online</span></span>  <br/> <span data-ttu-id="6cea1-183">5000 для Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="6cea1-183">5000 for Exchange 2013</span></span>  <br/> |<span data-ttu-id="6cea1-184">Максимальное число подписок с неистекшим сроком действия, которые могут одновременно находиться в учетной записи.</span><span class="sxs-lookup"><span data-stu-id="6cea1-184">The maximum number of nonexpired subscriptions that an account can have at one time.</span></span> <span data-ttu-id="6cea1-185">Это значение уменьшается при создании подписки на сервере.</span><span class="sxs-lookup"><span data-stu-id="6cea1-185">This value is decremented when the subscription is created on the server.</span></span>  <br/> |
   
<span data-ttu-id="6cea1-186">В приведенном ниже примере показано, как будут обрабатываться бюджеты между любым целевым почтовым ящиком и учетной записью службы, которой назначена роль [ApplicationImpersonation](https://technet.microsoft.com/library/dd776119%28v=exchg.150%29.aspx) для целевых почтовых ящиков.</span><span class="sxs-lookup"><span data-stu-id="6cea1-186">The following example shows how budgets are handled between any target mailbox and the service account that has the [ApplicationImpersonation](https://technet.microsoft.com/library/dd776119%28v=exchg.150%29.aspx) role assigned for the target mailboxes.</span></span> 
  
- <span data-ttu-id="6cea1-187">ServiceAccount1 (SA1) олицетворяет многих пользователей (M1, m2, M3 и т. д.) и создает подписки для каждого почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="6cea1-187">ServiceAccount1 (sa1) impersonates many users (m1, m2, m3, and so on) and creates subscriptions for each mailbox.</span></span> <span data-ttu-id="6cea1-188">Обратите внимание на то, что при создании подписок владелец подписки — SA1, поэтому когда SA1 открывает подключение с подписками, EWS применяет к ним владельца SA1.</span><span class="sxs-lookup"><span data-stu-id="6cea1-188">Note that when the subscriptions are created, the subscription owner is sa1, so when sa1 opens a connection with the subscriptions, EWS enforces that the subscriptions are owned by sa1.</span></span>
    
- <span data-ttu-id="6cea1-189">SA1 может открыть подключение следующими способами:</span><span class="sxs-lookup"><span data-stu-id="6cea1-189">Sa1 can open the connection in the following ways:</span></span>
    
1. <span data-ttu-id="6cea1-190">Без олицетворения, поэтому соединение будет взиматься с SA1.</span><span class="sxs-lookup"><span data-stu-id="6cea1-190">Without impersonation, so the connection is charged against sa1.</span></span>
    
2. <span data-ttu-id="6cea1-191">Выполнив олицетворение любого пользователя (например, M1), чтобы подключение было взимать копию бюджета m1's.</span><span class="sxs-lookup"><span data-stu-id="6cea1-191">By impersonating any of the users — m1 for example — so that the connection is charged against a copy of m1's budget.</span></span> <span data-ttu-id="6cea1-192">(M1 может открыть десять подключений с помощью Exchange Online, а все учетные записи служб, вызывающие M1, могут открыть десять подключений с помощью скопированного бюджета.)</span><span class="sxs-lookup"><span data-stu-id="6cea1-192">(M1 itself can open ten connections by using Exchange Online, and all service accounts impersonating m1 can open ten connections by using the copied budget.)</span></span>
    
- <span data-ttu-id="6cea1-193">Если достигнуто максимальное число подключений, доступны следующие обходные пути:</span><span class="sxs-lookup"><span data-stu-id="6cea1-193">If the connection limit is hit, the following workarounds are available:</span></span>
    
  - <span data-ttu-id="6cea1-194">Если используется вариант 1, администратор может создать несколько учетных записей служб для олицетворения дополнительных пользователей.</span><span class="sxs-lookup"><span data-stu-id="6cea1-194">If option 1 is used, the administrator can create multiple service accounts to impersonate additional users.</span></span>
    
  - <span data-ttu-id="6cea1-195">Если используется вариант 2, код может олицетворять другого пользователя — m2 для примера.</span><span class="sxs-lookup"><span data-stu-id="6cea1-195">If option 2 is used, the code can impersonate another user — m2 for example.</span></span>
    
## <a name="example-maintaining-affinity-between-a-group-of-subscriptions-and-the-mailbox-server"></a><span data-ttu-id="6cea1-196">Пример: поддержание сходства между группой подписок и сервером почтовых ящиков</span><span class="sxs-lookup"><span data-stu-id="6cea1-196">Example: Maintaining affinity between a group of subscriptions and the Mailbox server</span></span>
<span data-ttu-id="6cea1-197"><a name="bk_ce"> </a></span><span class="sxs-lookup"><span data-stu-id="6cea1-197"><a name="bk_ce"> </a></span></span>

<span data-ttu-id="6cea1-198">Итак, давайте посмотрим, как это выполняется в действии.</span><span class="sxs-lookup"><span data-stu-id="6cea1-198">Okay, let's see it in action.</span></span> <span data-ttu-id="6cea1-199">В приведенном ниже примере кода показано, как группировать пользователей и использовать заголовки X AnchorMailbox и X Преферсервераффинити, а также файл cookie X – Баккендоверридекукие для поддержки сходства с сервером почтовых ящиков.</span><span class="sxs-lookup"><span data-stu-id="6cea1-199">The following code example shows you how to group users and use the X-AnchorMailbox and X-PreferServerAffinity headers and the X-BackendOverrideCookie cookie to maintain affinity with the Mailbox server.</span></span> <span data-ttu-id="6cea1-200">Так как заголовки и файлы cookie являются основным уровнем важности в цепочке сходства, в этом примере основное внимание уделяется запросам и ответам XML EWS.</span><span class="sxs-lookup"><span data-stu-id="6cea1-200">Because the headers and the cookie are of primary importance in the affinity story, this example focuses on the EWS XML requests and responses.</span></span> <span data-ttu-id="6cea1-201">Чтобы использовать управляемый API EWS для создания основного текста запросов и ответов на подписку, обратитесь к разделу [Отправка уведомлений о событиях почтовых ящиков с помощью EWS в Exchange](how-to-stream-notifications-about-mailbox-events-by-using-ews-in-exchange.md) и [уведомления о событиях почтовых ящиков с помощью EWS в Exchange](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="6cea1-201">To use the EWS Managed API to create the body of the subscription requests and responses, see [Stream notifications about mailbox events by using EWS in Exchange](how-to-stream-notifications-about-mailbox-events-by-using-ews-in-exchange.md) and [Pull notifications about mailbox events by using EWS in Exchange](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md).</span></span> <span data-ttu-id="6cea1-202">В этом разделе приводятся дополнительные действия для поддержки сходства и добавления заголовков в запросы.</span><span class="sxs-lookup"><span data-stu-id="6cea1-202">This section includes additional steps particular to maintaining affinity and adding the headers to your requests.</span></span>
  
<span data-ttu-id="6cea1-203">В этом примере имеются четыре пользователя: alfred@contoso.com, alisa@contoso.com, ronnie@contoso.com и sadie@contoso.com.</span><span class="sxs-lookup"><span data-stu-id="6cea1-203">This example has four users: alfred@contoso.com, alisa@contoso.com, ronnie@contoso.com, and sadie@contoso.com.</span></span> <span data-ttu-id="6cea1-204">На следующем рисунке показаны [Параметры автообнаружения](how-to-get-user-settings-from-exchange-by-using-autodiscover.md) Граупингинформатион и екстерналевсурл для пользователей.</span><span class="sxs-lookup"><span data-stu-id="6cea1-204">The following figure shows the GroupingInformation and ExternalEwsUrl [Autodiscover settings](how-to-get-user-settings-from-exchange-by-using-autodiscover.md) for the users.</span></span> 
  
<span data-ttu-id="6cea1-205">**Рис. 1. Параметры автообнаружения, используемые для групповых почтовых ящиков**</span><span class="sxs-lookup"><span data-stu-id="6cea1-205">**Figure 1. Autodiscover settings used to group mailboxes**</span></span>

![Таблица, в которой показаны значения параметров GroupingInformation и ExternalEwsUrl для каждого из пользователей.](media/Exchange2013_NotificationAffinityAutoDResults.png)
  
<span data-ttu-id="6cea1-207">При использовании параметров из ответов автообнаружения почтовые ящики группируются по Объединенному значению параметров Граупингинформатион и Екстерналевсурл.</span><span class="sxs-lookup"><span data-stu-id="6cea1-207">Using the settings from the Autodiscover responses, the mailboxes are grouped by the concatenated value of the GroupingInformation and ExternalEwsUrl settings.</span></span> <span data-ttu-id="6cea1-208">В этом примере Алфред и Ольга имеют одинаковые значения, поэтому они находятся в одной группе, а Алиса и ронние имеют одни и те же значения, поэтому они находятся в другой группе.</span><span class="sxs-lookup"><span data-stu-id="6cea1-208">In this example, Alfred and Sadie have the same values, so they are in one group, and Alisa and Ronnie share the same values, so they are in another group.</span></span>
  
<span data-ttu-id="6cea1-209">**Рис. 2. Создание групп почтовых ящиков**</span><span class="sxs-lookup"><span data-stu-id="6cea1-209">**Figure 2. Creating mailbox groups**</span></span>

![Таблица, в которой показано, как группы почтовых ящиков создаются с помощью параметров автообнаружения.](media/Exchange2013_NotificationAffinityGrouping.png)
  
<span data-ttu-id="6cea1-211">В этом примере основное внимание уделяется группе A. Мы будем использовать одни и те же действия для группы B, но использовать другое значение X-AnchorMailbox для этой группы.</span><span class="sxs-lookup"><span data-stu-id="6cea1-211">For the purpose of this example, we'll focus on Group A. We would use the same steps for group B, but use a different X-AnchorMailbox value for that group.</span></span>
  
<span data-ttu-id="6cea1-212">С помощью [ApplicationImpersonation](https://technet.microsoft.com/library/dd776119%28v=exchg.150%29.aspx)создайте запрос на подписку для почтового ящика привязки (Alfred@contoso.com), для которого в заголовке x-AnchorMailbox задан адрес электронной почты, а для заголовка x-преферсервераффинити — значение true.</span><span class="sxs-lookup"><span data-stu-id="6cea1-212">Using [ApplicationImpersonation](https://technet.microsoft.com/library/dd776119%28v=exchg.150%29.aspx), create the subscription request for the anchor mailbox (alfred@contoso.com), with the X-AnchorMailbox header set to the their email address and an X-PreferServerAffinity header value of true.</span></span> <span data-ttu-id="6cea1-213">Установка этих двух значений заголовков приведет к запуску сервера для создания Баккендоверридекукие X для ответа.</span><span class="sxs-lookup"><span data-stu-id="6cea1-213">Setting these two header values will trigger the server to create an X-BackEndOverrideCookie for the response.</span></span>
  
<span data-ttu-id="6cea1-214">Если вы используете управляемый API EWS, используйте метод [хттфеадерс](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice_members%28v=exchg.80%29.aspx)[Add](https://msdn.microsoft.com/library/cy7xta5e) , чтобы добавить два заголовка в запрос на подписку, как показано ниже.</span><span class="sxs-lookup"><span data-stu-id="6cea1-214">If you're using the EWS Managed API, use the [HttpHeaders](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice_members%28v=exchg.80%29.aspx)[Add](https://msdn.microsoft.com/library/cy7xta5e) method to add the two headers to your subscription request, as shown.</span></span> 
  
```cs
service.HttpHeaders.Add("X-AnchorMailbox", Mailbox.SMTPAddress);
service.HttpHeaders.Add("X-PreferServerAffinity", "true");
```

<span data-ttu-id="6cea1-215">Поэтому запрос на подписку Алфред выглядит следующим образом.</span><span class="sxs-lookup"><span data-stu-id="6cea1-215">So Alfred's subscription request looks like this.</span></span>
  
```XML
POST https://outlook.office365.com/EWS/Exchange.asmx HTTP/1.1
Content-Type: text/xml; charset=utf-8
Accept: text/xml
User-Agent: ExchangeServicesClient/15.00.0516.014
X-AnchorMailbox: alfred@contoso.com
X-PreferServerAffinity: true
Host: outlook.office365.com
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2013" />
    <t:ExchangeImpersonation>
      <t:ConnectingSID>
        <t:SmtpAddress>alfred@contoso.com</t:SmtpAddress>
      </t:ConnectingSID>
    </t:ExchangeImpersonation>
  </soap:Header>
  <soap:Body>
    <m:Subscribe>
      <m:StreamingSubscriptionRequest>
        <t:FolderIds>
          <t:DistinguishedFolderId Id="inbox" />
        </t:FolderIds>
        <t:EventTypes>
          <t:EventType>NewMailEvent</t:EventType>
        </t:EventTypes>
      </m:StreamingSubscriptionRequest>
    </m:Subscribe>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="6cea1-216">Следующее XML-сообщение является ответом на запрос подписки Алфред и включает X-Баккендоверридекукие.</span><span class="sxs-lookup"><span data-stu-id="6cea1-216">The following XML message is the response to Alfred's subscription request, and it includes the X-BackEndOverrideCookie.</span></span> <span data-ttu-id="6cea1-217">Повторно отправить этот файл cookie для всех последующих запросов пользователей в этой группе.</span><span class="sxs-lookup"><span data-stu-id="6cea1-217">Resend this cookie for all subsequent requests for users in this group.</span></span> <span data-ttu-id="6cea1-218">Обратите внимание, что в ответе также содержатся дополнительные файлы cookie, например файл cookie ексчанжекукие, используемый Exchange 2010.</span><span class="sxs-lookup"><span data-stu-id="6cea1-218">Notice that the response also contains additional cookies, such as the exchangecookie cookie used by Exchange 2010.</span></span> <span data-ttu-id="6cea1-219">Exchange Online, Exchange Online в составе Office 365 и версии Exchange, начиная с Exchange 2013, игнорируйте ексчанжекукие, если он включен в последующие запросы подписки.</span><span class="sxs-lookup"><span data-stu-id="6cea1-219">Exchange Online, Exchange Online as part of Office 365, and versions of Exchange starting with Exchange 2013, ignore exchangecookie if it is included in subsequent subscription requests.</span></span>
  
```XML
HTTP/1.1 200 OK
Content-Type: text/xml; charset=utf-8
Set-Cookie: exchangecookie=ddb8c383aef34c7694132aa679744feb; expires=Thu, 25-Sep-2014 18:42:45 GMT; path=/;
    HttpOnly
Set-Cookie: X-BackEndOverrideCookie=CO1PR06MB222.namprd06.prod.outlook.com~1941996295; path=/; secure; HttpOnly
Set-Cookie: X-BackEndCookie=alfred@contoso.com=Ox8XKzcXLxg==; 
    expires=Wed, 25-Sep-2013 18:52:49 GMT; path=/EWS; secure; HttpOnly
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="775"
                         MinorBuildNumber="7"
                         Version="V2_4"
                         xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:SubscribeResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:SubscribeResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:SubscriptionId>JgBjbzFwcjA2bWIyMjIubmFtcHJkMDYucHJvZC5vdXRsb29rLmNvbRAAAAAUeGk+7JFdSaFM8/NI/gQQpVdgZX6H0Ag=</m:SubscriptionId>
        </m:SubscribeResponseMessage>
      </m:ResponseMessages>
    </m:SubscribeResponse>
  </s:Body>
</s:Envelope>
```

<span data-ttu-id="6cea1-220">При использовании ответа X-Баккендоверридекукие из отклика Алфред и заголовка X-AnchorMailbox запрос на подписку создается для Ольга, а другой участник группы A. Ольга-запроса на подписку выглядит следующим образом.</span><span class="sxs-lookup"><span data-stu-id="6cea1-220">Using the X-BackEndOverrideCookie from Alfred's response and the X-AnchorMailbox header, the subscription request is created for Sadie, the other member of Group A. Sadie's subscription request looks like this.</span></span>
  
```XML
POST https://outlook.office365.com/EWS/Exchange.asmx HTTP/1.1
Content-Type: text/xml; charset=utf-8
Accept: text/xml
User-Agent: ExchangeServicesClient/15.00.0516.014
X-AnchorMailbox: alfred@contoso.com
X-PreferServerAffinity: true
Host: outlook.office365.com
Cookie: X-BackEndOverrideCookie=CO1PR06MB222.namprd06.prod.outlook.com~1941996295
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2013" />
    <t:ExchangeImpersonation>
      <t:ConnectingSID>
        <t:SmtpAddress>sadie@contoso.com </t:SmtpAddress>
      </t:ConnectingSID>
    </t:ExchangeImpersonation>
  </soap:Header>
  <soap:Body>
    <m:Subscribe>
      <m:StreamingSubscriptionRequest>
        <t:FolderIds>
          <t:DistinguishedFolderId Id="inbox" />
        </t:FolderIds>
        <t:EventTypes>
          <t:EventType>NewMailEvent</t:EventType>
        </t:EventTypes>
      </m:StreamingSubscriptionRequest>
    </m:Subscribe>
  </soap:Body>
</soap:Envelope>

```

<span data-ttu-id="6cea1-221">Ответ на подписку Ольга выглядит следующим образом.</span><span class="sxs-lookup"><span data-stu-id="6cea1-221">Sadie's subscription response looks like this.</span></span> <span data-ttu-id="6cea1-222">Обратите внимание, что он не включает X – Баккендоверридекукие.</span><span class="sxs-lookup"><span data-stu-id="6cea1-222">Note that it does not include the X-BackEndOverrideCookie.</span></span> <span data-ttu-id="6cea1-223">Клиент отвечает за кэширование этого значения для будущих запросов.</span><span class="sxs-lookup"><span data-stu-id="6cea1-223">The client is responsible for caching that value for future requests.</span></span>
  
```XML
HTTP/1.1 200 OK
Content-Type: text/xml; charset=utf-8
Set-Cookie: exchangecookie=640ea858f69d47ff8cce8b44c337f6d9; path=/
Set-Cookie: X-BackEndCookie=alfred@contoso.com=Ox8XKzcXLxg==; 
   expires= Wed, 25-Sep-2013 18:53:06 GMT; path=/EWS; secure; HttpOnly
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="775"
                         MinorBuildNumber="7"
                         Version="V2_4"
                         xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:SubscribeResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:SubscribeResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:SubscriptionId>JgBjbzFwcjA2bWIyMjIubmFtcHJkMDYucHJvZC5vdXRsb29rLmNvbRAAAAB4EQOy2pfrQJfM3hzs/nZJIZssan6H0Ag=</m:SubscriptionId>
        </m:SubscribeResponseMessage>
      </m:ResponseMessages>
    </m:SubscribeResponse>
  </s:Body>
</s:Envelope>
```

<span data-ttu-id="6cea1-224">С помощью значений [SubscriptionId](https://msdn.microsoft.com/library/3f86c178-2311-4844-82db-c2a0e469d116%28Office.15%29.aspx) из ответов на подписку был создан запрос [GetStreamingEvents](https://msdn.microsoft.com/library/dbe83857-c4f8-4d98-813f-e03c289697a1%28Office.15%29.aspx) для всех подписок в группе.</span><span class="sxs-lookup"><span data-stu-id="6cea1-224">Using the [SubscriptionId](https://msdn.microsoft.com/library/3f86c178-2311-4844-82db-c2a0e469d116%28Office.15%29.aspx) values from the subscription responses, a [GetStreamingEvents](https://msdn.microsoft.com/library/dbe83857-c4f8-4d98-813f-e03c289697a1%28Office.15%29.aspx) operation request was created for all the subscriptions in the group.</span></span> <span data-ttu-id="6cea1-225">Так как в этой группе менее 200 подписок, все они отправляются в одном запросе.</span><span class="sxs-lookup"><span data-stu-id="6cea1-225">Because there are less than 200 subscriptions in this group, they are all sent in one request.</span></span> <span data-ttu-id="6cea1-226">Для заголовка X-Преферсервераффинити задано значение true, а также включен параметр X-Баккендоверридекукие.</span><span class="sxs-lookup"><span data-stu-id="6cea1-226">The X-PreferServerAffinity header is set to true and the X-BackEndOverrideCookie is included.</span></span> 
  
```XML
POST https://outlook.office365.com/EWS/Exchange.asmx HTTP/1.1
Content-Type: text/xml; charset=utf-8
Accept: text/xml
User-Agent: ExchangeServicesClient/15.00.0516.014
X-AnchorMailbox: alfred@contoso.com
X-PreferServerAffinity: true
Host: outlook.office365.com
Cookie: X-BackEndOverrideCookie=CO1PR06MB222.namprd06.prod.outlook.com~1941996295
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2013" />
    <t:ExchangeImpersonation>
      <t:ConnectingSID>
        <t:SmtpAddress>sadie@contoso.com</t:SmtpAddress>
      </t:ConnectingSID>
    </t:ExchangeImpersonation>
  </soap:Header>
  <soap:Body>
    <m:GetStreamingEvents>
      <m:SubscriptionIds>
        <t:SubscriptionId>JgBjbzFwcjA2bWIyMjIubmFtcHJkMDYucHJvZC5vdXRsb29rLmNvbRAAAAB4EQOy2pfrQJfM3hzs/nZJIZssan6H0Ag=</t:SubscriptionId>
        <t:SubscriptionId>JgBjbzFwcjA2bWIyMjIubmFtcHJkMDYucHJvZC5vdXRsb29rLmNvbRAAAAAUeGk+7JFdSaFM8/NI/gQQpVdgZX6H0Ag=</t:SubscriptionId>
      </m:SubscriptionIds>
      <m:ConnectionTimeout>10</m:ConnectionTimeout>
    </m:GetStreamingEvents>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="6cea1-227">Возвращаемые события затем передаются в отдельный поток для обработки.</span><span class="sxs-lookup"><span data-stu-id="6cea1-227">The returned events are then passed to a separate thread for processing.</span></span>
  
## <a name="how-has-affinity-changed"></a><span data-ttu-id="6cea1-228">Как изменилось сходство?</span><span class="sxs-lookup"><span data-stu-id="6cea1-228">How has affinity changed?</span></span>
<span data-ttu-id="6cea1-229"><a name="bk_howchanged"> </a></span><span class="sxs-lookup"><span data-stu-id="6cea1-229"><a name="bk_howchanged"> </a></span></span>

<span data-ttu-id="6cea1-230">В Exchange 2010 подписки хранятся на сервере клиентского доступа, как показано на рисунке 3.</span><span class="sxs-lookup"><span data-stu-id="6cea1-230">In Exchange 2010, subscriptions are maintained on the Client Access server, as shown in Figure 3.</span></span> <span data-ttu-id="6cea1-231">В более поздних версиях Exchange, чем Exchange 2010, подписки хранятся на сервере почтовых ящиков, как показано на рисунке 4.</span><span class="sxs-lookup"><span data-stu-id="6cea1-231">In versions of Exchange later than Exchange 2010, subscriptions are maintained on the Mailbox server, as shown in Figure 4.</span></span>
  
<span data-ttu-id="6cea1-232">**Рис. 3. Процесс поддержания сходства в Exchange 2010**</span><span class="sxs-lookup"><span data-stu-id="6cea1-232">**Figure 3. Process for maintaining affinity in Exchange 2010**</span></span>

![Иллюстрация, показывающая принцип поддержки таблицы активных подписок на сервере клиентского доступа в Exchange 2010.](media/Exchange2013_NoficationAffinity2010.png)
  
<span data-ttu-id="6cea1-234">**На рисунке 4. Процесс поддержания сходства в Exchange Online и Exchange 2013**</span><span class="sxs-lookup"><span data-stu-id="6cea1-234">**Figure 4. Process for maintaining affinity in Exchange Online and Exchange 2013**</span></span>

![Иллюстрация, показывающая, как балансировщик нагрузки и сервер клиентского доступа перенаправляют запросы на сервер почтовых ящиков, на котором хранится таблица активных подписок Exchange Server и Exchange Online.](media/Exchange2013_NoficationAffinity2013.png)
  
<span data-ttu-id="6cea1-236">В Exchange 2010 клиент знает только адрес подсистемы балансировки нагрузки, а ексчанжекукие, возвращенный сервером, гарантирует, что запрос перенаправляется на подходящий сервер клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="6cea1-236">In Exchange 2010, the client only knows the address of the load balancer, and the exchangecookie that is returned by the server ensures that the request is routed to the right Client Access server.</span></span> <span data-ttu-id="6cea1-237">Однако в более поздних версиях подсистема балансировки нагрузки и роли сервера клиентского доступа должны правильно маршрутизировать запросы, прежде чем они будут переданы на сервер почтовых ящиков.</span><span class="sxs-lookup"><span data-stu-id="6cea1-237">However, in later versions, the load balancer and the Client Access server roles both have to route the requests appropriately before they get to the Mailbox server.</span></span> <span data-ttu-id="6cea1-238">Для этого требуются дополнительные сведения, поэтому были введены новые заголовки и файлы cookie.</span><span class="sxs-lookup"><span data-stu-id="6cea1-238">To do that, additional information is required, which is why the new headers and cookie were introduced.</span></span> <span data-ttu-id="6cea1-239">Подписки на [уведомления, события почтовых ящиков и EWS в Exchange в Exchange](notification-subscriptions-mailbox-events-and-ews-in-exchange.md) поясняют, как поддерживаются подписки в Exchange 2013.</span><span class="sxs-lookup"><span data-stu-id="6cea1-239">The article [Notification subscriptions, mailbox events, and EWS in Exchange](notification-subscriptions-mailbox-events-and-ews-in-exchange.md) explains how subscriptions are maintained in Exchange 2013.</span></span> 
  
<span data-ttu-id="6cea1-240">Вы можете заметить, что ексчанжекукие, используемый Exchange 2010, по-прежнему возвращается в более поздних версиях.</span><span class="sxs-lookup"><span data-stu-id="6cea1-240">You might notice that the exchangecookie that Exchange 2010 uses is still returned by later versions.</span></span> <span data-ttu-id="6cea1-241">Включение этого файла cookie в запросы не является вредом, но последующие версии Exchange игнорируют его.</span><span class="sxs-lookup"><span data-stu-id="6cea1-241">There's no harm in including this cookie in requests, but later versions of Exchange ignore it.</span></span>
  
## <a name="see-also"></a><span data-ttu-id="6cea1-242">См. также</span><span class="sxs-lookup"><span data-stu-id="6cea1-242">See also</span></span>

- [<span data-ttu-id="6cea1-243">Подписки на уведомления, события почтовых ящиков и службы EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="6cea1-243">Notification subscriptions, mailbox events, and EWS in Exchange</span></span>](notification-subscriptions-mailbox-events-and-ews-in-exchange.md)
- [<span data-ttu-id="6cea1-244">Потоковая передача уведомлений о событиях почтовых ящиков с помощью веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="6cea1-244">Stream notifications about mailbox events by using EWS in Exchange</span></span>](how-to-stream-notifications-about-mailbox-events-by-using-ews-in-exchange.md)
- [<span data-ttu-id="6cea1-245">Уведомления по запросу о событиях почтовых ящиков с помощью веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="6cea1-245">Pull notifications about mailbox events by using EWS in Exchange</span></span>](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md)
- [<span data-ttu-id="6cea1-246">Обработка ошибок, связанных с уведомлениями, в EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="6cea1-246">Handling notification-related errors in EWS in Exchange</span></span>](handling-notification-related-errors-in-ews-in-exchange.md)
- [<span data-ttu-id="6cea1-247">Изменения в управлении сходством для подписок EWS...</span><span class="sxs-lookup"><span data-stu-id="6cea1-247">Changes in Managing Affinity for EWS Subscriptions…</span></span>](https://blogs.msdn.com/b/mstehle/archive/2013/04/17/changes-in-managing-affinity-for-ews-subscriptions.aspx)
- [<span data-ttu-id="6cea1-248">EWS регулирование в Exchange</span><span class="sxs-lookup"><span data-stu-id="6cea1-248">EWS throttling in Exchange</span></span>](ews-throttling-in-exchange.md)
    

