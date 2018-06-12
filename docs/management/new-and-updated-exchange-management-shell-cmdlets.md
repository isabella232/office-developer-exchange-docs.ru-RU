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
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761298"
---
# <a name="new-and-updated-exchange-management-shell-cmdlets"></a><span data-ttu-id="92070-103">Новые и обновленные командлеты командной консоли Exchange</span><span class="sxs-lookup"><span data-stu-id="92070-103">New and updated Exchange Management Shell cmdlets</span></span>

<span data-ttu-id="92070-104">Найдите сведения о новых возможностях в командной консоли Exchange в Exchange.</span><span class="sxs-lookup"><span data-stu-id="92070-104">Find information about what's new in the Exchange Management Shell in Exchange.</span></span>
  
<span data-ttu-id="92070-105">**Применимо к:** Exchange Online | Exchange Server 2013 | Office 365</span><span class="sxs-lookup"><span data-stu-id="92070-105">**Applies to:** Exchange Online | Exchange Server 2013 | Office 365</span></span>
  
<span data-ttu-id="92070-106">В этой статье сведения о новых командлетов командной консоли управления Exchange, командлеты, которые были изменены за и командлеты, которые были удалены из Exchange Online, Exchange Online в составе Office 365 или локальной версией Exchange.</span><span class="sxs-lookup"><span data-stu-id="92070-106">This article provides information about new Exchange Management shell cmdlets, cmdlets that were modified in, and cmdlets that were removed from Exchange Online, Exchange Online as part of Office 365, or an on-premises version of Exchange.</span></span>
  
## <a name="new-and-updated-cmdlets-in-exchange-2013-sp1"></a><span data-ttu-id="92070-107">Новые и обновленные командлеты в Exchange 2013 с пакетом обновления 1</span><span class="sxs-lookup"><span data-stu-id="92070-107">New and updated cmdlets in Exchange 2013 SP1</span></span>

### <a name="new-cmdlets"></a><span data-ttu-id="92070-108">Новые командлеты</span><span class="sxs-lookup"><span data-stu-id="92070-108">New cmdlets</span></span>

<span data-ttu-id="92070-109">Следующие командлеты были представлены в построении 15.00.0847.032 (Exchange Server 2013 с пакетом обновления 1):</span><span class="sxs-lookup"><span data-stu-id="92070-109">The following cmdlets were introduced in build 15.00.0847.032 (Exchange Server 2013 SP1):</span></span>
  
- <span data-ttu-id="92070-110">**Get-AuthRedirect**</span><span class="sxs-lookup"><span data-stu-id="92070-110">**Get-AuthRedirect**</span></span>
    
- <span data-ttu-id="92070-111">**Новый AuthRedirect**</span><span class="sxs-lookup"><span data-stu-id="92070-111">**New-AuthRedirect**</span></span>
    
- <span data-ttu-id="92070-112">**Remove-AuthRedirect**</span><span class="sxs-lookup"><span data-stu-id="92070-112">**Remove-AuthRedirect**</span></span>
    
- <span data-ttu-id="92070-113">**SET-AuthRedirect**</span><span class="sxs-lookup"><span data-stu-id="92070-113">**Set-AuthRedirect**</span></span>
    
- <span data-ttu-id="92070-114">**Новый DataClassification**</span><span class="sxs-lookup"><span data-stu-id="92070-114">**New-DataClassification**</span></span>
    
- <span data-ttu-id="92070-115">**Remove-DataClassification**</span><span class="sxs-lookup"><span data-stu-id="92070-115">**Remove-DataClassification**</span></span>
    
- <span data-ttu-id="92070-116">**SET-DataClassification**</span><span class="sxs-lookup"><span data-stu-id="92070-116">**Set-DataClassification**</span></span>
    
- <span data-ttu-id="92070-117">**Новый отпечаток**</span><span class="sxs-lookup"><span data-stu-id="92070-117">**New-FingerPrint**</span></span>
    
- <span data-ttu-id="92070-118">**Get-MapiVirtualDirectory\***</span><span class="sxs-lookup"><span data-stu-id="92070-118">**Get-MapiVirtualDirectory\***</span></span>
    
- <span data-ttu-id="92070-119">**Новый MapiVirtualDirectory\***</span><span class="sxs-lookup"><span data-stu-id="92070-119">**New-MapiVirtualDirectory\***</span></span>
    
- <span data-ttu-id="92070-120">**Remove-MapiVirtualDirectory\***</span><span class="sxs-lookup"><span data-stu-id="92070-120">**Remove-MapiVirtualDirectory\***</span></span>
    
- <span data-ttu-id="92070-121">**SET-MapiVirtualDirectory\***</span><span class="sxs-lookup"><span data-stu-id="92070-121">**Set-MapiVirtualDirectory\***</span></span>
    
- <span data-ttu-id="92070-122">**Get-OMEConfiguration**</span><span class="sxs-lookup"><span data-stu-id="92070-122">**Get-OMEConfiguration**</span></span>
    
- <span data-ttu-id="92070-123">**SET-OMEConfiguration**</span><span class="sxs-lookup"><span data-stu-id="92070-123">**Set-OMEConfiguration**</span></span>
    
- <span data-ttu-id="92070-124">**Get-SmimeConfig**</span><span class="sxs-lookup"><span data-stu-id="92070-124">**Get-SmimeConfig**</span></span>
    
- <span data-ttu-id="92070-125">**SET-SmimeConfig**</span><span class="sxs-lookup"><span data-stu-id="92070-125">**Set-SmimeConfig**</span></span>
    
- <span data-ttu-id="92070-126">**Get-IntraOrganizationConfiguration**</span><span class="sxs-lookup"><span data-stu-id="92070-126">**Get-IntraOrganizationConfiguration**</span></span>
    
- <span data-ttu-id="92070-127">**Get-IntraOrganizationConnector**</span><span class="sxs-lookup"><span data-stu-id="92070-127">**Get-IntraOrganizationConnector**</span></span>
    
- <span data-ttu-id="92070-128">**Новый IntraOrganizationConnector**</span><span class="sxs-lookup"><span data-stu-id="92070-128">**New-IntraOrganizationConnector**</span></span>
    
- <span data-ttu-id="92070-129">**Remove-IntraOrganizationConnector**</span><span class="sxs-lookup"><span data-stu-id="92070-129">**Remove-IntraOrganizationConnector**</span></span>
    
- <span data-ttu-id="92070-130">**SET-IntraOrganizationConnector**</span><span class="sxs-lookup"><span data-stu-id="92070-130">**Set-IntraOrganizationConnector**</span></span>
    
- <span data-ttu-id="92070-131">**Get-HistoricalSearch**</span><span class="sxs-lookup"><span data-stu-id="92070-131">**Get-HistoricalSearch**</span></span>
    
- <span data-ttu-id="92070-132">**Start-HistoricalSearch**</span><span class="sxs-lookup"><span data-stu-id="92070-132">**Start-HistoricalSearch**</span></span>
    
- <span data-ttu-id="92070-133">**STOP-HistoricalSearch**</span><span class="sxs-lookup"><span data-stu-id="92070-133">**Stop-HistoricalSearch**</span></span>
    
- <span data-ttu-id="92070-134">**Новый SearchDocumentFormat**</span><span class="sxs-lookup"><span data-stu-id="92070-134">**New-SearchDocumentFormat**</span></span>
    
- <span data-ttu-id="92070-135">**Remove-SearchDocumentFormat**</span><span class="sxs-lookup"><span data-stu-id="92070-135">**Remove-SearchDocumentFormat**</span></span>
    
### <a name="updated-cmdlets"></a><span data-ttu-id="92070-136">Обновленные командлеты</span><span class="sxs-lookup"><span data-stu-id="92070-136">Updated cmdlets</span></span>

<span data-ttu-id="92070-137">Следующие командлеты были обновлены в построении 15.00.0847.032 (Exchange 2013 с пакетом обновления 1):</span><span class="sxs-lookup"><span data-stu-id="92070-137">The following cmdlets were updated in build 15.00.0847.032 (Exchange 2013 SP1):</span></span>
  
- <span data-ttu-id="92070-138">**Get-AuditLogSearch**</span><span class="sxs-lookup"><span data-stu-id="92070-138">**Get-AuditLogSearch**</span></span>
    
- <span data-ttu-id="92070-139">**Get-QuarantineMessage**</span><span class="sxs-lookup"><span data-stu-id="92070-139">**Get-QuarantineMessage**</span></span>
    
- <span data-ttu-id="92070-140">**Новый InboundConnector**</span><span class="sxs-lookup"><span data-stu-id="92070-140">**New-InboundConnector**</span></span>
    
- <span data-ttu-id="92070-141">**Новый MailboxDatabase**</span><span class="sxs-lookup"><span data-stu-id="92070-141">**New-MailboxDatabase**</span></span>
    
- <span data-ttu-id="92070-142">**Новый PublicFolderMoveRequest**</span><span class="sxs-lookup"><span data-stu-id="92070-142">**New-PublicFolderMoveRequest**</span></span>
    
- <span data-ttu-id="92070-143">**New-TransportRule**</span><span class="sxs-lookup"><span data-stu-id="92070-143">**New-TransportRule**</span></span>
    
- <span data-ttu-id="92070-144">**SET-FrontendTransportService**</span><span class="sxs-lookup"><span data-stu-id="92070-144">**Set-FrontendTransportService**</span></span>
    
- <span data-ttu-id="92070-145">**SET-InboundConnector**</span><span class="sxs-lookup"><span data-stu-id="92070-145">**Set-InboundConnector**</span></span>
    
- <span data-ttu-id="92070-146">**Set-Mailbox**</span><span class="sxs-lookup"><span data-stu-id="92070-146">**Set-Mailbox**</span></span>
    
- <span data-ttu-id="92070-147">**SET-MailboxTransportService**</span><span class="sxs-lookup"><span data-stu-id="92070-147">**Set-MailboxTransportService**</span></span>
    
- <span data-ttu-id="92070-148">**SET-MoveRequest**</span><span class="sxs-lookup"><span data-stu-id="92070-148">**Set-MoveRequest**</span></span>
    
- <span data-ttu-id="92070-149">**SET-OrganizationConfig**</span><span class="sxs-lookup"><span data-stu-id="92070-149">**Set-OrganizationConfig**</span></span>
    
- <span data-ttu-id="92070-150">**SET-OwaMailboxPolicy**</span><span class="sxs-lookup"><span data-stu-id="92070-150">**Set-OwaMailboxPolicy**</span></span>
    
- <span data-ttu-id="92070-151">**SET-OwaVirtualDirectory**</span><span class="sxs-lookup"><span data-stu-id="92070-151">**Set-OwaVirtualDirectory**</span></span>
    
- <span data-ttu-id="92070-152">**Set-TransportConfig**</span><span class="sxs-lookup"><span data-stu-id="92070-152">**Set-TransportConfig**</span></span>
    
- <span data-ttu-id="92070-153">**SET-TransportRule**</span><span class="sxs-lookup"><span data-stu-id="92070-153">**Set-TransportRule**</span></span>
    
- <span data-ttu-id="92070-154">**SET-TransportServer**</span><span class="sxs-lookup"><span data-stu-id="92070-154">**Set-TransportServer**</span></span>
    
- <span data-ttu-id="92070-155">**SET-TransportService**</span><span class="sxs-lookup"><span data-stu-id="92070-155">**Set-TransportService**</span></span>
    
- <span data-ttu-id="92070-156">**Test-MRSHealth**</span><span class="sxs-lookup"><span data-stu-id="92070-156">**Test-MRSHealth**</span></span>
    
- <span data-ttu-id="92070-157">**Test-OAuthConnectivity**</span><span class="sxs-lookup"><span data-stu-id="92070-157">**Test-OAuthConnectivity**</span></span>
    
### <a name="removed-cmdlets"></a><span data-ttu-id="92070-158">Удаленные командлеты</span><span class="sxs-lookup"><span data-stu-id="92070-158">Removed cmdlets</span></span>

<span data-ttu-id="92070-159">Следующие командлеты были удалены из построения 15.00.0847.032 (Exchange 2013 с пакетом обновления 1):</span><span class="sxs-lookup"><span data-stu-id="92070-159">The following cmdlets were removed from build 15.00.0847.032 (Exchange 2013 SP1):</span></span>
  
- <span data-ttu-id="92070-160">**Get-AvailabilityReportOutage**</span><span class="sxs-lookup"><span data-stu-id="92070-160">**Get-AvailabilityReportOutage**</span></span>
    
- <span data-ttu-id="92070-161">**Новый AvailabilityReportOutage**</span><span class="sxs-lookup"><span data-stu-id="92070-161">**New-AvailabilityReportOutage**</span></span>
    
- <span data-ttu-id="92070-162">**Remove-AvailabilityReportOutage**</span><span class="sxs-lookup"><span data-stu-id="92070-162">**Remove-AvailabilityReportOutage**</span></span>
    
- <span data-ttu-id="92070-163">**SET-AvailabilityReportOutage**</span><span class="sxs-lookup"><span data-stu-id="92070-163">**Set-AvailabilityReportOutage**</span></span>
    
## <a name="new-and-updated-cmdlets-in-exchange-2013"></a><span data-ttu-id="92070-164">Новые и обновленные командлеты в Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="92070-164">New and updated cmdlets in Exchange 2013</span></span>

### <a name="new-cmdlets"></a><span data-ttu-id="92070-165">Новые командлеты</span><span class="sxs-lookup"><span data-stu-id="92070-165">New cmdlets</span></span>
<span data-ttu-id="92070-166"><a name="bk_new"> </a></span><span class="sxs-lookup"><span data-stu-id="92070-166"></span></span>

<span data-ttu-id="92070-167">В Exchange 2013 появились следующие командлеты:</span><span class="sxs-lookup"><span data-stu-id="92070-167">The following cmdlets were introduced in Exchange 2013:</span></span>
  
- <span data-ttu-id="92070-168">**Get-ActiveSyncDeviceAutoblockThreshold**</span><span class="sxs-lookup"><span data-stu-id="92070-168">**Get-ActiveSyncDeviceAutoblockThreshold**</span></span>
    
- <span data-ttu-id="92070-169">**SET-ActiveSyncDeviceAutoblockThreshold**</span><span class="sxs-lookup"><span data-stu-id="92070-169">**Set-ActiveSyncDeviceAutoblockThreshold**</span></span>
    
- <span data-ttu-id="92070-170">**Disable-App**</span><span class="sxs-lookup"><span data-stu-id="92070-170">**Disable-App**</span></span>
    
- <span data-ttu-id="92070-171">**Enable-App**</span><span class="sxs-lookup"><span data-stu-id="92070-171">**Enable-App**</span></span>
    
- <span data-ttu-id="92070-172">**Get-App**</span><span class="sxs-lookup"><span data-stu-id="92070-172">**Get-App**</span></span>
    
- <span data-ttu-id="92070-173">**Создание приложения**</span><span class="sxs-lookup"><span data-stu-id="92070-173">**New-App**</span></span>
    
- <span data-ttu-id="92070-174">**Remove-App**</span><span class="sxs-lookup"><span data-stu-id="92070-174">**Remove-App**</span></span>
    
- <span data-ttu-id="92070-175">**SET-App**</span><span class="sxs-lookup"><span data-stu-id="92070-175">**Set-App**</span></span>
    
- <span data-ttu-id="92070-176">**Get-AuthConfig**</span><span class="sxs-lookup"><span data-stu-id="92070-176">**Get-AuthConfig**</span></span>
    
- <span data-ttu-id="92070-177">**SET-AuthConfig**</span><span class="sxs-lookup"><span data-stu-id="92070-177">**Set-AuthConfig**</span></span>
    
- <span data-ttu-id="92070-178">**Get-AuthServer**</span><span class="sxs-lookup"><span data-stu-id="92070-178">**Get-AuthServer**</span></span>
    
- <span data-ttu-id="92070-179">**Новый AuthServer**</span><span class="sxs-lookup"><span data-stu-id="92070-179">**New-AuthServer**</span></span>
    
- <span data-ttu-id="92070-180">**Remove-AuthServer**</span><span class="sxs-lookup"><span data-stu-id="92070-180">**Remove-AuthServer**</span></span>
    
- <span data-ttu-id="92070-181">**SET-AuthServer**</span><span class="sxs-lookup"><span data-stu-id="92070-181">**Set-AuthServer**</span></span>
    
- <span data-ttu-id="92070-182">**Новый AvailabilityConfig**</span><span class="sxs-lookup"><span data-stu-id="92070-182">**New-AvailabilityConfig**</span></span>
    
- <span data-ttu-id="92070-183">**Remove-AvailabilityConfig**</span><span class="sxs-lookup"><span data-stu-id="92070-183">**Remove-AvailabilityConfig**</span></span>
    
- <span data-ttu-id="92070-184">**Get-CalendarDiagnosticAnalysis**</span><span class="sxs-lookup"><span data-stu-id="92070-184">**Get-CalendarDiagnosticAnalysis**</span></span>
    
- <span data-ttu-id="92070-185">**Get-ClassificationRuleCollection**</span><span class="sxs-lookup"><span data-stu-id="92070-185">**Get-ClassificationRuleCollection**</span></span>
    
- <span data-ttu-id="92070-186">**Новый ClassificationRuleCollection**</span><span class="sxs-lookup"><span data-stu-id="92070-186">**New-ClassificationRuleCollection**</span></span>
    
- <span data-ttu-id="92070-187">**Remove-ClassificationRuleCollection**</span><span class="sxs-lookup"><span data-stu-id="92070-187">**Remove-ClassificationRuleCollection**</span></span>
    
- <span data-ttu-id="92070-188">**SET-ClassificationRuleCollection**</span><span class="sxs-lookup"><span data-stu-id="92070-188">**Set-ClassificationRuleCollection**</span></span>
    
- <span data-ttu-id="92070-189">**Get-ConnectSubscription**</span><span class="sxs-lookup"><span data-stu-id="92070-189">**Get-ConnectSubscription**</span></span>
    
- <span data-ttu-id="92070-190">**Новый ConnectSubscription**</span><span class="sxs-lookup"><span data-stu-id="92070-190">**New-ConnectSubscription**</span></span>
    
- <span data-ttu-id="92070-191">**Remove-ConnectSubscription**</span><span class="sxs-lookup"><span data-stu-id="92070-191">**Remove-ConnectSubscription**</span></span>
    
- <span data-ttu-id="92070-192">**SET-ConnectSubscription**</span><span class="sxs-lookup"><span data-stu-id="92070-192">**Set-ConnectSubscription**</span></span>
    
- <span data-ttu-id="92070-193">**Get-DataClassification**</span><span class="sxs-lookup"><span data-stu-id="92070-193">**Get-DataClassification**</span></span>
    
- <span data-ttu-id="92070-194">**Get-DataClassificationConfig**</span><span class="sxs-lookup"><span data-stu-id="92070-194">**Get-DataClassificationConfig**</span></span>
    
- <span data-ttu-id="92070-195">**Get-DlpPolicy**</span><span class="sxs-lookup"><span data-stu-id="92070-195">**Get-DlpPolicy**</span></span>
    
- <span data-ttu-id="92070-196">**Новый DlpPolicy**</span><span class="sxs-lookup"><span data-stu-id="92070-196">**New-DlpPolicy**</span></span>
    
- <span data-ttu-id="92070-197">**Remove-DlpPolicy**</span><span class="sxs-lookup"><span data-stu-id="92070-197">**Remove-DlpPolicy**</span></span>
    
- <span data-ttu-id="92070-198">**SET-DlpPolicy**</span><span class="sxs-lookup"><span data-stu-id="92070-198">**Set-DlpPolicy**</span></span>
    
- <span data-ttu-id="92070-199">**Export-DlpPolicyCollection**</span><span class="sxs-lookup"><span data-stu-id="92070-199">**Export-DlpPolicyCollection**</span></span>
    
- <span data-ttu-id="92070-200">**Import-DlpPolicyCollection**</span><span class="sxs-lookup"><span data-stu-id="92070-200">**Import-DlpPolicyCollection**</span></span>
    
- <span data-ttu-id="92070-201">**Get-DlpPolicyTemplate**</span><span class="sxs-lookup"><span data-stu-id="92070-201">**Get-DlpPolicyTemplate**</span></span>
    
- <span data-ttu-id="92070-202">**Import-DlpPolicyTemplate**</span><span class="sxs-lookup"><span data-stu-id="92070-202">**Import-DlpPolicyTemplate**</span></span>
    
- <span data-ttu-id="92070-203">**Remove-DlpPolicyTemplate**</span><span class="sxs-lookup"><span data-stu-id="92070-203">**Remove-DlpPolicyTemplate**</span></span>
    
- <span data-ttu-id="92070-204">**Get-ExchangeServerAccessLicense**</span><span class="sxs-lookup"><span data-stu-id="92070-204">**Get-ExchangeServerAccessLicense**</span></span>
    
- <span data-ttu-id="92070-205">**Get-ExchangeServerAccessLicenseUser**</span><span class="sxs-lookup"><span data-stu-id="92070-205">**Get-ExchangeServerAccessLicenseUser**</span></span>
    
- <span data-ttu-id="92070-206">**Get-FfoMigrationReport**</span><span class="sxs-lookup"><span data-stu-id="92070-206">**Get-FfoMigrationReport**</span></span>
    
- <span data-ttu-id="92070-207">**Get-FrontendTransportService**</span><span class="sxs-lookup"><span data-stu-id="92070-207">**Get-FrontendTransportService**</span></span>
    
- <span data-ttu-id="92070-208">**SET-FrontendTransportService**</span><span class="sxs-lookup"><span data-stu-id="92070-208">**Set-FrontendTransportService**</span></span>
    
- <span data-ttu-id="92070-209">**Добавление GlobalMonitoringOverride**</span><span class="sxs-lookup"><span data-stu-id="92070-209">**Add-GlobalMonitoringOverride**</span></span>
    
- <span data-ttu-id="92070-210">**Get-GlobalMonitoringOverride**</span><span class="sxs-lookup"><span data-stu-id="92070-210">**Get-GlobalMonitoringOverride**</span></span>
    
- <span data-ttu-id="92070-211">**Remove-GlobalMonitoringOverride**</span><span class="sxs-lookup"><span data-stu-id="92070-211">**Remove-GlobalMonitoringOverride**</span></span>
    
- <span data-ttu-id="92070-212">**Get-GroupActivityReport**</span><span class="sxs-lookup"><span data-stu-id="92070-212">**Get-GroupActivityReport**</span></span>
    
- <span data-ttu-id="92070-213">**Get-HealthReport**</span><span class="sxs-lookup"><span data-stu-id="92070-213">**Get-HealthReport**</span></span>
    
- <span data-ttu-id="92070-214">**Get-HostedConnectionFilterPolicy**</span><span class="sxs-lookup"><span data-stu-id="92070-214">**Get-HostedConnectionFilterPolicy**</span></span>
    
- <span data-ttu-id="92070-215">**Новый HostedConnectionFilterPolicy**</span><span class="sxs-lookup"><span data-stu-id="92070-215">**New-HostedConnectionFilterPolicy**</span></span>
    
- <span data-ttu-id="92070-216">**Remove-HostedConnectionFilterPolicy**</span><span class="sxs-lookup"><span data-stu-id="92070-216">**Remove-HostedConnectionFilterPolicy**</span></span>
    
- <span data-ttu-id="92070-217">**SET-HostedConnectionFilterPolicy**</span><span class="sxs-lookup"><span data-stu-id="92070-217">**Set-HostedConnectionFilterPolicy**</span></span>
    
- <span data-ttu-id="92070-218">**Get-HostedContentFilterPolicy**</span><span class="sxs-lookup"><span data-stu-id="92070-218">**Get-HostedContentFilterPolicy**</span></span>
    
- <span data-ttu-id="92070-219">**New-HostedContentFilterPolicy**</span><span class="sxs-lookup"><span data-stu-id="92070-219">**New-HostedContentFilterPolicy**</span></span>
    
- <span data-ttu-id="92070-220">**Remove-HostedContentFilterPolicy**</span><span class="sxs-lookup"><span data-stu-id="92070-220">**Remove-HostedContentFilterPolicy**</span></span>
    
- <span data-ttu-id="92070-221">**SET-HostedContentFilterPolicy**</span><span class="sxs-lookup"><span data-stu-id="92070-221">**Set-HostedContentFilterPolicy**</span></span>
    
- <span data-ttu-id="92070-222">**Get-HostedOutboundSpamFilterPolicy**</span><span class="sxs-lookup"><span data-stu-id="92070-222">**Get-HostedOutboundSpamFilterPolicy**</span></span>
    
- <span data-ttu-id="92070-223">**SET-HostedOutboundSpamFilterPolicy**</span><span class="sxs-lookup"><span data-stu-id="92070-223">**Set-HostedOutboundSpamFilterPolicy**</span></span>
    
- <span data-ttu-id="92070-224">**Remove-HybridConfiguration**</span><span class="sxs-lookup"><span data-stu-id="92070-224">**Remove-HybridConfiguration**</span></span>
    
- <span data-ttu-id="92070-225">**Get-HybridMailflow**</span><span class="sxs-lookup"><span data-stu-id="92070-225">**Get-HybridMailflow**</span></span>
    
- <span data-ttu-id="92070-226">**SET Hybridmailflowиспользуется**</span><span class="sxs-lookup"><span data-stu-id="92070-226">**Set-HybridMailflow**</span></span>
    
- <span data-ttu-id="92070-227">**Get-HybridMailflowDatacenterIPs**</span><span class="sxs-lookup"><span data-stu-id="92070-227">**Get-HybridMailflowDatacenterIPs**</span></span>
    
- <span data-ttu-id="92070-228">**Get-InboundConnector**</span><span class="sxs-lookup"><span data-stu-id="92070-228">**Get-InboundConnector**</span></span>
    
- <span data-ttu-id="92070-229">**Новый InboundConnector**</span><span class="sxs-lookup"><span data-stu-id="92070-229">**New-InboundConnector**</span></span>
    
- <span data-ttu-id="92070-230">**Remove-InboundConnector**</span><span class="sxs-lookup"><span data-stu-id="92070-230">**Remove-InboundConnector**</span></span>
    
- <span data-ttu-id="92070-231">**SET-InboundConnector**</span><span class="sxs-lookup"><span data-stu-id="92070-231">**Set-InboundConnector**</span></span>
    
- <span data-ttu-id="92070-232">**Get-MailboxActivityReport**</span><span class="sxs-lookup"><span data-stu-id="92070-232">**Get-MailboxActivityReport**</span></span>
    
- <span data-ttu-id="92070-233">**Disable-MailboxQuarantine**</span><span class="sxs-lookup"><span data-stu-id="92070-233">**Disable-MailboxQuarantine**</span></span>
    
- <span data-ttu-id="92070-234">**Enable-MailboxQuarantine**</span><span class="sxs-lookup"><span data-stu-id="92070-234">**Enable-MailboxQuarantine**</span></span>
    
- <span data-ttu-id="92070-235">**Get-MailboxTransportService**</span><span class="sxs-lookup"><span data-stu-id="92070-235">**Get-MailboxTransportService**</span></span>
    
- <span data-ttu-id="92070-236">**SET-MailboxTransportService**</span><span class="sxs-lookup"><span data-stu-id="92070-236">**Set-MailboxTransportService**</span></span>
    
- <span data-ttu-id="92070-237">**Get-MailDetailDlpPolicyReport**</span><span class="sxs-lookup"><span data-stu-id="92070-237">**Get-MailDetailDlpPolicyReport**</span></span>
    
- <span data-ttu-id="92070-238">**Get-MailDetailMalwareReport**</span><span class="sxs-lookup"><span data-stu-id="92070-238">**Get-MailDetailMalwareReport**</span></span>
    
- <span data-ttu-id="92070-239">**Get-MailDetailReport**</span><span class="sxs-lookup"><span data-stu-id="92070-239">**Get-MailDetailReport**</span></span>
    
- <span data-ttu-id="92070-240">**Get-MailDetailSpamReport**</span><span class="sxs-lookup"><span data-stu-id="92070-240">**Get-MailDetailSpamReport**</span></span>
    
- <span data-ttu-id="92070-241">**Get-MailDetailTransportRuleReport**</span><span class="sxs-lookup"><span data-stu-id="92070-241">**Get-MailDetailTransportRuleReport**</span></span>
    
- <span data-ttu-id="92070-242">**Get-MailFilterListReport**</span><span class="sxs-lookup"><span data-stu-id="92070-242">**Get-MailFilterListReport**</span></span>
    
- <span data-ttu-id="92070-243">**Get-MailTrafficPolicyReport**</span><span class="sxs-lookup"><span data-stu-id="92070-243">**Get-MailTrafficPolicyReport**</span></span>
    
- <span data-ttu-id="92070-244">**Get-MailTrafficReport**</span><span class="sxs-lookup"><span data-stu-id="92070-244">**Get-MailTrafficReport**</span></span>
    
- <span data-ttu-id="92070-245">**Get-MailTrafficSummaryReport**</span><span class="sxs-lookup"><span data-stu-id="92070-245">**Get-MailTrafficSummaryReport**</span></span>
    
- <span data-ttu-id="92070-246">**Get-MailTrafficTopReport**</span><span class="sxs-lookup"><span data-stu-id="92070-246">**Get-MailTrafficTopReport**</span></span>
    
- <span data-ttu-id="92070-247">**Get-MalwareFilteringServer**</span><span class="sxs-lookup"><span data-stu-id="92070-247">**Get-MalwareFilteringServer**</span></span>
    
- <span data-ttu-id="92070-248">**SET-MalwareFilteringServer**</span><span class="sxs-lookup"><span data-stu-id="92070-248">**Set-MalwareFilteringServer**</span></span>
    
- <span data-ttu-id="92070-249">**Get-MalwareFilterPolicy**</span><span class="sxs-lookup"><span data-stu-id="92070-249">**Get-MalwareFilterPolicy**</span></span>
    
- <span data-ttu-id="92070-250">**New-MalwareFilterPolicy**</span><span class="sxs-lookup"><span data-stu-id="92070-250">**New-MalwareFilterPolicy**</span></span>
    
- <span data-ttu-id="92070-251">**Remove-MalwareFilterPolicy**</span><span class="sxs-lookup"><span data-stu-id="92070-251">**Remove-MalwareFilterPolicy**</span></span>
    
- <span data-ttu-id="92070-252">**SET-MalwareFilterPolicy**</span><span class="sxs-lookup"><span data-stu-id="92070-252">**Set-MalwareFilterPolicy**</span></span>
    
- <span data-ttu-id="92070-253">**Get-MalwareFilterRecoveryItem**</span><span class="sxs-lookup"><span data-stu-id="92070-253">**Get-MalwareFilterRecoveryItem**</span></span>
    
- <span data-ttu-id="92070-254">**Remove-MalwareFilterRecoveryItem**</span><span class="sxs-lookup"><span data-stu-id="92070-254">**Remove-MalwareFilterRecoveryItem**</span></span>
    
- <span data-ttu-id="92070-255">**Возобновление MalwareFilterRecoveryItem**</span><span class="sxs-lookup"><span data-stu-id="92070-255">**Resume-MalwareFilterRecoveryItem**</span></span>
    
- <span data-ttu-id="92070-256">**Отправить MapiSubmitSystemProbe**</span><span class="sxs-lookup"><span data-stu-id="92070-256">**Send-MapiSubmitSystemProbe**</span></span>
    
- <span data-ttu-id="92070-257">**Перенаправление сообщения**</span><span class="sxs-lookup"><span data-stu-id="92070-257">**Redirect-Message**</span></span>
    
- <span data-ttu-id="92070-258">**Get-MessageTrace**</span><span class="sxs-lookup"><span data-stu-id="92070-258">**Get-MessageTrace**</span></span>
    
- <span data-ttu-id="92070-259">**Get-MessageTraceDetail**</span><span class="sxs-lookup"><span data-stu-id="92070-259">**Get-MessageTraceDetail**</span></span>
    
- <span data-ttu-id="92070-260">**Завершить MigrationBatch**</span><span class="sxs-lookup"><span data-stu-id="92070-260">**Complete-MigrationBatch**</span></span>
    
- <span data-ttu-id="92070-261">**Remove-MigrationBatch**</span><span class="sxs-lookup"><span data-stu-id="92070-261">**Remove-MigrationBatch**</span></span>
    
- <span data-ttu-id="92070-262">**Get-MigrationConfig**</span><span class="sxs-lookup"><span data-stu-id="92070-262">**Get-MigrationConfig**</span></span>
    
- <span data-ttu-id="92070-263">**SET-MigrationConfig**</span><span class="sxs-lookup"><span data-stu-id="92070-263">**Set-MigrationConfig**</span></span>
    
- <span data-ttu-id="92070-264">**Get-MigrationEndpoint**</span><span class="sxs-lookup"><span data-stu-id="92070-264">**Get-MigrationEndpoint**</span></span>
    
- <span data-ttu-id="92070-265">**Новый MigrationEndpoint**</span><span class="sxs-lookup"><span data-stu-id="92070-265">**New-MigrationEndpoint**</span></span>
    
- <span data-ttu-id="92070-266">**Remove-MigrationEndpoint**</span><span class="sxs-lookup"><span data-stu-id="92070-266">**Remove-MigrationEndpoint**</span></span>
    
- <span data-ttu-id="92070-267">**SET-MigrationEndpoint**</span><span class="sxs-lookup"><span data-stu-id="92070-267">**Set-MigrationEndpoint**</span></span>
    
- <span data-ttu-id="92070-268">**Get-MigrationStatistics**</span><span class="sxs-lookup"><span data-stu-id="92070-268">**Get-MigrationStatistics**</span></span>
    
- <span data-ttu-id="92070-269">**Get-MigrationUser**</span><span class="sxs-lookup"><span data-stu-id="92070-269">**Get-MigrationUser**</span></span>
    
- <span data-ttu-id="92070-270">**Remove-MigrationUser**</span><span class="sxs-lookup"><span data-stu-id="92070-270">**Remove-MigrationUser**</span></span>
    
- <span data-ttu-id="92070-271">**Get-MigrationUserStatistics**</span><span class="sxs-lookup"><span data-stu-id="92070-271">**Get-MigrationUserStatistics**</span></span>
    
- <span data-ttu-id="92070-272">**Clear-MobileDevice**</span><span class="sxs-lookup"><span data-stu-id="92070-272">**Clear-MobileDevice**</span></span>
    
- <span data-ttu-id="92070-273">**Get-MobileDevice**</span><span class="sxs-lookup"><span data-stu-id="92070-273">**Get-MobileDevice**</span></span>
    
- <span data-ttu-id="92070-274">**Remove-MobileDevice**</span><span class="sxs-lookup"><span data-stu-id="92070-274">**Remove-MobileDevice**</span></span>
    
- <span data-ttu-id="92070-275">**Get-MobileDeviceMailboxPolicy**</span><span class="sxs-lookup"><span data-stu-id="92070-275">**Get-MobileDeviceMailboxPolicy**</span></span>
    
- <span data-ttu-id="92070-276">**Новый MobileDeviceMailboxPolicy**</span><span class="sxs-lookup"><span data-stu-id="92070-276">**New-MobileDeviceMailboxPolicy**</span></span>
    
- <span data-ttu-id="92070-277">**Remove-MobileDeviceMailboxPolicy**</span><span class="sxs-lookup"><span data-stu-id="92070-277">**Remove-MobileDeviceMailboxPolicy**</span></span>
    
- <span data-ttu-id="92070-278">**SET-MobileDeviceMailboxPolicy**</span><span class="sxs-lookup"><span data-stu-id="92070-278">**Set-MobileDeviceMailboxPolicy**</span></span>
    
- <span data-ttu-id="92070-279">**Get-MobileDeviceStatistics**</span><span class="sxs-lookup"><span data-stu-id="92070-279">**Get-MobileDeviceStatistics**</span></span>
    
- <span data-ttu-id="92070-280">**Get-MonitoringItemHelp**</span><span class="sxs-lookup"><span data-stu-id="92070-280">**Get-MonitoringItemHelp**</span></span>
    
- <span data-ttu-id="92070-281">**Get-MonitoringItemIdentity**</span><span class="sxs-lookup"><span data-stu-id="92070-281">**Get-MonitoringItemIdentity**</span></span>
    
- <span data-ttu-id="92070-282">**Invoke-MonitoringProbe**</span><span class="sxs-lookup"><span data-stu-id="92070-282">**Invoke-MonitoringProbe**</span></span>
    
- <span data-ttu-id="92070-283">**Get уведомлений**</span><span class="sxs-lookup"><span data-stu-id="92070-283">**Get-Notification**</span></span>
    
- <span data-ttu-id="92070-284">**SET уведомлений**</span><span class="sxs-lookup"><span data-stu-id="92070-284">**Set-Notification**</span></span>
    
- <span data-ttu-id="92070-285">**Test-OAuthConnectivity**</span><span class="sxs-lookup"><span data-stu-id="92070-285">**Test-OAuthConnectivity**</span></span>
    
- <span data-ttu-id="92070-286">**Get-OnPremisesOrganization**</span><span class="sxs-lookup"><span data-stu-id="92070-286">**Get-OnPremisesOrganization**</span></span>
    
- <span data-ttu-id="92070-287">**Новые локальной организации**</span><span class="sxs-lookup"><span data-stu-id="92070-287">**New-OnPremisesOrganization**</span></span>
    
- <span data-ttu-id="92070-288">**Remove-OnPremisesOrganization**</span><span class="sxs-lookup"><span data-stu-id="92070-288">**Remove-OnPremisesOrganization**</span></span>
    
- <span data-ttu-id="92070-289">**SET-OnPremisesOrganization**</span><span class="sxs-lookup"><span data-stu-id="92070-289">**Set-OnPremisesOrganization**</span></span>
    
- <span data-ttu-id="92070-290">**Enable-OrganizationCustomization**</span><span class="sxs-lookup"><span data-stu-id="92070-290">**Enable-OrganizationCustomization**</span></span>
    
- <span data-ttu-id="92070-291">**Get-OutboundConnector**</span><span class="sxs-lookup"><span data-stu-id="92070-291">**Get-OutboundConnector**</span></span>
    
- <span data-ttu-id="92070-292">**Новый OutboundConnector**</span><span class="sxs-lookup"><span data-stu-id="92070-292">**New-OutboundConnector**</span></span>
    
- <span data-ttu-id="92070-293">**Remove-OutboundConnector**</span><span class="sxs-lookup"><span data-stu-id="92070-293">**Remove-OutboundConnector**</span></span>
    
- <span data-ttu-id="92070-294">**SET-OutboundConnector**</span><span class="sxs-lookup"><span data-stu-id="92070-294">**Set-OutboundConnector**</span></span>
    
- <span data-ttu-id="92070-295">**Get-PartnerApplication**</span><span class="sxs-lookup"><span data-stu-id="92070-295">**Get-PartnerApplication**</span></span>
    
- <span data-ttu-id="92070-296">**Новый PartnerApplication**</span><span class="sxs-lookup"><span data-stu-id="92070-296">**New-PartnerApplication**</span></span>
    
- <span data-ttu-id="92070-297">**Remove-PartnerApplication**</span><span class="sxs-lookup"><span data-stu-id="92070-297">**Remove-PartnerApplication**</span></span>
    
- <span data-ttu-id="92070-298">**SET-PartnerApplication**</span><span class="sxs-lookup"><span data-stu-id="92070-298">**Set-PartnerApplication**</span></span>
    
- <span data-ttu-id="92070-299">**Get-PendingFederatedDomain**</span><span class="sxs-lookup"><span data-stu-id="92070-299">**Get-PendingFederatedDomain**</span></span>
    
- <span data-ttu-id="92070-300">**SET-PendingFederatedDomain**</span><span class="sxs-lookup"><span data-stu-id="92070-300">**Set-PendingFederatedDomain**</span></span>
    
- <span data-ttu-id="92070-301">**Get-PolicyTipConfig**</span><span class="sxs-lookup"><span data-stu-id="92070-301">**Get-PolicyTipConfig**</span></span>
    
- <span data-ttu-id="92070-302">**Новый PolicyTipConfig**</span><span class="sxs-lookup"><span data-stu-id="92070-302">**New-PolicyTipConfig**</span></span>
    
- <span data-ttu-id="92070-303">**Remove-PolicyTipConfig**</span><span class="sxs-lookup"><span data-stu-id="92070-303">**Remove-PolicyTipConfig**</span></span>
    
- <span data-ttu-id="92070-304">**SET-PolicyTipConfig**</span><span class="sxs-lookup"><span data-stu-id="92070-304">**Set-PolicyTipConfig**</span></span>
    
- <span data-ttu-id="92070-305">**Dump-ProvisioningCache**</span><span class="sxs-lookup"><span data-stu-id="92070-305">**Dump-ProvisioningCache**</span></span>
    
- <span data-ttu-id="92070-306">**Сброс ProvisioningCache**</span><span class="sxs-lookup"><span data-stu-id="92070-306">**Reset-ProvisioningCache**</span></span>
    
- <span data-ttu-id="92070-307">**Update-PublicFolderMailbox**</span><span class="sxs-lookup"><span data-stu-id="92070-307">**Update-PublicFolderMailbox**</span></span>
    
- <span data-ttu-id="92070-308">**Get-PublicFolderMailboxDiagnostics**</span><span class="sxs-lookup"><span data-stu-id="92070-308">**Get-PublicFolderMailboxDiagnostics**</span></span>
    
- <span data-ttu-id="92070-309">**Get-PublicFolderMigrationRequest**</span><span class="sxs-lookup"><span data-stu-id="92070-309">**Get-PublicFolderMigrationRequest**</span></span>
    
- <span data-ttu-id="92070-310">**Новый PublicFolderMigrationRequest**</span><span class="sxs-lookup"><span data-stu-id="92070-310">**New-PublicFolderMigrationRequest**</span></span>
    
- <span data-ttu-id="92070-311">**Remove-PublicFolderMigrationRequest**</span><span class="sxs-lookup"><span data-stu-id="92070-311">**Remove-PublicFolderMigrationRequest**</span></span>
    
- <span data-ttu-id="92070-312">**Resume-PublicFolderMigrationRequest**</span><span class="sxs-lookup"><span data-stu-id="92070-312">**Resume-PublicFolderMigrationRequest**</span></span>
    
- <span data-ttu-id="92070-313">**SET-PublicFolderMigrationRequest**</span><span class="sxs-lookup"><span data-stu-id="92070-313">**Set-PublicFolderMigrationRequest**</span></span>
    
- <span data-ttu-id="92070-314">**Приостановить PublicFolderMigrationRequest**</span><span class="sxs-lookup"><span data-stu-id="92070-314">**Suspend-PublicFolderMigrationRequest**</span></span>
    
- <span data-ttu-id="92070-315">**Get-PublicFolderMigrationRequestStatistics**</span><span class="sxs-lookup"><span data-stu-id="92070-315">**Get-PublicFolderMigrationRequestStatistics**</span></span>
    
- <span data-ttu-id="92070-316">**Get-QuarantineMessage**</span><span class="sxs-lookup"><span data-stu-id="92070-316">**Get-QuarantineMessage**</span></span>
    
- <span data-ttu-id="92070-317">**Выпуск QuarantineMessage**</span><span class="sxs-lookup"><span data-stu-id="92070-317">**Release-QuarantineMessage**</span></span>
    
- <span data-ttu-id="92070-318">**Get-QueueDigest**</span><span class="sxs-lookup"><span data-stu-id="92070-318">**Get-QueueDigest**</span></span>
    
- <span data-ttu-id="92070-319">**Get-ResourcePolicy**</span><span class="sxs-lookup"><span data-stu-id="92070-319">**Get-ResourcePolicy**</span></span>
    
- <span data-ttu-id="92070-320">**Новый ResourcePolicy**</span><span class="sxs-lookup"><span data-stu-id="92070-320">**New-ResourcePolicy**</span></span>
    
- <span data-ttu-id="92070-321">**Remove-ResourcePolicy**</span><span class="sxs-lookup"><span data-stu-id="92070-321">**Remove-ResourcePolicy**</span></span>
    
- <span data-ttu-id="92070-322">**SET-ResourcePolicy**</span><span class="sxs-lookup"><span data-stu-id="92070-322">**Set-ResourcePolicy**</span></span>
    
- <span data-ttu-id="92070-323">**Добавление ResubmitRequest**</span><span class="sxs-lookup"><span data-stu-id="92070-323">**Add-ResubmitRequest**</span></span>
    
- <span data-ttu-id="92070-324">**Get-ResubmitRequest**</span><span class="sxs-lookup"><span data-stu-id="92070-324">**Get-ResubmitRequest**</span></span>
    
- <span data-ttu-id="92070-325">**Remove-ResubmitRequest**</span><span class="sxs-lookup"><span data-stu-id="92070-325">**Remove-ResubmitRequest**</span></span>
    
- <span data-ttu-id="92070-326">**SET-ResubmitRequest**</span><span class="sxs-lookup"><span data-stu-id="92070-326">**Set-ResubmitRequest**</span></span>
    
- <span data-ttu-id="92070-327">**Get-ServerComponentState**</span><span class="sxs-lookup"><span data-stu-id="92070-327">**Get-ServerComponentState**</span></span>
    
- <span data-ttu-id="92070-328">**SET-ServerComponentState**</span><span class="sxs-lookup"><span data-stu-id="92070-328">**Set-ServerComponentState**</span></span>
    
- <span data-ttu-id="92070-329">**Get-ServerHealth**</span><span class="sxs-lookup"><span data-stu-id="92070-329">**Get-ServerHealth**</span></span>
    
- <span data-ttu-id="92070-330">**SET-ServerMonitor**</span><span class="sxs-lookup"><span data-stu-id="92070-330">**Set-ServerMonitor**</span></span>
    
- <span data-ttu-id="92070-331">**Добавление ServerMonitoringOverride**</span><span class="sxs-lookup"><span data-stu-id="92070-331">**Add-ServerMonitoringOverride**</span></span>
    
- <span data-ttu-id="92070-332">**Get-ServerMonitoringOverride**</span><span class="sxs-lookup"><span data-stu-id="92070-332">**Get-ServerMonitoringOverride**</span></span>
    
- <span data-ttu-id="92070-333">**Get-SiteMailbox**</span><span class="sxs-lookup"><span data-stu-id="92070-333">**Get-SiteMailbox**</span></span>
    
- <span data-ttu-id="92070-334">**Новый SiteMailbox**</span><span class="sxs-lookup"><span data-stu-id="92070-334">**New-SiteMailbox**</span></span>
    
- <span data-ttu-id="92070-335">**SET-SiteMailbox**</span><span class="sxs-lookup"><span data-stu-id="92070-335">**Set-SiteMailbox**</span></span>
    
- <span data-ttu-id="92070-336">**Test-SiteMailbox**</span><span class="sxs-lookup"><span data-stu-id="92070-336">**Test-SiteMailbox**</span></span>
    
- <span data-ttu-id="92070-337">**Обновление SiteMailbox**</span><span class="sxs-lookup"><span data-stu-id="92070-337">**Update-SiteMailbox**</span></span>
    
- <span data-ttu-id="92070-338">**Get-SiteMailboxDiagnostics**</span><span class="sxs-lookup"><span data-stu-id="92070-338">**Get-SiteMailboxDiagnostics**</span></span>
    
- <span data-ttu-id="92070-339">**Get-SiteMailboxProvisioningPolicy**</span><span class="sxs-lookup"><span data-stu-id="92070-339">**Get-SiteMailboxProvisioningPolicy**</span></span>
    
- <span data-ttu-id="92070-340">**Новый SiteMailboxProvisioningPolicy**</span><span class="sxs-lookup"><span data-stu-id="92070-340">**New-SiteMailboxProvisioningPolicy**</span></span>
    
- <span data-ttu-id="92070-341">**Remove-SiteMailboxProvisioningPolicy**</span><span class="sxs-lookup"><span data-stu-id="92070-341">**Remove-SiteMailboxProvisioningPolicy**</span></span>
    
- <span data-ttu-id="92070-342">**SET-SiteMailboxProvisioningPolicy**</span><span class="sxs-lookup"><span data-stu-id="92070-342">**Set-SiteMailboxProvisioningPolicy**</span></span>
    
- <span data-ttu-id="92070-343">**Отмена SoftDeletedMailbox**</span><span class="sxs-lookup"><span data-stu-id="92070-343">**Undo-SoftDeletedMailbox**</span></span>
    
- <span data-ttu-id="92070-344">**Get-StaleMailboxDetailReport**</span><span class="sxs-lookup"><span data-stu-id="92070-344">**Get-StaleMailboxDetailReport**</span></span>
    
- <span data-ttu-id="92070-345">**Get-StaleMailboxReport**</span><span class="sxs-lookup"><span data-stu-id="92070-345">**Get-StaleMailboxReport**</span></span>
    
- <span data-ttu-id="92070-346">**Update-storemailboxstate, можно**</span><span class="sxs-lookup"><span data-stu-id="92070-346">**Update-StoreMailboxState**</span></span>
    
- <span data-ttu-id="92070-347">**Новый SyncMailPublicFolder**</span><span class="sxs-lookup"><span data-stu-id="92070-347">**New-SyncMailPublicFolder**</span></span>
    
- <span data-ttu-id="92070-348">**Get-TransportService**</span><span class="sxs-lookup"><span data-stu-id="92070-348">**Get-TransportService**</span></span>
    
- <span data-ttu-id="92070-349">**SET-TransportService**</span><span class="sxs-lookup"><span data-stu-id="92070-349">**Set-TransportService**</span></span>
    
- <span data-ttu-id="92070-350">**Disable-UMCallAnsweringRule**</span><span class="sxs-lookup"><span data-stu-id="92070-350">**Disable-UMCallAnsweringRule**</span></span>
    
- <span data-ttu-id="92070-351">**Enable-UMCallAnsweringRule**</span><span class="sxs-lookup"><span data-stu-id="92070-351">**Enable-UMCallAnsweringRule**</span></span>
    
- <span data-ttu-id="92070-352">**Get-UMCallAnsweringRule**</span><span class="sxs-lookup"><span data-stu-id="92070-352">**Get-UMCallAnsweringRule**</span></span>
    
- <span data-ttu-id="92070-353">**Новый UMCallAnsweringRule**</span><span class="sxs-lookup"><span data-stu-id="92070-353">**New-UMCallAnsweringRule**</span></span>
    
- <span data-ttu-id="92070-354">**Remove-UMCallAnsweringRule**</span><span class="sxs-lookup"><span data-stu-id="92070-354">**Remove-UMCallAnsweringRule**</span></span>
    
- <span data-ttu-id="92070-355">**SET-UMCallAnsweringRule**</span><span class="sxs-lookup"><span data-stu-id="92070-355">**Set-UMCallAnsweringRule**</span></span>
    
- <span data-ttu-id="92070-356">**Get-UMCallRouterSettings**</span><span class="sxs-lookup"><span data-stu-id="92070-356">**Get-UMCallRouterSettings**</span></span>
    
- <span data-ttu-id="92070-357">**SET-UMCallRouterSettings**</span><span class="sxs-lookup"><span data-stu-id="92070-357">**Set-UMCallRouterSettings**</span></span>
    
- <span data-ttu-id="92070-358">**Disable-UMService**</span><span class="sxs-lookup"><span data-stu-id="92070-358">**Disable-UMService**</span></span>
    
- <span data-ttu-id="92070-359">**Enable-UMService**</span><span class="sxs-lookup"><span data-stu-id="92070-359">**Enable-UMService**</span></span>
    
- <span data-ttu-id="92070-360">**Get-UMService**</span><span class="sxs-lookup"><span data-stu-id="92070-360">**Get-UMService**</span></span>
    
- <span data-ttu-id="92070-361">**SET-UMService**</span><span class="sxs-lookup"><span data-stu-id="92070-361">**Set-UMService**</span></span>
    
- <span data-ttu-id="92070-362">**Get-UserPhoto**</span><span class="sxs-lookup"><span data-stu-id="92070-362">**Get-UserPhoto**</span></span>
    
- <span data-ttu-id="92070-363">**Remove-UserPhoto**</span><span class="sxs-lookup"><span data-stu-id="92070-363">**Remove-UserPhoto**</span></span>
    
- <span data-ttu-id="92070-364">**SET-UserPhoto**</span><span class="sxs-lookup"><span data-stu-id="92070-364">**Set-UserPhoto**</span></span>
    
- <span data-ttu-id="92070-365">**Get-WorkloadManagementPolicy**</span><span class="sxs-lookup"><span data-stu-id="92070-365">**Get-WorkloadManagementPolicy**</span></span>
    
- <span data-ttu-id="92070-366">**Новый WorkloadManagementPolicy**</span><span class="sxs-lookup"><span data-stu-id="92070-366">**New-WorkloadManagementPolicy**</span></span>
    
- <span data-ttu-id="92070-367">**Remove-WorkloadManagementPolicy**</span><span class="sxs-lookup"><span data-stu-id="92070-367">**Remove-WorkloadManagementPolicy**</span></span>
    
- <span data-ttu-id="92070-368">**Get-WorkloadPolicy**</span><span class="sxs-lookup"><span data-stu-id="92070-368">**Get-WorkloadPolicy**</span></span>
    
- <span data-ttu-id="92070-369">**Новый WorkloadPolicy**</span><span class="sxs-lookup"><span data-stu-id="92070-369">**New-WorkloadPolicy**</span></span>
    
- <span data-ttu-id="92070-370">**Remove-WorkloadPolicy**</span><span class="sxs-lookup"><span data-stu-id="92070-370">**Remove-WorkloadPolicy**</span></span>
    
- <span data-ttu-id="92070-371">**SET-WorkloadPolicy**</span><span class="sxs-lookup"><span data-stu-id="92070-371">**Set-WorkloadPolicy**</span></span>
    
### <a name="modified-cmdlets"></a><span data-ttu-id="92070-372">Измененные командлеты</span><span class="sxs-lookup"><span data-stu-id="92070-372">Modified cmdlets</span></span>
<span data-ttu-id="92070-373"><a name="bk_update"> </a></span><span class="sxs-lookup"><span data-stu-id="92070-373"></span></span>

<span data-ttu-id="92070-374">Типы ввода-вывода для следующих командлетов были изменены в Exchange 2013:</span><span class="sxs-lookup"><span data-stu-id="92070-374">The input or output types for following cmdlets were modified in Exchange 2013:</span></span>
  
- <span data-ttu-id="92070-375">**Clear-ActiveSyncDevice**</span><span class="sxs-lookup"><span data-stu-id="92070-375">**Clear-ActiveSyncDevice**</span></span>
    
- <span data-ttu-id="92070-376">**Remove-ActiveSyncDevice**</span><span class="sxs-lookup"><span data-stu-id="92070-376">**Remove-ActiveSyncDevice**</span></span>
    
- <span data-ttu-id="92070-377">**Get-ActiveSyncMailboxPolicy**</span><span class="sxs-lookup"><span data-stu-id="92070-377">**Get-ActiveSyncMailboxPolicy**</span></span>
    
- <span data-ttu-id="92070-378">**Новый ActiveSyncMailboxPolicy**</span><span class="sxs-lookup"><span data-stu-id="92070-378">**New-ActiveSyncMailboxPolicy**</span></span>
    
- <span data-ttu-id="92070-379">**Новый ActiveSyncVirtualDirectory**</span><span class="sxs-lookup"><span data-stu-id="92070-379">**New-ActiveSyncVirtualDirectory**</span></span>
    
- <span data-ttu-id="92070-380">**Новый AutodiscoverVirtualDirectory**</span><span class="sxs-lookup"><span data-stu-id="92070-380">**New-AutodiscoverVirtualDirectory**</span></span>
    
- <span data-ttu-id="92070-381">**SET-AvailabilityConfig**</span><span class="sxs-lookup"><span data-stu-id="92070-381">**Set-AvailabilityConfig**</span></span>
    
- <span data-ttu-id="92070-382">**Enable-ExchangeCertificate**</span><span class="sxs-lookup"><span data-stu-id="92070-382">**Enable-ExchangeCertificate**</span></span>
    
- <span data-ttu-id="92070-383">**Export-ExchangeCertificate**</span><span class="sxs-lookup"><span data-stu-id="92070-383">**Export-ExchangeCertificate**</span></span>
    
- <span data-ttu-id="92070-384">**Import-ExchangeCertificate**</span><span class="sxs-lookup"><span data-stu-id="92070-384">**Import-ExchangeCertificate**</span></span>
    
- <span data-ttu-id="92070-385">**Remove-ExchangeCertificate**</span><span class="sxs-lookup"><span data-stu-id="92070-385">**Remove-ExchangeCertificate**</span></span>
    
- <span data-ttu-id="92070-386">**Get-FailedContentIndexDocuments**</span><span class="sxs-lookup"><span data-stu-id="92070-386">**Get-FailedContentIndexDocuments**</span></span>
    
- <span data-ttu-id="92070-387">**Get-FederationInformation**</span><span class="sxs-lookup"><span data-stu-id="92070-387">**Get-FederationInformation**</span></span>
    
- <span data-ttu-id="92070-388">**Новый HybridConfiguration**</span><span class="sxs-lookup"><span data-stu-id="92070-388">**New-HybridConfiguration**</span></span>
    
- <span data-ttu-id="92070-389">**SET-HybridConfiguration**</span><span class="sxs-lookup"><span data-stu-id="92070-389">**Set-HybridConfiguration**</span></span>
    
- <span data-ttu-id="92070-390">**Новый почтовый ящик**</span><span class="sxs-lookup"><span data-stu-id="92070-390">**New-Mailbox**</span></span>
    
- <span data-ttu-id="92070-391">**Resume-MailboxDatabaseCopy**</span><span class="sxs-lookup"><span data-stu-id="92070-391">**Resume-MailboxDatabaseCopy**</span></span>
    
- <span data-ttu-id="92070-392">**SET-MailboxDatabaseCopy**</span><span class="sxs-lookup"><span data-stu-id="92070-392">**Set-MailboxDatabaseCopy**</span></span>
    
- <span data-ttu-id="92070-393">**Приостановить MailboxDatabaseCopy**</span><span class="sxs-lookup"><span data-stu-id="92070-393">**Suspend-MailboxDatabaseCopy**</span></span>
    
- <span data-ttu-id="92070-394">**Update-MailboxDatabaseCopy**</span><span class="sxs-lookup"><span data-stu-id="92070-394">**Update-MailboxDatabaseCopy**</span></span>
    
- <span data-ttu-id="92070-395">**Get-MailboxExportRequest**</span><span class="sxs-lookup"><span data-stu-id="92070-395">**Get-MailboxExportRequest**</span></span>
    
- <span data-ttu-id="92070-396">**SET-MailboxExportRequest**</span><span class="sxs-lookup"><span data-stu-id="92070-396">**Set-MailboxExportRequest**</span></span>
    
- <span data-ttu-id="92070-397">**Добавление MailboxFolderPermission**</span><span class="sxs-lookup"><span data-stu-id="92070-397">**Add-MailboxFolderPermission**</span></span>
    
- <span data-ttu-id="92070-398">**Remove-MailboxFolderPermission**</span><span class="sxs-lookup"><span data-stu-id="92070-398">**Remove-MailboxFolderPermission**</span></span>
    
- <span data-ttu-id="92070-399">**SET-MailboxFolderPermission**</span><span class="sxs-lookup"><span data-stu-id="92070-399">**Set-MailboxFolderPermission**</span></span>
    
- <span data-ttu-id="92070-400">**Get-MailboxImportRequest**</span><span class="sxs-lookup"><span data-stu-id="92070-400">**Get-MailboxImportRequest**</span></span>
    
- <span data-ttu-id="92070-401">**SET-MailboxImportRequest**</span><span class="sxs-lookup"><span data-stu-id="92070-401">**Set-MailboxImportRequest**</span></span>
    
- <span data-ttu-id="92070-402">**Get-MailboxRestoreRequest**</span><span class="sxs-lookup"><span data-stu-id="92070-402">**Get-MailboxRestoreRequest**</span></span>
    
- <span data-ttu-id="92070-403">**SET-MailboxRestoreRequest**</span><span class="sxs-lookup"><span data-stu-id="92070-403">**Set-MailboxRestoreRequest**</span></span>
    
- <span data-ttu-id="92070-404">**Get-MailboxSearch**</span><span class="sxs-lookup"><span data-stu-id="92070-404">**Get-MailboxSearch**</span></span>
    
- <span data-ttu-id="92070-405">**Remove-MailboxSearch**</span><span class="sxs-lookup"><span data-stu-id="92070-405">**Remove-MailboxSearch**</span></span>
    
- <span data-ttu-id="92070-406">**SET-MailboxSearch**</span><span class="sxs-lookup"><span data-stu-id="92070-406">**Set-MailboxSearch**</span></span>
    
- <span data-ttu-id="92070-407">**Start-MailboxSearch**</span><span class="sxs-lookup"><span data-stu-id="92070-407">**Start-MailboxSearch**</span></span>
    
- <span data-ttu-id="92070-408">**STOP-MailboxSearch**</span><span class="sxs-lookup"><span data-stu-id="92070-408">**Stop-MailboxSearch**</span></span>
    
- <span data-ttu-id="92070-409">**Disable-MailPublicFolder**</span><span class="sxs-lookup"><span data-stu-id="92070-409">**Disable-MailPublicFolder**</span></span>
    
- <span data-ttu-id="92070-410">**Get-MailPublicFolder**</span><span class="sxs-lookup"><span data-stu-id="92070-410">**Get-MailPublicFolder**</span></span>
    
- <span data-ttu-id="92070-411">**SET-MailPublicFolder**</span><span class="sxs-lookup"><span data-stu-id="92070-411">**Set-MailPublicFolder**</span></span>
    
- <span data-ttu-id="92070-412">**Get-MigrationBatch**</span><span class="sxs-lookup"><span data-stu-id="92070-412">**Get-MigrationBatch**</span></span>
    
- <span data-ttu-id="92070-413">**Новый MigrationBatch**</span><span class="sxs-lookup"><span data-stu-id="92070-413">**New-MigrationBatch**</span></span>
    
- <span data-ttu-id="92070-414">**SET-MigrationBatch**</span><span class="sxs-lookup"><span data-stu-id="92070-414">**Set-MigrationBatch**</span></span>
    
- <span data-ttu-id="92070-415">**Test-MigrationServerAvailability**</span><span class="sxs-lookup"><span data-stu-id="92070-415">**Test-MigrationServerAvailability**</span></span>
    
- <span data-ttu-id="92070-416">**Get-MoveRequest**</span><span class="sxs-lookup"><span data-stu-id="92070-416">**Get-MoveRequest**</span></span>
    
- <span data-ttu-id="92070-417">**Новый OfflineAddressBook**</span><span class="sxs-lookup"><span data-stu-id="92070-417">**New-OfflineAddressBook**</span></span>
    
- <span data-ttu-id="92070-418">**Get-OrganizationConfig**</span><span class="sxs-lookup"><span data-stu-id="92070-418">**Get-OrganizationConfig**</span></span>
    
- <span data-ttu-id="92070-419">**SET-OrganizationConfig**</span><span class="sxs-lookup"><span data-stu-id="92070-419">**Set-OrganizationConfig**</span></span>
    
- <span data-ttu-id="92070-420">**Test-OutlookConnectivity**</span><span class="sxs-lookup"><span data-stu-id="92070-420">**Test-OutlookConnectivity**</span></span>
    
- <span data-ttu-id="92070-421">**Test-OutlookWebServices**</span><span class="sxs-lookup"><span data-stu-id="92070-421">**Test-OutlookWebServices**</span></span>
    
- <span data-ttu-id="92070-422">**Get-OwaMailboxPolicy**</span><span class="sxs-lookup"><span data-stu-id="92070-422">**Get-OwaMailboxPolicy**</span></span>
    
- <span data-ttu-id="92070-423">**Новые OwaVirtualDirectory**</span><span class="sxs-lookup"><span data-stu-id="92070-423">**New-OwaVirtualDirectory**</span></span>
    
- <span data-ttu-id="92070-424">**Новый PowerShellVirtualDirectory**</span><span class="sxs-lookup"><span data-stu-id="92070-424">**New-PowerShellVirtualDirectory**</span></span>
    
- <span data-ttu-id="92070-425">**Get-PublicFolder**</span><span class="sxs-lookup"><span data-stu-id="92070-425">**Get-PublicFolder**</span></span>
    
- <span data-ttu-id="92070-426">**Новые PublicFolder**</span><span class="sxs-lookup"><span data-stu-id="92070-426">**New-PublicFolder**</span></span>
    
- <span data-ttu-id="92070-427">**SET-PublicFolder**</span><span class="sxs-lookup"><span data-stu-id="92070-427">**Set-PublicFolder**</span></span>
    
- <span data-ttu-id="92070-428">**Добавление PublicFolderClientPermission**</span><span class="sxs-lookup"><span data-stu-id="92070-428">**Add-PublicFolderClientPermission**</span></span>
    
- <span data-ttu-id="92070-429">**Get-PublicFolderClientPermission**</span><span class="sxs-lookup"><span data-stu-id="92070-429">**Get-PublicFolderClientPermission**</span></span>
    
- <span data-ttu-id="92070-430">**Remove-PublicFolderClientPermission**</span><span class="sxs-lookup"><span data-stu-id="92070-430">**Remove-PublicFolderClientPermission**</span></span>
    
- <span data-ttu-id="92070-431">**Get-PublicFolderItemStatistics**</span><span class="sxs-lookup"><span data-stu-id="92070-431">**Get-PublicFolderItemStatistics**</span></span>
    
- <span data-ttu-id="92070-432">**Get-PublicFolderStatistics**</span><span class="sxs-lookup"><span data-stu-id="92070-432">**Get-PublicFolderStatistics**</span></span>
    
- <span data-ttu-id="92070-433">**Get-Recipient**</span><span class="sxs-lookup"><span data-stu-id="92070-433">**Get-Recipient**</span></span>
    
- <span data-ttu-id="92070-434">**SET-ResourceConfig**</span><span class="sxs-lookup"><span data-stu-id="92070-434">**Set-ResourceConfig**</span></span>
    
- <span data-ttu-id="92070-435">**Test-WebServicesConnectivity**</span><span class="sxs-lookup"><span data-stu-id="92070-435">**Test-WebServicesConnectivity**</span></span>
    
- <span data-ttu-id="92070-436">**Новый WebServicesVirtualDirectory**</span><span class="sxs-lookup"><span data-stu-id="92070-436">**New-WebServicesVirtualDirectory**</span></span>
    
### <a name="removed-cmdlets"></a><span data-ttu-id="92070-437">Удаленные командлеты</span><span class="sxs-lookup"><span data-stu-id="92070-437">Removed cmdlets</span></span>
<span data-ttu-id="92070-438"><a name="bk_removed"> </a></span><span class="sxs-lookup"><span data-stu-id="92070-438"></span></span>

<span data-ttu-id="92070-439">Следующие командлеты были удалены из Exchange 2013.</span><span class="sxs-lookup"><span data-stu-id="92070-439">The following cmdlets were removed from Exchange 2013:</span></span>
  
- <span data-ttu-id="92070-440">**Обновление FileDistributionService**</span><span class="sxs-lookup"><span data-stu-id="92070-440">**Update-FileDistributionService**</span></span>
    
- <span data-ttu-id="92070-441">**Почтовый ящик восстановления**</span><span class="sxs-lookup"><span data-stu-id="92070-441">**Restore-Mailbox**</span></span>
    
- <span data-ttu-id="92070-442">**Очистить MailboxDatabase**</span><span class="sxs-lookup"><span data-stu-id="92070-442">**Clean-MailboxDatabase**</span></span>
    
- <span data-ttu-id="92070-443">**Выполнения переноса**</span><span class="sxs-lookup"><span data-stu-id="92070-443">**Complete-Migration**</span></span>
    
- <span data-ttu-id="92070-444">**Get-MigrationStatus**</span><span class="sxs-lookup"><span data-stu-id="92070-444">**Get-MigrationStatus**</span></span>
    
- <span data-ttu-id="92070-445">**Update-PublicFolder**</span><span class="sxs-lookup"><span data-stu-id="92070-445">**Update-PublicFolder**</span></span>
    
- <span data-ttu-id="92070-446">**Добавление PublicFolderAdministrativePermission**</span><span class="sxs-lookup"><span data-stu-id="92070-446">**Add-PublicFolderAdministrativePermission**</span></span>
    
- <span data-ttu-id="92070-447">**Get-PublicFolderAdministrativePermission**</span><span class="sxs-lookup"><span data-stu-id="92070-447">**Get-PublicFolderAdministrativePermission**</span></span>
    
- <span data-ttu-id="92070-448">**Remove-PublicFolderAdministrativePermission**</span><span class="sxs-lookup"><span data-stu-id="92070-448">**Remove-PublicFolderAdministrativePermission**</span></span>
    
- <span data-ttu-id="92070-449">**Новый PublicFolderDatabase**</span><span class="sxs-lookup"><span data-stu-id="92070-449">**New-PublicFolderDatabase**</span></span>
    
- <span data-ttu-id="92070-450">**Remove-PublicFolderDatabase**</span><span class="sxs-lookup"><span data-stu-id="92070-450">**Remove-PublicFolderDatabase**</span></span>
    
- <span data-ttu-id="92070-451">**SET-PublicFolderDatabase**</span><span class="sxs-lookup"><span data-stu-id="92070-451">**Set-PublicFolderDatabase**</span></span>
    
- <span data-ttu-id="92070-452">**Новый PublicFolderDatabaseRepairRequest**</span><span class="sxs-lookup"><span data-stu-id="92070-452">**New-PublicFolderDatabaseRepairRequest**</span></span>
    
- <span data-ttu-id="92070-453">**Обновление PublicFolderHierarchy**</span><span class="sxs-lookup"><span data-stu-id="92070-453">**Update-PublicFolderHierarchy**</span></span>
    
- <span data-ttu-id="92070-454">**Возобновление PublicFolderReplication**</span><span class="sxs-lookup"><span data-stu-id="92070-454">**Resume-PublicFolderReplication**</span></span>
    
- <span data-ttu-id="92070-455">**Приостановка PublicFolderReplication**</span><span class="sxs-lookup"><span data-stu-id="92070-455">**Suspend-PublicFolderReplication**</span></span>
    
- <span data-ttu-id="92070-456">**Start-RetentionAutoTagLearning**</span><span class="sxs-lookup"><span data-stu-id="92070-456">**Start-RetentionAutoTagLearning**</span></span>
    
- <span data-ttu-id="92070-457">**Test-SystemHealth**</span><span class="sxs-lookup"><span data-stu-id="92070-457">**Test-SystemHealth**</span></span>
    
- <span data-ttu-id="92070-458">**Отключить свойств**</span><span class="sxs-lookup"><span data-stu-id="92070-458">**Disable-UMServer**</span></span>
    
- <span data-ttu-id="92070-459">**Enable свойств**</span><span class="sxs-lookup"><span data-stu-id="92070-459">**Enable-UMServer**</span></span>
    
- <span data-ttu-id="92070-460">**Get свойств**</span><span class="sxs-lookup"><span data-stu-id="92070-460">**Get-UMServer**</span></span>
    
- <span data-ttu-id="92070-461">**Свойств**</span><span class="sxs-lookup"><span data-stu-id="92070-461">**Set-UMServer**</span></span>
    
## <a name="see-also"></a><span data-ttu-id="92070-462">См. также</span><span class="sxs-lookup"><span data-stu-id="92070-462">See also</span></span>

- [<span data-ttu-id="92070-463">Входные данные командлета Командная консоль Exchange и вывод типов</span><span class="sxs-lookup"><span data-stu-id="92070-463">Exchange Management Shell cmdlet input and output types</span></span>](exchange-management-shell-cmdlet-input-and-output-types.md)    
- [<span data-ttu-id="92070-464">Ознакомьтесь со списком пользователей почты с помощью командной консоли Exchange</span><span class="sxs-lookup"><span data-stu-id="92070-464">Get a list of mail users by using the Exchange Management Shell</span></span>](how-to-get-a-list-of-mail-users-by-using-the-exchange-management-shell.md)    
- [<span data-ttu-id="92070-465">Командлеты Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="92070-465">Exchange 2013 cmdlets</span></span>](http://technet.microsoft.com/en-us/library/bb124413%28v=exchg.150%29.aspx)
    

