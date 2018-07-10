---
title: Новые и обновленные командлеты командной консоли Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 5941a439-94d2-4133-81fc-7240863a13df
description: Найдите сведения о новых возможностях в командной консоли Exchange в Exchange.
ms.openlocfilehash: 906e078ab6d500a2cb3d364957ffc2fee67a06b4
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761298"
---
# <a name="new-and-updated-exchange-management-shell-cmdlets"></a><span data-ttu-id="63558-103">Новые и обновленные командлеты командной консоли Exchange</span><span class="sxs-lookup"><span data-stu-id="63558-103">New and updated Exchange Management Shell cmdlets</span></span>

<span data-ttu-id="63558-104">Найдите сведения о новых возможностях в командной консоли Exchange в Exchange.</span><span class="sxs-lookup"><span data-stu-id="63558-104">Find information about what's new in the Exchange Management Shell in Exchange.</span></span>
  
<span data-ttu-id="63558-105">**Применимо к:** Exchange Online | Exchange Server 2013 | Office 365</span><span class="sxs-lookup"><span data-stu-id="63558-105">**Applies to:** Exchange Online | Exchange Server 2013 | Office 365</span></span>
  
<span data-ttu-id="63558-106">В этой статье сведения о новых командлетов командной консоли управления Exchange, командлеты, которые были изменены за и командлеты, которые были удалены из Exchange Online, Exchange Online в составе Office 365 или локальной версией Exchange.</span><span class="sxs-lookup"><span data-stu-id="63558-106">This article provides information about new Exchange Management shell cmdlets, cmdlets that were modified in, and cmdlets that were removed from Exchange Online, Exchange Online as part of Office 365, or an on-premises version of Exchange.</span></span>
  
## <a name="new-and-updated-cmdlets-in-exchange-2013-sp1"></a><span data-ttu-id="63558-107">Новые и обновленные командлеты в Exchange 2013 с пакетом обновления 1</span><span class="sxs-lookup"><span data-stu-id="63558-107">New and updated cmdlets in Exchange 2013 SP1</span></span>

### <a name="new-cmdlets"></a><span data-ttu-id="63558-108">Новые командлеты</span><span class="sxs-lookup"><span data-stu-id="63558-108">New cmdlets</span></span>

<span data-ttu-id="63558-109">Следующие командлеты были представлены в построении 15.00.0847.032 (Exchange Server 2013 с пакетом обновления 1):</span><span class="sxs-lookup"><span data-stu-id="63558-109">The following cmdlets were introduced in build 15.00.0847.032 (Exchange Server 2013 SP1):</span></span>
  
- <span data-ttu-id="63558-110">**Get-AuthRedirect**</span><span class="sxs-lookup"><span data-stu-id="63558-110">**Get-AuthRedirect**</span></span>
    
- <span data-ttu-id="63558-111">**Новый AuthRedirect**</span><span class="sxs-lookup"><span data-stu-id="63558-111">**New-AuthRedirect**</span></span>
    
- <span data-ttu-id="63558-112">**Remove-AuthRedirect**</span><span class="sxs-lookup"><span data-stu-id="63558-112">**Remove-AuthRedirect**</span></span>
    
- <span data-ttu-id="63558-113">**SET-AuthRedirect**</span><span class="sxs-lookup"><span data-stu-id="63558-113">**Set-AuthRedirect**</span></span>
    
- <span data-ttu-id="63558-114">**Новый DataClassification**</span><span class="sxs-lookup"><span data-stu-id="63558-114">**New-DataClassification**</span></span>
    
- <span data-ttu-id="63558-115">**Remove-DataClassification**</span><span class="sxs-lookup"><span data-stu-id="63558-115">**Remove-DataClassification**</span></span>
    
- <span data-ttu-id="63558-116">**SET-DataClassification**</span><span class="sxs-lookup"><span data-stu-id="63558-116">**Set-DataClassification**</span></span>
    
- <span data-ttu-id="63558-117">**Новый отпечаток**</span><span class="sxs-lookup"><span data-stu-id="63558-117">**New-FingerPrint**</span></span>
    
- <span data-ttu-id="63558-118">**Get-MapiVirtualDirectory\***</span><span class="sxs-lookup"><span data-stu-id="63558-118">**Get-MapiVirtualDirectory\***</span></span>
    
- <span data-ttu-id="63558-119">**Новый MapiVirtualDirectory\***</span><span class="sxs-lookup"><span data-stu-id="63558-119">**New-MapiVirtualDirectory\***</span></span>
    
- <span data-ttu-id="63558-120">**Remove-MapiVirtualDirectory\***</span><span class="sxs-lookup"><span data-stu-id="63558-120">**Remove-MapiVirtualDirectory\***</span></span>
    
- <span data-ttu-id="63558-121">**SET-MapiVirtualDirectory\***</span><span class="sxs-lookup"><span data-stu-id="63558-121">**Set-MapiVirtualDirectory\***</span></span>
    
- <span data-ttu-id="63558-122">**Get-OMEConfiguration**</span><span class="sxs-lookup"><span data-stu-id="63558-122">**Get-OMEConfiguration**</span></span>
    
- <span data-ttu-id="63558-123">**SET-OMEConfiguration**</span><span class="sxs-lookup"><span data-stu-id="63558-123">**Set-OMEConfiguration**</span></span>
    
- <span data-ttu-id="63558-124">**Get-SmimeConfig**</span><span class="sxs-lookup"><span data-stu-id="63558-124">**Get-SmimeConfig**</span></span>
    
- <span data-ttu-id="63558-125">**SET-SmimeConfig**</span><span class="sxs-lookup"><span data-stu-id="63558-125">**Set-SmimeConfig**</span></span>
    
- <span data-ttu-id="63558-126">**Get-IntraOrganizationConfiguration**</span><span class="sxs-lookup"><span data-stu-id="63558-126">**Get-IntraOrganizationConfiguration**</span></span>
    
- <span data-ttu-id="63558-127">**Get-IntraOrganizationConnector**</span><span class="sxs-lookup"><span data-stu-id="63558-127">**Get-IntraOrganizationConnector**</span></span>
    
- <span data-ttu-id="63558-128">**Новый IntraOrganizationConnector**</span><span class="sxs-lookup"><span data-stu-id="63558-128">**New-IntraOrganizationConnector**</span></span>
    
- <span data-ttu-id="63558-129">**Remove-IntraOrganizationConnector**</span><span class="sxs-lookup"><span data-stu-id="63558-129">**Remove-IntraOrganizationConnector**</span></span>
    
- <span data-ttu-id="63558-130">**SET-IntraOrganizationConnector**</span><span class="sxs-lookup"><span data-stu-id="63558-130">**Set-IntraOrganizationConnector**</span></span>
    
- <span data-ttu-id="63558-131">**Get-HistoricalSearch**</span><span class="sxs-lookup"><span data-stu-id="63558-131">**Get-HistoricalSearch**</span></span>
    
- <span data-ttu-id="63558-132">**Start-HistoricalSearch**</span><span class="sxs-lookup"><span data-stu-id="63558-132">**Start-HistoricalSearch**</span></span>
    
- <span data-ttu-id="63558-133">**STOP-HistoricalSearch**</span><span class="sxs-lookup"><span data-stu-id="63558-133">**Stop-HistoricalSearch**</span></span>
    
- <span data-ttu-id="63558-134">**Новый SearchDocumentFormat**</span><span class="sxs-lookup"><span data-stu-id="63558-134">**New-SearchDocumentFormat**</span></span>
    
- <span data-ttu-id="63558-135">**Remove-SearchDocumentFormat**</span><span class="sxs-lookup"><span data-stu-id="63558-135">**Remove-SearchDocumentFormat**</span></span>
    
### <a name="updated-cmdlets"></a><span data-ttu-id="63558-136">Обновленные командлеты</span><span class="sxs-lookup"><span data-stu-id="63558-136">Updated cmdlets</span></span>

<span data-ttu-id="63558-137">Следующие командлеты были обновлены в построении 15.00.0847.032 (Exchange 2013 с пакетом обновления 1):</span><span class="sxs-lookup"><span data-stu-id="63558-137">The following cmdlets were updated in build 15.00.0847.032 (Exchange 2013 SP1):</span></span>
  
- <span data-ttu-id="63558-138">**Get-AuditLogSearch**</span><span class="sxs-lookup"><span data-stu-id="63558-138">**Get-AuditLogSearch**</span></span>
    
- <span data-ttu-id="63558-139">**Get-QuarantineMessage**</span><span class="sxs-lookup"><span data-stu-id="63558-139">**Get-QuarantineMessage**</span></span>
    
- <span data-ttu-id="63558-140">**Новый InboundConnector**</span><span class="sxs-lookup"><span data-stu-id="63558-140">**New-InboundConnector**</span></span>
    
- <span data-ttu-id="63558-141">**Новый MailboxDatabase**</span><span class="sxs-lookup"><span data-stu-id="63558-141">**New-MailboxDatabase**</span></span>
    
- <span data-ttu-id="63558-142">**Новый PublicFolderMoveRequest**</span><span class="sxs-lookup"><span data-stu-id="63558-142">**New-PublicFolderMoveRequest**</span></span>
    
- <span data-ttu-id="63558-143">**New-TransportRule**</span><span class="sxs-lookup"><span data-stu-id="63558-143">**New-TransportRule**</span></span>
    
- <span data-ttu-id="63558-144">**SET-FrontendTransportService**</span><span class="sxs-lookup"><span data-stu-id="63558-144">**Set-FrontendTransportService**</span></span>
    
- <span data-ttu-id="63558-145">**SET-InboundConnector**</span><span class="sxs-lookup"><span data-stu-id="63558-145">**Set-InboundConnector**</span></span>
    
- <span data-ttu-id="63558-146">**Set-Mailbox**</span><span class="sxs-lookup"><span data-stu-id="63558-146">**Set-Mailbox**</span></span>
    
- <span data-ttu-id="63558-147">**SET-MailboxTransportService**</span><span class="sxs-lookup"><span data-stu-id="63558-147">**Set-MailboxTransportService**</span></span>
    
- <span data-ttu-id="63558-148">**SET-MoveRequest**</span><span class="sxs-lookup"><span data-stu-id="63558-148">**Set-MoveRequest**</span></span>
    
- <span data-ttu-id="63558-149">**SET-OrganizationConfig**</span><span class="sxs-lookup"><span data-stu-id="63558-149">**Set-OrganizationConfig**</span></span>
    
- <span data-ttu-id="63558-150">**SET-OwaMailboxPolicy**</span><span class="sxs-lookup"><span data-stu-id="63558-150">**Set-OwaMailboxPolicy**</span></span>
    
- <span data-ttu-id="63558-151">**SET-OwaVirtualDirectory**</span><span class="sxs-lookup"><span data-stu-id="63558-151">**Set-OwaVirtualDirectory**</span></span>
    
- <span data-ttu-id="63558-152">**Set-TransportConfig**</span><span class="sxs-lookup"><span data-stu-id="63558-152">**Set-TransportConfig**</span></span>
    
- <span data-ttu-id="63558-153">**SET-TransportRule**</span><span class="sxs-lookup"><span data-stu-id="63558-153">**Set-TransportRule**</span></span>
    
- <span data-ttu-id="63558-154">**SET-TransportServer**</span><span class="sxs-lookup"><span data-stu-id="63558-154">**Set-TransportServer**</span></span>
    
- <span data-ttu-id="63558-155">**SET-TransportService**</span><span class="sxs-lookup"><span data-stu-id="63558-155">**Set-TransportService**</span></span>
    
- <span data-ttu-id="63558-156">**Test-MRSHealth**</span><span class="sxs-lookup"><span data-stu-id="63558-156">**Test-MRSHealth**</span></span>
    
- <span data-ttu-id="63558-157">**Test-OAuthConnectivity**</span><span class="sxs-lookup"><span data-stu-id="63558-157">**Test-OAuthConnectivity**</span></span>
    
### <a name="removed-cmdlets"></a><span data-ttu-id="63558-158">Удаленные командлеты</span><span class="sxs-lookup"><span data-stu-id="63558-158">Removed cmdlets</span></span>

<span data-ttu-id="63558-159">Следующие командлеты были удалены из построения 15.00.0847.032 (Exchange 2013 с пакетом обновления 1):</span><span class="sxs-lookup"><span data-stu-id="63558-159">The following cmdlets were removed from build 15.00.0847.032 (Exchange 2013 SP1):</span></span>
  
- <span data-ttu-id="63558-160">**Get-AvailabilityReportOutage**</span><span class="sxs-lookup"><span data-stu-id="63558-160">**Get-AvailabilityReportOutage**</span></span>
    
- <span data-ttu-id="63558-161">**Новый AvailabilityReportOutage**</span><span class="sxs-lookup"><span data-stu-id="63558-161">**New-AvailabilityReportOutage**</span></span>
    
- <span data-ttu-id="63558-162">**Remove-AvailabilityReportOutage**</span><span class="sxs-lookup"><span data-stu-id="63558-162">**Remove-AvailabilityReportOutage**</span></span>
    
- <span data-ttu-id="63558-163">**SET-AvailabilityReportOutage**</span><span class="sxs-lookup"><span data-stu-id="63558-163">**Set-AvailabilityReportOutage**</span></span>
    
## <a name="new-and-updated-cmdlets-in-exchange-2013"></a><span data-ttu-id="63558-164">Новые и обновленные командлеты в Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="63558-164">New and updated cmdlets in Exchange 2013</span></span>

### <a name="new-cmdlets"></a><span data-ttu-id="63558-165">Новые командлеты</span><span class="sxs-lookup"><span data-stu-id="63558-165">New cmdlets</span></span>
<span data-ttu-id="63558-166"><a name="bk_new"> </a></span><span class="sxs-lookup"><span data-stu-id="63558-166"></span></span>

<span data-ttu-id="63558-167">В Exchange 2013 появились следующие командлеты:</span><span class="sxs-lookup"><span data-stu-id="63558-167">The following cmdlets were introduced in Exchange 2013:</span></span>
  
- <span data-ttu-id="63558-168">**Get-ActiveSyncDeviceAutoblockThreshold**</span><span class="sxs-lookup"><span data-stu-id="63558-168">**Get-ActiveSyncDeviceAutoblockThreshold**</span></span>
    
- <span data-ttu-id="63558-169">**SET-ActiveSyncDeviceAutoblockThreshold**</span><span class="sxs-lookup"><span data-stu-id="63558-169">**Set-ActiveSyncDeviceAutoblockThreshold**</span></span>
    
- <span data-ttu-id="63558-170">**Disable-App**</span><span class="sxs-lookup"><span data-stu-id="63558-170">**Disable-App**</span></span>
    
- <span data-ttu-id="63558-171">**Enable-App**</span><span class="sxs-lookup"><span data-stu-id="63558-171">**Enable-App**</span></span>
    
- <span data-ttu-id="63558-172">**Get-App**</span><span class="sxs-lookup"><span data-stu-id="63558-172">**Get-App**</span></span>
    
- <span data-ttu-id="63558-173">**Создание приложения**</span><span class="sxs-lookup"><span data-stu-id="63558-173">**New-App**</span></span>
    
- <span data-ttu-id="63558-174">**Remove-App**</span><span class="sxs-lookup"><span data-stu-id="63558-174">**Remove-App**</span></span>
    
- <span data-ttu-id="63558-175">**SET-App**</span><span class="sxs-lookup"><span data-stu-id="63558-175">**Set-App**</span></span>
    
- <span data-ttu-id="63558-176">**Get-AuthConfig**</span><span class="sxs-lookup"><span data-stu-id="63558-176">**Get-AuthConfig**</span></span>
    
- <span data-ttu-id="63558-177">**SET-AuthConfig**</span><span class="sxs-lookup"><span data-stu-id="63558-177">**Set-AuthConfig**</span></span>
    
- <span data-ttu-id="63558-178">**Get-AuthServer**</span><span class="sxs-lookup"><span data-stu-id="63558-178">**Get-AuthServer**</span></span>
    
- <span data-ttu-id="63558-179">**Новый AuthServer**</span><span class="sxs-lookup"><span data-stu-id="63558-179">**New-AuthServer**</span></span>
    
- <span data-ttu-id="63558-180">**Remove-AuthServer**</span><span class="sxs-lookup"><span data-stu-id="63558-180">**Remove-AuthServer**</span></span>
    
- <span data-ttu-id="63558-181">**SET-AuthServer**</span><span class="sxs-lookup"><span data-stu-id="63558-181">**Set-AuthServer**</span></span>
    
- <span data-ttu-id="63558-182">**Новый AvailabilityConfig**</span><span class="sxs-lookup"><span data-stu-id="63558-182">**New-AvailabilityConfig**</span></span>
    
- <span data-ttu-id="63558-183">**Remove-AvailabilityConfig**</span><span class="sxs-lookup"><span data-stu-id="63558-183">**Remove-AvailabilityConfig**</span></span>
    
- <span data-ttu-id="63558-184">**Get-CalendarDiagnosticAnalysis**</span><span class="sxs-lookup"><span data-stu-id="63558-184">**Get-CalendarDiagnosticAnalysis**</span></span>
    
- <span data-ttu-id="63558-185">**Get-ClassificationRuleCollection**</span><span class="sxs-lookup"><span data-stu-id="63558-185">**Get-ClassificationRuleCollection**</span></span>
    
- <span data-ttu-id="63558-186">**Новый ClassificationRuleCollection**</span><span class="sxs-lookup"><span data-stu-id="63558-186">**New-ClassificationRuleCollection**</span></span>
    
- <span data-ttu-id="63558-187">**Remove-ClassificationRuleCollection**</span><span class="sxs-lookup"><span data-stu-id="63558-187">**Remove-ClassificationRuleCollection**</span></span>
    
- <span data-ttu-id="63558-188">**SET-ClassificationRuleCollection**</span><span class="sxs-lookup"><span data-stu-id="63558-188">**Set-ClassificationRuleCollection**</span></span>
    
- <span data-ttu-id="63558-189">**Get-ConnectSubscription**</span><span class="sxs-lookup"><span data-stu-id="63558-189">**Get-ConnectSubscription**</span></span>
    
- <span data-ttu-id="63558-190">**Новый ConnectSubscription**</span><span class="sxs-lookup"><span data-stu-id="63558-190">**New-ConnectSubscription**</span></span>
    
- <span data-ttu-id="63558-191">**Remove-ConnectSubscription**</span><span class="sxs-lookup"><span data-stu-id="63558-191">**Remove-ConnectSubscription**</span></span>
    
- <span data-ttu-id="63558-192">**SET-ConnectSubscription**</span><span class="sxs-lookup"><span data-stu-id="63558-192">**Set-ConnectSubscription**</span></span>
    
- <span data-ttu-id="63558-193">**Get-DataClassification**</span><span class="sxs-lookup"><span data-stu-id="63558-193">**Get-DataClassification**</span></span>
    
- <span data-ttu-id="63558-194">**Get-DataClassificationConfig**</span><span class="sxs-lookup"><span data-stu-id="63558-194">**Get-DataClassificationConfig**</span></span>
    
- <span data-ttu-id="63558-195">**Get-DlpPolicy**</span><span class="sxs-lookup"><span data-stu-id="63558-195">**Get-DlpPolicy**</span></span>
    
- <span data-ttu-id="63558-196">**Новый DlpPolicy**</span><span class="sxs-lookup"><span data-stu-id="63558-196">**New-DlpPolicy**</span></span>
    
- <span data-ttu-id="63558-197">**Remove-DlpPolicy**</span><span class="sxs-lookup"><span data-stu-id="63558-197">**Remove-DlpPolicy**</span></span>
    
- <span data-ttu-id="63558-198">**SET-DlpPolicy**</span><span class="sxs-lookup"><span data-stu-id="63558-198">**Set-DlpPolicy**</span></span>
    
- <span data-ttu-id="63558-199">**Export-DlpPolicyCollection**</span><span class="sxs-lookup"><span data-stu-id="63558-199">**Export-DlpPolicyCollection**</span></span>
    
- <span data-ttu-id="63558-200">**Import-DlpPolicyCollection**</span><span class="sxs-lookup"><span data-stu-id="63558-200">**Import-DlpPolicyCollection**</span></span>
    
- <span data-ttu-id="63558-201">**Get-DlpPolicyTemplate**</span><span class="sxs-lookup"><span data-stu-id="63558-201">**Get-DlpPolicyTemplate**</span></span>
    
- <span data-ttu-id="63558-202">**Import-DlpPolicyTemplate**</span><span class="sxs-lookup"><span data-stu-id="63558-202">**Import-DlpPolicyTemplate**</span></span>
    
- <span data-ttu-id="63558-203">**Remove-DlpPolicyTemplate**</span><span class="sxs-lookup"><span data-stu-id="63558-203">**Remove-DlpPolicyTemplate**</span></span>
    
- <span data-ttu-id="63558-204">**Get-ExchangeServerAccessLicense**</span><span class="sxs-lookup"><span data-stu-id="63558-204">**Get-ExchangeServerAccessLicense**</span></span>
    
- <span data-ttu-id="63558-205">**Get-ExchangeServerAccessLicenseUser**</span><span class="sxs-lookup"><span data-stu-id="63558-205">**Get-ExchangeServerAccessLicenseUser**</span></span>
    
- <span data-ttu-id="63558-206">**Get-FfoMigrationReport**</span><span class="sxs-lookup"><span data-stu-id="63558-206">**Get-FfoMigrationReport**</span></span>
    
- <span data-ttu-id="63558-207">**Get-FrontendTransportService**</span><span class="sxs-lookup"><span data-stu-id="63558-207">**Get-FrontendTransportService**</span></span>
    
- <span data-ttu-id="63558-208">**SET-FrontendTransportService**</span><span class="sxs-lookup"><span data-stu-id="63558-208">**Set-FrontendTransportService**</span></span>
    
- <span data-ttu-id="63558-209">**Добавление GlobalMonitoringOverride**</span><span class="sxs-lookup"><span data-stu-id="63558-209">**Add-GlobalMonitoringOverride**</span></span>
    
- <span data-ttu-id="63558-210">**Get-GlobalMonitoringOverride**</span><span class="sxs-lookup"><span data-stu-id="63558-210">**Get-GlobalMonitoringOverride**</span></span>
    
- <span data-ttu-id="63558-211">**Remove-GlobalMonitoringOverride**</span><span class="sxs-lookup"><span data-stu-id="63558-211">**Remove-GlobalMonitoringOverride**</span></span>
    
- <span data-ttu-id="63558-212">**Get-GroupActivityReport**</span><span class="sxs-lookup"><span data-stu-id="63558-212">**Get-GroupActivityReport**</span></span>
    
- <span data-ttu-id="63558-213">**Get-HealthReport**</span><span class="sxs-lookup"><span data-stu-id="63558-213">**Get-HealthReport**</span></span>
    
- <span data-ttu-id="63558-214">**Get-HostedConnectionFilterPolicy**</span><span class="sxs-lookup"><span data-stu-id="63558-214">**Get-HostedConnectionFilterPolicy**</span></span>
    
- <span data-ttu-id="63558-215">**Новый HostedConnectionFilterPolicy**</span><span class="sxs-lookup"><span data-stu-id="63558-215">**New-HostedConnectionFilterPolicy**</span></span>
    
- <span data-ttu-id="63558-216">**Remove-HostedConnectionFilterPolicy**</span><span class="sxs-lookup"><span data-stu-id="63558-216">**Remove-HostedConnectionFilterPolicy**</span></span>
    
- <span data-ttu-id="63558-217">**SET-HostedConnectionFilterPolicy**</span><span class="sxs-lookup"><span data-stu-id="63558-217">**Set-HostedConnectionFilterPolicy**</span></span>
    
- <span data-ttu-id="63558-218">**Get-HostedContentFilterPolicy**</span><span class="sxs-lookup"><span data-stu-id="63558-218">**Get-HostedContentFilterPolicy**</span></span>
    
- <span data-ttu-id="63558-219">**New-HostedContentFilterPolicy**</span><span class="sxs-lookup"><span data-stu-id="63558-219">**New-HostedContentFilterPolicy**</span></span>
    
- <span data-ttu-id="63558-220">**Remove-HostedContentFilterPolicy**</span><span class="sxs-lookup"><span data-stu-id="63558-220">**Remove-HostedContentFilterPolicy**</span></span>
    
- <span data-ttu-id="63558-221">**SET-HostedContentFilterPolicy**</span><span class="sxs-lookup"><span data-stu-id="63558-221">**Set-HostedContentFilterPolicy**</span></span>
    
- <span data-ttu-id="63558-222">**Get-HostedOutboundSpamFilterPolicy**</span><span class="sxs-lookup"><span data-stu-id="63558-222">**Get-HostedOutboundSpamFilterPolicy**</span></span>
    
- <span data-ttu-id="63558-223">**SET-HostedOutboundSpamFilterPolicy**</span><span class="sxs-lookup"><span data-stu-id="63558-223">**Set-HostedOutboundSpamFilterPolicy**</span></span>
    
- <span data-ttu-id="63558-224">**Remove-HybridConfiguration**</span><span class="sxs-lookup"><span data-stu-id="63558-224">**Remove-HybridConfiguration**</span></span>
    
- <span data-ttu-id="63558-225">**Get-HybridMailflow**</span><span class="sxs-lookup"><span data-stu-id="63558-225">**Get-HybridMailflow**</span></span>
    
- <span data-ttu-id="63558-226">**SET Hybridmailflowиспользуется**</span><span class="sxs-lookup"><span data-stu-id="63558-226">**Set-HybridMailflow**</span></span>
    
- <span data-ttu-id="63558-227">**Get-HybridMailflowDatacenterIPs**</span><span class="sxs-lookup"><span data-stu-id="63558-227">**Get-HybridMailflowDatacenterIPs**</span></span>
    
- <span data-ttu-id="63558-228">**Get-InboundConnector**</span><span class="sxs-lookup"><span data-stu-id="63558-228">**Get-InboundConnector**</span></span>
    
- <span data-ttu-id="63558-229">**Новый InboundConnector**</span><span class="sxs-lookup"><span data-stu-id="63558-229">**New-InboundConnector**</span></span>
    
- <span data-ttu-id="63558-230">**Remove-InboundConnector**</span><span class="sxs-lookup"><span data-stu-id="63558-230">**Remove-InboundConnector**</span></span>
    
- <span data-ttu-id="63558-231">**SET-InboundConnector**</span><span class="sxs-lookup"><span data-stu-id="63558-231">**Set-InboundConnector**</span></span>
    
- <span data-ttu-id="63558-232">**Get-MailboxActivityReport**</span><span class="sxs-lookup"><span data-stu-id="63558-232">**Get-MailboxActivityReport**</span></span>
    
- <span data-ttu-id="63558-233">**Disable-MailboxQuarantine**</span><span class="sxs-lookup"><span data-stu-id="63558-233">**Disable-MailboxQuarantine**</span></span>
    
- <span data-ttu-id="63558-234">**Enable-MailboxQuarantine**</span><span class="sxs-lookup"><span data-stu-id="63558-234">**Enable-MailboxQuarantine**</span></span>
    
- <span data-ttu-id="63558-235">**Get-MailboxTransportService**</span><span class="sxs-lookup"><span data-stu-id="63558-235">**Get-MailboxTransportService**</span></span>
    
- <span data-ttu-id="63558-236">**SET-MailboxTransportService**</span><span class="sxs-lookup"><span data-stu-id="63558-236">**Set-MailboxTransportService**</span></span>
    
- <span data-ttu-id="63558-237">**Get-MailDetailDlpPolicyReport**</span><span class="sxs-lookup"><span data-stu-id="63558-237">**Get-MailDetailDlpPolicyReport**</span></span>
    
- <span data-ttu-id="63558-238">**Get-MailDetailMalwareReport**</span><span class="sxs-lookup"><span data-stu-id="63558-238">**Get-MailDetailMalwareReport**</span></span>
    
- <span data-ttu-id="63558-239">**Get-MailDetailReport**</span><span class="sxs-lookup"><span data-stu-id="63558-239">**Get-MailDetailReport**</span></span>
    
- <span data-ttu-id="63558-240">**Get-MailDetailSpamReport**</span><span class="sxs-lookup"><span data-stu-id="63558-240">**Get-MailDetailSpamReport**</span></span>
    
- <span data-ttu-id="63558-241">**Get-MailDetailTransportRuleReport**</span><span class="sxs-lookup"><span data-stu-id="63558-241">**Get-MailDetailTransportRuleReport**</span></span>
    
- <span data-ttu-id="63558-242">**Get-MailFilterListReport**</span><span class="sxs-lookup"><span data-stu-id="63558-242">**Get-MailFilterListReport**</span></span>
    
- <span data-ttu-id="63558-243">**Get-MailTrafficPolicyReport**</span><span class="sxs-lookup"><span data-stu-id="63558-243">**Get-MailTrafficPolicyReport**</span></span>
    
- <span data-ttu-id="63558-244">**Get-MailTrafficReport**</span><span class="sxs-lookup"><span data-stu-id="63558-244">**Get-MailTrafficReport**</span></span>
    
- <span data-ttu-id="63558-245">**Get-MailTrafficSummaryReport**</span><span class="sxs-lookup"><span data-stu-id="63558-245">**Get-MailTrafficSummaryReport**</span></span>
    
- <span data-ttu-id="63558-246">**Get-MailTrafficTopReport**</span><span class="sxs-lookup"><span data-stu-id="63558-246">**Get-MailTrafficTopReport**</span></span>
    
- <span data-ttu-id="63558-247">**Get-MalwareFilteringServer**</span><span class="sxs-lookup"><span data-stu-id="63558-247">**Get-MalwareFilteringServer**</span></span>
    
- <span data-ttu-id="63558-248">**SET-MalwareFilteringServer**</span><span class="sxs-lookup"><span data-stu-id="63558-248">**Set-MalwareFilteringServer**</span></span>
    
- <span data-ttu-id="63558-249">**Get-MalwareFilterPolicy**</span><span class="sxs-lookup"><span data-stu-id="63558-249">**Get-MalwareFilterPolicy**</span></span>
    
- <span data-ttu-id="63558-250">**New-MalwareFilterPolicy**</span><span class="sxs-lookup"><span data-stu-id="63558-250">**New-MalwareFilterPolicy**</span></span>
    
- <span data-ttu-id="63558-251">**Remove-MalwareFilterPolicy**</span><span class="sxs-lookup"><span data-stu-id="63558-251">**Remove-MalwareFilterPolicy**</span></span>
    
- <span data-ttu-id="63558-252">**SET-MalwareFilterPolicy**</span><span class="sxs-lookup"><span data-stu-id="63558-252">**Set-MalwareFilterPolicy**</span></span>
    
- <span data-ttu-id="63558-253">**Get-MalwareFilterRecoveryItem**</span><span class="sxs-lookup"><span data-stu-id="63558-253">**Get-MalwareFilterRecoveryItem**</span></span>
    
- <span data-ttu-id="63558-254">**Remove-MalwareFilterRecoveryItem**</span><span class="sxs-lookup"><span data-stu-id="63558-254">**Remove-MalwareFilterRecoveryItem**</span></span>
    
- <span data-ttu-id="63558-255">**Возобновление MalwareFilterRecoveryItem**</span><span class="sxs-lookup"><span data-stu-id="63558-255">**Resume-MalwareFilterRecoveryItem**</span></span>
    
- <span data-ttu-id="63558-256">**Отправить MapiSubmitSystemProbe**</span><span class="sxs-lookup"><span data-stu-id="63558-256">**Send-MapiSubmitSystemProbe**</span></span>
    
- <span data-ttu-id="63558-257">**Перенаправление сообщения**</span><span class="sxs-lookup"><span data-stu-id="63558-257">**Redirect-Message**</span></span>
    
- <span data-ttu-id="63558-258">**Get-MessageTrace**</span><span class="sxs-lookup"><span data-stu-id="63558-258">**Get-MessageTrace**</span></span>
    
- <span data-ttu-id="63558-259">**Get-MessageTraceDetail**</span><span class="sxs-lookup"><span data-stu-id="63558-259">**Get-MessageTraceDetail**</span></span>
    
- <span data-ttu-id="63558-260">**Завершить MigrationBatch**</span><span class="sxs-lookup"><span data-stu-id="63558-260">**Complete-MigrationBatch**</span></span>
    
- <span data-ttu-id="63558-261">**Remove-MigrationBatch**</span><span class="sxs-lookup"><span data-stu-id="63558-261">**Remove-MigrationBatch**</span></span>
    
- <span data-ttu-id="63558-262">**Get-MigrationConfig**</span><span class="sxs-lookup"><span data-stu-id="63558-262">**Get-MigrationConfig**</span></span>
    
- <span data-ttu-id="63558-263">**SET-MigrationConfig**</span><span class="sxs-lookup"><span data-stu-id="63558-263">**Set-MigrationConfig**</span></span>
    
- <span data-ttu-id="63558-264">**Get-MigrationEndpoint**</span><span class="sxs-lookup"><span data-stu-id="63558-264">**Get-MigrationEndpoint**</span></span>
    
- <span data-ttu-id="63558-265">**Новый MigrationEndpoint**</span><span class="sxs-lookup"><span data-stu-id="63558-265">**New-MigrationEndpoint**</span></span>
    
- <span data-ttu-id="63558-266">**Remove-MigrationEndpoint**</span><span class="sxs-lookup"><span data-stu-id="63558-266">**Remove-MigrationEndpoint**</span></span>
    
- <span data-ttu-id="63558-267">**SET-MigrationEndpoint**</span><span class="sxs-lookup"><span data-stu-id="63558-267">**Set-MigrationEndpoint**</span></span>
    
- <span data-ttu-id="63558-268">**Get-MigrationStatistics**</span><span class="sxs-lookup"><span data-stu-id="63558-268">**Get-MigrationStatistics**</span></span>
    
- <span data-ttu-id="63558-269">**Get-MigrationUser**</span><span class="sxs-lookup"><span data-stu-id="63558-269">**Get-MigrationUser**</span></span>
    
- <span data-ttu-id="63558-270">**Remove-MigrationUser**</span><span class="sxs-lookup"><span data-stu-id="63558-270">**Remove-MigrationUser**</span></span>
    
- <span data-ttu-id="63558-271">**Get-MigrationUserStatistics**</span><span class="sxs-lookup"><span data-stu-id="63558-271">**Get-MigrationUserStatistics**</span></span>
    
- <span data-ttu-id="63558-272">**Clear-MobileDevice**</span><span class="sxs-lookup"><span data-stu-id="63558-272">**Clear-MobileDevice**</span></span>
    
- <span data-ttu-id="63558-273">**Get-MobileDevice**</span><span class="sxs-lookup"><span data-stu-id="63558-273">**Get-MobileDevice**</span></span>
    
- <span data-ttu-id="63558-274">**Remove-MobileDevice**</span><span class="sxs-lookup"><span data-stu-id="63558-274">**Remove-MobileDevice**</span></span>
    
- <span data-ttu-id="63558-275">**Get-MobileDeviceMailboxPolicy**</span><span class="sxs-lookup"><span data-stu-id="63558-275">**Get-MobileDeviceMailboxPolicy**</span></span>
    
- <span data-ttu-id="63558-276">**Новый MobileDeviceMailboxPolicy**</span><span class="sxs-lookup"><span data-stu-id="63558-276">**New-MobileDeviceMailboxPolicy**</span></span>
    
- <span data-ttu-id="63558-277">**Remove-MobileDeviceMailboxPolicy**</span><span class="sxs-lookup"><span data-stu-id="63558-277">**Remove-MobileDeviceMailboxPolicy**</span></span>
    
- <span data-ttu-id="63558-278">**SET-MobileDeviceMailboxPolicy**</span><span class="sxs-lookup"><span data-stu-id="63558-278">**Set-MobileDeviceMailboxPolicy**</span></span>
    
- <span data-ttu-id="63558-279">**Get-MobileDeviceStatistics**</span><span class="sxs-lookup"><span data-stu-id="63558-279">**Get-MobileDeviceStatistics**</span></span>
    
- <span data-ttu-id="63558-280">**Get-MonitoringItemHelp**</span><span class="sxs-lookup"><span data-stu-id="63558-280">**Get-MonitoringItemHelp**</span></span>
    
- <span data-ttu-id="63558-281">**Get-MonitoringItemIdentity**</span><span class="sxs-lookup"><span data-stu-id="63558-281">**Get-MonitoringItemIdentity**</span></span>
    
- <span data-ttu-id="63558-282">**Invoke-MonitoringProbe**</span><span class="sxs-lookup"><span data-stu-id="63558-282">**Invoke-MonitoringProbe**</span></span>
    
- <span data-ttu-id="63558-283">**Get уведомлений**</span><span class="sxs-lookup"><span data-stu-id="63558-283">**Get-Notification**</span></span>
    
- <span data-ttu-id="63558-284">**SET уведомлений**</span><span class="sxs-lookup"><span data-stu-id="63558-284">**Set-Notification**</span></span>
    
- <span data-ttu-id="63558-285">**Test-OAuthConnectivity**</span><span class="sxs-lookup"><span data-stu-id="63558-285">**Test-OAuthConnectivity**</span></span>
    
- <span data-ttu-id="63558-286">**Get-OnPremisesOrganization**</span><span class="sxs-lookup"><span data-stu-id="63558-286">**Get-OnPremisesOrganization**</span></span>
    
- <span data-ttu-id="63558-287">**Новые локальной организации**</span><span class="sxs-lookup"><span data-stu-id="63558-287">**New-OnPremisesOrganization**</span></span>
    
- <span data-ttu-id="63558-288">**Remove-OnPremisesOrganization**</span><span class="sxs-lookup"><span data-stu-id="63558-288">**Remove-OnPremisesOrganization**</span></span>
    
- <span data-ttu-id="63558-289">**SET-OnPremisesOrganization**</span><span class="sxs-lookup"><span data-stu-id="63558-289">**Set-OnPremisesOrganization**</span></span>
    
- <span data-ttu-id="63558-290">**Enable-OrganizationCustomization**</span><span class="sxs-lookup"><span data-stu-id="63558-290">**Enable-OrganizationCustomization**</span></span>
    
- <span data-ttu-id="63558-291">**Get-OutboundConnector**</span><span class="sxs-lookup"><span data-stu-id="63558-291">**Get-OutboundConnector**</span></span>
    
- <span data-ttu-id="63558-292">**Новый OutboundConnector**</span><span class="sxs-lookup"><span data-stu-id="63558-292">**New-OutboundConnector**</span></span>
    
- <span data-ttu-id="63558-293">**Remove-OutboundConnector**</span><span class="sxs-lookup"><span data-stu-id="63558-293">**Remove-OutboundConnector**</span></span>
    
- <span data-ttu-id="63558-294">**SET-OutboundConnector**</span><span class="sxs-lookup"><span data-stu-id="63558-294">**Set-OutboundConnector**</span></span>
    
- <span data-ttu-id="63558-295">**Get-PartnerApplication**</span><span class="sxs-lookup"><span data-stu-id="63558-295">**Get-PartnerApplication**</span></span>
    
- <span data-ttu-id="63558-296">**Новый PartnerApplication**</span><span class="sxs-lookup"><span data-stu-id="63558-296">**New-PartnerApplication**</span></span>
    
- <span data-ttu-id="63558-297">**Remove-PartnerApplication**</span><span class="sxs-lookup"><span data-stu-id="63558-297">**Remove-PartnerApplication**</span></span>
    
- <span data-ttu-id="63558-298">**SET-PartnerApplication**</span><span class="sxs-lookup"><span data-stu-id="63558-298">**Set-PartnerApplication**</span></span>
    
- <span data-ttu-id="63558-299">**Get-PendingFederatedDomain**</span><span class="sxs-lookup"><span data-stu-id="63558-299">**Get-PendingFederatedDomain**</span></span>
    
- <span data-ttu-id="63558-300">**SET-PendingFederatedDomain**</span><span class="sxs-lookup"><span data-stu-id="63558-300">**Set-PendingFederatedDomain**</span></span>
    
- <span data-ttu-id="63558-301">**Get-PolicyTipConfig**</span><span class="sxs-lookup"><span data-stu-id="63558-301">**Get-PolicyTipConfig**</span></span>
    
- <span data-ttu-id="63558-302">**Новый PolicyTipConfig**</span><span class="sxs-lookup"><span data-stu-id="63558-302">**New-PolicyTipConfig**</span></span>
    
- <span data-ttu-id="63558-303">**Remove-PolicyTipConfig**</span><span class="sxs-lookup"><span data-stu-id="63558-303">**Remove-PolicyTipConfig**</span></span>
    
- <span data-ttu-id="63558-304">**SET-PolicyTipConfig**</span><span class="sxs-lookup"><span data-stu-id="63558-304">**Set-PolicyTipConfig**</span></span>
    
- <span data-ttu-id="63558-305">**Dump-ProvisioningCache**</span><span class="sxs-lookup"><span data-stu-id="63558-305">**Dump-ProvisioningCache**</span></span>
    
- <span data-ttu-id="63558-306">**Сброс ProvisioningCache**</span><span class="sxs-lookup"><span data-stu-id="63558-306">**Reset-ProvisioningCache**</span></span>
    
- <span data-ttu-id="63558-307">**Update-PublicFolderMailbox**</span><span class="sxs-lookup"><span data-stu-id="63558-307">**Update-PublicFolderMailbox**</span></span>
    
- <span data-ttu-id="63558-308">**Get-PublicFolderMailboxDiagnostics**</span><span class="sxs-lookup"><span data-stu-id="63558-308">**Get-PublicFolderMailboxDiagnostics**</span></span>
    
- <span data-ttu-id="63558-309">**Get-PublicFolderMigrationRequest**</span><span class="sxs-lookup"><span data-stu-id="63558-309">**Get-PublicFolderMigrationRequest**</span></span>
    
- <span data-ttu-id="63558-310">**Новый PublicFolderMigrationRequest**</span><span class="sxs-lookup"><span data-stu-id="63558-310">**New-PublicFolderMigrationRequest**</span></span>
    
- <span data-ttu-id="63558-311">**Remove-PublicFolderMigrationRequest**</span><span class="sxs-lookup"><span data-stu-id="63558-311">**Remove-PublicFolderMigrationRequest**</span></span>
    
- <span data-ttu-id="63558-312">**Resume-PublicFolderMigrationRequest**</span><span class="sxs-lookup"><span data-stu-id="63558-312">**Resume-PublicFolderMigrationRequest**</span></span>
    
- <span data-ttu-id="63558-313">**SET-PublicFolderMigrationRequest**</span><span class="sxs-lookup"><span data-stu-id="63558-313">**Set-PublicFolderMigrationRequest**</span></span>
    
- <span data-ttu-id="63558-314">**Приостановить PublicFolderMigrationRequest**</span><span class="sxs-lookup"><span data-stu-id="63558-314">**Suspend-PublicFolderMigrationRequest**</span></span>
    
- <span data-ttu-id="63558-315">**Get-PublicFolderMigrationRequestStatistics**</span><span class="sxs-lookup"><span data-stu-id="63558-315">**Get-PublicFolderMigrationRequestStatistics**</span></span>
    
- <span data-ttu-id="63558-316">**Get-QuarantineMessage**</span><span class="sxs-lookup"><span data-stu-id="63558-316">**Get-QuarantineMessage**</span></span>
    
- <span data-ttu-id="63558-317">**Выпуск QuarantineMessage**</span><span class="sxs-lookup"><span data-stu-id="63558-317">**Release-QuarantineMessage**</span></span>
    
- <span data-ttu-id="63558-318">**Get-QueueDigest**</span><span class="sxs-lookup"><span data-stu-id="63558-318">**Get-QueueDigest**</span></span>
    
- <span data-ttu-id="63558-319">**Get-ResourcePolicy**</span><span class="sxs-lookup"><span data-stu-id="63558-319">**Get-ResourcePolicy**</span></span>
    
- <span data-ttu-id="63558-320">**Новый ResourcePolicy**</span><span class="sxs-lookup"><span data-stu-id="63558-320">**New-ResourcePolicy**</span></span>
    
- <span data-ttu-id="63558-321">**Remove-ResourcePolicy**</span><span class="sxs-lookup"><span data-stu-id="63558-321">**Remove-ResourcePolicy**</span></span>
    
- <span data-ttu-id="63558-322">**SET-ResourcePolicy**</span><span class="sxs-lookup"><span data-stu-id="63558-322">**Set-ResourcePolicy**</span></span>
    
- <span data-ttu-id="63558-323">**Добавление ResubmitRequest**</span><span class="sxs-lookup"><span data-stu-id="63558-323">**Add-ResubmitRequest**</span></span>
    
- <span data-ttu-id="63558-324">**Get-ResubmitRequest**</span><span class="sxs-lookup"><span data-stu-id="63558-324">**Get-ResubmitRequest**</span></span>
    
- <span data-ttu-id="63558-325">**Remove-ResubmitRequest**</span><span class="sxs-lookup"><span data-stu-id="63558-325">**Remove-ResubmitRequest**</span></span>
    
- <span data-ttu-id="63558-326">**SET-ResubmitRequest**</span><span class="sxs-lookup"><span data-stu-id="63558-326">**Set-ResubmitRequest**</span></span>
    
- <span data-ttu-id="63558-327">**Get-ServerComponentState**</span><span class="sxs-lookup"><span data-stu-id="63558-327">**Get-ServerComponentState**</span></span>
    
- <span data-ttu-id="63558-328">**SET-ServerComponentState**</span><span class="sxs-lookup"><span data-stu-id="63558-328">**Set-ServerComponentState**</span></span>
    
- <span data-ttu-id="63558-329">**Get-ServerHealth**</span><span class="sxs-lookup"><span data-stu-id="63558-329">**Get-ServerHealth**</span></span>
    
- <span data-ttu-id="63558-330">**SET-ServerMonitor**</span><span class="sxs-lookup"><span data-stu-id="63558-330">**Set-ServerMonitor**</span></span>
    
- <span data-ttu-id="63558-331">**Добавление ServerMonitoringOverride**</span><span class="sxs-lookup"><span data-stu-id="63558-331">**Add-ServerMonitoringOverride**</span></span>
    
- <span data-ttu-id="63558-332">**Get-ServerMonitoringOverride**</span><span class="sxs-lookup"><span data-stu-id="63558-332">**Get-ServerMonitoringOverride**</span></span>
    
- <span data-ttu-id="63558-333">**Get-SiteMailbox**</span><span class="sxs-lookup"><span data-stu-id="63558-333">**Get-SiteMailbox**</span></span>
    
- <span data-ttu-id="63558-334">**Новый SiteMailbox**</span><span class="sxs-lookup"><span data-stu-id="63558-334">**New-SiteMailbox**</span></span>
    
- <span data-ttu-id="63558-335">**SET-SiteMailbox**</span><span class="sxs-lookup"><span data-stu-id="63558-335">**Set-SiteMailbox**</span></span>
    
- <span data-ttu-id="63558-336">**Test-SiteMailbox**</span><span class="sxs-lookup"><span data-stu-id="63558-336">**Test-SiteMailbox**</span></span>
    
- <span data-ttu-id="63558-337">**Обновление SiteMailbox**</span><span class="sxs-lookup"><span data-stu-id="63558-337">**Update-SiteMailbox**</span></span>
    
- <span data-ttu-id="63558-338">**Get-SiteMailboxDiagnostics**</span><span class="sxs-lookup"><span data-stu-id="63558-338">**Get-SiteMailboxDiagnostics**</span></span>
    
- <span data-ttu-id="63558-339">**Get-SiteMailboxProvisioningPolicy**</span><span class="sxs-lookup"><span data-stu-id="63558-339">**Get-SiteMailboxProvisioningPolicy**</span></span>
    
- <span data-ttu-id="63558-340">**Новый SiteMailboxProvisioningPolicy**</span><span class="sxs-lookup"><span data-stu-id="63558-340">**New-SiteMailboxProvisioningPolicy**</span></span>
    
- <span data-ttu-id="63558-341">**Remove-SiteMailboxProvisioningPolicy**</span><span class="sxs-lookup"><span data-stu-id="63558-341">**Remove-SiteMailboxProvisioningPolicy**</span></span>
    
- <span data-ttu-id="63558-342">**SET-SiteMailboxProvisioningPolicy**</span><span class="sxs-lookup"><span data-stu-id="63558-342">**Set-SiteMailboxProvisioningPolicy**</span></span>
    
- <span data-ttu-id="63558-343">**Отмена SoftDeletedMailbox**</span><span class="sxs-lookup"><span data-stu-id="63558-343">**Undo-SoftDeletedMailbox**</span></span>
    
- <span data-ttu-id="63558-344">**Get-StaleMailboxDetailReport**</span><span class="sxs-lookup"><span data-stu-id="63558-344">**Get-StaleMailboxDetailReport**</span></span>
    
- <span data-ttu-id="63558-345">**Get-StaleMailboxReport**</span><span class="sxs-lookup"><span data-stu-id="63558-345">**Get-StaleMailboxReport**</span></span>
    
- <span data-ttu-id="63558-346">**Update-storemailboxstate, можно**</span><span class="sxs-lookup"><span data-stu-id="63558-346">**Update-StoreMailboxState**</span></span>
    
- <span data-ttu-id="63558-347">**Новый SyncMailPublicFolder**</span><span class="sxs-lookup"><span data-stu-id="63558-347">**New-SyncMailPublicFolder**</span></span>
    
- <span data-ttu-id="63558-348">**Get-TransportService**</span><span class="sxs-lookup"><span data-stu-id="63558-348">**Get-TransportService**</span></span>
    
- <span data-ttu-id="63558-349">**SET-TransportService**</span><span class="sxs-lookup"><span data-stu-id="63558-349">**Set-TransportService**</span></span>
    
- <span data-ttu-id="63558-350">**Disable-UMCallAnsweringRule**</span><span class="sxs-lookup"><span data-stu-id="63558-350">**Disable-UMCallAnsweringRule**</span></span>
    
- <span data-ttu-id="63558-351">**Enable-UMCallAnsweringRule**</span><span class="sxs-lookup"><span data-stu-id="63558-351">**Enable-UMCallAnsweringRule**</span></span>
    
- <span data-ttu-id="63558-352">**Get-UMCallAnsweringRule**</span><span class="sxs-lookup"><span data-stu-id="63558-352">**Get-UMCallAnsweringRule**</span></span>
    
- <span data-ttu-id="63558-353">**Новый UMCallAnsweringRule**</span><span class="sxs-lookup"><span data-stu-id="63558-353">**New-UMCallAnsweringRule**</span></span>
    
- <span data-ttu-id="63558-354">**Remove-UMCallAnsweringRule**</span><span class="sxs-lookup"><span data-stu-id="63558-354">**Remove-UMCallAnsweringRule**</span></span>
    
- <span data-ttu-id="63558-355">**SET-UMCallAnsweringRule**</span><span class="sxs-lookup"><span data-stu-id="63558-355">**Set-UMCallAnsweringRule**</span></span>
    
- <span data-ttu-id="63558-356">**Get-UMCallRouterSettings**</span><span class="sxs-lookup"><span data-stu-id="63558-356">**Get-UMCallRouterSettings**</span></span>
    
- <span data-ttu-id="63558-357">**SET-UMCallRouterSettings**</span><span class="sxs-lookup"><span data-stu-id="63558-357">**Set-UMCallRouterSettings**</span></span>
    
- <span data-ttu-id="63558-358">**Disable-UMService**</span><span class="sxs-lookup"><span data-stu-id="63558-358">**Disable-UMService**</span></span>
    
- <span data-ttu-id="63558-359">**Enable-UMService**</span><span class="sxs-lookup"><span data-stu-id="63558-359">**Enable-UMService**</span></span>
    
- <span data-ttu-id="63558-360">**Get-UMService**</span><span class="sxs-lookup"><span data-stu-id="63558-360">**Get-UMService**</span></span>
    
- <span data-ttu-id="63558-361">**SET-UMService**</span><span class="sxs-lookup"><span data-stu-id="63558-361">**Set-UMService**</span></span>
    
- <span data-ttu-id="63558-362">**Get-UserPhoto**</span><span class="sxs-lookup"><span data-stu-id="63558-362">**Get-UserPhoto**</span></span>
    
- <span data-ttu-id="63558-363">**Remove-UserPhoto**</span><span class="sxs-lookup"><span data-stu-id="63558-363">**Remove-UserPhoto**</span></span>
    
- <span data-ttu-id="63558-364">**SET-UserPhoto**</span><span class="sxs-lookup"><span data-stu-id="63558-364">**Set-UserPhoto**</span></span>
    
- <span data-ttu-id="63558-365">**Get-WorkloadManagementPolicy**</span><span class="sxs-lookup"><span data-stu-id="63558-365">**Get-WorkloadManagementPolicy**</span></span>
    
- <span data-ttu-id="63558-366">**Новый WorkloadManagementPolicy**</span><span class="sxs-lookup"><span data-stu-id="63558-366">**New-WorkloadManagementPolicy**</span></span>
    
- <span data-ttu-id="63558-367">**Remove-WorkloadManagementPolicy**</span><span class="sxs-lookup"><span data-stu-id="63558-367">**Remove-WorkloadManagementPolicy**</span></span>
    
- <span data-ttu-id="63558-368">**Get-WorkloadPolicy**</span><span class="sxs-lookup"><span data-stu-id="63558-368">**Get-WorkloadPolicy**</span></span>
    
- <span data-ttu-id="63558-369">**Новый WorkloadPolicy**</span><span class="sxs-lookup"><span data-stu-id="63558-369">**New-WorkloadPolicy**</span></span>
    
- <span data-ttu-id="63558-370">**Remove-WorkloadPolicy**</span><span class="sxs-lookup"><span data-stu-id="63558-370">**Remove-WorkloadPolicy**</span></span>
    
- <span data-ttu-id="63558-371">**SET-WorkloadPolicy**</span><span class="sxs-lookup"><span data-stu-id="63558-371">**Set-WorkloadPolicy**</span></span>
    
### <a name="modified-cmdlets"></a><span data-ttu-id="63558-372">Измененные командлеты</span><span class="sxs-lookup"><span data-stu-id="63558-372">Modified cmdlets</span></span>
<span data-ttu-id="63558-373"><a name="bk_update"> </a></span><span class="sxs-lookup"><span data-stu-id="63558-373"></span></span>

<span data-ttu-id="63558-374">Типы ввода-вывода для следующих командлетов были изменены в Exchange 2013:</span><span class="sxs-lookup"><span data-stu-id="63558-374">The input or output types for following cmdlets were modified in Exchange 2013:</span></span>
  
- <span data-ttu-id="63558-375">**Clear-ActiveSyncDevice**</span><span class="sxs-lookup"><span data-stu-id="63558-375">**Clear-ActiveSyncDevice**</span></span>
    
- <span data-ttu-id="63558-376">**Remove-ActiveSyncDevice**</span><span class="sxs-lookup"><span data-stu-id="63558-376">**Remove-ActiveSyncDevice**</span></span>
    
- <span data-ttu-id="63558-377">**Get-ActiveSyncMailboxPolicy**</span><span class="sxs-lookup"><span data-stu-id="63558-377">**Get-ActiveSyncMailboxPolicy**</span></span>
    
- <span data-ttu-id="63558-378">**Новый ActiveSyncMailboxPolicy**</span><span class="sxs-lookup"><span data-stu-id="63558-378">**New-ActiveSyncMailboxPolicy**</span></span>
    
- <span data-ttu-id="63558-379">**Новый ActiveSyncVirtualDirectory**</span><span class="sxs-lookup"><span data-stu-id="63558-379">**New-ActiveSyncVirtualDirectory**</span></span>
    
- <span data-ttu-id="63558-380">**Новый AutodiscoverVirtualDirectory**</span><span class="sxs-lookup"><span data-stu-id="63558-380">**New-AutodiscoverVirtualDirectory**</span></span>
    
- <span data-ttu-id="63558-381">**SET-AvailabilityConfig**</span><span class="sxs-lookup"><span data-stu-id="63558-381">**Set-AvailabilityConfig**</span></span>
    
- <span data-ttu-id="63558-382">**Enable-ExchangeCertificate**</span><span class="sxs-lookup"><span data-stu-id="63558-382">**Enable-ExchangeCertificate**</span></span>
    
- <span data-ttu-id="63558-383">**Export-ExchangeCertificate**</span><span class="sxs-lookup"><span data-stu-id="63558-383">**Export-ExchangeCertificate**</span></span>
    
- <span data-ttu-id="63558-384">**Import-ExchangeCertificate**</span><span class="sxs-lookup"><span data-stu-id="63558-384">**Import-ExchangeCertificate**</span></span>
    
- <span data-ttu-id="63558-385">**Remove-ExchangeCertificate**</span><span class="sxs-lookup"><span data-stu-id="63558-385">**Remove-ExchangeCertificate**</span></span>
    
- <span data-ttu-id="63558-386">**Get-FailedContentIndexDocuments**</span><span class="sxs-lookup"><span data-stu-id="63558-386">**Get-FailedContentIndexDocuments**</span></span>
    
- <span data-ttu-id="63558-387">**Get-FederationInformation**</span><span class="sxs-lookup"><span data-stu-id="63558-387">**Get-FederationInformation**</span></span>
    
- <span data-ttu-id="63558-388">**Новый HybridConfiguration**</span><span class="sxs-lookup"><span data-stu-id="63558-388">**New-HybridConfiguration**</span></span>
    
- <span data-ttu-id="63558-389">**SET-HybridConfiguration**</span><span class="sxs-lookup"><span data-stu-id="63558-389">**Set-HybridConfiguration**</span></span>
    
- <span data-ttu-id="63558-390">**Новый почтовый ящик**</span><span class="sxs-lookup"><span data-stu-id="63558-390">**New-Mailbox**</span></span>
    
- <span data-ttu-id="63558-391">**Resume-MailboxDatabaseCopy**</span><span class="sxs-lookup"><span data-stu-id="63558-391">**Resume-MailboxDatabaseCopy**</span></span>
    
- <span data-ttu-id="63558-392">**SET-MailboxDatabaseCopy**</span><span class="sxs-lookup"><span data-stu-id="63558-392">**Set-MailboxDatabaseCopy**</span></span>
    
- <span data-ttu-id="63558-393">**Приостановить MailboxDatabaseCopy**</span><span class="sxs-lookup"><span data-stu-id="63558-393">**Suspend-MailboxDatabaseCopy**</span></span>
    
- <span data-ttu-id="63558-394">**Update-MailboxDatabaseCopy**</span><span class="sxs-lookup"><span data-stu-id="63558-394">**Update-MailboxDatabaseCopy**</span></span>
    
- <span data-ttu-id="63558-395">**Get-MailboxExportRequest**</span><span class="sxs-lookup"><span data-stu-id="63558-395">**Get-MailboxExportRequest**</span></span>
    
- <span data-ttu-id="63558-396">**SET-MailboxExportRequest**</span><span class="sxs-lookup"><span data-stu-id="63558-396">**Set-MailboxExportRequest**</span></span>
    
- <span data-ttu-id="63558-397">**Добавление MailboxFolderPermission**</span><span class="sxs-lookup"><span data-stu-id="63558-397">**Add-MailboxFolderPermission**</span></span>
    
- <span data-ttu-id="63558-398">**Remove-MailboxFolderPermission**</span><span class="sxs-lookup"><span data-stu-id="63558-398">**Remove-MailboxFolderPermission**</span></span>
    
- <span data-ttu-id="63558-399">**SET-MailboxFolderPermission**</span><span class="sxs-lookup"><span data-stu-id="63558-399">**Set-MailboxFolderPermission**</span></span>
    
- <span data-ttu-id="63558-400">**Get-MailboxImportRequest**</span><span class="sxs-lookup"><span data-stu-id="63558-400">**Get-MailboxImportRequest**</span></span>
    
- <span data-ttu-id="63558-401">**SET-MailboxImportRequest**</span><span class="sxs-lookup"><span data-stu-id="63558-401">**Set-MailboxImportRequest**</span></span>
    
- <span data-ttu-id="63558-402">**Get-MailboxRestoreRequest**</span><span class="sxs-lookup"><span data-stu-id="63558-402">**Get-MailboxRestoreRequest**</span></span>
    
- <span data-ttu-id="63558-403">**SET-MailboxRestoreRequest**</span><span class="sxs-lookup"><span data-stu-id="63558-403">**Set-MailboxRestoreRequest**</span></span>
    
- <span data-ttu-id="63558-404">**Get-MailboxSearch**</span><span class="sxs-lookup"><span data-stu-id="63558-404">**Get-MailboxSearch**</span></span>
    
- <span data-ttu-id="63558-405">**Remove-MailboxSearch**</span><span class="sxs-lookup"><span data-stu-id="63558-405">**Remove-MailboxSearch**</span></span>
    
- <span data-ttu-id="63558-406">**SET-MailboxSearch**</span><span class="sxs-lookup"><span data-stu-id="63558-406">**Set-MailboxSearch**</span></span>
    
- <span data-ttu-id="63558-407">**Start-MailboxSearch**</span><span class="sxs-lookup"><span data-stu-id="63558-407">**Start-MailboxSearch**</span></span>
    
- <span data-ttu-id="63558-408">**STOP-MailboxSearch**</span><span class="sxs-lookup"><span data-stu-id="63558-408">**Stop-MailboxSearch**</span></span>
    
- <span data-ttu-id="63558-409">**Disable-MailPublicFolder**</span><span class="sxs-lookup"><span data-stu-id="63558-409">**Disable-MailPublicFolder**</span></span>
    
- <span data-ttu-id="63558-410">**Get-MailPublicFolder**</span><span class="sxs-lookup"><span data-stu-id="63558-410">**Get-MailPublicFolder**</span></span>
    
- <span data-ttu-id="63558-411">**SET-MailPublicFolder**</span><span class="sxs-lookup"><span data-stu-id="63558-411">**Set-MailPublicFolder**</span></span>
    
- <span data-ttu-id="63558-412">**Get-MigrationBatch**</span><span class="sxs-lookup"><span data-stu-id="63558-412">**Get-MigrationBatch**</span></span>
    
- <span data-ttu-id="63558-413">**Новый MigrationBatch**</span><span class="sxs-lookup"><span data-stu-id="63558-413">**New-MigrationBatch**</span></span>
    
- <span data-ttu-id="63558-414">**SET-MigrationBatch**</span><span class="sxs-lookup"><span data-stu-id="63558-414">**Set-MigrationBatch**</span></span>
    
- <span data-ttu-id="63558-415">**Test-MigrationServerAvailability**</span><span class="sxs-lookup"><span data-stu-id="63558-415">**Test-MigrationServerAvailability**</span></span>
    
- <span data-ttu-id="63558-416">**Get-MoveRequest**</span><span class="sxs-lookup"><span data-stu-id="63558-416">**Get-MoveRequest**</span></span>
    
- <span data-ttu-id="63558-417">**Новый OfflineAddressBook**</span><span class="sxs-lookup"><span data-stu-id="63558-417">**New-OfflineAddressBook**</span></span>
    
- <span data-ttu-id="63558-418">**Get-OrganizationConfig**</span><span class="sxs-lookup"><span data-stu-id="63558-418">**Get-OrganizationConfig**</span></span>
    
- <span data-ttu-id="63558-419">**SET-OrganizationConfig**</span><span class="sxs-lookup"><span data-stu-id="63558-419">**Set-OrganizationConfig**</span></span>
    
- <span data-ttu-id="63558-420">**Test-OutlookConnectivity**</span><span class="sxs-lookup"><span data-stu-id="63558-420">**Test-OutlookConnectivity**</span></span>
    
- <span data-ttu-id="63558-421">**Test-OutlookWebServices**</span><span class="sxs-lookup"><span data-stu-id="63558-421">**Test-OutlookWebServices**</span></span>
    
- <span data-ttu-id="63558-422">**Get-OwaMailboxPolicy**</span><span class="sxs-lookup"><span data-stu-id="63558-422">**Get-OwaMailboxPolicy**</span></span>
    
- <span data-ttu-id="63558-423">**Новые OwaVirtualDirectory**</span><span class="sxs-lookup"><span data-stu-id="63558-423">**New-OwaVirtualDirectory**</span></span>
    
- <span data-ttu-id="63558-424">**Новый PowerShellVirtualDirectory**</span><span class="sxs-lookup"><span data-stu-id="63558-424">**New-PowerShellVirtualDirectory**</span></span>
    
- <span data-ttu-id="63558-425">**Get-PublicFolder**</span><span class="sxs-lookup"><span data-stu-id="63558-425">**Get-PublicFolder**</span></span>
    
- <span data-ttu-id="63558-426">**Новые PublicFolder**</span><span class="sxs-lookup"><span data-stu-id="63558-426">**New-PublicFolder**</span></span>
    
- <span data-ttu-id="63558-427">**SET-PublicFolder**</span><span class="sxs-lookup"><span data-stu-id="63558-427">**Set-PublicFolder**</span></span>
    
- <span data-ttu-id="63558-428">**Добавление PublicFolderClientPermission**</span><span class="sxs-lookup"><span data-stu-id="63558-428">**Add-PublicFolderClientPermission**</span></span>
    
- <span data-ttu-id="63558-429">**Get-PublicFolderClientPermission**</span><span class="sxs-lookup"><span data-stu-id="63558-429">**Get-PublicFolderClientPermission**</span></span>
    
- <span data-ttu-id="63558-430">**Remove-PublicFolderClientPermission**</span><span class="sxs-lookup"><span data-stu-id="63558-430">**Remove-PublicFolderClientPermission**</span></span>
    
- <span data-ttu-id="63558-431">**Get-PublicFolderItemStatistics**</span><span class="sxs-lookup"><span data-stu-id="63558-431">**Get-PublicFolderItemStatistics**</span></span>
    
- <span data-ttu-id="63558-432">**Get-PublicFolderStatistics**</span><span class="sxs-lookup"><span data-stu-id="63558-432">**Get-PublicFolderStatistics**</span></span>
    
- <span data-ttu-id="63558-433">**Get-Recipient**</span><span class="sxs-lookup"><span data-stu-id="63558-433">**Get-Recipient**</span></span>
    
- <span data-ttu-id="63558-434">**SET-ResourceConfig**</span><span class="sxs-lookup"><span data-stu-id="63558-434">**Set-ResourceConfig**</span></span>
    
- <span data-ttu-id="63558-435">**Test-WebServicesConnectivity**</span><span class="sxs-lookup"><span data-stu-id="63558-435">**Test-WebServicesConnectivity**</span></span>
    
- <span data-ttu-id="63558-436">**Новый WebServicesVirtualDirectory**</span><span class="sxs-lookup"><span data-stu-id="63558-436">**New-WebServicesVirtualDirectory**</span></span>
    
### <a name="removed-cmdlets"></a><span data-ttu-id="63558-437">Удаленные командлеты</span><span class="sxs-lookup"><span data-stu-id="63558-437">Removed cmdlets</span></span>
<span data-ttu-id="63558-438"><a name="bk_removed"> </a></span><span class="sxs-lookup"><span data-stu-id="63558-438"></span></span>

<span data-ttu-id="63558-439">Следующие командлеты были удалены из Exchange 2013.</span><span class="sxs-lookup"><span data-stu-id="63558-439">The following cmdlets were removed from Exchange 2013:</span></span>
  
- <span data-ttu-id="63558-440">**Обновление FileDistributionService**</span><span class="sxs-lookup"><span data-stu-id="63558-440">**Update-FileDistributionService**</span></span>
    
- <span data-ttu-id="63558-441">**Почтовый ящик восстановления**</span><span class="sxs-lookup"><span data-stu-id="63558-441">**Restore-Mailbox**</span></span>
    
- <span data-ttu-id="63558-442">**Очистить MailboxDatabase**</span><span class="sxs-lookup"><span data-stu-id="63558-442">**Clean-MailboxDatabase**</span></span>
    
- <span data-ttu-id="63558-443">**Выполнения переноса**</span><span class="sxs-lookup"><span data-stu-id="63558-443">**Complete-Migration**</span></span>
    
- <span data-ttu-id="63558-444">**Get-MigrationStatus**</span><span class="sxs-lookup"><span data-stu-id="63558-444">**Get-MigrationStatus**</span></span>
    
- <span data-ttu-id="63558-445">**Update-PublicFolder**</span><span class="sxs-lookup"><span data-stu-id="63558-445">**Update-PublicFolder**</span></span>
    
- <span data-ttu-id="63558-446">**Добавление PublicFolderAdministrativePermission**</span><span class="sxs-lookup"><span data-stu-id="63558-446">**Add-PublicFolderAdministrativePermission**</span></span>
    
- <span data-ttu-id="63558-447">**Get-PublicFolderAdministrativePermission**</span><span class="sxs-lookup"><span data-stu-id="63558-447">**Get-PublicFolderAdministrativePermission**</span></span>
    
- <span data-ttu-id="63558-448">**Remove-PublicFolderAdministrativePermission**</span><span class="sxs-lookup"><span data-stu-id="63558-448">**Remove-PublicFolderAdministrativePermission**</span></span>
    
- <span data-ttu-id="63558-449">**Новый PublicFolderDatabase**</span><span class="sxs-lookup"><span data-stu-id="63558-449">**New-PublicFolderDatabase**</span></span>
    
- <span data-ttu-id="63558-450">**Remove-PublicFolderDatabase**</span><span class="sxs-lookup"><span data-stu-id="63558-450">**Remove-PublicFolderDatabase**</span></span>
    
- <span data-ttu-id="63558-451">**SET-PublicFolderDatabase**</span><span class="sxs-lookup"><span data-stu-id="63558-451">**Set-PublicFolderDatabase**</span></span>
    
- <span data-ttu-id="63558-452">**Новый PublicFolderDatabaseRepairRequest**</span><span class="sxs-lookup"><span data-stu-id="63558-452">**New-PublicFolderDatabaseRepairRequest**</span></span>
    
- <span data-ttu-id="63558-453">**Обновление PublicFolderHierarchy**</span><span class="sxs-lookup"><span data-stu-id="63558-453">**Update-PublicFolderHierarchy**</span></span>
    
- <span data-ttu-id="63558-454">**Возобновление PublicFolderReplication**</span><span class="sxs-lookup"><span data-stu-id="63558-454">**Resume-PublicFolderReplication**</span></span>
    
- <span data-ttu-id="63558-455">**Приостановка PublicFolderReplication**</span><span class="sxs-lookup"><span data-stu-id="63558-455">**Suspend-PublicFolderReplication**</span></span>
    
- <span data-ttu-id="63558-456">**Start-RetentionAutoTagLearning**</span><span class="sxs-lookup"><span data-stu-id="63558-456">**Start-RetentionAutoTagLearning**</span></span>
    
- <span data-ttu-id="63558-457">**Test-SystemHealth**</span><span class="sxs-lookup"><span data-stu-id="63558-457">**Test-SystemHealth**</span></span>
    
- <span data-ttu-id="63558-458">**Отключить свойств**</span><span class="sxs-lookup"><span data-stu-id="63558-458">**Disable-UMServer**</span></span>
    
- <span data-ttu-id="63558-459">**Enable свойств**</span><span class="sxs-lookup"><span data-stu-id="63558-459">**Enable-UMServer**</span></span>
    
- <span data-ttu-id="63558-460">**Get свойств**</span><span class="sxs-lookup"><span data-stu-id="63558-460">**Get-UMServer**</span></span>
    
- <span data-ttu-id="63558-461">**Свойств**</span><span class="sxs-lookup"><span data-stu-id="63558-461">**Set-UMServer**</span></span>
    
## <a name="see-also"></a><span data-ttu-id="63558-462">См. также</span><span class="sxs-lookup"><span data-stu-id="63558-462">See also</span></span>

- [<span data-ttu-id="63558-463">Входные данные командлета Командная консоль Exchange и вывод типов</span><span class="sxs-lookup"><span data-stu-id="63558-463">Exchange Management Shell cmdlet input and output types</span></span>](exchange-management-shell-cmdlet-input-and-output-types.md)    
- [<span data-ttu-id="63558-464">Ознакомьтесь со списком пользователей почты с помощью командной консоли Exchange</span><span class="sxs-lookup"><span data-stu-id="63558-464">Get a list of mail users by using the Exchange Management Shell</span></span>](how-to-get-a-list-of-mail-users-by-using-the-exchange-management-shell.md)    
- [<span data-ttu-id="63558-465">Командлеты Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="63558-465">Exchange 2013 cmdlets</span></span>](http://technet.microsoft.com/ru-ru/library/bb124413%28v=exchg.150%29.aspx)
    

