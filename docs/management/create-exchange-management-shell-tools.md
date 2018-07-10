---
title: Создание средств управления Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 46e4812f-37a8-449f-bd37-bc4a94605db9
description: Найдите сведения, чтобы приступить к созданию средств управления Exchange для Exchange.
ms.openlocfilehash: e8414460007f333e50c9d596bf977792977b1e4e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761248"
---
# <a name="create-exchange-management-shell-tools"></a><span data-ttu-id="ae099-103">Создание средств управления Exchange</span><span class="sxs-lookup"><span data-stu-id="ae099-103">Create Exchange Management Shell tools</span></span>

<span data-ttu-id="ae099-104">Найдите сведения, чтобы приступить к созданию средств управления Exchange для Exchange.</span><span class="sxs-lookup"><span data-stu-id="ae099-104">Find information to get started creating Exchange Management Shell tools for Exchange.</span></span>

<span data-ttu-id="ae099-105">**Применимо к:** Exchange Online | Exchange Server 2013 | Office 365</span><span class="sxs-lookup"><span data-stu-id="ae099-105">**Applies to:** Exchange Online | Exchange Server 2013 | Office 365</span></span>
  
<span data-ttu-id="ae099-106">Командная консоль Exchange предоставляет набор команд, вычисленное на платформе Windows PowerShell для управления Exchange Online, Exchange Online в составе Office 365 или более в локальной версии Exchange, начиная с Exchange 2013.</span><span class="sxs-lookup"><span data-stu-id="ae099-106">The Exchange Management Shell provides a rich set of commands, based on the Windows PowerShell platform, for managing Exchange Online, Exchange Online as part of Office 365, or an on-premises version of Exchange starting with Exchange 2013.</span></span> <span data-ttu-id="ae099-107">Можно использовать команды в консоли управления Exchange для автоматизации администрирования сервера путем выполнения команды непосредственно или с помощью сценариев.</span><span class="sxs-lookup"><span data-stu-id="ae099-107">You can use Exchange Management Shell commands to automate the administration of a server by directly executing the commands, or by using command scripts.</span></span>
  
<span data-ttu-id="ae099-108">Если необходимо использовать команды командной консоли Exchange в приложение внешнего размещения, таких как административное приложение, на котором работает на рабочем столе администратора или с помощью веб-приложения, можно позвонить командлетам командной консоли Exchange из в приложении Visual Basic или C# для управления Exchange server.</span><span class="sxs-lookup"><span data-stu-id="ae099-108">If you need to use Exchange Management Shell commands from within a hosting application, such as an administrative application that is running on the administrator's desktop or through a web-based application, you can call Exchange Management Shell cmdlets from within your Visual Basic or C# application to manage an Exchange server.</span></span>
  
## <a name="get-started-with-exchange-management-shell-tools"></a><span data-ttu-id="ae099-109">Начало работы со средствами командной консоли Exchange</span><span class="sxs-lookup"><span data-stu-id="ae099-109">Get started with Exchange Management Shell tools</span></span>
<span data-ttu-id="ae099-110"><a name="SP15GettingStartedTemplate_WhatDoYouNeed"> </a></span><span class="sxs-lookup"><span data-stu-id="ae099-110"></span></span>

<span data-ttu-id="ae099-111">Если вы знакомы с созданием Windows PowerShell ведущие приложения, для просмотра пример, в котором показано, как вызывать командлетов командной консоли Exchange из приложения или пример типы приложений, которые можно создать с помощью Exchange Командлеты командной консоли управления, в разделе [получить список почтовых пользователей с помощью командной консоли Exchange](how-to-get-a-list-of-mail-users-by-using-the-exchange-management-shell.md).</span><span class="sxs-lookup"><span data-stu-id="ae099-111">If you are familiar with creating Windows PowerShell host applications and want to see an example that shows how to call the Exchange Management Shell cmdlets from an application, or to see an example of the types of applications that you can create by using the Exchange Management Shell cmdlets, see [Get a list of mail users by using the Exchange Management Shell](how-to-get-a-list-of-mail-users-by-using-the-exchange-management-shell.md).</span></span>
  
<span data-ttu-id="ae099-112">Командлеты командной консоли Exchange представляют собой расширения на основе задач оболочка командной строки и язык сценариев, предназначенный специально для администрирования системы Windows PowerShell.</span><span class="sxs-lookup"><span data-stu-id="ae099-112">The Exchange Management Shell cmdlets are extensions to Windows PowerShell, a task-based command-line shell and scripting language that is designed specifically for system administration.</span></span> <span data-ttu-id="ae099-113">Windows PowerShell создан на основе .NET Framework и предоставляет объектно ориентированные API-Интерфейс для командлета, поставщика и разработчиков приложений узла.</span><span class="sxs-lookup"><span data-stu-id="ae099-113">Windows PowerShell is built on the .NET Framework, and provides an object-oriented API for cmdlet, provider, and host application developers.</span></span> <span data-ttu-id="ae099-114">Чтобы узнать о программировании решений на базе Windows PowerShell, обратитесь к разделу [Пакет SDK для Windows PowerShell](http://msdn.microsoft.com/ru-ru/library/dd835506%28VS.85%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="ae099-114">To learn about Windows PowerShell programming, see the [Windows PowerShell SDK](http://msdn.microsoft.com/ru-ru/library/dd835506%28VS.85%29.aspx).</span></span>
  
<span data-ttu-id="ae099-115">Командлеты командной консоли Exchange принимают и возвращают объекты.</span><span class="sxs-lookup"><span data-stu-id="ae099-115">The Exchange Management Shell cmdlets accept and return objects.</span></span> <span data-ttu-id="ae099-116">Список командлетов командной консоли управления Exchange и их типы ввода-вывода, в разделе [командлет командной консоли Exchange ввода и вывода типов](exchange-management-shell-cmdlet-input-and-output-types.md).</span><span class="sxs-lookup"><span data-stu-id="ae099-116">For a list of Exchange management shell cmdlets and their input and output types, see [Exchange Management Shell cmdlet input and output types](exchange-management-shell-cmdlet-input-and-output-types.md).</span></span>
  
## <a name="in-this-section"></a><span data-ttu-id="ae099-117">В этом разделе</span><span class="sxs-lookup"><span data-stu-id="ae099-117">In this section</span></span>

- [<span data-ttu-id="ae099-118">Новые и обновленные командлеты командной консоли Exchange</span><span class="sxs-lookup"><span data-stu-id="ae099-118">New and updated Exchange Management Shell cmdlets</span></span>](new-and-updated-exchange-management-shell-cmdlets.md)  
- [<span data-ttu-id="ae099-119">Входные данные командлета Командная консоль Exchange и вывод типов</span><span class="sxs-lookup"><span data-stu-id="ae099-119">Exchange Management Shell cmdlet input and output types</span></span>](exchange-management-shell-cmdlet-input-and-output-types.md)
- [<span data-ttu-id="ae099-120">Ознакомьтесь со списком пользователей почты с помощью командной консоли Exchange</span><span class="sxs-lookup"><span data-stu-id="ae099-120">Get a list of mail users by using the Exchange Management Shell</span></span>](how-to-get-a-list-of-mail-users-by-using-the-exchange-management-shell.md)
- [<span data-ttu-id="ae099-121">Использование ответа командлет командной консоли Exchange</span><span class="sxs-lookup"><span data-stu-id="ae099-121">Use the Exchange Management Shell cmdlet response</span></span>](how-to-use-the-exchange-management-shell-cmdlet-response.md)


## <a name="see-also"></a><span data-ttu-id="ae099-122">См. также</span><span class="sxs-lookup"><span data-stu-id="ae099-122">See also</span></span>

- [<span data-ttu-id="ae099-123">Пространства имен Командная консоль Exchange</span><span class="sxs-lookup"><span data-stu-id="ae099-123">Exchange Management Shell namespaces</span></span>](exchange-management-shell-namespaces.md)  
- [<span data-ttu-id="ae099-124">Exchange Server PowerShell (Командная консоль Exchange)</span><span class="sxs-lookup"><span data-stu-id="ae099-124">Exchange Server PowerShell (Exchange Management Shell)</span></span>](https://docs.microsoft.com/ru-ru/powershell/exchange/exchange-server/exchange-management-shell?view=exchange-ps)  
- [<span data-ttu-id="ae099-125">Windows PowerShell</span><span class="sxs-lookup"><span data-stu-id="ae099-125">Windows PowerShell</span></span>](http://msdn.microsoft.com/ru-ru/library/dd835506%28v=vs.85%29.aspx)
    

