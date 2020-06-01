---
title: Настройка олицетворения
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
ms.assetid: efcef39f-e26d-4eed-95ac-36a5bf8c089f
description: Сведения о предоставлении роли олицетворения учетной записи службы с помощью командной консоли Exchange.
localization_priority: Priority
ms.openlocfilehash: f8fe95536213e347840af082d765a9cc2fbce819
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44455900"
---
# <a name="configure-impersonation"></a><span data-ttu-id="9258d-103">Настройка олицетворения</span><span class="sxs-lookup"><span data-stu-id="9258d-103">Configure impersonation</span></span>

<span data-ttu-id="9258d-104">Сведения о предоставлении роли олицетворения учетной записи службы с помощью командной консоли Exchange.</span><span class="sxs-lookup"><span data-stu-id="9258d-104">Learn how to grant the impersonation role to a service account by using the Exchange Management Shell.</span></span> 
  
<span data-ttu-id="9258d-105">С помощью олицетворения вызывающая сторона, например приложение службы, может олицетворять учетную запись пользователя.</span><span class="sxs-lookup"><span data-stu-id="9258d-105">Impersonation enables a caller, such as a service application, to impersonate a user account.</span></span> <span data-ttu-id="9258d-106">Вызывающая сторона может выполнять операции, используя вместо разрешений своей учетной записи те, которые сопоставлены с олицетворенной учетной записью.</span><span class="sxs-lookup"><span data-stu-id="9258d-106">The caller can perform operations by using the permissions that are associated with the impersonated account instead of the permissions associated with the caller's account.</span></span>
  
<span data-ttu-id="9258d-107">Для назначения разрешений учетным записям в Exchange Online (автономной службе и в составе Office 365) и всех версиях Exchange, начиная с Exchange 2013, используется управление доступом на основе ролей (RBAC).</span><span class="sxs-lookup"><span data-stu-id="9258d-107">Exchange Online, Exchange Online as part of Office 365, and versions of Exchange starting with Exchange 2013 use role-based access control (RBAC) to assign permissions to accounts.</span></span> <span data-ttu-id="9258d-108">Чтобы учетная запись службы могла олицетворять других пользователей, администратору сервера Exchange Server потребуется предоставить ей роль **ApplicationImpersonation** с помощью командлета [New-ManagementRoleAssignment](https://msdn.microsoft.com/library/34d4f2e3-f2c5-49e1-a6a9-1366da65a78c.aspx).</span><span class="sxs-lookup"><span data-stu-id="9258d-108">Your Exchange server administrator will need to grant any service account that will be impersonating other users the **ApplicationImpersonation** role by using the [New-ManagementRoleAssignment](https://msdn.microsoft.com/library/34d4f2e3-f2c5-49e1-a6a9-1366da65a78c.aspx) cmdlet.</span></span> 
  
## <a name="configuring-the-applicationimpersonation-role"></a><span data-ttu-id="9258d-109">Настройка роли ApplicationImpersonation</span><span class="sxs-lookup"><span data-stu-id="9258d-109">Configuring the ApplicationImpersonation role</span></span>

<span data-ttu-id="9258d-110">Вам или администратору сервера Exchange Server следует использовать указанные ниже параметры командлета **New-ManagementRoleAssignment** при назначении роли **ApplicationImpersonation**.</span><span class="sxs-lookup"><span data-stu-id="9258d-110">When you or your Exchanger server administrator assigns the **ApplicationImpersonation** role, use the following parameters of the **New-ManagementRoleAssignment** cmdlet:</span></span> 
  
-  <span data-ttu-id="9258d-111">_Name_ &ndash; — понятное имя назначения роли.</span><span class="sxs-lookup"><span data-stu-id="9258d-111">_Name_ &ndash; The friendly name of the role assignment.</span></span> <span data-ttu-id="9258d-112">При каждом назначении роли запись о ней вносится в список ролей RBAC.</span><span class="sxs-lookup"><span data-stu-id="9258d-112">Each time that you assign a role, an entry is made in the RBAC roles list.</span></span> <span data-ttu-id="9258d-113">Используйте командлет [Get-ManagementRoleAssignment](https://msdn.microsoft.com/library/a3a6ee46-061b-444a-8639-43a416309445.aspx), чтобы проверить назначения ролей.</span><span class="sxs-lookup"><span data-stu-id="9258d-113">You can verify role assignments by using the [Get-ManagementRoleAssignment](https://msdn.microsoft.com/library/a3a6ee46-061b-444a-8639-43a416309445.aspx) cmdlet.</span></span> 
    
-  <span data-ttu-id="9258d-114">_Role_ &ndash; — роль RBAC, которую нужно назначить.</span><span class="sxs-lookup"><span data-stu-id="9258d-114">_Role_ &ndash; The RBAC role to assign.</span></span> <span data-ttu-id="9258d-115">Для настройки олицетворения нужно назначить роль **ApplicationImpersonation**.</span><span class="sxs-lookup"><span data-stu-id="9258d-115">When you set up impersonation, you assign the **ApplicationImpersonation** role.</span></span> 
    
-  <span data-ttu-id="9258d-116">_User_ &ndash; — учетная запись службы.</span><span class="sxs-lookup"><span data-stu-id="9258d-116">_User_ &ndash; The service account.</span></span> 
    
-  <span data-ttu-id="9258d-117">_CustomRecipientScope_ &ndash; — область пользователей, которых может олицетворять учетная запись службы.</span><span class="sxs-lookup"><span data-stu-id="9258d-117">_CustomRecipientScope_ &ndash; The scope of users that the service account can impersonate.</span></span> <span data-ttu-id="9258d-118">Учетная запись службы может олицетворять только тех пользователей, которые входят в указанную область.</span><span class="sxs-lookup"><span data-stu-id="9258d-118">The service account will only be allowed to impersonate other users within the specified scope.</span></span> <span data-ttu-id="9258d-119">Если область не указана, учетная запись службы получает роль **ApplicationImpersonation** для всех пользователей организации.</span><span class="sxs-lookup"><span data-stu-id="9258d-119">If no scope is specified, the service account is granted the **ApplicationImpersonation** role over all users in an organization.</span></span> <span data-ttu-id="9258d-120">Можно создавать специальные области управления с помощью командлета [New-ManagementScope](https://msdn.microsoft.com/library/1ea1f474-69d6-48c0-9beb-bfa4442c5dab.aspx).</span><span class="sxs-lookup"><span data-stu-id="9258d-120">You can create custom management scopes by using the [New-ManagementScope](https://msdn.microsoft.com/library/1ea1f474-69d6-48c0-9beb-bfa4442c5dab.aspx) cmdlet.</span></span> 
    
<span data-ttu-id="9258d-121">Перед настройкой олицетворения вам понадобятся:</span><span class="sxs-lookup"><span data-stu-id="9258d-121">Before you can configure impersonation, you need:</span></span>
  
- <span data-ttu-id="9258d-122">Учетные данные администратора для сервера Exchange Server.</span><span class="sxs-lookup"><span data-stu-id="9258d-122">Administrative credentials for the Exchange server.</span></span>
    
- <span data-ttu-id="9258d-123">Учетные данные администратора домена или другие учетные данные с разрешением на создание и назначение ролей и областей.</span><span class="sxs-lookup"><span data-stu-id="9258d-123">Domain Administrator credentials, or other credentials with the permission to create and assign roles and scopes.</span></span>
    
- <span data-ttu-id="9258d-p106">Средства управления Exchange. Их нужно установить на компьютере, с которого будут выполняться команды.</span><span class="sxs-lookup"><span data-stu-id="9258d-p106">Exchange management tools. These are installed on the computer from which you will run the commands.</span></span>
    
### <a name="to-configure-impersonation-for-all-users-in-an-organization"></a><span data-ttu-id="9258d-126">Настройка олицетворения для всех пользователей в организации</span><span class="sxs-lookup"><span data-stu-id="9258d-126">To configure impersonation for all users in an organization</span></span>

1. <span data-ttu-id="9258d-127">Запустите командную консоль Exchange.</span><span class="sxs-lookup"><span data-stu-id="9258d-127">Open the Exchange Management Shell.</span></span> <span data-ttu-id="9258d-128">В меню "Пуск" выберите **Все приложения** >  > **Microsoft Exchange Server 2013**.</span><span class="sxs-lookup"><span data-stu-id="9258d-128">From the Start menu, choose **All Programs** > **Microsoft Exchange Server 2013**.</span></span> 
    
2. <span data-ttu-id="9258d-129">Запустите командлет **New-ManagementRoleAssignment**, чтобы добавить разрешение на олицетворение для указанного пользователя.</span><span class="sxs-lookup"><span data-stu-id="9258d-129">Run the **New-ManagementRoleAssignment** cmdlet to add the impersonation permission to the specified user.</span></span> <span data-ttu-id="9258d-130">В приведенном ниже примере показано, как настроить олицетворение так, чтобы учетная запись службы могла олицетворять всех остальных пользователей в организации.</span><span class="sxs-lookup"><span data-stu-id="9258d-130">The following example shows how to configure impersonation to enable a service account to impersonate all other users in an organization.</span></span> 
    
   ```powershell
   New-ManagementRoleAssignment -name:impersonationAssignmentName -Role:ApplicationImpersonation -User:serviceAccount 
   ```

### <a name="to-configure-impersonation-for-specific-users-or-groups-of-users"></a><span data-ttu-id="9258d-131">Настройка олицетворения для определенных пользователей или групп пользователей</span><span class="sxs-lookup"><span data-stu-id="9258d-131">To configure impersonation for specific users or groups of users</span></span>

1. <span data-ttu-id="9258d-132">Запустите командную консоль Exchange.</span><span class="sxs-lookup"><span data-stu-id="9258d-132">Open the Exchange Management Shell.</span></span> <span data-ttu-id="9258d-133">В меню "Пуск" выберите **Все приложения** >  > **Microsoft Exchange Server 2013**.</span><span class="sxs-lookup"><span data-stu-id="9258d-133">From the Start menu, choose **All Programs** > **Microsoft Exchange Server 2013**.</span></span> 
    
2. <span data-ttu-id="9258d-134">Запустите командлет **New-ManagementScope**, чтобы создать область, которой можно назначить роль олицетворения.</span><span class="sxs-lookup"><span data-stu-id="9258d-134">Run the **New-ManagementScope** cmdlet to create a scope to which the impersonation role can be assigned.</span></span> <span data-ttu-id="9258d-135">Если такая область уже есть, этот шаг можно пропустить.</span><span class="sxs-lookup"><span data-stu-id="9258d-135">If an existing scope is available, you can skip this step.</span></span> <span data-ttu-id="9258d-136">В приведенном ниже примере показано, как создать область управления для определенной группы.</span><span class="sxs-lookup"><span data-stu-id="9258d-136">The following example shows how to create a management scope for a specific group.</span></span> 
    
   ```powershell
    New-ManagementScope -Name:scopeName -RecipientRestrictionFilter:recipientFilter
   ```

   <span data-ttu-id="9258d-137">Параметр _RecipientRestrictionFilter_ командлета**New-ManagementScope** определяет участников области.</span><span class="sxs-lookup"><span data-stu-id="9258d-137">The _RecipientRestrictionFilter_ parameter of the **New-ManagementScope** cmdlet defines the members of the scope.</span></span> <span data-ttu-id="9258d-138">Можно использовать свойства объекта **Identity**, чтобы создать фильтр.</span><span class="sxs-lookup"><span data-stu-id="9258d-138">You can use the properties of the **Identity** object to create the filter.</span></span> <span data-ttu-id="9258d-139">В примере ниже показан фильтр, который ограничивает результаты одним пользователем с именем "john".</span><span class="sxs-lookup"><span data-stu-id="9258d-139">The following example is a filter that restricts the result to a single user with the user name "john."</span></span> 
    
   ```powershell
   Name -eq "john"
   ```

3. <span data-ttu-id="9258d-140">Запустите командлет **New-ManagementRoleAssignment**, чтобы добавить разрешение на олицетворение пользователей, входящих в указанную область.</span><span class="sxs-lookup"><span data-stu-id="9258d-140">Run the **New-ManagementRoleAssignment** cmdlet to add the permission to impersonate the members of the specified scope.</span></span> <span data-ttu-id="9258d-141">В приведенном ниже примере показано, как настроить учетную запись службы так, чтобы она могла олицетворять всех пользователей в области.</span><span class="sxs-lookup"><span data-stu-id="9258d-141">The following example shows how to configure a service account to impersonate all users in a scope.</span></span> 
    
   ```powershell
    New-ManagementRoleAssignment -Name:impersonationAssignmentName -Role:ApplicationImpersonation -User:serviceAccount -CustomRecipientWriteScope:scopeName
    
   ```


<span data-ttu-id="9258d-142">Когда администратор предоставит разрешения на олицетворение, с помощью учетной записи службы можно будет вызывать учетные записи других пользователей.</span><span class="sxs-lookup"><span data-stu-id="9258d-142">After your administrator grants impersonation permissions, you can use the service account to make calls against other users' accounts.</span></span> <span data-ttu-id="9258d-143">Используйте командлет [Get-ManagementRoleAssignment](https://msdn.microsoft.com/library/a3a6ee46-061b-444a-8639-43a416309445.aspx), чтобы проверить назначения ролей.</span><span class="sxs-lookup"><span data-stu-id="9258d-143">You can verify role assignments by using the [Get-ManagementRoleAssignment](https://msdn.microsoft.com/library/a3a6ee46-061b-444a-8639-43a416309445.aspx) cmdlet.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="9258d-144">См. также</span><span class="sxs-lookup"><span data-stu-id="9258d-144">See also</span></span>

- [<span data-ttu-id="9258d-145">Олицетворение и EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="9258d-145">Impersonation and EWS in Exchange</span></span>](impersonation-and-ews-in-exchange.md)
- [<span data-ttu-id="9258d-146">Роль ApplicationImpersonation</span><span class="sxs-lookup"><span data-stu-id="9258d-146">ApplicationImpersonation role</span></span>](https://technet.microsoft.com/library/dd776119%28v=exchg.150%29.aspx)   
- [<span data-ttu-id="9258d-147">New-ManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="9258d-147">New-ManagementRoleAssignment</span></span>](https://msdn.microsoft.com/library/34d4f2e3-f2c5-49e1-a6a9-1366da65a78c.aspx)    
- [<span data-ttu-id="9258d-148">Get-ManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="9258d-148">Get-ManagementRoleAssignment</span></span>](https://msdn.microsoft.com/library/a3a6ee46-061b-444a-8639-43a416309445.aspx)
    

