---
title: Настройка олицетворения
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
localization_priority: Normal
ms.assetid: efcef39f-e26d-4eed-95ac-36a5bf8c089f
description: 'Сведения о предоставлении роли олицетворения учетной записи службы с помощью командной консоли Exchange. '
ms.openlocfilehash: 57ccef48a7553bcc06e3b3ae940b376b8555ef84
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760991"
---
# <a name="configure-impersonation"></a><span data-ttu-id="39f5c-103">Настройка олицетворения</span><span class="sxs-lookup"><span data-stu-id="39f5c-103">Configure impersonation</span></span>

<span data-ttu-id="39f5c-104">Сведения о предоставлении роли олицетворения учетной записи службы с помощью командной консоли Exchange. </span><span class="sxs-lookup"><span data-stu-id="39f5c-104">Learn how to grant the impersonation role to a service account by using the Exchange Management Shell.</span></span> 
  
<span data-ttu-id="39f5c-105">Олицетворение позволяет вызывающего абонента, такие как приложения-службы, чтобы олицетворять учетную запись пользователя.</span><span class="sxs-lookup"><span data-stu-id="39f5c-105">Impersonation enables a caller, such as a service application, to impersonate a user account.</span></span> <span data-ttu-id="39f5c-106">Звонящий операции можно выполнить с помощью разрешений, которые связаны с олицетворенным учетной записи вместо разрешения, связанные с учетной записью вызывающего абонента.</span><span class="sxs-lookup"><span data-stu-id="39f5c-106">The caller can perform operations by using the permissions that are associated with the impersonated account instead of the permissions associated with the caller's account.</span></span>
  
<span data-ttu-id="39f5c-107">Exchange Online, Exchange Online как часть Office 365 и версии Exchange, начиная с Exchange 2013 использование управления доступом на основе ролей (RBAC) для назначения разрешений учетным записям.</span><span class="sxs-lookup"><span data-stu-id="39f5c-107">Exchange Online, Exchange Online as part of Office 365, and versions of Exchange starting with Exchange 2013 use role-based access control (RBAC) to assign permissions to accounts.</span></span> <span data-ttu-id="39f5c-108">Администратор сервера Exchange, необходимо предоставить роль **ApplicationImpersonation** любой учетной записи службы, которая будет олицетворения другим пользователям с помощью командлета [New-ManagementRoleAssignment](http://msdn.microsoft.com/library/34d4f2e3-f2c5-49e1-a6a9-1366da65a78c.aspx) .</span><span class="sxs-lookup"><span data-stu-id="39f5c-108">Your Exchange server administrator will need to grant any service account that will be impersonating other users the **ApplicationImpersonation** role by using the [New-ManagementRoleAssignment](http://msdn.microsoft.com/library/34d4f2e3-f2c5-49e1-a6a9-1366da65a78c.aspx) cmdlet.</span></span> 
  
## <a name="configuring-the-applicationimpersonation-role"></a><span data-ttu-id="39f5c-109">Настройка роли ApplicationImpersonation</span><span class="sxs-lookup"><span data-stu-id="39f5c-109">Configuring the ApplicationImpersonation role</span></span>

<span data-ttu-id="39f5c-110">Когда пользователь или администратор сервера обменника присваивает роль **ApplicationImpersonation** , используйте следующие параметры командлета **New-ManagementRoleAssignment** :</span><span class="sxs-lookup"><span data-stu-id="39f5c-110">When you or your Exchanger server administrator assigns the **ApplicationImpersonation** role, use the following parameters of the **New-ManagementRoleAssignment** cmdlet:</span></span> 
  
-  <span data-ttu-id="39f5c-111">_Имя_ &ndash; Понятное имя назначения роли.</span><span class="sxs-lookup"><span data-stu-id="39f5c-111">_Name_ &ndash; The friendly name of the role assignment.</span></span> <span data-ttu-id="39f5c-112">Каждый раз, когда нужно назначить роль, записываются в списке роли RBAC.</span><span class="sxs-lookup"><span data-stu-id="39f5c-112">Each time that you assign a role, an entry is made in the RBAC roles list.</span></span> <span data-ttu-id="39f5c-113">Вы можете проверить назначения ролей с помощью командлета [Get-ManagementRoleAssignment](http://msdn.microsoft.com/library/a3a6ee46-061b-444a-8639-43a416309445.aspx) .</span><span class="sxs-lookup"><span data-stu-id="39f5c-113">You can verify role assignments by using the [Get-ManagementRoleAssignment](http://msdn.microsoft.com/library/a3a6ee46-061b-444a-8639-43a416309445.aspx) cmdlet.</span></span> 
    
-  <span data-ttu-id="39f5c-114">_Роль_ &ndash; Роль RBAC для назначения.</span><span class="sxs-lookup"><span data-stu-id="39f5c-114">_Role_ &ndash; The RBAC role to assign.</span></span> <span data-ttu-id="39f5c-115">При настройке олицетворения нужно назначить роль **ApplicationImpersonation** .</span><span class="sxs-lookup"><span data-stu-id="39f5c-115">When you set up impersonation, you assign the **ApplicationImpersonation** role.</span></span> 
    
-  <span data-ttu-id="39f5c-116">_Пользователь_ &ndash; Учетной записи службы.</span><span class="sxs-lookup"><span data-stu-id="39f5c-116">_User_ &ndash; The service account.</span></span> 
    
-  <span data-ttu-id="39f5c-117">_CustomRecipientScope_ &ndash; Область пользователей, которые могут олицетворять учетную запись службы.</span><span class="sxs-lookup"><span data-stu-id="39f5c-117">_CustomRecipientScope_ &ndash; The scope of users that the service account can impersonate.</span></span> <span data-ttu-id="39f5c-118">Учетная запись службы будет разрешено только для олицетворения другим пользователям в пределах указанной области.</span><span class="sxs-lookup"><span data-stu-id="39f5c-118">The service account will only be allowed to impersonate other users within the specified scope.</span></span> <span data-ttu-id="39f5c-119">Если диапазон не указан, учетную запись службы предоставляется роль **ApplicationImpersonation** по всем пользователям в организации.</span><span class="sxs-lookup"><span data-stu-id="39f5c-119">If no scope is specified, the service account is granted the **ApplicationImpersonation** role over all users in an organization.</span></span> <span data-ttu-id="39f5c-120">Можно создавать настраиваемые области управления с помощью командлета [New-ManagementScope](http://msdn.microsoft.com/library/1ea1f474-69d6-48c0-9beb-bfa4442c5dab.aspx) .</span><span class="sxs-lookup"><span data-stu-id="39f5c-120">You can create custom management scopes by using the [New-ManagementScope](http://msdn.microsoft.com/library/1ea1f474-69d6-48c0-9beb-bfa4442c5dab.aspx) cmdlet.</span></span> 
    
<span data-ttu-id="39f5c-121">Перед настройкой олицетворения вам понадобятся:</span><span class="sxs-lookup"><span data-stu-id="39f5c-121">Before you can configure impersonation, you need:</span></span>
  
- <span data-ttu-id="39f5c-122">Учетные данные администратора для сервера Exchange Server.</span><span class="sxs-lookup"><span data-stu-id="39f5c-122">Administrative credentials for the Exchange server.</span></span>
    
- <span data-ttu-id="39f5c-123">Учетные данные администратора домена или другие учетные данные с разрешением на создание и назначение ролей и областей.</span><span class="sxs-lookup"><span data-stu-id="39f5c-123">Domain Administrator credentials, or other credentials with the permission to create and assign roles and scopes.</span></span>
    
- <span data-ttu-id="39f5c-p106">Средства управления Exchange. Их нужно установить на компьютере, с которого будут выполняться команды.</span><span class="sxs-lookup"><span data-stu-id="39f5c-p106">Exchange management tools. These are installed on the computer from which you will run the commands.</span></span>
    
### <a name="to-configure-impersonation-for-all-users-in-an-organization"></a><span data-ttu-id="39f5c-126">Настройка олицетворения для всех пользователей в организации</span><span class="sxs-lookup"><span data-stu-id="39f5c-126">To configure impersonation for all users in an organization</span></span>

1. <span data-ttu-id="39f5c-127">Откройте консоль управления Exchange.</span><span class="sxs-lookup"><span data-stu-id="39f5c-127">Open the Exchange Management Shell.</span></span> <span data-ttu-id="39f5c-128">В меню Пуск выберите **Все программы** > **Microsoft Exchange Server 2013**.</span><span class="sxs-lookup"><span data-stu-id="39f5c-128">From the Start menu, choose **All Programs** > **Microsoft Exchange Server 2013**.</span></span> 
    
2. <span data-ttu-id="39f5c-129">Выполните командлет **New-ManagementRoleAssignment** , чтобы добавить разрешение олицетворения для указанного пользователя.</span><span class="sxs-lookup"><span data-stu-id="39f5c-129">Run the **New-ManagementRoleAssignment** cmdlet to add the impersonation permission to the specified user.</span></span> <span data-ttu-id="39f5c-130">Приведенный ниже показано, как настроить олицетворения для включения учетной записи службы для олицетворения всех пользователей в организации.</span><span class="sxs-lookup"><span data-stu-id="39f5c-130">The following example shows how to configure impersonation to enable a service account to impersonate all other users in an organization.</span></span> 
    
   ```powershell
   New-ManagementRoleAssignment -name:impersonationAssignmentName -Role:ApplicationImpersonation -User:serviceAccount 
   ```

### <a name="to-configure-impersonation-for-specific-users-or-groups-of-users"></a><span data-ttu-id="39f5c-131">Настройка олицетворения для определенных пользователей или групп пользователей</span><span class="sxs-lookup"><span data-stu-id="39f5c-131">To configure impersonation for specific users or groups of users</span></span>

1. <span data-ttu-id="39f5c-132">Откройте консоль управления Exchange.</span><span class="sxs-lookup"><span data-stu-id="39f5c-132">Open the Exchange Management Shell.</span></span> <span data-ttu-id="39f5c-133">В меню Пуск выберите **Все программы** > **Microsoft Exchange Server 2013**.</span><span class="sxs-lookup"><span data-stu-id="39f5c-133">From the Start menu, choose **All Programs** > **Microsoft Exchange Server 2013**.</span></span> 
    
2. <span data-ttu-id="39f5c-134">Выполните командлет **New-ManagementScope** , чтобы создать область, к которому можно назначить роль олицетворения.</span><span class="sxs-lookup"><span data-stu-id="39f5c-134">Run the **New-ManagementScope** cmdlet to create a scope to which the impersonation role can be assigned.</span></span> <span data-ttu-id="39f5c-135">Если существующей области, этот шаг можно пропустить.</span><span class="sxs-lookup"><span data-stu-id="39f5c-135">If an existing scope is available, you can skip this step.</span></span> <span data-ttu-id="39f5c-136">Приведенный ниже показано, как создавать области управления для конкретной группы.</span><span class="sxs-lookup"><span data-stu-id="39f5c-136">The following example shows how to create a management scope for a specific group.</span></span> 
    
   ```powershell
    New-ManagementScope -Name:scopeName -RecipientRestrictionFilter:recipientFilter
   ```

   <span data-ttu-id="39f5c-137">Параметр _RecipientRestrictionFilter_ командлет **New-ManagementScope** определяет элементы из области действия.</span><span class="sxs-lookup"><span data-stu-id="39f5c-137">The _RecipientRestrictionFilter_ parameter of the **New-ManagementScope** cmdlet defines the members of the scope.</span></span> <span data-ttu-id="39f5c-138">Можно использовать свойства объекта **удостоверения** для создания фильтра.</span><span class="sxs-lookup"><span data-stu-id="39f5c-138">You can use the properties of the **Identity** object to create the filter.</span></span> <span data-ttu-id="39f5c-139">В следующем примере представлен фильтр, который ограничивает результатов отдельному пользователю с именем пользователя «john.»</span><span class="sxs-lookup"><span data-stu-id="39f5c-139">The following example is a filter that restricts the result to a single user with the user name "john."</span></span> 
    
   ```powershell
   Name -eq "john"
   ```

3. <span data-ttu-id="39f5c-140">Выполните командлет **New-ManagementRoleAssignment** , чтобы добавить разрешением для олицетворения члены указанной области.</span><span class="sxs-lookup"><span data-stu-id="39f5c-140">Run the **New-ManagementRoleAssignment** cmdlet to add the permission to impersonate the members of the specified scope.</span></span> <span data-ttu-id="39f5c-141">Приведенный ниже показано, как настроить учетную запись службы для олицетворения всех пользователей в области.</span><span class="sxs-lookup"><span data-stu-id="39f5c-141">The following example shows how to configure a service account to impersonate all users in a scope.</span></span> 
    
   ```powershell
    New-ManagementRoleAssignment -Name:impersonationAssignmentName -Role:ApplicationImpersonation -User:serviceAccount -CustomRecipientWriteScope:scopeName
    
   ```


<span data-ttu-id="39f5c-142">После администратор предоставляет разрешений на олицетворение, можно использовать учетную запись службы для совершать звонки от учетные записи других пользователей.</span><span class="sxs-lookup"><span data-stu-id="39f5c-142">After your administrator grants impersonation permissions, you can use the service account to make calls against other users' accounts.</span></span> <span data-ttu-id="39f5c-143">Вы можете проверить назначения ролей с помощью командлета [Get-ManagementRoleAssignment](http://msdn.microsoft.com/library/a3a6ee46-061b-444a-8639-43a416309445.aspx) .</span><span class="sxs-lookup"><span data-stu-id="39f5c-143">You can verify role assignments by using the [Get-ManagementRoleAssignment](http://msdn.microsoft.com/library/a3a6ee46-061b-444a-8639-43a416309445.aspx) cmdlet.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="39f5c-144">См. также</span><span class="sxs-lookup"><span data-stu-id="39f5c-144">See also</span></span>

- [<span data-ttu-id="39f5c-145">Олицетворение и EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="39f5c-145">Impersonation and EWS in Exchange</span></span>](impersonation-and-ews-in-exchange.md)
- [<span data-ttu-id="39f5c-146">Роль ApplicationImpersonation</span><span class="sxs-lookup"><span data-stu-id="39f5c-146">ApplicationImpersonation role</span></span>](http://technet.microsoft.com/en-us/library/dd776119%28v=exchg.150%29.aspx)   
- [<span data-ttu-id="39f5c-147">New-ManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="39f5c-147">New-ManagementRoleAssignment</span></span>](http://msdn.microsoft.com/library/34d4f2e3-f2c5-49e1-a6a9-1366da65a78c.aspx)    
- [<span data-ttu-id="39f5c-148">Get-ManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="39f5c-148">Get-ManagementRoleAssignment</span></span>](http://msdn.microsoft.com/library/a3a6ee46-061b-444a-8639-43a416309445.aspx)
    

