---
title: Олицетворение и EWS в Exchange
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
localization_priority: Normal
ms.assetid: 7e1ea63c-eb29-43d2-827f-2f2b1846483b
description: Узнайте, как и когда использовать олицетворение в приложениях службы Exchange.
ms.openlocfilehash: f8a215874475034f0d147b80a05cae414e6438f9
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761131"
---
# <a name="impersonation-and-ews-in-exchange"></a><span data-ttu-id="a56ed-103">Олицетворение и EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="a56ed-103">Impersonation and EWS in Exchange</span></span>

<span data-ttu-id="a56ed-104">Узнайте, как и когда использовать олицетворение в [приложениях службы](ews-application-types.md)Exchange.</span><span class="sxs-lookup"><span data-stu-id="a56ed-104">Learn how and when to use impersonation in your Exchange [service applications](ews-application-types.md).</span></span>
  
<span data-ttu-id="a56ed-105">Вы можете разрешить пользователям доступ к почтовым ящикам других пользователей одним из трех способов:</span><span class="sxs-lookup"><span data-stu-id="a56ed-105">You can enable users to access other users' mailboxes in one of three ways:</span></span>
  
- <span data-ttu-id="a56ed-106">Путем добавления делегатов и указания разрешений для каждого делегата.</span><span class="sxs-lookup"><span data-stu-id="a56ed-106">By adding delegates and specifying permissions for each delegate.</span></span>
    
- <span data-ttu-id="a56ed-107">Путем непосредственного изменения разрешений на доступ к папке.</span><span class="sxs-lookup"><span data-stu-id="a56ed-107">By modifying folder permissions directly.</span></span>
    
- <span data-ttu-id="a56ed-108">С помощью олицетворения.</span><span class="sxs-lookup"><span data-stu-id="a56ed-108">By using impersonation.</span></span>
    
<span data-ttu-id="a56ed-109">Когда следует выбирать олицетворение для делегирования или разрешений для папки?</span><span class="sxs-lookup"><span data-stu-id="a56ed-109">When should you choose impersonation over delegation or folder permissions?</span></span> <span data-ttu-id="a56ed-110">Следующие рекомендации помогут вам принять решение:</span><span class="sxs-lookup"><span data-stu-id="a56ed-110">The following guidelines will help you decide:</span></span>
  
- <span data-ttu-id="a56ed-111">Используйте разрешения папки, если вы хотите предоставить пользователю доступ к папке, но не хотите, чтобы у пользователя были разрешения "Отправить от имени".</span><span class="sxs-lookup"><span data-stu-id="a56ed-111">Use folder permissions when you want to provide a user access to a folder but do not want the user to have "send on behalf of" permissions.</span></span> 
    
- <span data-ttu-id="a56ed-112">Используйте делегированный доступ, если вы хотите предоставить одному пользователю разрешение на выполнение действий от имени другого пользователя.</span><span class="sxs-lookup"><span data-stu-id="a56ed-112">Use delegate access when you want to give one user permission to perform work on behalf of another user.</span></span> <span data-ttu-id="a56ed-113">Обычно это разрешение "один к одному" или "один ко многим" — например, один помощник по администрированию управляет календарем для администратора или планировщиком одной комнаты, управляющим календарями для группы комнат для собраний.</span><span class="sxs-lookup"><span data-stu-id="a56ed-113">Typically, this is a one-to-one or one-to-a-few permission - for example, a single administrative assistant managing the calendar for an administrator, or a single room scheduler managing the calendars for a group of meeting rooms.</span></span>
    
- <span data-ttu-id="a56ed-114">Используйте олицетворение, если у вас есть приложение службы, которому требуется доступ к нескольким почтовым ящикам, и "работа от имени владельца почтового ящика".</span><span class="sxs-lookup"><span data-stu-id="a56ed-114">Use impersonation when you have a service application that needs to access multiple mailboxes and "act as" the mailbox owner.</span></span>
    
<span data-ttu-id="a56ed-115">Олицетворение является лучшим выбором при работе с несколькими почтовыми ящиками, так как вы можете легко предоставить доступ к одному учетной записи службы для каждого почтового ящика в базе данных.</span><span class="sxs-lookup"><span data-stu-id="a56ed-115">Impersonation is the best choice when you're dealing with multiple mailboxes because you can easily grant one service account access to every mailbox in a database.</span></span> <span data-ttu-id="a56ed-116">Разрешения на делегирование и папки лучше всего предоставить доступ только нескольким пользователям, так как необходимо добавлять разрешения по отдельности для каждого почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="a56ed-116">Delegation and folder permissions are best when you're only granting access to a few users, because you have to add permissions individually to each mailbox.</span></span> <span data-ttu-id="a56ed-117">На рисунке 1 показаны некоторые различия между типами доступа.</span><span class="sxs-lookup"><span data-stu-id="a56ed-117">Figure 1 shows some of the differences between each type of access.</span></span>
  
<span data-ttu-id="a56ed-118">**Рис. 1. Способы доступа к почтовым ящикам других пользователей**</span><span class="sxs-lookup"><span data-stu-id="a56ed-118">**Figure 1. Ways to access other users' mailboxes**</span></span>

![Схема, на которой показаны типы доступа к почтовому ящику, связь между владельцами почтовых ящиков и делегатом для каждого типа, а также тип разрешения. Отправка от лица разрешений для делегирования и разрешений папок. Отправка как разрешений для олицетворения.](media/Ex15_Delegate_Overview.png)
  
<span data-ttu-id="a56ed-122">Олицетворение идеально подходит для приложений, которые подключаются к Exchange Online, Exchange Online в составе Office 365 и локальных версий Exchange, а также выполняют операции, такие как архивирование электронной почты, Автоматическое Ручное задание на отпуск или любые другие задачи, которые требуют, чтобы приложение действовало в качестве владельца почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="a56ed-122">Impersonation is ideal for applications that connect to Exchange Online, Exchange Online as part of Office 365, and on-premises versions of Exchange and perform operations, such as archiving email, setting OOF automatically for users on vacation, or any other task that requires that the application act as the owner of a mailbox.</span></span> <span data-ttu-id="a56ed-123">Когда приложение использует олицетворение для отправки сообщения, оно отправляется от владельца почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="a56ed-123">When an application uses impersonation to send a message, the email appears to be sent from the mailbox owner.</span></span> <span data-ttu-id="a56ed-124">У получателя нет способа узнать, что почта была отправлена учетной записью службы.</span><span class="sxs-lookup"><span data-stu-id="a56ed-124">There is no way for the recipient to know the mail was sent by the service account.</span></span> <span data-ttu-id="a56ed-125">Делегирование, с другой стороны, дает другой учетной записи почтового ящика разрешение на действие от имени владельца почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="a56ed-125">Delegation, on the other hand, gives another mailbox account permission to act on behalf of a mailbox owner.</span></span> <span data-ttu-id="a56ed-126">Когда представителю отправляется сообщение электронной почты, значение "от" определяет владельца почтового ящика, а значение "sender" определяет делегата, который отправил почту.</span><span class="sxs-lookup"><span data-stu-id="a56ed-126">When an email message is sent by a delegate, the "from" value identifies the mailbox owner, and the "sender" value identifies the delegate that sent the mail.</span></span> 
  
## <a name="security-considerations-for-impersonation"></a><span data-ttu-id="a56ed-127">Вопросы безопасности для олицетворения</span><span class="sxs-lookup"><span data-stu-id="a56ed-127">Security considerations for impersonation</span></span>

<span data-ttu-id="a56ed-128">Олицетворение позволяет вызывающему абоненту олицетворять определенную учетную запись пользователя.</span><span class="sxs-lookup"><span data-stu-id="a56ed-128">Impersonation enables a caller to impersonate a given user account.</span></span> <span data-ttu-id="a56ed-129">Это позволяет вызывающему абоненту выполнять операции с помощью разрешений, которые связаны с олицетворенной учетной записью, а не с разрешениями, связанными с учетной записью вызывающего абонента.</span><span class="sxs-lookup"><span data-stu-id="a56ed-129">This enables the caller to perform operations by using the permissions that are associated with the impersonated account, instead of the permissions that are associated with the caller's account.</span></span> <span data-ttu-id="a56ed-130">По этой причине следует учитывать следующие вопросы безопасности:</span><span class="sxs-lookup"><span data-stu-id="a56ed-130">For this reason, you should be aware of the following security considerations:</span></span>
  
- <span data-ttu-id="a56ed-131">Только учетные записи, которым администратор сервера Exchange предоставил роль **ApplicationImpersonation** , могут использовать олицетворение.</span><span class="sxs-lookup"><span data-stu-id="a56ed-131">Only accounts that have been granted the **ApplicationImpersonation** role by an Exchange server administrator can use impersonation.</span></span> 
    
- <span data-ttu-id="a56ed-132">Необходимо создать область управления, ограничивающую олицетворение указанной группой учетных записей.</span><span class="sxs-lookup"><span data-stu-id="a56ed-132">You should create a management scope that limits impersonation to a specified group of accounts.</span></span> <span data-ttu-id="a56ed-133">Если область управления не создана, роль **ApplicationImpersonation** предоставляется всем учетным записям в Организации.</span><span class="sxs-lookup"><span data-stu-id="a56ed-133">If you do not create a management scope, the **ApplicationImpersonation** role is granted to all accounts in an organization.</span></span> 
    
- <span data-ttu-id="a56ed-134">Как правило, роль **ApplicationImpersonation** предоставляется учетной записи службы, выделенной для конкретного приложения или группы приложений, а не учетной записи пользователя.</span><span class="sxs-lookup"><span data-stu-id="a56ed-134">Typically, the **ApplicationImpersonation** role is granted to a service account dedicated to a particular application or group of applications, rather than a user account.</span></span> <span data-ttu-id="a56ed-135">Можно создать любое необходимое количество учетных записей служб.</span><span class="sxs-lookup"><span data-stu-id="a56ed-135">You can create as many or as few service accounts as you need.</span></span> 
    
<span data-ttu-id="a56ed-136">Вы можете ознакомиться с дополнительными сведениями о [настройке олицетворения](how-to-configure-impersonation.md), но вы должны обратиться к администратору Exchange, чтобы убедиться, что созданы учетные записи служб с [разрешениями и доступом](http://technet.microsoft.com/en-us/library/dd351175%28v=exchg.150%29.aspx) , удовлетворяющими требованиям безопасности Организации.</span><span class="sxs-lookup"><span data-stu-id="a56ed-136">You can read more about [configuring impersonation](how-to-configure-impersonation.md), but you should work with your Exchange administrator to ensure that the service accounts that you need are created with the [permissions and access](http://technet.microsoft.com/en-us/library/dd351175%28v=exchg.150%29.aspx) that meet the security requirements of your organization.</span></span> 
  
## <a name="in-this-section"></a><span data-ttu-id="a56ed-137">В этом разделе</span><span class="sxs-lookup"><span data-stu-id="a56ed-137">In this section</span></span>

- [<span data-ttu-id="a56ed-138">Настройка олицетворения</span><span class="sxs-lookup"><span data-stu-id="a56ed-138">Configure impersonation</span></span>](how-to-configure-impersonation.md)
    
- [<span data-ttu-id="a56ed-139">Идентификация учетной записи для олицетворения</span><span class="sxs-lookup"><span data-stu-id="a56ed-139">Identify the account to impersonate</span></span>](how-to-identify-the-account-to-impersonate.md)
    
- [<span data-ttu-id="a56ed-140">Добавление встреч с помощью олицетворения Exchange</span><span class="sxs-lookup"><span data-stu-id="a56ed-140">Add appointments by using Exchange impersonation</span></span>](how-to-add-appointments-by-using-exchange-impersonation.md)
    
## <a name="see-also"></a><span data-ttu-id="a56ed-141">См. также</span><span class="sxs-lookup"><span data-stu-id="a56ed-141">See also</span></span>


- [<span data-ttu-id="a56ed-142">Разработка клиентов веб-служб для Exchange</span><span class="sxs-lookup"><span data-stu-id="a56ed-142">Develop web service clients for Exchange</span></span>](develop-web-service-clients-for-exchange.md)
    
- [<span data-ttu-id="a56ed-143">Передача прав доступа и EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="a56ed-143">Delegate access and EWS in Exchange</span></span>](delegate-access-and-ews-in-exchange.md)
    
- [<span data-ttu-id="a56ed-144">Разрешения Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="a56ed-144">Exchange 2013 Permissions</span></span>](http://technet.microsoft.com/en-us/library/dd351175%28v=exchg.150%29.aspx)
    

