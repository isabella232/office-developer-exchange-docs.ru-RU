---
title: Настройка олицетворения
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
localization_priority: Normal
ms.assetid: efcef39f-e26d-4eed-95ac-36a5bf8c089f
description: Сведения о предоставлении роли олицетворения учетной записи службы с помощью командной консоли Exchange.
ms.openlocfilehash: 57ccef48a7553bcc06e3b3ae940b376b8555ef84
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760991"
---
# <a name="configure-impersonation"></a><span data-ttu-id="cbe01-103">Настройка олицетворения</span><span class="sxs-lookup"><span data-stu-id="cbe01-103">How to: Configure impersonation</span></span>

<span data-ttu-id="cbe01-104">Сведения о предоставлении роли олицетворения учетной записи службы с помощью командной консоли Exchange.</span><span class="sxs-lookup"><span data-stu-id="cbe01-104">Learn how to grant the impersonation role to a service account by using the Exchange Management Shell.</span></span> 
  
<span data-ttu-id="cbe01-105">С помощью олицетворения вызывающая сторона, например приложение службы, может олицетворять учетную запись пользователя.</span><span class="sxs-lookup"><span data-stu-id="cbe01-105">Impersonation enables a caller, such as a service application, to impersonate a user account.</span></span> <span data-ttu-id="cbe01-106">Вызывающая сторона может выполнять операции, используя вместо разрешений своей учетной записи те, которые сопоставлены с олицетворенной учетной записью.</span><span class="sxs-lookup"><span data-stu-id="cbe01-106">Impersonation enables a caller, such as a service application, to impersonate a user account. The caller can perform operations by using the permissions that are associated with the impersonated account instead of the permissions associated with the caller’s account.</span></span>
  
<span data-ttu-id="cbe01-107">Для назначения разрешений учетным записям в Exchange Online (автономной службе и в составе Office 365) и всех версиях Exchange, начиная с Exchange 2013, используется управление доступом на основе ролей (RBAC).</span><span class="sxs-lookup"><span data-stu-id="cbe01-107">Exchange Online, Exchange Online as part of Office 365, and versions of Exchange starting with Exchange 2013 use role-based access control (RBAC) to assign permissions to accounts. Your Exchange server administrator will need to grant any service account that will be impersonating other users the ApplicationImpersonation role by using the New-ManagementRoleAssignment cmdlet.</span></span> <span data-ttu-id="cbe01-108">Чтобы учетная запись службы могла олицетворять других пользователей, администратору сервера Exchange Server потребуется предоставить ей роль **ApplicationImpersonation** с помощью командлета [New-ManagementRoleAssignment](http://msdn.microsoft.com/library/34d4f2e3-f2c5-49e1-a6a9-1366da65a78c.aspx).</span><span class="sxs-lookup"><span data-stu-id="cbe01-108">Exchange Online, Exchange Online as part of Office 365, and versions of Exchange starting with Exchange 2013 use role-based access control (RBAC) to assign permissions to accounts. Your Exchange server administrator will need to grant any service account that will be impersonating other users the **ApplicationImpersonation** role by using the [New-ManagementRoleAssignment](http://msdn.microsoft.com/library/34d4f2e3-f2c5-49e1-a6a9-1366da65a78c.aspx) cmdlet.</span></span> 
  
## <a name="configuring-the-applicationimpersonation-role"></a><span data-ttu-id="cbe01-109">Настройка роли ApplicationImpersonation</span><span class="sxs-lookup"><span data-stu-id="cbe01-109">Configuring the ApplicationImpersonation role</span></span>

<span data-ttu-id="cbe01-110">Вам или администратору сервера Exchange Server следует использовать указанные ниже параметры командлета **New-ManagementRoleAssignment** при назначении роли **ApplicationImpersonation**.</span><span class="sxs-lookup"><span data-stu-id="cbe01-110">When you or your Exchanger server administrator assigns the **ApplicationImpersonation** role, use the following parameters of the **New-ManagementRoleAssignment** cmdlet:</span></span> 
  
-  <span data-ttu-id="cbe01-111">_Name_ &ndash; — понятное имя назначения роли.</span><span class="sxs-lookup"><span data-stu-id="cbe01-111">_Name_ &ndash; The friendly name of the role assignment.</span></span> <span data-ttu-id="cbe01-112">При каждом назначении роли запись о ней вносится в список ролей RBAC.</span><span class="sxs-lookup"><span data-stu-id="cbe01-112">Name — The friendly name of the role assignment. Each time that you assign a role, an entry is made in the RBAC roles list. You can verify role assignments by using the Get-ManagementRoleAssignment cmdlet.</span></span> <span data-ttu-id="cbe01-113">Используйте командлет [Get-ManagementRoleAssignment](http://msdn.microsoft.com/library/a3a6ee46-061b-444a-8639-43a416309445.aspx), чтобы проверить назначения ролей.</span><span class="sxs-lookup"><span data-stu-id="cbe01-113">You can verify role assignments by using the [Get-ManagementRoleAssignment](http://msdn.microsoft.com/library/a3a6ee46-061b-444a-8639-43a416309445.aspx) cmdlet.</span></span> 
    
-  <span data-ttu-id="cbe01-114">_Role_ &ndash; — роль RBAC, которую нужно назначить.</span><span class="sxs-lookup"><span data-stu-id="cbe01-114">_Role_ &ndash; The RBAC role to assign.</span></span> <span data-ttu-id="cbe01-115">Для настройки олицетворения нужно назначить роль **ApplicationImpersonation**.</span><span class="sxs-lookup"><span data-stu-id="cbe01-115">Role — The RBAC role to assign. When you set up impersonation, you assign the **ApplicationImpersonation** role.</span></span> 
    
-  <span data-ttu-id="cbe01-116">_User_ &ndash; — учетная запись службы.</span><span class="sxs-lookup"><span data-stu-id="cbe01-116">_User_ &ndash; The service account.</span></span> 
    
-  <span data-ttu-id="cbe01-117">_CustomRecipientScope_ &ndash; — область пользователей, которых может олицетворять учетная запись службы.</span><span class="sxs-lookup"><span data-stu-id="cbe01-117">_CustomRecipientScope_ &ndash; The scope of users that the service account can impersonate.</span></span> <span data-ttu-id="cbe01-118">Учетная запись службы может олицетворять только тех пользователей, которые входят в указанную область.</span><span class="sxs-lookup"><span data-stu-id="cbe01-118">The service account will only be allowed to impersonate other users within the specified scope.</span></span> <span data-ttu-id="cbe01-119">Если область не указана, учетная запись службы получает роль **ApplicationImpersonation** для всех пользователей организации.</span><span class="sxs-lookup"><span data-stu-id="cbe01-119">If no scope is specified, the service account is granted the **ApplicationImpersonation** role over all users in an organization.</span></span> <span data-ttu-id="cbe01-120">Можно создавать специальные области управления с помощью командлета [New-ManagementScope](http://msdn.microsoft.com/library/1ea1f474-69d6-48c0-9beb-bfa4442c5dab.aspx).</span><span class="sxs-lookup"><span data-stu-id="cbe01-120">You can create custom management scopes by using the [New-ManagementScope](http://msdn.microsoft.com/library/1ea1f474-69d6-48c0-9beb-bfa4442c5dab.aspx) cmdlet.</span></span> 
    
<span data-ttu-id="cbe01-121">Перед настройкой олицетворения вам понадобятся:</span><span class="sxs-lookup"><span data-stu-id="cbe01-121">Before you can configure impersonation, you need:</span></span>
  
- <span data-ttu-id="cbe01-122">Учетные данные администратора для сервера Exchange Server.</span><span class="sxs-lookup"><span data-stu-id="cbe01-122">Administrative credentials for the Exchange server.</span></span>
    
- <span data-ttu-id="cbe01-123">Учетные данные администратора домена или другие учетные данные с разрешением на создание и назначение ролей и областей.</span><span class="sxs-lookup"><span data-stu-id="cbe01-123">Domain Administrator credentials, or other credentials with the permission to create and assign roles and scopes.</span></span>
    
- <span data-ttu-id="cbe01-p106">Средства управления Exchange. Их нужно установить на компьютере, с которого будут выполняться команды.</span><span class="sxs-lookup"><span data-stu-id="cbe01-p106">Exchange management tools. These are installed on the computer from which you will run the commands.</span></span>
    
### <a name="to-configure-impersonation-for-all-users-in-an-organization"></a><span data-ttu-id="cbe01-126">Настройка олицетворения для всех пользователей в организации</span><span class="sxs-lookup"><span data-stu-id="cbe01-126">To configure impersonation for all users in an organization</span></span>

1. <span data-ttu-id="cbe01-127">Запустите командную консоль Exchange.</span><span class="sxs-lookup"><span data-stu-id="cbe01-127">Open the Exchange Management Shell.</span></span> <span data-ttu-id="cbe01-128">В меню "Пуск" выберите **Все приложения** >  > **Microsoft Exchange Server 2013**.</span><span class="sxs-lookup"><span data-stu-id="cbe01-128">Open the Exchange Management Shell. From the Start menu, choose All Programs > Microsoft Exchange Server 2013.</span></span> 
    
2. <span data-ttu-id="cbe01-129">Запустите командлет **New-ManagementRoleAssignment**, чтобы добавить разрешение на олицетворение для указанного пользователя.</span><span class="sxs-lookup"><span data-stu-id="cbe01-129">Run the **New-ManagementRoleAssignment** cmdlet to add the impersonation permission to the specified user.</span></span> <span data-ttu-id="cbe01-130">В приведенном ниже примере показано, как настроить олицетворение так, чтобы учетная запись службы могла олицетворять всех остальных пользователей в организации.</span><span class="sxs-lookup"><span data-stu-id="cbe01-130">Run the New-ManagementRoleAssignment cmdlet to add the impersonation permission to the specified user. The following example shows how to configure impersonation to enable a service account to impersonate all other users in an organization.</span></span> 
    
   ```powershell
   New-ManagementRoleAssignment -name:impersonationAssignmentName -Role:ApplicationImpersonation -User:serviceAccount 
   ```

### <a name="to-configure-impersonation-for-specific-users-or-groups-of-users"></a><span data-ttu-id="cbe01-131">Настройка олицетворения для определенных пользователей или групп пользователей</span><span class="sxs-lookup"><span data-stu-id="cbe01-131">To configure impersonation for specific users or groups of users</span></span>

1. <span data-ttu-id="cbe01-132">Запустите командную консоль Exchange.</span><span class="sxs-lookup"><span data-stu-id="cbe01-132">Open the Exchange Management Shell.</span></span> <span data-ttu-id="cbe01-133">В меню "Пуск" выберите **Все приложения** >  > **Microsoft Exchange Server 2013**.</span><span class="sxs-lookup"><span data-stu-id="cbe01-133">Open the Exchange Management Shell. From the Start menu, choose All Programs > Microsoft Exchange Server 2013.</span></span> 
    
2. <span data-ttu-id="cbe01-134">Запустите командлет **New-ManagementScope**, чтобы создать область, которой можно назначить роль олицетворения.</span><span class="sxs-lookup"><span data-stu-id="cbe01-134">Run the **New-ManagementScope** cmdlet to create a scope to which the impersonation role can be assigned.</span></span> <span data-ttu-id="cbe01-135">Если такая область уже есть, этот шаг можно пропустить.</span><span class="sxs-lookup"><span data-stu-id="cbe01-135">If an existing scope is available, you can skip this step.</span></span> <span data-ttu-id="cbe01-136">В приведенном ниже примере показано, как создать область управления для определенной группы.</span><span class="sxs-lookup"><span data-stu-id="cbe01-136">The following example shows how to create a management scope for a specific group.</span></span> 
    
   ```powershell
    New-ManagementScope -Name:scopeName -RecipientRestrictionFilter:recipientFilter
   ```

   <span data-ttu-id="cbe01-137">Параметр _RecipientRestrictionFilter_ командлета**New-ManagementScope** определяет участников области.</span><span class="sxs-lookup"><span data-stu-id="cbe01-137">The _RecipientRestrictionFilter_ parameter of the **New-ManagementScope** cmdlet defines the members of the scope.</span></span> <span data-ttu-id="cbe01-138">Можно использовать свойства объекта **Identity**, чтобы создать фильтр.</span><span class="sxs-lookup"><span data-stu-id="cbe01-138">You can use the properties of the **Identity** object to create the filter.</span></span> <span data-ttu-id="cbe01-139">В примере ниже показан фильтр, который ограничивает результаты одним пользователем с именем "john".</span><span class="sxs-lookup"><span data-stu-id="cbe01-139">The following example is a filter that restricts the result to a single user with the user name "john."</span></span> 
    
   ```powershell
   Name -eq "john"
   ```

3. <span data-ttu-id="cbe01-140">Запустите командлет **New-ManagementRoleAssignment**, чтобы добавить разрешение на олицетворение пользователей, входящих в указанную область.</span><span class="sxs-lookup"><span data-stu-id="cbe01-140">Run the **New-ManagementRoleAssignment** cmdlet to add the permission to impersonate the members of the specified scope. The following example shows how to configure a service account to impersonate all users in a scope.</span></span> <span data-ttu-id="cbe01-141">В приведенном ниже примере показано, как настроить учетную запись службы так, чтобы она могла олицетворять всех пользователей в области.</span><span class="sxs-lookup"><span data-stu-id="cbe01-141">Run the New-ManagementRoleAssignment cmdlet to add the permission to impersonate the members of the specified scope. The following example shows how to configure a service account to impersonate all users in a scope.</span></span> 
    
   ```powershell
    New-ManagementRoleAssignment -Name:impersonationAssignmentName -Role:ApplicationImpersonation -User:serviceAccount -CustomRecipientWriteScope:scopeName
    
   ```


<span data-ttu-id="cbe01-142">Когда администратор предоставит разрешения на олицетворение, с помощью учетной записи службы можно будет вызывать учетные записи других пользователей.</span><span class="sxs-lookup"><span data-stu-id="cbe01-142">After your administrator grants impersonation permissions, you can use the service account to make calls against other users’ accounts. You can verify role assignments by using the Get-ManagementRoleAssignment cmdlet.</span></span> <span data-ttu-id="cbe01-143">Используйте командлет [Get-ManagementRoleAssignment](http://msdn.microsoft.com/library/a3a6ee46-061b-444a-8639-43a416309445.aspx), чтобы проверить назначения ролей.</span><span class="sxs-lookup"><span data-stu-id="cbe01-143">You can verify role assignments by using the [Get-ManagementRoleAssignment](http://msdn.microsoft.com/library/a3a6ee46-061b-444a-8639-43a416309445.aspx) cmdlet.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="cbe01-144">См. также</span><span class="sxs-lookup"><span data-stu-id="cbe01-144">See also</span></span>

- [<span data-ttu-id="cbe01-145">Олицетворение и EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="cbe01-145">Impersonation and EWS in Exchange</span></span>](impersonation-and-ews-in-exchange.md)
- [<span data-ttu-id="cbe01-146">Роль ApplicationImpersonation</span><span class="sxs-lookup"><span data-stu-id="cbe01-146">Configuring the ApplicationImpersonation role</span></span>](http://technet.microsoft.com/ru-RU/library/dd776119%28v=exchg.150%29.aspx)   
- [<span data-ttu-id="cbe01-147">New-ManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="cbe01-147">New-ManagementRoleAssignment</span></span>](http://msdn.microsoft.com/library/34d4f2e3-f2c5-49e1-a6a9-1366da65a78c.aspx)    
- [<span data-ttu-id="cbe01-148">Get-ManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="cbe01-148">Get-ManagementRoleAssignment</span></span>](http://msdn.microsoft.com/library/a3a6ee46-061b-444a-8639-43a416309445.aspx)
    

