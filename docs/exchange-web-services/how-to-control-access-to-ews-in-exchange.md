---
title: Контроль доступа к EWS в Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 61e29e54-e3e5-404a-84c0-93b61a25ca58
description: Узнайте, как управлять доступом к EWS для пользователей, приложений или всей Организации.
ms.openlocfilehash: 956c28faba105ecf2a6b1452abe629ea2fc930e1
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760986"
---
# <a name="control-access-to-ews-in-exchange"></a><span data-ttu-id="070d4-103">Контроль доступа к EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="070d4-103">Control access to EWS in Exchange</span></span>

<span data-ttu-id="070d4-104">Узнайте, как управлять доступом к EWS для пользователей, приложений или всей Организации.</span><span class="sxs-lookup"><span data-stu-id="070d4-104">Find out how to control access to EWS for users, applications, or the entire organization.</span></span>
  
<span data-ttu-id="070d4-105">Независимо от того, используется ли управляемый API EWS или веб-сайт EWS напрямую, вы можете управлять доступом к веб-службам Exchange (EWS).</span><span class="sxs-lookup"><span data-stu-id="070d4-105">Whether you are using the EWS Managed API, or EWS directly, in your application, you can control access to Exchange Web Services (EWS).</span></span> <span data-ttu-id="070d4-106">Если вы обладаете правами администратора на доступ к серверу Exchange Server, вы можете управлять доступом к EWS, используя командную консоль Exchange для глобального управления доступом, для каждого пользователя и для каждого приложения.</span><span class="sxs-lookup"><span data-stu-id="070d4-106">If you have administrator access to your Exchange server, you can manage access to EWS by using the Exchange Management Shell to control access globally, for each user, and for each application.</span></span>
  
## <a name="exchange-management-shell-cmdlets-for-configuring-access-control"></a><span data-ttu-id="070d4-107">Командлеты командной консоли Exchange для настройки управления доступом</span><span class="sxs-lookup"><span data-stu-id="070d4-107">Exchange Management Shell cmdlets for configuring access control</span></span>
<span data-ttu-id="070d4-108"><a name="bk_Cmdlets"> </a></span><span class="sxs-lookup"><span data-stu-id="070d4-108"><a name="bk_Cmdlets"> </a></span></span>

<span data-ttu-id="070d4-109">Вы можете использовать следующие командлеты командной консоли Exchange для просмотра текущей конфигурации доступа и задания средств контроля доступа EWS:</span><span class="sxs-lookup"><span data-stu-id="070d4-109">You can use the following Exchange Management Shell cmdlets to view the current access configuration and set EWS access controls:</span></span>
  
- <span data-ttu-id="070d4-110">[Get – CASMailbox](http://technet.microsoft.com/en-us/library/bb124754.aspx) — показывает, какие параметры задаются для определенного почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="070d4-110">[Get-CASMailbox](http://technet.microsoft.com/en-us/library/bb124754.aspx) - Shows you what parameters are set for a particular mailbox.</span></span>   
- <span data-ttu-id="070d4-111">[Set – CASMailbox](http://technet.microsoft.com/en-us/library/bb125264.aspx) — задает параметры для определенного почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="070d4-111">[Set-CASMailbox](http://technet.microsoft.com/en-us/library/bb125264.aspx) - Sets parameters for a particular mailbox.</span></span>    
- <span data-ttu-id="070d4-112">[Get – OrganizationConfig](http://technet.microsoft.com/en-us/library/aa997571.aspx) — показывает параметры для всей Организации.</span><span class="sxs-lookup"><span data-stu-id="070d4-112">[Get-OrganizationConfig](http://technet.microsoft.com/en-us/library/aa997571.aspx) - Shows you the parameters for the entire organization.</span></span>    
- <span data-ttu-id="070d4-113">[Set – OrganizationConfig](http://technet.microsoft.com/en-us/library/aa997443.aspx) — задает параметры для всей Организации.</span><span class="sxs-lookup"><span data-stu-id="070d4-113">[Set-OrganizationConfig](http://technet.microsoft.com/en-us/library/aa997443.aspx) - Sets the parameters for the entire organization.</span></span> 

<span data-ttu-id="070d4-114"><a name="bk_Examples"> </a></span><span class="sxs-lookup"><span data-stu-id="070d4-114"><a name="bk_Examples"> </a></span></span>

## <a name="examples-controlling-access-to-ews"></a><span data-ttu-id="070d4-115">Примеры: Управление доступом к EWS</span><span class="sxs-lookup"><span data-stu-id="070d4-115">Examples: Controlling access to EWS</span></span>

<span data-ttu-id="070d4-116">Рассмотрим несколько сценариев, показывающих, как можно управлять доступом к приложению.</span><span class="sxs-lookup"><span data-stu-id="070d4-116">Let's take a look at a few scenarios that show you how you can control access to your application.</span></span>
  
<span data-ttu-id="070d4-117">**Таблица 1. Команды для управления доступом к EWS**</span><span class="sxs-lookup"><span data-stu-id="070d4-117">**Table 1. Commands for controlling access to EWS**</span></span>

|<span data-ttu-id="070d4-118">Задача</span><span class="sxs-lookup"><span data-stu-id="070d4-118">If you want to</span></span> |<span data-ttu-id="070d4-119">Используйте эту команду</span><span class="sxs-lookup"><span data-stu-id="070d4-119">Use this command</span></span>|
|:-----|:-----|
|<span data-ttu-id="070d4-120">Блокировать использование EWS всеми клиентскими приложениями.</span><span class="sxs-lookup"><span data-stu-id="070d4-120">Block all client applications from using EWS.</span></span> | `Set-OrganizationConfig -EwsApplicationAccessPolicy:EnforceAllowList`<br/><br/><span data-ttu-id="070d4-121">Это позволяет приложениям, перечисленным в Алловлист, подключаться.</span><span class="sxs-lookup"><span data-stu-id="070d4-121">This allows applications listed in the AllowList to connect.</span></span> <span data-ttu-id="070d4-122">В этом примере приложения не включены в Алловлист, поэтому приложения не могут использовать EWS.</span><span class="sxs-lookup"><span data-stu-id="070d4-122">In this example, no applications are included in the AllowList, so no applications can use EWS.</span></span> |
|<span data-ttu-id="070d4-123">Разрешить списку клиентских приложений использовать EWS.</span><span class="sxs-lookup"><span data-stu-id="070d4-123">Allow a list of client applications to use EWS.</span></span> | `Set-OrganizationConfig -EwsApplicationAccessPolicy:EnforceAllowList -EwsAllowList:"OWA/*"`<br/><br/><span data-ttu-id="070d4-124">Это позволяет определенным приложениям использовать EWS.</span><span class="sxs-lookup"><span data-stu-id="070d4-124">This allows specific applications to use EWS.</span></span> <span data-ttu-id="070d4-125">В этом примере доступ к приложению, имеющему строку агента пользователя, начинающуюся с "OWA/", разрешено.</span><span class="sxs-lookup"><span data-stu-id="070d4-125">In this example, any application that has a user agent string that starts with "OWA/" is allowed access.</span></span> |
|<span data-ttu-id="070d4-126">Разрешите всем клиентским приложениям использовать EWS, кроме специально заблокированных.</span><span class="sxs-lookup"><span data-stu-id="070d4-126">Allow all client applications to use EWS except those that are specifically blocked.</span></span> | `Set-OrganizationConfig -EwsApplicationAccessPolicy:EnforceBlockList -EwsBlockList:"OWA/*"`<br/> <br/><span data-ttu-id="070d4-127">В этом примере приложения не могут использовать веб-служб EWS, у которых есть строка агента пользователя, начинающаяся с "OWA/".</span><span class="sxs-lookup"><span data-stu-id="070d4-127">This example only blocks applications from using EWS that have a user agent string that starts with "OWA/".</span></span> |
|<span data-ttu-id="070d4-128">Разрешите всем клиентским приложениям использовать EWS.</span><span class="sxs-lookup"><span data-stu-id="070d4-128">Allow all client applications to use EWS.</span></span> | `Set-OrganizationConfig -EwsApplicationAccessPolicy:EnforceBlockList` <br/><br/> <span data-ttu-id="070d4-129">Так как Блокклист не указан, все приложения могут использовать EWS.</span><span class="sxs-lookup"><span data-stu-id="070d4-129">Because no BlockList is specified, all applications can use EWS.</span></span> |
|<span data-ttu-id="070d4-130">Блокировать использование EWS всей Организацией.</span><span class="sxs-lookup"><span data-stu-id="070d4-130">Block the entire organization from using EWS.</span></span> | `Set-OrganizationConfig -EwsEnabled:$false` |
|<span data-ttu-id="070d4-131">Разрешите всей Организации использовать EWS.</span><span class="sxs-lookup"><span data-stu-id="070d4-131">Allow the entire organization to use EWS.</span></span> | `Set-OrganizationConfig -EwsEnabled:$true`|
|<span data-ttu-id="070d4-132">Блокировка отдельного почтового ящика с помощью EWS.</span><span class="sxs-lookup"><span data-stu-id="070d4-132">Block an individual mailbox from using EWS.</span></span> | `Set-CASMailbox -Identity adam@contoso.com -EwsEnabled:$false`|
|<span data-ttu-id="070d4-133">Разрешить отдельному почтовому ящику использовать EWS.</span><span class="sxs-lookup"><span data-stu-id="070d4-133">Allow an individual mailbox to use EWS.</span></span> | `Set-CASMailbox -Identity adam@contoso.com -EwsEnabled:$true`|
   
## <a name="see-also"></a><span data-ttu-id="070d4-134">См. также</span><span class="sxs-lookup"><span data-stu-id="070d4-134">See also</span></span>

- [<span data-ttu-id="070d4-135">Настройка приложения веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="070d4-135">Setting up your EWS application</span></span>](setting-up-your-ews-application.md)    
- [<span data-ttu-id="070d4-136">Управление доступом клиентских приложений к EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="070d4-136">Controlling client application access to EWS in Exchange</span></span>](controlling-client-application-access-to-ews-in-exchange.md)   
- [<span data-ttu-id="070d4-137">PowerShell в Exchange Server (Командная консоль Exchange)</span><span class="sxs-lookup"><span data-stu-id="070d4-137">Exchange Server PowerShell (Exchange Management Shell)</span></span>](https://docs.microsoft.com/en-us/powershell/exchange/exchange-server/exchange-management-shell?view=exchange-ps) 
- [<span data-ttu-id="070d4-138">Windows PowerShell</span><span class="sxs-lookup"><span data-stu-id="070d4-138">Windows PowerShell</span></span>](http://msdn.microsoft.com/en-us/library/dd835506%28v=vs.85%29.aspx)
    

