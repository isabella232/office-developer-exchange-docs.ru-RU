---
title: Управление доступом пользователей с помощью веб-служб Exchange в Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 48f0170c-8786-405f-86cb-568b7314a425
description: Узнайте, какие существуют возможности для управления доступом к учетной записи пользователя с сервером Exchange.
ms.openlocfilehash: d93f521f08f93b44b4ecc1f258b03ed24ebdd3dd
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761147"
---
# <a name="managing-user-access-by-using-ews-in-exchange"></a><span data-ttu-id="c384d-103">Управление доступом пользователей с помощью веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="c384d-103">Managing user access by using EWS in Exchange</span></span>

<span data-ttu-id="c384d-104">Узнайте, какие существуют возможности для управления доступом к учетной записи пользователя с сервером Exchange.</span><span class="sxs-lookup"><span data-stu-id="c384d-104">Find out what your options are for managing user account access to your Exchange server.</span></span>
  
<span data-ttu-id="c384d-105">Веб-служб Exchange (EWS) и веб-служб Exchange с управляемым API предоставляют ограниченное количество операций, которые можно использовать для управления учетными записями в Exchange Online, Exchange Online в составе Office 365 или версии Exchange, начиная с Exchange 2013.</span><span class="sxs-lookup"><span data-stu-id="c384d-105">Exchange Web Services (EWS) and the EWS managed API provide a limited number of operations that you can use to manage accounts on Exchange Online, Exchange Online as part of Office 365, or a version of Exchange starting with Exchange 2013.</span></span> <span data-ttu-id="c384d-106">Управление представителями и задавать права доступа к папкам для других учетных записей можно использовать операции, показано на следующем рисунке.</span><span class="sxs-lookup"><span data-stu-id="c384d-106">You can use the operations shown in the following figure to manage delegates and to set folder access permissions for other accounts.</span></span> 
  
<span data-ttu-id="c384d-107">**Операции веб-служб Exchange для доступа делегата и папки**</span><span class="sxs-lookup"><span data-stu-id="c384d-107">**EWS operations for delegate and folder access**</span></span>

![Параметры управления пользователями EWS.](media/Exchange_ManagingUserAccess_1.png)
  
<span data-ttu-id="c384d-109">Если приложению дополнительные контроль учетных записей на сервере Exchange, можно использовать командлеты командной консоли Exchange к управлению учетными записями.</span><span class="sxs-lookup"><span data-stu-id="c384d-109">If your application needs additional control over the accounts on an Exchange server, you can use Exchange Management Shell cmdlets to manage the accounts.</span></span> <span data-ttu-id="c384d-110">Можно вызвать командлетов командной консоли Exchange, выполнив одно из следующих:</span><span class="sxs-lookup"><span data-stu-id="c384d-110">You can call the Exchange Management Shell cmdlets by doing one of the following:</span></span>
  
- <span data-ttu-id="c384d-111">Создание приложения с помощью C# или Visual Basic, который вызывает командлетов командной консоли Exchange.</span><span class="sxs-lookup"><span data-stu-id="c384d-111">Writing an application using C# or Visual Basic that calls the Exchange Management Shell cmdlets.</span></span> <span data-ttu-id="c384d-112">Можно просмотреть пример кода на [Документация по API -интерфейса командной консоли управления Exchange](../management/exchange-management-shell.md) , чтобы узнать, как для вызова командлета.</span><span class="sxs-lookup"><span data-stu-id="c384d-112">You can look at the sample code in the [Exchange Management Shell API documentation](../management/exchange-management-shell.md) to learn how to call a cmdlet.</span></span> 
    
- <span data-ttu-id="c384d-113">С помощью Windows PowerShell и сценарии Windows PowerShell для вызова командлетов командной консоли Exchange.</span><span class="sxs-lookup"><span data-stu-id="c384d-113">Using Windows PowerShell and Windows PowerShell scripts to call Exchange Management Shell cmdlets.</span></span> <span data-ttu-id="c384d-114">Можно найти полный список [Exchange Server PowerShell (Командная консоль Exchange)](https://docs.microsoft.com/en-us/powershell/exchange/exchange-server/exchange-management-shell?view=exchange-ps), а также примеры, показывающие, как их использовать.</span><span class="sxs-lookup"><span data-stu-id="c384d-114">You can find a complete list of the [Exchange Server PowerShell (Exchange Management Shell)](https://docs.microsoft.com/en-us/powershell/exchange/exchange-server/exchange-management-shell?view=exchange-ps), along with examples that show how to use them.</span></span> 
    
## <a name="see-also"></a><span data-ttu-id="c384d-115">См. также</span><span class="sxs-lookup"><span data-stu-id="c384d-115">See also</span></span>

- [<span data-ttu-id="c384d-116">Настройка приложения веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="c384d-116">Setting up your EWS application</span></span>](setting-up-your-ews-application.md)   
- [<span data-ttu-id="c384d-117">Командлеты Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="c384d-117">Exchange 2013 Cmdlets</span></span>](https://docs.microsoft.com/en-us/powershell/exchange/?view=exchange-ps)  
    

