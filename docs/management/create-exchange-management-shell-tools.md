---
title: Создание средств командной консоли Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 46e4812f-37a8-449f-bd37-bc4a94605db9
description: Найдите сведения, чтобы приступить к созданию средств командной консоли Exchange для Exchange.
ms.openlocfilehash: e8414460007f333e50c9d596bf977792977b1e4e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761248"
---
# <a name="create-exchange-management-shell-tools"></a><span data-ttu-id="4c1fc-103">Создание средств командной консоли Exchange</span><span class="sxs-lookup"><span data-stu-id="4c1fc-103">Create Exchange Management Shell tools</span></span>

<span data-ttu-id="4c1fc-104">Найдите сведения, чтобы приступить к созданию средств командной консоли Exchange для Exchange.</span><span class="sxs-lookup"><span data-stu-id="4c1fc-104">Find information to get started creating Exchange Management Shell tools for Exchange.</span></span>

<span data-ttu-id="4c1fc-105">**Применимо к:** Exchange Online | Exchange Server 2013 | Office 365</span><span class="sxs-lookup"><span data-stu-id="4c1fc-105">**Applies to:** Exchange Online | Exchange Server 2013 | Office 365</span></span>
  
<span data-ttu-id="4c1fc-106">Командная консоль Exchange предоставляет богатый набор команд, основанный на платформе Windows PowerShell, для управления Exchange Online, Exchange Online в составе Office 365 или локальной версии Exchange, начиная с Exchange 2013.</span><span class="sxs-lookup"><span data-stu-id="4c1fc-106">The Exchange Management Shell provides a rich set of commands, based on the Windows PowerShell platform, for managing Exchange Online, Exchange Online as part of Office 365, or an on-premises version of Exchange starting with Exchange 2013.</span></span> <span data-ttu-id="4c1fc-107">Команды командной консоли Exchange можно использовать для автоматизации администрирования сервера путем непосредственного выполнения команд или с помощью командных сценариев.</span><span class="sxs-lookup"><span data-stu-id="4c1fc-107">You can use Exchange Management Shell commands to automate the administration of a server by directly executing the commands, or by using command scripts.</span></span>
  
<span data-ttu-id="4c1fc-108">Если вы хотите использовать команды командной консоли Exchange из приложения для хостинга, такого как административное приложение, запущенное на настольном компьютере администратора или через веб-приложение, вы можете вызвать командлеты командной консоли Exchange из приложения Visual Basic или C# для управления сервером Exchange.</span><span class="sxs-lookup"><span data-stu-id="4c1fc-108">If you need to use Exchange Management Shell commands from within a hosting application, such as an administrative application that is running on the administrator's desktop or through a web-based application, you can call Exchange Management Shell cmdlets from within your Visual Basic or C# application to manage an Exchange server.</span></span>
  
## <a name="get-started-with-exchange-management-shell-tools"></a><span data-ttu-id="4c1fc-109">Начало работы с инструментами командной консоли Exchange</span><span class="sxs-lookup"><span data-stu-id="4c1fc-109">Get started with Exchange Management Shell tools</span></span>
<span data-ttu-id="4c1fc-110"><a name="SP15GettingStartedTemplate_WhatDoYouNeed"> </a></span><span class="sxs-lookup"><span data-stu-id="4c1fc-110"><a name="SP15GettingStartedTemplate_WhatDoYouNeed"> </a></span></span>

<span data-ttu-id="4c1fc-111">Если вы знакомы с созданием ведущих приложений Windows PowerShell и хотите увидеть пример, в котором показано, как вызвать командлеты командной консоли Exchange из приложения или просмотреть пример типов приложений, которые можно создать с помощью командлетов командной консоли Exchange, ознакомьтесь со [статьей получение списка почтовых пользователей с помощью командной консоли Exchange](how-to-get-a-list-of-mail-users-by-using-the-exchange-management-shell.md).</span><span class="sxs-lookup"><span data-stu-id="4c1fc-111">If you are familiar with creating Windows PowerShell host applications and want to see an example that shows how to call the Exchange Management Shell cmdlets from an application, or to see an example of the types of applications that you can create by using the Exchange Management Shell cmdlets, see [Get a list of mail users by using the Exchange Management Shell](how-to-get-a-list-of-mail-users-by-using-the-exchange-management-shell.md).</span></span>
  
<span data-ttu-id="4c1fc-112">Командлеты командной консоли Exchange — это расширения для Windows PowerShell, Командная консоль командной строки на основе задач и язык сценариев, предназначенный специально для администрирования системы.</span><span class="sxs-lookup"><span data-stu-id="4c1fc-112">The Exchange Management Shell cmdlets are extensions to Windows PowerShell, a task-based command-line shell and scripting language that is designed specifically for system administration.</span></span> <span data-ttu-id="4c1fc-113">Windows PowerShell построен на платформе .NET Framework и предоставляет объектно-ориентированный API для разработчиков командлетов, поставщиков и ведущих приложений.</span><span class="sxs-lookup"><span data-stu-id="4c1fc-113">Windows PowerShell is built on the .NET Framework, and provides an object-oriented API for cmdlet, provider, and host application developers.</span></span> <span data-ttu-id="4c1fc-114">Чтобы узнать о программировании Windows PowerShell, обратитесь к [пакету SDK для Windows PowerShell](http://msdn.microsoft.com/en-us/library/dd835506%28VS.85%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="4c1fc-114">To learn about Windows PowerShell programming, see the [Windows PowerShell SDK](http://msdn.microsoft.com/en-us/library/dd835506%28VS.85%29.aspx).</span></span>
  
<span data-ttu-id="4c1fc-115">Командлеты командной консоли Exchange принимают и возвращают объекты.</span><span class="sxs-lookup"><span data-stu-id="4c1fc-115">The Exchange Management Shell cmdlets accept and return objects.</span></span> <span data-ttu-id="4c1fc-116">Список командлетов командной консоли Exchange и их входных и выходных данных можно найти в разделе [input and Output Type командлета командной консоли Exchange](exchange-management-shell-cmdlet-input-and-output-types.md).</span><span class="sxs-lookup"><span data-stu-id="4c1fc-116">For a list of Exchange management shell cmdlets and their input and output types, see [Exchange Management Shell cmdlet input and output types](exchange-management-shell-cmdlet-input-and-output-types.md).</span></span>
  
## <a name="in-this-section"></a><span data-ttu-id="4c1fc-117">В этом разделе</span><span class="sxs-lookup"><span data-stu-id="4c1fc-117">In this section</span></span>

- [<span data-ttu-id="4c1fc-118">Новые и обновленные командлеты командной консоли Exchange</span><span class="sxs-lookup"><span data-stu-id="4c1fc-118">New and updated Exchange Management Shell cmdlets</span></span>](new-and-updated-exchange-management-shell-cmdlets.md)  
- [<span data-ttu-id="4c1fc-119">Типы входных и выходных данных командлетов командной консоли Exchange</span><span class="sxs-lookup"><span data-stu-id="4c1fc-119">Exchange Management Shell cmdlet input and output types</span></span>](exchange-management-shell-cmdlet-input-and-output-types.md)
- [<span data-ttu-id="4c1fc-120">Получение списка пользователей почты с помощью командной консоли Exchange</span><span class="sxs-lookup"><span data-stu-id="4c1fc-120">Get a list of mail users by using the Exchange Management Shell</span></span>](how-to-get-a-list-of-mail-users-by-using-the-exchange-management-shell.md)
- [<span data-ttu-id="4c1fc-121">Использование ответа командлета командной консоли Exchange</span><span class="sxs-lookup"><span data-stu-id="4c1fc-121">Use the Exchange Management Shell cmdlet response</span></span>](how-to-use-the-exchange-management-shell-cmdlet-response.md)


## <a name="see-also"></a><span data-ttu-id="4c1fc-122">См. также</span><span class="sxs-lookup"><span data-stu-id="4c1fc-122">See also</span></span>

- [<span data-ttu-id="4c1fc-123">Пространства имен командной консоли Exchange</span><span class="sxs-lookup"><span data-stu-id="4c1fc-123">Exchange Management Shell namespaces</span></span>](exchange-management-shell-namespaces.md)  
- [<span data-ttu-id="4c1fc-124">PowerShell в Exchange Server (Командная консоль Exchange)</span><span class="sxs-lookup"><span data-stu-id="4c1fc-124">Exchange Server PowerShell (Exchange Management Shell)</span></span>](https://docs.microsoft.com/en-us/powershell/exchange/exchange-server/exchange-management-shell?view=exchange-ps)  
- [<span data-ttu-id="4c1fc-125">Windows PowerShell</span><span class="sxs-lookup"><span data-stu-id="4c1fc-125">Windows PowerShell</span></span>](http://msdn.microsoft.com/en-us/library/dd835506%28v=vs.85%29.aspx)
    

