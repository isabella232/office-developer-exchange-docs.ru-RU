---
title: Управление доступом к клиентского приложения для веб-служб Exchange в Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 60ac3f7b-ba8a-4c93-99f7-c27002caff93
description: Сведения о параметрах для управления доступом к клиентских приложений для веб-служб Exchange.
ms.openlocfilehash: 29a640178afc9814a0b2232225ae4307e49afed2
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760938"
---
# <a name="controlling-client-application-access-to-ews-in-exchange"></a><span data-ttu-id="740dc-103">Управление доступом к клиентского приложения для веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="740dc-103">Controlling client application access to EWS in Exchange</span></span>

<span data-ttu-id="740dc-104">Сведения о параметрах для управления доступом к клиентских приложений для веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="740dc-104">Learn about the options for managing client application access to EWS.</span></span>
  
<span data-ttu-id="740dc-105">Любое клиентское приложение веб-служб Exchange, создаваемого должна иметь доступ к Exchange Online, Exchange Online, как набор Office 365 или версия Exchange начиная с Exchange 2013, перед его можно вызвать операции веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="740dc-105">Any EWS client application that you create must be granted access to Exchange Online, Exchange Online as part of Office 365, or version of Exchange starting with Exchange 2013 before it can call EWS operations.</span></span> <span data-ttu-id="740dc-106">Проверки или производства server администраторы могут использовать консоль управления Exchange для ограничения доступа к веб-служб Exchange для всех пользователей и приложений, для отдельных пользователей или для отдельных приложений.</span><span class="sxs-lookup"><span data-stu-id="740dc-106">Test or production server administrators can use the Exchange Management Shell to limit access to EWS either for all users and applications, for individual users, or for individual applications.</span></span> <span data-ttu-id="740dc-107">Управление доступом для веб-служб Exchange основано на учетные записи домена.</span><span class="sxs-lookup"><span data-stu-id="740dc-107">Access control for EWS is based on domain accounts.</span></span> <span data-ttu-id="740dc-108">При подключении с использованием учетных данных, проходящих проверку подлинности с локальным администратором безопасности, сервер возвращает ошибку, указывающую, что могут подключаться только учетные записи домена.</span><span class="sxs-lookup"><span data-stu-id="740dc-108">When a connection is made with credentials that are authenticated by the local security authority, the server returns an error that indicates that only domain accounts can connect.</span></span> 
  
## <a name="access-control-for-ews-clients-and-users"></a><span data-ttu-id="740dc-109">Управление доступом клиентов веб-служб Exchange и пользователей</span><span class="sxs-lookup"><span data-stu-id="740dc-109">Access control for EWS clients and users</span></span>
<span data-ttu-id="740dc-110"><a name="bk_configure"> </a></span><span class="sxs-lookup"><span data-stu-id="740dc-110"></span></span>

<span data-ttu-id="740dc-111">Администратор сервера проверки или производства можно настроить управление доступом для клиентов, которые подключаются к веб-служб Exchange следующим образом:</span><span class="sxs-lookup"><span data-stu-id="740dc-111">Your test or production server administrator can configure access control for clients that connect to EWS in the following ways:</span></span> 
  
- <span data-ttu-id="740dc-112">Блокировка всех клиентских приложений запрещается подключение.</span><span class="sxs-lookup"><span data-stu-id="740dc-112">By blocking all client applications from connecting.</span></span>
    
- <span data-ttu-id="740dc-113">Посредством создания определенного клиентского приложения только для подключения.</span><span class="sxs-lookup"><span data-stu-id="740dc-113">By allowing specific client applications only to connect.</span></span>
    
- <span data-ttu-id="740dc-114">Посредством создания любого клиентского приложения для подключения за исключением тех, которые были заблокированы.</span><span class="sxs-lookup"><span data-stu-id="740dc-114">By allowing any client application to connect except those that are specifically blocked.</span></span>
    
- <span data-ttu-id="740dc-115">Посредством создания любого клиентского приложения для подключения.</span><span class="sxs-lookup"><span data-stu-id="740dc-115">By allowing any client application to connect.</span></span>
    
<span data-ttu-id="740dc-116">Приложения идентифицируются по строка агента пользователя, который они передают в веб-запросов HTTP.</span><span class="sxs-lookup"><span data-stu-id="740dc-116">Applications are identified by the user agent string that they send in the HTTP web request.</span></span>
  
> [! Примечание по безопасности]<span data-ttu-id="740dc-117"> уровня приложения блокировка не функция безопасности.</span><span class="sxs-lookup"><span data-stu-id="740dc-117"> Application-level blocking is not a security feature.</span></span> <span data-ttu-id="740dc-118">Строка агента пользователя легко подменить.</span><span class="sxs-lookup"><span data-stu-id="740dc-118">The user agent string is easily spoofed.</span></span> <span data-ttu-id="740dc-119">Если приложения разрешен доступ к веб-служб Exchange, оно должно по-прежнему предоставить учетные данные, сервер проверяет подлинность перед приложения могут подключаться к веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="740dc-119">If an application is allowed access to EWS, the application must still present credentials that the server authenticates before the application can connect to EWS.</span></span> 
  
<span data-ttu-id="740dc-120">Можно настроить управление доступом для владельцев почтовых ящиков, которые подключаются к веб-служб Exchange следующим образом:</span><span class="sxs-lookup"><span data-stu-id="740dc-120">Administrators can also configure access control for mailbox owners that connect to EWS in the following ways:</span></span> 
  
- <span data-ttu-id="740dc-121">Блокирование или разрешение всей организации.</span><span class="sxs-lookup"><span data-stu-id="740dc-121">By blocking or allowing an entire organization.</span></span>
    
- <span data-ttu-id="740dc-122">Блокирование или разрешение группы пользователей, определяемую средством проверки подлинности на основе ролей область, которая включает или исключает владельцев почтовых ящиков, у которых нет доступа к веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="740dc-122">By blocking or allowing a group of users identified by a role-based authentication scope that includes or excludes mailbox owners that do not have access to EWS.</span></span>
    
- <span data-ttu-id="740dc-123">Блокирование или разрешение владельца по отдельным почтовым ящикам.</span><span class="sxs-lookup"><span data-stu-id="740dc-123">By blocking or allowing an individual mailbox owner.</span></span>
    
<span data-ttu-id="740dc-124">Параметры управления доступом конкретного переопределять параметры управления общего доступа.</span><span class="sxs-lookup"><span data-stu-id="740dc-124">Specific access control settings override general access control settings.</span></span> <span data-ttu-id="740dc-125">К примеру организации по отдельным почтовым ящикам владельца разрешен доступ к приложениям доступа к веб-служб Exchange, имеет отдельный параметр приоритет и доступ разрешен.</span><span class="sxs-lookup"><span data-stu-id="740dc-125">For example, if an organization denies EWS access but an individual mailbox owner is allowed application access, the individual setting prevails and access is allowed.</span></span> 
  
## <a name="delegation-and-ews-access-management"></a><span data-ttu-id="740dc-126">Делегирование и управления доступом к веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="740dc-126">Delegation and EWS access management</span></span>
<span data-ttu-id="740dc-127"><a name="bk_delegation"> </a></span><span class="sxs-lookup"><span data-stu-id="740dc-127"></span></span>

<span data-ttu-id="740dc-128">Если делегат пользователи, у которых нет доступа к веб-служб Exchange использовать клиентское приложение, они не смогут работать в основной почтовый ящик, используя доступ к веб-служб Exchange, даже если пользователь-участник имеет веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="740dc-128">When delegate users who do not have access to EWS use your client application, they will not be able to access the principal user's mailbox by using EWS, even if the principal user has EWS access.</span></span> <span data-ttu-id="740dc-129">Если делегат пользователь имеет доступ на веб-служб Exchange, делегат сможет использовать клиентское приложение веб-служб Exchange для доступа к почтовому ящику пользователь-участник даже в том случае, если пользователь-участник не имеет веб-служб Exchange доступа.</span><span class="sxs-lookup"><span data-stu-id="740dc-129">If the delegate user has EWS access, the delegate will be able to use your EWS client application to access the principal user's mailbox even if the principal user does not have EWS access.</span></span> 
  
## <a name="impersonation-and-ews-access-management"></a><span data-ttu-id="740dc-130">Олицетворение и управления доступом к веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="740dc-130">Impersonation and EWS access management</span></span>
<span data-ttu-id="740dc-131"><a name="bk_impersonation"> </a></span><span class="sxs-lookup"><span data-stu-id="740dc-131"></span></span>

<span data-ttu-id="740dc-132">Клиентские приложения, которые подключаются к веб-служб Exchange от имени владельцев почтовых ящиков не могут использовать параметры веб-служб Exchange для владельца почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="740dc-132">Client applications that connect to EWS on behalf of mailbox owners might not be able to use the EWS settings of the mailbox owner.</span></span> <span data-ttu-id="740dc-133">Например приложение, которое архивирует сообщения для у компании есть для подключения к веб-служб Exchange, вне зависимости от параметров почтового ящика пользователя, электронной почты.</span><span class="sxs-lookup"><span data-stu-id="740dc-133">For example, an application that archives email messages for a company has to connect to EWS regardless of what the mailbox users' settings are.</span></span> <span data-ttu-id="740dc-134">Есть ли у других приложений, таких как почтовые клиенты для использования параметров веб-служб Exchange владельца почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="740dc-134">Other applications, such as mail clients, do have to use the mailbox owner's EWS settings.</span></span> 
  
<span data-ttu-id="740dc-135">Администраторам необходимо создать учетную запись олицетворения для каждого приложения или класс приложения, который они используют на сервере.</span><span class="sxs-lookup"><span data-stu-id="740dc-135">Administrators should create an impersonation account for each application or application class that they use on their server.</span></span> <span data-ttu-id="740dc-136">Это позволяет администратору настроить область управления доступом на основе ролей для всех пользователей, у которых нет разрешения веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="740dc-136">This will enable the administrator to configure the role-based access control scope for all users that do not have EWS permissions.</span></span> 
  
<span data-ttu-id="740dc-137">Чтобы включить олицетворение учетных записей, администратор сервера тестовой или производственной следует один из следующих:</span><span class="sxs-lookup"><span data-stu-id="740dc-137">To enable impersonation accounts, your test or production server administrator should do one of the following:</span></span> 
  
- <span data-ttu-id="740dc-138">Добавление группы пользователей, прошедших проверку группу доступа совместимые версии, предшествующей Win2K.</span><span class="sxs-lookup"><span data-stu-id="740dc-138">Add the Authenticated Users group to the Pre-Win2K Compatible Access Group.</span></span> 
    
- <span data-ttu-id="740dc-139">Добавление группы серверов Exchange в группе авторизации доступа Windows.</span><span class="sxs-lookup"><span data-stu-id="740dc-139">Add the Exchange Servers group to the Windows Authorization Access group.</span></span> 
    
## <a name="exchange-management-shell-cmdlets-for-access-management"></a><span data-ttu-id="740dc-140">Командлеты командной консоли Exchange для управления доступом</span><span class="sxs-lookup"><span data-stu-id="740dc-140">Exchange Management Shell cmdlets for access management</span></span>
<span data-ttu-id="740dc-141"><a name="bk_cmdlets"> </a></span><span class="sxs-lookup"><span data-stu-id="740dc-141"></span></span>

<span data-ttu-id="740dc-142">Администраторы используют следующие командлеты командной консоли Exchange для настройки доступа к элементам управления веб-служб Exchange:</span><span class="sxs-lookup"><span data-stu-id="740dc-142">Administrators use the following Exchange Management Shell cmdlets to configure EWS access controls:</span></span> 
  
- [<span data-ttu-id="740dc-143">Get-CASMailbox</span><span class="sxs-lookup"><span data-stu-id="740dc-143">Get-CASMailbox</span></span>](http://technet.microsoft.com/ru-ru/library/bb124754.aspx)
    
- [<span data-ttu-id="740dc-144">SET-CASMailbox</span><span class="sxs-lookup"><span data-stu-id="740dc-144">Set-CASMailbox</span></span>](http://technet.microsoft.com/ru-ru/library/bb125264.aspx)
    
- [<span data-ttu-id="740dc-145">Get-OrganizationConfig</span><span class="sxs-lookup"><span data-stu-id="740dc-145">Get-OrganizationConfig</span></span>](http://technet.microsoft.com/ru-ru/library/aa997571.aspx)
    
- [<span data-ttu-id="740dc-146">SET-OrganizationConfig</span><span class="sxs-lookup"><span data-stu-id="740dc-146">Set-OrganizationConfig</span></span>](http://technet.microsoft.com/ru-ru/library/aa997443.aspx)
    
## <a name="see-also"></a><span data-ttu-id="740dc-147">См. также</span><span class="sxs-lookup"><span data-stu-id="740dc-147">See also</span></span>

- [<span data-ttu-id="740dc-148">Начать работу с использованием веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="740dc-148">Start using web services in Exchange</span></span>](start-using-web-services-in-exchange.md)  
- [<span data-ttu-id="740dc-149">Управление доступом к веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="740dc-149">Control access to EWS in Exchange</span></span>](how-to-control-access-to-ews-in-exchange.md)
- [<span data-ttu-id="740dc-150">Exchange Server PowerShell (Командная консоль Exchange)</span><span class="sxs-lookup"><span data-stu-id="740dc-150">Exchange Server PowerShell (Exchange Management Shell)</span></span>](https://docs.microsoft.com/ru-ru/powershell/exchange/exchange-server/exchange-management-shell?view=exchange-ps)
- [<span data-ttu-id="740dc-151">Windows PowerShell</span><span class="sxs-lookup"><span data-stu-id="740dc-151">Windows PowerShell</span></span>](http://msdn.microsoft.com/ru-ru/library/dd835506%28v=vs.85%29.aspx)
    

