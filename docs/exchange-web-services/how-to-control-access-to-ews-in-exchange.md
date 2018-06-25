---
title: Управление доступом к веб-служб Exchange в Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 61e29e54-e3e5-404a-84c0-93b61a25ca58
description: Узнайте, как для управления доступом к веб-служб Exchange для пользователей, приложений или во всей организации.
ms.openlocfilehash: 956c28faba105ecf2a6b1452abe629ea2fc930e1
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760986"
---
# <a name="control-access-to-ews-in-exchange"></a><span data-ttu-id="5faf8-103">Управление доступом к веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="5faf8-103">Control access to EWS in Exchange</span></span>

<span data-ttu-id="5faf8-104">Узнайте, как для управления доступом к веб-служб Exchange для пользователей, приложений или во всей организации.</span><span class="sxs-lookup"><span data-stu-id="5faf8-104">Find out how to control access to EWS for users, applications, or the entire organization.</span></span>
  
<span data-ttu-id="5faf8-105">Используется ли управляемый API EWS или веб-служб Exchange напрямую, в приложении, можно управлять доступом для веб-служб Exchange (EWS).</span><span class="sxs-lookup"><span data-stu-id="5faf8-105">Whether you are using the EWS Managed API, or EWS directly, in your application, you can control access to Exchange Web Services (EWS).</span></span> <span data-ttu-id="5faf8-106">Если имеется доступ с правами администратора на сервере Exchange, доступ к веб-служб Exchange можно управлять с помощью командной консоли Exchange для управления доступом к глобально, для каждого пользователя и для каждого приложения.</span><span class="sxs-lookup"><span data-stu-id="5faf8-106">If you have administrator access to your Exchange server, you can manage access to EWS by using the Exchange Management Shell to control access globally, for each user, and for each application.</span></span>
  
## <a name="exchange-management-shell-cmdlets-for-configuring-access-control"></a><span data-ttu-id="5faf8-107">Командлеты командной консоли Exchange для настройки управления доступом</span><span class="sxs-lookup"><span data-stu-id="5faf8-107">Exchange Management Shell cmdlets for configuring access control</span></span>
<span data-ttu-id="5faf8-108"><a name="bk_Cmdlets"> </a></span><span class="sxs-lookup"><span data-stu-id="5faf8-108"></span></span>

<span data-ttu-id="5faf8-109">Можно использовать следующие командлеты командной консоли Exchange для просмотра текущих настроек доступа и задания элементов управления доступа к веб-служб Exchange:</span><span class="sxs-lookup"><span data-stu-id="5faf8-109">You can use the following Exchange Management Shell cmdlets to view the current access configuration and set EWS access controls:</span></span>
  
- <span data-ttu-id="5faf8-110">[Get-CASMailbox](http://technet.microsoft.com/en-us/library/bb124754.aspx) - показано, какие параметры настраиваются для определенного почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="5faf8-110">[Get-CASMailbox](http://technet.microsoft.com/en-us/library/bb124754.aspx) - Shows you what parameters are set for a particular mailbox.</span></span>   
- <span data-ttu-id="5faf8-111">[Set-CASMailbox](http://technet.microsoft.com/en-us/library/bb125264.aspx) - наборов параметров для определенного почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="5faf8-111">[Set-CASMailbox](http://technet.microsoft.com/en-us/library/bb125264.aspx) - Sets parameters for a particular mailbox.</span></span>    
- <span data-ttu-id="5faf8-112">[Get-OrganizationConfig](http://technet.microsoft.com/en-us/library/aa997571.aspx) - указываются параметры для всей организации.</span><span class="sxs-lookup"><span data-stu-id="5faf8-112">[Get-OrganizationConfig](http://technet.microsoft.com/en-us/library/aa997571.aspx) - Shows you the parameters for the entire organization.</span></span>    
- <span data-ttu-id="5faf8-113">[Set-OrganizationConfig](http://technet.microsoft.com/en-us/library/aa997443.aspx) - задает параметры для всей организации.</span><span class="sxs-lookup"><span data-stu-id="5faf8-113">[Set-OrganizationConfig](http://technet.microsoft.com/en-us/library/aa997443.aspx) - Sets the parameters for the entire organization.</span></span> 

<span data-ttu-id="5faf8-114"><a name="bk_Examples"> </a></span><span class="sxs-lookup"><span data-stu-id="5faf8-114"></span></span>

## <a name="examples-controlling-access-to-ews"></a><span data-ttu-id="5faf8-115">Примеры: Управление доступом к веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="5faf8-115">Examples: Controlling access to EWS</span></span>

<span data-ttu-id="5faf8-116">Давайте рассмотрим несколько сценариев, которые показывают, как контролировать доступ к приложению.</span><span class="sxs-lookup"><span data-stu-id="5faf8-116">Let's take a look at a few scenarios that show you how you can control access to your application.</span></span>
  
<span data-ttu-id="5faf8-117">**В таблице 1. Команды для управления доступом к веб-служб Exchange**</span><span class="sxs-lookup"><span data-stu-id="5faf8-117">**Table 1. Commands for controlling access to EWS**</span></span>

|<span data-ttu-id="5faf8-118">Назначение</span><span class="sxs-lookup"><span data-stu-id="5faf8-118">If you want to</span></span> |<span data-ttu-id="5faf8-119">Используйте следующую команду</span><span class="sxs-lookup"><span data-stu-id="5faf8-119">Use this command</span></span>|
|:-----|:-----|
|<span data-ttu-id="5faf8-120">Блокировать все клиентские приложения с помощью веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="5faf8-120">Block all client applications from using EWS.</span></span> | `Set-OrganizationConfig -EwsApplicationAccessPolicy:EnforceAllowList`<br/><br/><span data-ttu-id="5faf8-121">Это позволяет приложений, перечисленных в AllowList для подключения.</span><span class="sxs-lookup"><span data-stu-id="5faf8-121">This allows applications listed in the AllowList to connect.</span></span> <span data-ttu-id="5faf8-122">В этом примере приложения не включены в AllowList, поэтому приложения не могут использовать веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="5faf8-122">In this example, no applications are included in the AllowList, so no applications can use EWS.</span></span> |
|<span data-ttu-id="5faf8-123">Разрешить список клиентских приложений для использования веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="5faf8-123">Allow a list of client applications to use EWS.</span></span> | `Set-OrganizationConfig -EwsApplicationAccessPolicy:EnforceAllowList -EwsAllowList:"OWA/*"`<br/><br/><span data-ttu-id="5faf8-124">Это позволяет определенные приложения для использования веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="5faf8-124">This allows specific applications to use EWS.</span></span> <span data-ttu-id="5faf8-125">В этом примере любого приложения, которое имеет строка агента пользователя начинается с «OWA /» разрешения на доступ.</span><span class="sxs-lookup"><span data-stu-id="5faf8-125">In this example, any application that has a user agent string that starts with "OWA/" is allowed access.</span></span> |
|<span data-ttu-id="5faf8-126">Разрешить все клиентские приложения для использования веб-служб Exchange, за исключением тех, которые были заблокированы.</span><span class="sxs-lookup"><span data-stu-id="5faf8-126">Allow all client applications to use EWS except those that are specifically blocked.</span></span> | `Set-OrganizationConfig -EwsApplicationAccessPolicy:EnforceBlockList -EwsBlockList:"OWA/*"`<br/> <br/><span data-ttu-id="5faf8-127">В этом примере блокирует только приложений с помощью веб-служб Exchange, для которого строка агента пользователя, который начинается с «OWA /».</span><span class="sxs-lookup"><span data-stu-id="5faf8-127">This example only blocks applications from using EWS that have a user agent string that starts with "OWA/".</span></span> |
|<span data-ttu-id="5faf8-128">Разрешить все клиентские приложения для использования веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="5faf8-128">Allow all client applications to use EWS.</span></span> | `Set-OrganizationConfig -EwsApplicationAccessPolicy:EnforceBlockList` <br/><br/> <span data-ttu-id="5faf8-129">Так как нет блокировки не указан, то все приложения могут использовать веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="5faf8-129">Because no BlockList is specified, all applications can use EWS.</span></span> |
|<span data-ttu-id="5faf8-130">Блокировка во всей организации с помощью веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="5faf8-130">Block the entire organization from using EWS.</span></span> | `Set-OrganizationConfig -EwsEnabled:$false` |
|<span data-ttu-id="5faf8-131">Разрешить во всей организации, для использования веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="5faf8-131">Allow the entire organization to use EWS.</span></span> | `Set-OrganizationConfig -EwsEnabled:$true`|
|<span data-ttu-id="5faf8-132">Блокировка отдельных почтовых ящиков с помощью веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="5faf8-132">Block an individual mailbox from using EWS.</span></span> | `Set-CASMailbox -Identity adam@contoso.com -EwsEnabled:$false`|
|<span data-ttu-id="5faf8-133">Разрешить отдельным почтовым ящикам для использования веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="5faf8-133">Allow an individual mailbox to use EWS.</span></span> | `Set-CASMailbox -Identity adam@contoso.com -EwsEnabled:$true`|
   
## <a name="see-also"></a><span data-ttu-id="5faf8-134">См. также</span><span class="sxs-lookup"><span data-stu-id="5faf8-134">See also</span></span>

- [<span data-ttu-id="5faf8-135">Настройка приложения веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="5faf8-135">Setting up your EWS application</span></span>](setting-up-your-ews-application.md)    
- [<span data-ttu-id="5faf8-136">Управление доступом к клиентского приложения для веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="5faf8-136">Controlling client application access to EWS in Exchange</span></span>](controlling-client-application-access-to-ews-in-exchange.md)   
- [<span data-ttu-id="5faf8-137">Exchange Server PowerShell (Командная консоль Exchange)</span><span class="sxs-lookup"><span data-stu-id="5faf8-137">Exchange Server PowerShell (Exchange Management Shell)</span></span>](https://docs.microsoft.com/en-us/powershell/exchange/exchange-server/exchange-management-shell?view=exchange-ps) 
- [<span data-ttu-id="5faf8-138">Windows PowerShell</span><span class="sxs-lookup"><span data-stu-id="5faf8-138">Windows PowerShell</span></span>](http://msdn.microsoft.com/en-us/library/dd835506%28v=vs.85%29.aspx)
    

