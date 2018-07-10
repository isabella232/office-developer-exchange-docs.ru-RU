---
title: Олицетворение и веб-службах Exchange
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
localization_priority: Normal
ms.assetid: 7e1ea63c-eb29-43d2-827f-2f2b1846483b
description: Узнайте, как и когда использование олицетворения в приложениях службы Exchange.
ms.openlocfilehash: f8a215874475034f0d147b80a05cae414e6438f9
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761131"
---
# <a name="impersonation-and-ews-in-exchange"></a><span data-ttu-id="bf1fb-103">Олицетворение и веб-службах Exchange</span><span class="sxs-lookup"><span data-stu-id="bf1fb-103">Impersonation and EWS in Exchange</span></span>

<span data-ttu-id="bf1fb-104">Узнайте, как и когда использование олицетворения в [приложений-служб](ews-application-types.md)Exchange.</span><span class="sxs-lookup"><span data-stu-id="bf1fb-104">Learn how and when to use impersonation in your Exchange [service applications](ews-application-types.md).</span></span>
  
<span data-ttu-id="bf1fb-105">Можно предоставить пользователям возможность доступа к почтовым ящикам других пользователей в одном из трех следующих способов:</span><span class="sxs-lookup"><span data-stu-id="bf1fb-105">You can enable users to access other users' mailboxes in one of three ways:</span></span>
  
- <span data-ttu-id="bf1fb-106">Добавление делегатов и задание разрешений для каждого делегата.</span><span class="sxs-lookup"><span data-stu-id="bf1fb-106">By adding delegates and specifying permissions for each delegate.</span></span>
    
- <span data-ttu-id="bf1fb-107">Путем изменения разрешений для папки напрямую.</span><span class="sxs-lookup"><span data-stu-id="bf1fb-107">By modifying folder permissions directly.</span></span>
    
- <span data-ttu-id="bf1fb-108">С помощью олицетворения.</span><span class="sxs-lookup"><span data-stu-id="bf1fb-108">By using impersonation.</span></span>
    
<span data-ttu-id="bf1fb-109">Когда следует выбрать олицетворения через разрешения делегирования или папки</span><span class="sxs-lookup"><span data-stu-id="bf1fb-109">When should you choose impersonation over delegation or folder permissions?</span></span> <span data-ttu-id="bf1fb-110">Следующие рекомендации помогут выбрать подходящий:</span><span class="sxs-lookup"><span data-stu-id="bf1fb-110">The following guidelines will help you decide:</span></span>
  
- <span data-ttu-id="bf1fb-111">Используйте разрешений папки необходимо предоставить пользователю доступ к папке, но не требуется, чтобы пользователь имеет разрешения «Отправить от имени».</span><span class="sxs-lookup"><span data-stu-id="bf1fb-111">Use folder permissions when you want to provide a user access to a folder but do not want the user to have "send on behalf of" permissions.</span></span> 
    
- <span data-ttu-id="bf1fb-112">Используйте делегированный доступ, если вы хотите указать одного разрешения пользователя для выполнения операций от имени другого пользователя.</span><span class="sxs-lookup"><span data-stu-id="bf1fb-112">Use delegate access when you want to give one user permission to perform work on behalf of another user.</span></span> <span data-ttu-id="bf1fb-113">Как правило это разрешение одному "или" один к несколько -, например одного помощника управление календаря для администратора или планировщик единого места, управление календарями для группы комнаты для собраний.</span><span class="sxs-lookup"><span data-stu-id="bf1fb-113">Typically, this is a one-to-one or one-to-a-few permission - for example, a single administrative assistant managing the calendar for an administrator, or a single room scheduler managing the calendars for a group of meeting rooms.</span></span>
    
- <span data-ttu-id="bf1fb-114">Использование олицетворения при наличии приложения-службы, которую требуется получить доступ к нескольким почтовым ящикам и «выступать в качестве» владельца почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="bf1fb-114">Use impersonation when you have a service application that needs to access multiple mailboxes and "act as" the mailbox owner.</span></span>
    
<span data-ttu-id="bf1fb-115">Олицетворение является оптимальным выбором, когда вы имеете дело с нескольких почтовых ящиков, так как можно легко предоставлять одной учетной записи службы доступа для всех почтовых ящиков в базе данных.</span><span class="sxs-lookup"><span data-stu-id="bf1fb-115">Impersonation is the best choice when you're dealing with multiple mailboxes because you can easily grant one service account access to every mailbox in a database.</span></span> <span data-ttu-id="bf1fb-116">Разрешения для делегирования и папок, наиболее при только в случае предоставления доступа для нескольких пользователей, так как требуется добавить разрешения отдельно для каждого почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="bf1fb-116">Delegation and folder permissions are best when you're only granting access to a few users, because you have to add permissions individually to each mailbox.</span></span> <span data-ttu-id="bf1fb-117">На рисунке 1 показаны некоторые различия между каждый тип доступа.</span><span class="sxs-lookup"><span data-stu-id="bf1fb-117">Figure 1 shows some of the differences between each type of access.</span></span>
  
<span data-ttu-id="bf1fb-118">**На рисунке 1. Способы доступа к почтовым ящикам других пользователей**</span><span class="sxs-lookup"><span data-stu-id="bf1fb-118">**Figure 1. Ways to access other users' mailboxes**</span></span>

![Схема, на которой показаны типы доступа к почтовому ящику, связь между владельцами почтовых ящиков и делегатом для каждого типа, а также тип разрешения. Отправка от лица разрешений для делегирования и разрешений папок. Отправка как разрешений для олицетворения.](media/Ex15_Delegate_Overview.png)
  
<span data-ttu-id="bf1fb-122">Олицетворение идеально подходит для приложений, которые подключаются к Exchange Online, Exchange Online в составе Office 365 и локальной версии Exchange и выполнения операций, таких как архивации электронной почты, параметр об отсутствии на работе автоматически для пользователей, отпуска или любой другой задачи который требуется, что приложение выступать в качестве владельца почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="bf1fb-122">Impersonation is ideal for applications that connect to Exchange Online, Exchange Online as part of Office 365, and on-premises versions of Exchange and perform operations, such as archiving email, setting OOF automatically for users on vacation, or any other task that requires that the application act as the owner of a mailbox.</span></span> <span data-ttu-id="bf1fb-123">Когда приложение использует олицетворение для отправки сообщения, появится сообщение электронной почты для отправки из владельца почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="bf1fb-123">When an application uses impersonation to send a message, the email appears to be sent from the mailbox owner.</span></span> <span data-ttu-id="bf1fb-124">Нет возможности для получателя о том, что сообщение было отправлено функцией учетной записи службы.</span><span class="sxs-lookup"><span data-stu-id="bf1fb-124">There is no way for the recipient to know the mail was sent by the service account.</span></span> <span data-ttu-id="bf1fb-125">Делегирование, с другой стороны, предоставляет другой учетной записи почтовому ящику действовать от имени владельца почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="bf1fb-125">Delegation, on the other hand, gives another mailbox account permission to act on behalf of a mailbox owner.</span></span> <span data-ttu-id="bf1fb-126">При отправке сообщения электронной почты с делегата, значение «от» определяет владельца почтового ящика и значение «отправитель» определяет делегата, отправленных сообщений.</span><span class="sxs-lookup"><span data-stu-id="bf1fb-126">When an email message is sent by a delegate, the "from" value identifies the mailbox owner, and the "sender" value identifies the delegate that sent the mail.</span></span> 
  
## <a name="security-considerations-for-impersonation"></a><span data-ttu-id="bf1fb-127">Рекомендации по безопасности для олицетворения</span><span class="sxs-lookup"><span data-stu-id="bf1fb-127">Security considerations for impersonation</span></span>

<span data-ttu-id="bf1fb-128">Олицетворение позволяет абоненту просматривать олицетворять учетную запись указанного пользователя.</span><span class="sxs-lookup"><span data-stu-id="bf1fb-128">Impersonation enables a caller to impersonate a given user account.</span></span> <span data-ttu-id="bf1fb-129">Это позволяет вызывающего абонента для выполнения операций с помощью разрешений, которые связаны с олицетворенным учетную запись, вместо разрешения, которые связаны с учетной записью вызывающего абонента.</span><span class="sxs-lookup"><span data-stu-id="bf1fb-129">This enables the caller to perform operations by using the permissions that are associated with the impersonated account, instead of the permissions that are associated with the caller's account.</span></span> <span data-ttu-id="bf1fb-130">По этой причине необходимо принять во внимание следующее:</span><span class="sxs-lookup"><span data-stu-id="bf1fb-130">For this reason, you should be aware of the following security considerations:</span></span>
  
- <span data-ttu-id="bf1fb-131">Только учетные записи, которым были присвоены роль **ApplicationImpersonation** администратором Exchange server можно использовать олицетворения.</span><span class="sxs-lookup"><span data-stu-id="bf1fb-131">Only accounts that have been granted the **ApplicationImpersonation** role by an Exchange server administrator can use impersonation.</span></span> 
    
- <span data-ttu-id="bf1fb-132">Необходимо создать области управления, которая ограничивает олицетворения для указанной группы учетных записей.</span><span class="sxs-lookup"><span data-stu-id="bf1fb-132">You should create a management scope that limits impersonation to a specified group of accounts.</span></span> <span data-ttu-id="bf1fb-133">Если не создавать области управления, роль **ApplicationImpersonation** предоставляется для всех учетных записей в организации.</span><span class="sxs-lookup"><span data-stu-id="bf1fb-133">If you do not create a management scope, the **ApplicationImpersonation** role is granted to all accounts in an organization.</span></span> 
    
- <span data-ttu-id="bf1fb-134">Как правило роль **ApplicationImpersonation** предоставляется учетной записи службы, выделенным для отдельного приложения или группы приложений, а не учетной записи пользователя.</span><span class="sxs-lookup"><span data-stu-id="bf1fb-134">Typically, the **ApplicationImpersonation** role is granted to a service account dedicated to a particular application or group of applications, rather than a user account.</span></span> <span data-ttu-id="bf1fb-135">При необходимости можно создать как числа учетных записей служб.</span><span class="sxs-lookup"><span data-stu-id="bf1fb-135">You can create as many or as few service accounts as you need.</span></span> 
    
<span data-ttu-id="bf1fb-136">Вы можете читать Дополнительные сведения о [настройке олицетворения](how-to-configure-impersonation.md), но должны работать с администратор Exchange, чтобы убедиться, что созданы учетные записи служб, которые необходимы [разрешения и доступ](http://technet.microsoft.com/ru-ru/library/dd351175%28v=exchg.150%29.aspx) , соответствующие требованиям безопасности вашей организация.</span><span class="sxs-lookup"><span data-stu-id="bf1fb-136">You can read more about [configuring impersonation](how-to-configure-impersonation.md), but you should work with your Exchange administrator to ensure that the service accounts that you need are created with the [permissions and access](http://technet.microsoft.com/ru-ru/library/dd351175%28v=exchg.150%29.aspx) that meet the security requirements of your organization.</span></span> 
  
## <a name="in-this-section"></a><span data-ttu-id="bf1fb-137">В этом разделе</span><span class="sxs-lookup"><span data-stu-id="bf1fb-137">In this section</span></span>

- [<span data-ttu-id="bf1fb-138">Настройка олицетворения</span><span class="sxs-lookup"><span data-stu-id="bf1fb-138">Configure impersonation</span></span>](how-to-configure-impersonation.md)
    
- [<span data-ttu-id="bf1fb-139">Идентификация учетной записи для олицетворения</span><span class="sxs-lookup"><span data-stu-id="bf1fb-139">Identify the account to impersonate</span></span>](how-to-identify-the-account-to-impersonate.md)
    
- [<span data-ttu-id="bf1fb-140">Добавление встреч с использованием олицетворения Exchange</span><span class="sxs-lookup"><span data-stu-id="bf1fb-140">Add appointments by using Exchange impersonation</span></span>](how-to-add-appointments-by-using-exchange-impersonation.md)
    
## <a name="see-also"></a><span data-ttu-id="bf1fb-141">См. также</span><span class="sxs-lookup"><span data-stu-id="bf1fb-141">See also</span></span>


- [<span data-ttu-id="bf1fb-142">Разработка клиентов веб-служб для Exchange</span><span class="sxs-lookup"><span data-stu-id="bf1fb-142">Develop web service clients for Exchange</span></span>](develop-web-service-clients-for-exchange.md)
    
- [<span data-ttu-id="bf1fb-143">Передача прав доступа и EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="bf1fb-143">Delegate access and EWS in Exchange</span></span>](delegate-access-and-ews-in-exchange.md)
    
- [<span data-ttu-id="bf1fb-144">Разрешения Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="bf1fb-144">Exchange 2013 Permissions</span></span>](http://technet.microsoft.com/ru-ru/library/dd351175%28v=exchg.150%29.aspx)
    

