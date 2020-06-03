---
title: Управление доступом клиентских приложений к EWS в Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.assetid: 60ac3f7b-ba8a-4c93-99f7-c27002caff93
description: Узнайте о параметрах управления доступом клиентского приложения к EWS.
localization_priority: Priority
ms.openlocfilehash: b887b8167e3d38946b1d6caffe12655ded89569f
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44528463"
---
# <a name="controlling-client-application-access-to-ews-in-exchange"></a><span data-ttu-id="f696d-103">Управление доступом клиентских приложений к EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="f696d-103">Controlling client application access to EWS in Exchange</span></span>

<span data-ttu-id="f696d-104">Узнайте о параметрах управления доступом клиентского приложения к EWS.</span><span class="sxs-lookup"><span data-stu-id="f696d-104">Learn about the options for managing client application access to EWS.</span></span>
  
<span data-ttu-id="f696d-105">Любое созданное клиентское приложение EWS должно иметь доступ к Exchange Online, Exchange Online в составе Office 365 или версии Exchange, начиная с Exchange 2013, прежде чем она сможет вызвать операции EWS.</span><span class="sxs-lookup"><span data-stu-id="f696d-105">Any EWS client application that you create must be granted access to Exchange Online, Exchange Online as part of Office 365, or version of Exchange starting with Exchange 2013 before it can call EWS operations.</span></span> <span data-ttu-id="f696d-106">Администраторы тестовых или рабочих серверов могут использовать командную консоль Exchange для ограничения доступа к EWS для всех пользователей и приложений, для отдельных пользователей или для отдельных приложений.</span><span class="sxs-lookup"><span data-stu-id="f696d-106">Test or production server administrators can use the Exchange Management Shell to limit access to EWS either for all users and applications, for individual users, or for individual applications.</span></span> <span data-ttu-id="f696d-107">Управление доступом для EWS основано на учетных записях доменов.</span><span class="sxs-lookup"><span data-stu-id="f696d-107">Access control for EWS is based on domain accounts.</span></span> <span data-ttu-id="f696d-108">Когда подключение устанавливается с учетными данными, которые проходят проверку подлинности локальным администратором безопасности, сервер возвращает сообщение об ошибке, свидетельствующее о том, что только учетные записи домена могут подключаться.</span><span class="sxs-lookup"><span data-stu-id="f696d-108">When a connection is made with credentials that are authenticated by the local security authority, the server returns an error that indicates that only domain accounts can connect.</span></span> 
  
## <a name="access-control-for-ews-clients-and-users"></a><span data-ttu-id="f696d-109">Управление доступом для клиентов и пользователей EWS</span><span class="sxs-lookup"><span data-stu-id="f696d-109">Access control for EWS clients and users</span></span>
<span data-ttu-id="f696d-110"><a name="bk_configure"> </a></span><span class="sxs-lookup"><span data-stu-id="f696d-110"><a name="bk_configure"> </a></span></span>

<span data-ttu-id="f696d-111">Администратор тестового или рабочего сервера может настроить управление доступом для клиентов, подключающихся к EWS, следующими способами:</span><span class="sxs-lookup"><span data-stu-id="f696d-111">Your test or production server administrator can configure access control for clients that connect to EWS in the following ways:</span></span> 
  
- <span data-ttu-id="f696d-112">, Блокируя все клиентские приложения.</span><span class="sxs-lookup"><span data-stu-id="f696d-112">By blocking all client applications from connecting.</span></span>
    
- <span data-ttu-id="f696d-113">Разрешая только определенным клиентским приложениям подключаться.</span><span class="sxs-lookup"><span data-stu-id="f696d-113">By allowing specific client applications only to connect.</span></span>
    
- <span data-ttu-id="f696d-114">Разрешить подключаться к любому клиентскому приложению за исключением тех случаев, когда они блокируются специально.</span><span class="sxs-lookup"><span data-stu-id="f696d-114">By allowing any client application to connect except those that are specifically blocked.</span></span>
    
- <span data-ttu-id="f696d-115">Разрешить подключаться к любому клиентскому приложению.</span><span class="sxs-lookup"><span data-stu-id="f696d-115">By allowing any client application to connect.</span></span>
    
<span data-ttu-id="f696d-116">Приложения определяются строкой агента пользователя, отправляемой в веб-запросе HTTP.</span><span class="sxs-lookup"><span data-stu-id="f696d-116">Applications are identified by the user agent string that they send in the HTTP web request.</span></span>
  
> [!IMPORTANT]
> <span data-ttu-id="f696d-117">Блокировка на уровне приложения не является компонентом безопасности.</span><span class="sxs-lookup"><span data-stu-id="f696d-117">Application-level blocking is not a security feature.</span></span> <span data-ttu-id="f696d-118">Строка агента пользователя легко подделываться.</span><span class="sxs-lookup"><span data-stu-id="f696d-118">The user agent string is easily spoofed.</span></span> <span data-ttu-id="f696d-119">Если приложению разрешен доступ к EWS, приложение должно по-прежнему показывать учетные данные, которые сервер выполняет проверку подлинности, прежде чем приложение сможет подключиться к EWS.</span><span class="sxs-lookup"><span data-stu-id="f696d-119">If an application is allowed access to EWS, the application must still present credentials that the server authenticates before the application can connect to EWS.</span></span> 
  
<span data-ttu-id="f696d-120">Кроме того, администраторы могут настроить управление доступом для владельцев почтовых ящиков, которые подключаются к EWS, следующими способами:</span><span class="sxs-lookup"><span data-stu-id="f696d-120">Administrators can also configure access control for mailbox owners that connect to EWS in the following ways:</span></span> 
  
- <span data-ttu-id="f696d-121">, Блокируя или разрешив всю организацию.</span><span class="sxs-lookup"><span data-stu-id="f696d-121">By blocking or allowing an entire organization.</span></span>
    
- <span data-ttu-id="f696d-122">С помощью блокировки или предоставления группе пользователей, которая определяется областью проверки подлинности на основе ролей, включает или исключает владельцев почтовых ящиков, у которых нет доступа к EWS.</span><span class="sxs-lookup"><span data-stu-id="f696d-122">By blocking or allowing a group of users identified by a role-based authentication scope that includes or excludes mailbox owners that do not have access to EWS.</span></span>
    
- <span data-ttu-id="f696d-123">С помощью блокировки или разрешения отдельного владельца почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="f696d-123">By blocking or allowing an individual mailbox owner.</span></span>
    
<span data-ttu-id="f696d-124">Особые параметры управления доступом переопределяют параметры управления общим доступом.</span><span class="sxs-lookup"><span data-stu-id="f696d-124">Specific access control settings override general access control settings.</span></span> <span data-ttu-id="f696d-125">Например, если Организация запрещает доступ к EWS, но индивидуальный владелец почтового ящика разрешает доступ к приложениям, то индивидуальные параметры, а также доступ к ним разрешены.</span><span class="sxs-lookup"><span data-stu-id="f696d-125">For example, if an organization denies EWS access but an individual mailbox owner is allowed application access, the individual setting prevails and access is allowed.</span></span> 
  
## <a name="delegation-and-ews-access-management"></a><span data-ttu-id="f696d-126">Управление доступом для делегирования и EWS</span><span class="sxs-lookup"><span data-stu-id="f696d-126">Delegation and EWS access management</span></span>
<span data-ttu-id="f696d-127"><a name="bk_delegation"> </a></span><span class="sxs-lookup"><span data-stu-id="f696d-127"><a name="bk_delegation"> </a></span></span>

<span data-ttu-id="f696d-128">При делегировании пользователям, у которых нет доступа к EWS, использовать клиентское приложение, они не смогут получить доступ к почтовому ящику основного пользователя с помощью EWS, даже если основной пользователь имеет доступ к EWS.</span><span class="sxs-lookup"><span data-stu-id="f696d-128">When delegate users who do not have access to EWS use your client application, they will not be able to access the principal user's mailbox by using EWS, even if the principal user has EWS access.</span></span> <span data-ttu-id="f696d-129">Если представитель имеет доступ к EWS, он сможет использовать клиентское приложение EWS для доступа к почтовому ящику основного пользователя, даже если основной пользователь не имеет доступа EWS.</span><span class="sxs-lookup"><span data-stu-id="f696d-129">If the delegate user has EWS access, the delegate will be able to use your EWS client application to access the principal user's mailbox even if the principal user does not have EWS access.</span></span> 
  
## <a name="impersonation-and-ews-access-management"></a><span data-ttu-id="f696d-130">Управление доступом к олицетворению и EWS</span><span class="sxs-lookup"><span data-stu-id="f696d-130">Impersonation and EWS access management</span></span>
<span data-ttu-id="f696d-131"><a name="bk_impersonation"> </a></span><span class="sxs-lookup"><span data-stu-id="f696d-131"><a name="bk_impersonation"> </a></span></span>

<span data-ttu-id="f696d-132">Клиентские приложения, которые подключаются к EWS от имени владельцев почтовых ящиков, могут не иметь возможность использовать параметры EWS владельца почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="f696d-132">Client applications that connect to EWS on behalf of mailbox owners might not be able to use the EWS settings of the mailbox owner.</span></span> <span data-ttu-id="f696d-133">Например, приложение, которое архивирует сообщения электронной почты для компании, должно подключаться к службам EWS независимо от параметров пользователей почтовых ящиков.</span><span class="sxs-lookup"><span data-stu-id="f696d-133">For example, an application that archives email messages for a company has to connect to EWS regardless of what the mailbox users' settings are.</span></span> <span data-ttu-id="f696d-134">Другие приложения, такие как почтовые клиенты, должны использовать параметры EWS владельца почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="f696d-134">Other applications, such as mail clients, do have to use the mailbox owner's EWS settings.</span></span> 
  
<span data-ttu-id="f696d-135">Администраторы должны создать учетную запись олицетворения для каждого класса приложения или приложения, который они используют на своем сервере.</span><span class="sxs-lookup"><span data-stu-id="f696d-135">Administrators should create an impersonation account for each application or application class that they use on their server.</span></span> <span data-ttu-id="f696d-136">Это позволит администратору настроить область управления доступом на основе ролей для всех пользователей, у которых нет разрешений EWS.</span><span class="sxs-lookup"><span data-stu-id="f696d-136">This will enable the administrator to configure the role-based access control scope for all users that do not have EWS permissions.</span></span> 
  
<span data-ttu-id="f696d-137">Чтобы включить учетные записи олицетворения, администратору тестового или рабочего сервера необходимо выполнить одно из следующих действий:</span><span class="sxs-lookup"><span data-stu-id="f696d-137">To enable impersonation accounts, your test or production server administrator should do one of the following:</span></span> 
  
- <span data-ttu-id="f696d-138">Добавьте группу Пользователи, прошедшие проверку подлинности, в группу доступа пред – Win2K.</span><span class="sxs-lookup"><span data-stu-id="f696d-138">Add the Authenticated Users group to the Pre-Win2K Compatible Access Group.</span></span> 
    
- <span data-ttu-id="f696d-139">Добавьте группу серверов Exchange в группу авторизации доступа Windows.</span><span class="sxs-lookup"><span data-stu-id="f696d-139">Add the Exchange Servers group to the Windows Authorization Access group.</span></span> 
    
## <a name="exchange-management-shell-cmdlets-for-access-management"></a><span data-ttu-id="f696d-140">Командлеты командной консоли Exchange для управления доступом</span><span class="sxs-lookup"><span data-stu-id="f696d-140">Exchange Management Shell cmdlets for access management</span></span>
<span data-ttu-id="f696d-141"><a name="bk_cmdlets"> </a></span><span class="sxs-lookup"><span data-stu-id="f696d-141"><a name="bk_cmdlets"> </a></span></span>

<span data-ttu-id="f696d-142">Администраторы используют следующие командлеты командной консоли Exchange для настройки средств контроля доступа EWS:</span><span class="sxs-lookup"><span data-stu-id="f696d-142">Administrators use the following Exchange Management Shell cmdlets to configure EWS access controls:</span></span> 
  
- [<span data-ttu-id="f696d-143">Get-CASMailbox</span><span class="sxs-lookup"><span data-stu-id="f696d-143">Get-CASMailbox</span></span>](https://technet.microsoft.com/library/bb124754.aspx)   
- [<span data-ttu-id="f696d-144">Set-CASMailbox</span><span class="sxs-lookup"><span data-stu-id="f696d-144">Set-CASMailbox</span></span>](https://technet.microsoft.com/library/bb125264.aspx)   
- [<span data-ttu-id="f696d-145">Get — OrganizationConfig</span><span class="sxs-lookup"><span data-stu-id="f696d-145">Get-OrganizationConfig</span></span>](https://technet.microsoft.com/library/aa997571.aspx)   
- [<span data-ttu-id="f696d-146">Set — OrganizationConfig</span><span class="sxs-lookup"><span data-stu-id="f696d-146">Set-OrganizationConfig</span></span>](https://technet.microsoft.com/library/aa997443.aspx)
    
## <a name="see-also"></a><span data-ttu-id="f696d-147">См. также</span><span class="sxs-lookup"><span data-stu-id="f696d-147">See also</span></span>

- [<span data-ttu-id="f696d-148">Начало работы с веб-службами Exchange</span><span class="sxs-lookup"><span data-stu-id="f696d-148">Start using web services in Exchange</span></span>](start-using-web-services-in-exchange.md)  
- [<span data-ttu-id="f696d-149">Контроль доступа к EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="f696d-149">Control access to EWS in Exchange</span></span>](how-to-control-access-to-ews-in-exchange.md)
- [<span data-ttu-id="f696d-150">PowerShell в Exchange Server (Командная консоль Exchange)</span><span class="sxs-lookup"><span data-stu-id="f696d-150">Exchange Server PowerShell (Exchange Management Shell)</span></span>](https://docs.microsoft.com/powershell/exchange/exchange-server/exchange-management-shell?view=exchange-ps)
- [<span data-ttu-id="f696d-151">Windows PowerShell</span><span class="sxs-lookup"><span data-stu-id="f696d-151">Windows PowerShell</span></span>](https://msdn.microsoft.com/library/dd835506%28v=vs.85%29.aspx)
    

