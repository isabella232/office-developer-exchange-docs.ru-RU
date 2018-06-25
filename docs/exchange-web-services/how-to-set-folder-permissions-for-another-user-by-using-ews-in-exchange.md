---
title: Настройка разрешений папки другого пользователя с помощью веб-служб Exchange в Exchange
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 7eb81676-a780-4c56-b4f2-c4ed2697107d
description: Узнайте, как установить уровни разрешений для папки с помощью управляемого интерфейса API веб-служб Exchange или веб-служб Exchange в Exchange.
ms.openlocfilehash: 5bf570612d6349628e7f3abf858daa33daa13745
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761120"
---
# <a name="set-folder-permissions-for-another-user-by-using-ews-in-exchange"></a><span data-ttu-id="1b246-103">Настройка разрешений папки другого пользователя с помощью веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="1b246-103">Set folder permissions for another user by using EWS in Exchange</span></span>

<span data-ttu-id="1b246-104">Узнайте, как установить уровни разрешений для папки с помощью управляемого интерфейса API веб-служб Exchange или веб-служб Exchange в Exchange.</span><span class="sxs-lookup"><span data-stu-id="1b246-104">Learn how to set permission levels on a folder by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="1b246-105">Разрешения на уровне папки позволяют пользователям получать доступ к одной или нескольких папок в почтового ящика другого пользователя.</span><span class="sxs-lookup"><span data-stu-id="1b246-105">Folder-level permissions enable users to access one or more folders in another user's mailbox.</span></span> <span data-ttu-id="1b246-106">Разрешения для папки, аналогичны делегированный доступ, но они отличаются следующими способами:</span><span class="sxs-lookup"><span data-stu-id="1b246-106">Folder permissions are similar to delegate access, but they differ in the following ways:</span></span> 
  
- <span data-ttu-id="1b246-107">Разрешения для папки не следует включать пользователю «отправить от имени» или «отправить как» другому пользователю.</span><span class="sxs-lookup"><span data-stu-id="1b246-107">Folder permissions do not enable a user to "send on behalf of" or "send as" another user.</span></span> <span data-ttu-id="1b246-108">Они только разрешение доступа к папкам.</span><span class="sxs-lookup"><span data-stu-id="1b246-108">They only enable access to folders.</span></span> <span data-ttu-id="1b246-109">Пользователи могут создавать элементы в папках, но они не могут отправлять их.</span><span class="sxs-lookup"><span data-stu-id="1b246-109">Users can create items in those folders, but they can't send them.</span></span>
    
- <span data-ttu-id="1b246-110">Можно задать разрешения для папки на любой папки в почтовом ящике, но можно только добавить делегата к папкам календаря, контакты, папки "Входящие", журнала, заметки и задачи.</span><span class="sxs-lookup"><span data-stu-id="1b246-110">You can set folder permissions on any folder in the mailbox, but you can only add a delegate to the Calendar, Contacts, Inbox, Journal, Notes, and Tasks folders.</span></span>
    
- <span data-ttu-id="1b246-111">Можно задать число [разрешения для указанной папки](#bk_folderperms).</span><span class="sxs-lookup"><span data-stu-id="1b246-111">You can set a number of [permissions on a specific folder](#bk_folderperms).</span></span> <span data-ttu-id="1b246-112">При добавлении делегата, можно назначить один из только [пять уровней разрешений](delegate-access-and-ews-in-exchange.md#bk_delegateperms).</span><span class="sxs-lookup"><span data-stu-id="1b246-112">When you add a delegate, you can assign one of only [five permission levels](delegate-access-and-ews-in-exchange.md#bk_delegateperms).</span></span>
    
- <span data-ttu-id="1b246-113">Можно задать разрешения для папки для анонимных и по умолчанию пользователи.</span><span class="sxs-lookup"><span data-stu-id="1b246-113">You can set folder permissions for anonymous and default users.</span></span> <span data-ttu-id="1b246-114">Можно предоставить делегированный доступ к учетной записи электронной почты.</span><span class="sxs-lookup"><span data-stu-id="1b246-114">You can only grant delegate access to a mail-enabled account.</span></span>
    
<span data-ttu-id="1b246-115">Если вы знакомы с помощью элементов управления доступом (ACE) и списки управления доступом (доступом), значит, что пользователь может иметь только один набор разрешений для каждой папки.</span><span class="sxs-lookup"><span data-stu-id="1b246-115">If you're familiar with Access Control Entries (ACEs) and Discretionary Access Control Lists (DACLs), you know that a user can only have one set of permissions for each folder.</span></span> <span data-ttu-id="1b246-116">При попытке добавить набор разрешений для пользователя, и они уже имеют набор разрешений, приведет к ошибке.</span><span class="sxs-lookup"><span data-stu-id="1b246-116">If you try to add a set of permissions for a user and they already have a set of permissions, you'll get an error.</span></span> <span data-ttu-id="1b246-117">При Добавление, удаление или обновление разрешений для папки, вы получение текущего на уровне пользователей, добавьте или удалите все элементы управления доступом и выберите отправить обновленные на уровне пользователей.</span><span class="sxs-lookup"><span data-stu-id="1b246-117">When you add, remove, or update permissions on a folder, you get the current DACL, add or remove any ACEs, and then send the updated DACL.</span></span> <span data-ttu-id="1b246-118">Не удается добавить несколько элементов управления доступом для одного пользователя.</span><span class="sxs-lookup"><span data-stu-id="1b246-118">You cannot add multiple ACEs for the same user.</span></span> <span data-ttu-id="1b246-119">При обновлении разрешения с помощью управляемого интерфейса API веб-служб Exchange, необходимо удалить элемент управления ДОСТУПОМ текущего пользователя, а затем добавьте свой новый элемент управления ДОСТУПОМ к коллекции.</span><span class="sxs-lookup"><span data-stu-id="1b246-119">When you update permissions by using the EWS Managed API, you need to remove the user's current ACE and then add their new ACE to the collection.</span></span> <span data-ttu-id="1b246-120">Если вы используете веб-служб Exchange, просто замените предыдущий набор элементов ACE с помощью новых структур.</span><span class="sxs-lookup"><span data-stu-id="1b246-120">If you're using EWS, you just replace the previous set of ACEs with the new ones.</span></span>
  
<span data-ttu-id="1b246-121">Если вы выполняете нескольких изменения разрешений в одной папке, можно batch добавления, удаления или обновления — только что Обратите внимание на то, что нельзя пакета обновления пользователя на несколько папок.</span><span class="sxs-lookup"><span data-stu-id="1b246-121">If you're making multiple permission changes to a single folder, you can batch additions, removals, or updates —just note that you cannot batch user updates on multiple folders.</span></span> <span data-ttu-id="1b246-122">Для получения разрешений для одной папке необходимо один звонок, а второй вызов требуется обновить разрешения для этой папки.</span><span class="sxs-lookup"><span data-stu-id="1b246-122">One call is required to get the permissions on a single folder, and a second call is required to update the permissions on that folder.</span></span> <span data-ttu-id="1b246-123">При Добавление, удаление или обновление разрешений пользователя, используется один и тот же вызовы двух методов или операции для каждой задачи.</span><span class="sxs-lookup"><span data-stu-id="1b246-123">When you add, remove, or update user permissions, you use the same two method calls or operations for each task.</span></span>
  
<span data-ttu-id="1b246-124">**В таблице 1. Управляемый API EWS методы и операции веб-служб Exchange для настройки разрешений папки**</span><span class="sxs-lookup"><span data-stu-id="1b246-124">**Table 1. EWS Managed API methods and EWS operations for setting folder permissions**</span></span>

|<span data-ttu-id="1b246-125">Задача</span><span class="sxs-lookup"><span data-stu-id="1b246-125">If you want to…</span></span>|<span data-ttu-id="1b246-126">Используйте этот метод управляемый API EWS...</span><span class="sxs-lookup"><span data-stu-id="1b246-126">Use this EWS Managed API method…</span></span>|<span data-ttu-id="1b246-127">Используйте эту операцию EWS...</span><span class="sxs-lookup"><span data-stu-id="1b246-127">Use this EWS operation…</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="1b246-128">Включение, удаление или обновление разрешений для папки</span><span class="sxs-lookup"><span data-stu-id="1b246-128">Enable, remove, or update folder permissions</span></span>  <br/> |<span data-ttu-id="1b246-129">[Folder.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) , а затем [Folder.Update](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.reply%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="1b246-129">[Folder.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) followed by [Folder.Update](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.reply%28v=exchg.80%29.aspx)</span></span> <br/> |<span data-ttu-id="1b246-130">[GetFolder](http://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) следуют [UpdateFolder](http://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="1b246-130">[GetFolder](http://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) followed by [UpdateFolder](http://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx)</span></span> <br/> |
|<span data-ttu-id="1b246-131">Создайте папку и определите разрешения для папки</span><span class="sxs-lookup"><span data-stu-id="1b246-131">Create a folder and define folder permissions</span></span>  <br/> |[<span data-ttu-id="1b246-132">Folder.Save</span><span class="sxs-lookup"><span data-stu-id="1b246-132">Folder.Save</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.save%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="1b246-133">CreateFolder</span><span class="sxs-lookup"><span data-stu-id="1b246-133">CreateFolder</span></span>](http://msdn.microsoft.com/library/6f6c334c-b190-4e55-8f0a-38f2a018d1b3%28Office.15%29.aspx) <br/> |
   
## <a name="folder-permissions"></a><span data-ttu-id="1b246-134">Разрешения для папки</span><span class="sxs-lookup"><span data-stu-id="1b246-134">Folder permissions</span></span>
<span data-ttu-id="1b246-135"><a name="bk_folderperms"> </a></span><span class="sxs-lookup"><span data-stu-id="1b246-135"></span></span>

<span data-ttu-id="1b246-136">Имеется довольно много параметров, когда речь идет о Установка разрешений для папки на указанной папки.</span><span class="sxs-lookup"><span data-stu-id="1b246-136">You have quite a few options when it comes to setting folder permissions on a specific folder.</span></span> <span data-ttu-id="1b246-137">Можно задать уровень разрешений для папки для каждого пользователя, который добавляет набор предварительно заданных отдельных разрешений в СПИСКЕ, или можно задать отдельные разрешения на папку, но нельзя смешивать и соответствует.</span><span class="sxs-lookup"><span data-stu-id="1b246-137">You can set a permission level on a folder for each user, which adds a set of predefined individual permissions to the DACL, or you can set individual permissions on a folder — but you can't mix and match.</span></span>
  
<span data-ttu-id="1b246-138">Доступны следующие отдельные разрешения:</span><span class="sxs-lookup"><span data-stu-id="1b246-138">The following individual permissions are available:</span></span>
  
- <span data-ttu-id="1b246-139">Можно создать</span><span class="sxs-lookup"><span data-stu-id="1b246-139">Can create</span></span>
- <span data-ttu-id="1b246-140">Можно создать вложенные папки</span><span class="sxs-lookup"><span data-stu-id="1b246-140">Can create subfolders</span></span>    
- <span data-ttu-id="1b246-141">— Это владелец</span><span class="sxs-lookup"><span data-stu-id="1b246-141">Is folder owner</span></span>    
- <span data-ttu-id="1b246-142">Отображается папки</span><span class="sxs-lookup"><span data-stu-id="1b246-142">Is folder visible</span></span>    
- <span data-ttu-id="1b246-143">— Это папка контактов</span><span class="sxs-lookup"><span data-stu-id="1b246-143">Is folder contact</span></span>    
- <span data-ttu-id="1b246-144">Изменение элементов</span><span class="sxs-lookup"><span data-stu-id="1b246-144">Edit items</span></span>    
- <span data-ttu-id="1b246-145">Удаление элементов</span><span class="sxs-lookup"><span data-stu-id="1b246-145">Delete items</span></span>    
- <span data-ttu-id="1b246-146">Чтение элементов</span><span class="sxs-lookup"><span data-stu-id="1b246-146">Read items</span></span>
    
<span data-ttu-id="1b246-147">Кроме того следующие уровни разрешений доступны, который определять подмножество отдельные разрешения и значения, как показано в таблице 2:</span><span class="sxs-lookup"><span data-stu-id="1b246-147">In addition, the following permission levels are available, which define a subset of individual permissions and values, as shown in Table 2:</span></span>
  
- <span data-ttu-id="1b246-148">Нет</span><span class="sxs-lookup"><span data-stu-id="1b246-148">None</span></span>    
- <span data-ttu-id="1b246-149">Owner</span><span class="sxs-lookup"><span data-stu-id="1b246-149">Owner</span></span>    
- <span data-ttu-id="1b246-150">PublishingEditor</span><span class="sxs-lookup"><span data-stu-id="1b246-150">PublishingEditor</span></span>    
- <span data-ttu-id="1b246-151">Редактор</span><span class="sxs-lookup"><span data-stu-id="1b246-151">Editor</span></span>    
- <span data-ttu-id="1b246-152">PublishingAuthor</span><span class="sxs-lookup"><span data-stu-id="1b246-152">PublishingAuthor</span></span>    
- <span data-ttu-id="1b246-153">Author</span><span class="sxs-lookup"><span data-stu-id="1b246-153">Author</span></span>    
- <span data-ttu-id="1b246-154">NoneditingAuthor</span><span class="sxs-lookup"><span data-stu-id="1b246-154">NoneditingAuthor</span></span>    
- <span data-ttu-id="1b246-155">Редактор</span><span class="sxs-lookup"><span data-stu-id="1b246-155">Reviewer</span></span>    
- <span data-ttu-id="1b246-156">Участник</span><span class="sxs-lookup"><span data-stu-id="1b246-156">Contributor</span></span>   
- <span data-ttu-id="1b246-157">Custom — это значение не могут задаваться для приложения.</span><span class="sxs-lookup"><span data-stu-id="1b246-157">Custom - This value cannot be set by the application.</span></span> <span data-ttu-id="1b246-158">Сервер задает это значение, если приложение включает пользовательский набор отдельных разрешений.</span><span class="sxs-lookup"><span data-stu-id="1b246-158">The server sets this value if the application includes a custom collection of individual permissions.</span></span>    
- <span data-ttu-id="1b246-159">FreeBusyTimeOnly — это может устанавливаться только для папок календаря.</span><span class="sxs-lookup"><span data-stu-id="1b246-159">FreeBusyTimeOnly - This can only be set on Calendar folders.</span></span>   
- <span data-ttu-id="1b246-160">FreeBusyTimeAndSubjectAndLocation — это может устанавливаться только для папок календаря.</span><span class="sxs-lookup"><span data-stu-id="1b246-160">FreeBusyTimeAndSubjectAndLocation - This can only be set on Calendar folders.</span></span>
    
<span data-ttu-id="1b246-161">В следующей таблице показаны какие отдельных разрешений по умолчанию, в зависимости от уровня разрешений.</span><span class="sxs-lookup"><span data-stu-id="1b246-161">The following table shows which individual permissions are applied by default based on permission level.</span></span>
  
<span data-ttu-id="1b246-162">**В таблице 2. Отдельные разрешения, уровень разрешений**</span><span class="sxs-lookup"><span data-stu-id="1b246-162">**Table 2. Individual permissions by permission level**</span></span>

|<span data-ttu-id="1b246-163">Уровень разрешений</span><span class="sxs-lookup"><span data-stu-id="1b246-163">Permission level</span></span>|<span data-ttu-id="1b246-164">Можно создавать элементы</span><span class="sxs-lookup"><span data-stu-id="1b246-164">Can create items</span></span>|<span data-ttu-id="1b246-165">Можно создать вложенные папки</span><span class="sxs-lookup"><span data-stu-id="1b246-165">Can create sub folders</span></span>|<span data-ttu-id="1b246-166">— Это владелец</span><span class="sxs-lookup"><span data-stu-id="1b246-166">Is folder owner</span></span>|<span data-ttu-id="1b246-167">Отображается папки</span><span class="sxs-lookup"><span data-stu-id="1b246-167">Is folder visible</span></span>|<span data-ttu-id="1b246-168">— Это папка контактов</span><span class="sxs-lookup"><span data-stu-id="1b246-168">Is folder contact</span></span>|<span data-ttu-id="1b246-169">Изменение элементов</span><span class="sxs-lookup"><span data-stu-id="1b246-169">Edit items</span></span>|<span data-ttu-id="1b246-170">Удаление элементов</span><span class="sxs-lookup"><span data-stu-id="1b246-170">Delete items</span></span>|<span data-ttu-id="1b246-171">Чтение элементов</span><span class="sxs-lookup"><span data-stu-id="1b246-171">Can read items</span></span>|
|:-----|:-----|:-----|:-----|:-----|:-----|:-----|:-----|:-----|
|<span data-ttu-id="1b246-172">Нет</span><span class="sxs-lookup"><span data-stu-id="1b246-172">None</span></span>  <br/> |<span data-ttu-id="1b246-173">Ложь</span><span class="sxs-lookup"><span data-stu-id="1b246-173">False</span></span>  <br/> |<span data-ttu-id="1b246-174">Ложь</span><span class="sxs-lookup"><span data-stu-id="1b246-174">False</span></span>  <br/> |<span data-ttu-id="1b246-175">Ложь</span><span class="sxs-lookup"><span data-stu-id="1b246-175">False</span></span>  <br/> |<span data-ttu-id="1b246-176">Ложь</span><span class="sxs-lookup"><span data-stu-id="1b246-176">False</span></span>  <br/> |<span data-ttu-id="1b246-177">Ложь</span><span class="sxs-lookup"><span data-stu-id="1b246-177">False</span></span>  <br/> |<span data-ttu-id="1b246-178">Нет</span><span class="sxs-lookup"><span data-stu-id="1b246-178">None</span></span>  <br/> |<span data-ttu-id="1b246-179">Нет</span><span class="sxs-lookup"><span data-stu-id="1b246-179">None</span></span>  <br/> |<span data-ttu-id="1b246-180">Нет</span><span class="sxs-lookup"><span data-stu-id="1b246-180">None</span></span>  <br/> |
|<span data-ttu-id="1b246-181">Owner</span><span class="sxs-lookup"><span data-stu-id="1b246-181">Owner</span></span>  <br/> |<span data-ttu-id="1b246-182">True</span><span class="sxs-lookup"><span data-stu-id="1b246-182">True</span></span>  <br/> |<span data-ttu-id="1b246-183">True</span><span class="sxs-lookup"><span data-stu-id="1b246-183">True</span></span>  <br/> |<span data-ttu-id="1b246-184">True</span><span class="sxs-lookup"><span data-stu-id="1b246-184">True</span></span>  <br/> |<span data-ttu-id="1b246-185">True</span><span class="sxs-lookup"><span data-stu-id="1b246-185">True</span></span>  <br/> |<span data-ttu-id="1b246-186">True</span><span class="sxs-lookup"><span data-stu-id="1b246-186">True</span></span>  <br/> |<span data-ttu-id="1b246-187">Все</span><span class="sxs-lookup"><span data-stu-id="1b246-187">All</span></span>  <br/> |<span data-ttu-id="1b246-188">Все</span><span class="sxs-lookup"><span data-stu-id="1b246-188">All</span></span>  <br/> |<span data-ttu-id="1b246-189">FullDetails</span><span class="sxs-lookup"><span data-stu-id="1b246-189">FullDetails</span></span>  <br/> |
|<span data-ttu-id="1b246-190">PublishingEditor</span><span class="sxs-lookup"><span data-stu-id="1b246-190">PublishingEditor</span></span>  <br/> |<span data-ttu-id="1b246-191">True</span><span class="sxs-lookup"><span data-stu-id="1b246-191">True</span></span>  <br/> |<span data-ttu-id="1b246-192">Истина</span><span class="sxs-lookup"><span data-stu-id="1b246-192">True</span></span>  <br/> |<span data-ttu-id="1b246-193">Ложь</span><span class="sxs-lookup"><span data-stu-id="1b246-193">False</span></span>  <br/> |<span data-ttu-id="1b246-194">Истина</span><span class="sxs-lookup"><span data-stu-id="1b246-194">True</span></span>  <br/> |<span data-ttu-id="1b246-195">Ложь</span><span class="sxs-lookup"><span data-stu-id="1b246-195">False</span></span>  <br/> |<span data-ttu-id="1b246-196">Все</span><span class="sxs-lookup"><span data-stu-id="1b246-196">All</span></span>  <br/> |<span data-ttu-id="1b246-197">Все</span><span class="sxs-lookup"><span data-stu-id="1b246-197">All</span></span>  <br/> |<span data-ttu-id="1b246-198">FullDetails</span><span class="sxs-lookup"><span data-stu-id="1b246-198">FullDetails</span></span>  <br/> |
|<span data-ttu-id="1b246-199">Редактор</span><span class="sxs-lookup"><span data-stu-id="1b246-199">Editor</span></span>  <br/> |<span data-ttu-id="1b246-200">Истина</span><span class="sxs-lookup"><span data-stu-id="1b246-200">True</span></span>  <br/> |<span data-ttu-id="1b246-201">Ложь</span><span class="sxs-lookup"><span data-stu-id="1b246-201">False</span></span>  <br/> |<span data-ttu-id="1b246-202">Ложь</span><span class="sxs-lookup"><span data-stu-id="1b246-202">False</span></span>  <br/> |<span data-ttu-id="1b246-203">Истина</span><span class="sxs-lookup"><span data-stu-id="1b246-203">True</span></span>  <br/> |<span data-ttu-id="1b246-204">Ложь</span><span class="sxs-lookup"><span data-stu-id="1b246-204">False</span></span>  <br/> |<span data-ttu-id="1b246-205">Все</span><span class="sxs-lookup"><span data-stu-id="1b246-205">All</span></span>  <br/> |<span data-ttu-id="1b246-206">Все</span><span class="sxs-lookup"><span data-stu-id="1b246-206">All</span></span>  <br/> |<span data-ttu-id="1b246-207">FullDetails</span><span class="sxs-lookup"><span data-stu-id="1b246-207">FullDetails</span></span>  <br/> |
|<span data-ttu-id="1b246-208">PublishingAuthor</span><span class="sxs-lookup"><span data-stu-id="1b246-208">PublishingAuthor</span></span>  <br/> |<span data-ttu-id="1b246-209">True</span><span class="sxs-lookup"><span data-stu-id="1b246-209">True</span></span>  <br/> |<span data-ttu-id="1b246-210">Истина</span><span class="sxs-lookup"><span data-stu-id="1b246-210">True</span></span>  <br/> |<span data-ttu-id="1b246-211">Ложь</span><span class="sxs-lookup"><span data-stu-id="1b246-211">False</span></span>  <br/> |<span data-ttu-id="1b246-212">Истина</span><span class="sxs-lookup"><span data-stu-id="1b246-212">True</span></span>  <br/> |<span data-ttu-id="1b246-213">Ложь</span><span class="sxs-lookup"><span data-stu-id="1b246-213">False</span></span>  <br/> |<span data-ttu-id="1b246-214">Владельцем</span><span class="sxs-lookup"><span data-stu-id="1b246-214">Owned</span></span>  <br/> |<span data-ttu-id="1b246-215">Владельцем</span><span class="sxs-lookup"><span data-stu-id="1b246-215">Owned</span></span>  <br/> |<span data-ttu-id="1b246-216">FullDetails</span><span class="sxs-lookup"><span data-stu-id="1b246-216">FullDetails</span></span>  <br/> |
|<span data-ttu-id="1b246-217">Author</span><span class="sxs-lookup"><span data-stu-id="1b246-217">Author</span></span>  <br/> |<span data-ttu-id="1b246-218">Истина</span><span class="sxs-lookup"><span data-stu-id="1b246-218">True</span></span>  <br/> |<span data-ttu-id="1b246-219">Ложь</span><span class="sxs-lookup"><span data-stu-id="1b246-219">False</span></span>  <br/> |<span data-ttu-id="1b246-220">Ложь</span><span class="sxs-lookup"><span data-stu-id="1b246-220">False</span></span>  <br/> |<span data-ttu-id="1b246-221">Истина</span><span class="sxs-lookup"><span data-stu-id="1b246-221">True</span></span>  <br/> |<span data-ttu-id="1b246-222">Ложь</span><span class="sxs-lookup"><span data-stu-id="1b246-222">False</span></span>  <br/> |<span data-ttu-id="1b246-223">Владельцем</span><span class="sxs-lookup"><span data-stu-id="1b246-223">Owned</span></span>  <br/> |<span data-ttu-id="1b246-224">Владельцем</span><span class="sxs-lookup"><span data-stu-id="1b246-224">Owned</span></span>  <br/> |<span data-ttu-id="1b246-225">FullDetails</span><span class="sxs-lookup"><span data-stu-id="1b246-225">FullDetails</span></span>  <br/> |
|<span data-ttu-id="1b246-226">NoneditingAuthor</span><span class="sxs-lookup"><span data-stu-id="1b246-226">NoneditingAuthor</span></span>  <br/> |<span data-ttu-id="1b246-227">Истина</span><span class="sxs-lookup"><span data-stu-id="1b246-227">True</span></span>  <br/> |<span data-ttu-id="1b246-228">Ложь</span><span class="sxs-lookup"><span data-stu-id="1b246-228">False</span></span>  <br/> |<span data-ttu-id="1b246-229">Ложь</span><span class="sxs-lookup"><span data-stu-id="1b246-229">False</span></span>  <br/> |<span data-ttu-id="1b246-230">Истина</span><span class="sxs-lookup"><span data-stu-id="1b246-230">True</span></span>  <br/> |<span data-ttu-id="1b246-231">Ложь</span><span class="sxs-lookup"><span data-stu-id="1b246-231">False</span></span>  <br/> |<span data-ttu-id="1b246-232">Нет</span><span class="sxs-lookup"><span data-stu-id="1b246-232">None</span></span>  <br/> |<span data-ttu-id="1b246-233">Владельцем</span><span class="sxs-lookup"><span data-stu-id="1b246-233">Owned</span></span>  <br/> |<span data-ttu-id="1b246-234">FullDetails</span><span class="sxs-lookup"><span data-stu-id="1b246-234">FullDetails</span></span>  <br/> |
|<span data-ttu-id="1b246-235">Редактор</span><span class="sxs-lookup"><span data-stu-id="1b246-235">Reviewer</span></span>  <br/> |<span data-ttu-id="1b246-236">Ложь</span><span class="sxs-lookup"><span data-stu-id="1b246-236">False</span></span>  <br/> |<span data-ttu-id="1b246-237">Ложь</span><span class="sxs-lookup"><span data-stu-id="1b246-237">False</span></span>  <br/> |<span data-ttu-id="1b246-238">Ложь</span><span class="sxs-lookup"><span data-stu-id="1b246-238">False</span></span>  <br/> |<span data-ttu-id="1b246-239">Истина</span><span class="sxs-lookup"><span data-stu-id="1b246-239">True</span></span>  <br/> |<span data-ttu-id="1b246-240">Ложь</span><span class="sxs-lookup"><span data-stu-id="1b246-240">False</span></span>  <br/> |<span data-ttu-id="1b246-241">Нет</span><span class="sxs-lookup"><span data-stu-id="1b246-241">None</span></span>  <br/> |<span data-ttu-id="1b246-242">Нет</span><span class="sxs-lookup"><span data-stu-id="1b246-242">None</span></span>  <br/> |<span data-ttu-id="1b246-243">FullDetails</span><span class="sxs-lookup"><span data-stu-id="1b246-243">FullDetails</span></span>  <br/> |
|<span data-ttu-id="1b246-244">Участник</span><span class="sxs-lookup"><span data-stu-id="1b246-244">Contributor</span></span>  <br/> |<span data-ttu-id="1b246-245">Истина</span><span class="sxs-lookup"><span data-stu-id="1b246-245">True</span></span>  <br/> |<span data-ttu-id="1b246-246">Ложь</span><span class="sxs-lookup"><span data-stu-id="1b246-246">False</span></span>  <br/> |<span data-ttu-id="1b246-247">Ложь</span><span class="sxs-lookup"><span data-stu-id="1b246-247">False</span></span>  <br/> |<span data-ttu-id="1b246-248">Истина</span><span class="sxs-lookup"><span data-stu-id="1b246-248">True</span></span>  <br/> |<span data-ttu-id="1b246-249">Ложь</span><span class="sxs-lookup"><span data-stu-id="1b246-249">False</span></span>  <br/> |<span data-ttu-id="1b246-250">Нет</span><span class="sxs-lookup"><span data-stu-id="1b246-250">None</span></span>  <br/> |<span data-ttu-id="1b246-251">Нет</span><span class="sxs-lookup"><span data-stu-id="1b246-251">None</span></span>  <br/> |<span data-ttu-id="1b246-252">Нет</span><span class="sxs-lookup"><span data-stu-id="1b246-252">None</span></span>  <br/> |
   
<span data-ttu-id="1b246-253">При указании уровня разрешений ненастраиваемых в запросе на разрешения на уровне папки, не нужно указать параметры отдельных разрешений.</span><span class="sxs-lookup"><span data-stu-id="1b246-253">If you specify a non-custom permission level in the folder-level permissions request, you don't need to specify the individual permission settings.</span></span> <span data-ttu-id="1b246-254">При указании отдельных разрешений при установке на уровень разрешений, ошибка **ErrorInvalidPermissionSettings** , возвращается в ответе.</span><span class="sxs-lookup"><span data-stu-id="1b246-254">If you do specify an individual permission when you set a permission level, an **ErrorInvalidPermissionSettings** error will be returned in the response.</span></span> 
  
## <a name="adding-folder-permissions-by-using-the-ews-managed-api"></a><span data-ttu-id="1b246-255">Добавление разрешений для папки с помощью управляемого интерфейса API веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="1b246-255">Adding folder permissions by using the EWS Managed API</span></span>
<span data-ttu-id="1b246-256"><a name="bk_enableewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="1b246-256"></span></span>

<span data-ttu-id="1b246-257">В следующем примере кода показано, как использовать управляемый API EWS для:</span><span class="sxs-lookup"><span data-stu-id="1b246-257">The following code example shows how to use the EWS Managed API to:</span></span> 
  
- <span data-ttu-id="1b246-258">Создание нового объекта [FolderPermission](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folderpermission%28v=exchg.80%29.aspx) для нового пользователя.</span><span class="sxs-lookup"><span data-stu-id="1b246-258">Create a new [FolderPermission](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folderpermission%28v=exchg.80%29.aspx) object for the new user.</span></span> 
    
- <span data-ttu-id="1b246-259">Получение текущих разрешений для папки с помощью метода [привязки](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="1b246-259">Get the current permissions for a folder by using the [Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) method.</span></span> 
    
- <span data-ttu-id="1b246-260">Добавьте новый **FolderPermissions** свойство [Folder.Permissions](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.permissions%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="1b246-260">Add the new **FolderPermissions** to the [Folder.Permissions](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.permissions%28v=exchg.80%29.aspx) property.</span></span> 
    
- <span data-ttu-id="1b246-261">Вызовите метод [Update](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.update%28v=exchg.80%29.aspx) , чтобы сохранить новые разрешения на сервере.</span><span class="sxs-lookup"><span data-stu-id="1b246-261">Call the [Update](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.update%28v=exchg.80%29.aspx) method to save the new permissions to the server.</span></span> 
    
<span data-ttu-id="1b246-262">В этом примере предполагается, что эта **Служба** является допустимым объектом [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) владельца почтового ящика, который пользователь прошел проверку подлинности на сервере Exchange.</span><span class="sxs-lookup"><span data-stu-id="1b246-262">This example assumes that **service** is a valid [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object for the mailbox owner and that the user has been authenticated to an Exchange server.</span></span> 
  
```cs
static void EnableFolderPermissions(ExchangeService service)
{
    // Create a property set to use for folder binding.
    PropertySet propSet = new PropertySet(BasePropertySet.IdOnly, FolderSchema.Permissions);
    // Specify the SMTP address of the new user and the folder permissions level.
    FolderPermission fldperm = new FolderPermission("sadie@contoso.com", FolderPermissionLevel.Editor);
    
    // Bind to the folder and get the current permissions. 
    // This call results in a GetFolder call to EWS.
    Folder sentItemsFolder = Folder.Bind(service, WellKnownFolderName.SentItems, propSet);
 
    // Add the permissions for the new user to the Sent Items DACL.
    sentItemsFolder.Permissions.Add(fldperm);
    // This call results in a UpdateFolder call to EWS.
    sentItemsFolder.Update();
}
```

<span data-ttu-id="1b246-263">Следующая строка кода указывает уровень разрешений.</span><span class="sxs-lookup"><span data-stu-id="1b246-263">The following line of code specifies the permission level.</span></span>
  
```cs
    FolderPermission fldperm = new FolderPermission("sadie@contoso.com", FolderPermissionLevel.Editor);
```

<span data-ttu-id="1b246-264">Если вы хотите использовать пользовательский уровень разрешений, используйте следующий код.</span><span class="sxs-lookup"><span data-stu-id="1b246-264">If you want to use the custom permission level, use this code instead.</span></span>
  
```cs
FolderPermission fldperm = new FolderPermission();
fldperm.UserId = "sadie@Contoso1000.onmicrosoft.com";
fldperm.CanCreateItems = true;
fldperm.CanCreateSubFolders = true;
…
```

<span data-ttu-id="1b246-265">Можно установить одно или несколько для записи [FolderPermission свойства](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folderpermission_properties%28v=exchg.80%29.aspx) при создании объекта **FolderPermission** с пользовательский уровень разрешений.</span><span class="sxs-lookup"><span data-stu-id="1b246-265">You can set any or all of the writable [FolderPermission properties](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folderpermission_properties%28v=exchg.80%29.aspx) when you create a **FolderPermission** object with a custom permission level.</span></span> <span data-ttu-id="1b246-266">Тем не менее, [FolderPermissionLevel](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folderpermissionlevel%28v=exchg.80%29.aspx) включена никогда не явным образом для **настраиваемого** приложения.</span><span class="sxs-lookup"><span data-stu-id="1b246-266">Note, however, that the [FolderPermissionLevel](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folderpermissionlevel%28v=exchg.80%29.aspx) is never explicitly set to **Custom** by the application.</span></span> <span data-ttu-id="1b246-267">**FolderPermissionLevel** настраиваемых имеет значение только в том случае, если создание объекта **FolderPermission** и задать отдельные разрешения.</span><span class="sxs-lookup"><span data-stu-id="1b246-267">The **FolderPermissionLevel** is set to Custom only when you create a **FolderPermission** object and set individual permissions.</span></span> 
  
## <a name="adding-folder-permissions-by-using-ews"></a><span data-ttu-id="1b246-268">Добавление разрешений для папки с помощью веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="1b246-268">Adding folder permissions by using EWS</span></span>
<span data-ttu-id="1b246-269"><a name="bk_enableews"> </a></span><span class="sxs-lookup"><span data-stu-id="1b246-269"></span></span>

<span data-ttu-id="1b246-270">В следующих примерах кода веб-служб Exchange показано, как для добавления разрешений к конкретной папке путем получения текущих разрешений и затем отправить список новые разрешения.</span><span class="sxs-lookup"><span data-stu-id="1b246-270">The following EWS code examples show how to add permissions to a specific folder by retrieving the current permissions and then submitting a list of new permissions.</span></span>
  
<span data-ttu-id="1b246-271">Первый шаг — отправить запрос [GetFolder](http://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) , где значение [DistinguishedFolderId](http://msdn.microsoft.com/library/50018162-2941-4227-8a5b-d6b4686bb32f%28Office.15%29.aspx) указывает папку, в которой для добавления разрешений (папка Отправленные в данном примере), а значение [FieldURI](http://msdn.microsoft.com/library/24af8e3b-3074-4c8c-8d0a-52446508d044%28Office.15%29.aspx) включает в себя папки: PermissionSet.</span><span class="sxs-lookup"><span data-stu-id="1b246-271">The first step is to send a [GetFolder](http://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) request, where the [DistinguishedFolderId](http://msdn.microsoft.com/library/50018162-2941-4227-8a5b-d6b4686bb32f%28Office.15%29.aspx) value specifies the folder in which to add permissions (the Sent Items folder in this example) and the [FieldURI](http://msdn.microsoft.com/library/24af8e3b-3074-4c8c-8d0a-52446508d044%28Office.15%29.aspx) value includes folder:PermissionSet.</span></span> <span data-ttu-id="1b246-272">Этот запрос будет получить параметры разрешений для указанной папки.</span><span class="sxs-lookup"><span data-stu-id="1b246-272">This request will retrieve the permission settings for the folder specified.</span></span> 
  
<span data-ttu-id="1b246-273">Это также XML-запрос, который отправляет управляемый API EWS при вызове метода **привязки** для [добавления разрешений для папки](#bk_enableewsma).</span><span class="sxs-lookup"><span data-stu-id="1b246-273">This is also the XML request that the EWS Managed API sends when you call the **Bind** method to [add folder permissions](#bk_enableewsma).</span></span>
  
```XML
  <?xml version="1.0" encoding="utf-8"?>
  <soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
                 xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                 xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                 xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
    <soap:Header>
      <t:RequestServerVersion Version="Exchange2007_SP1" />
    </soap:Header>
    <soap:Body>
      <m:GetFolder>
        <m:FolderShape>
          <t:BaseShape>IdOnly</t:BaseShape>
          <t:AdditionalProperties>
            <t:FieldURI FieldURI="folder:PermissionSet" />
          </t:AdditionalProperties>
        </m:FolderShape>
        <m:FolderIds>
          <t:DistinguishedFolderId Id="sentitems" />
        </m:FolderIds>
      </m:GetFolder>
    </soap:Body>
  </soap:Envelope>
```

<span data-ttu-id="1b246-274">Сервер отвечает на запрос **GetFolder** [GetFolderResponse](http://msdn.microsoft.com/library/47abeec8-78dd-4297-8525-099174ec880d%28Office.15%29.aspx) сообщение, которое содержит значение элемента [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) **NoError**, это означает, что папка был успешно извлечен.</span><span class="sxs-lookup"><span data-stu-id="1b246-274">The server responds to the **GetFolder** request with a [GetFolderResponse](http://msdn.microsoft.com/library/47abeec8-78dd-4297-8525-099174ec880d%28Office.15%29.aspx) message that includes a [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) element value of **NoError**, which indicates that the folder was retrieved successfully.</span></span> <span data-ttu-id="1b246-275">Для удобства чтения URL были сокращены [FolderId](http://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) и [ParentFolderId](http://msdn.microsoft.com/library/258f4b1f-367e-4c7d-9c29-eb775a2398c7%28Office.15%29.aspx) значения.</span><span class="sxs-lookup"><span data-stu-id="1b246-275">The [FolderId](http://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) and [ParentFolderId](http://msdn.microsoft.com/library/258f4b1f-367e-4c7d-9c29-eb775a2398c7%28Office.15%29.aspx) values have been shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="893"
                         MinorBuildNumber="17"
                         Version="V2_10"
                         xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:GetFolderResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:GetFolderResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Folders>
            <t:Folder>
              <t:FolderId Id="CgAAAA=="
                          ChangeKey="AQAAABYAAADOilbYa8KaT7ZgMoTz2P+hAAABiRd1" />
              <t:PermissionSet>
                <t:Permissions>
                  <t:Permission>
                    <t:UserId>
                      <t:DistinguishedUser>Default</t:DistinguishedUser>
                    </t:UserId>
                    <t:CanCreateItems>false</t:CanCreateItems>
                    <t:CanCreateSubFolders>false</t:CanCreateSubFolders>
                    <t:IsFolderOwner>false</t:IsFolderOwner>
                    <t:IsFolderVisible>false</t:IsFolderVisible>
                    <t:IsFolderContact>false</t:IsFolderContact>
                    <t:EditItems>None</t:EditItems>
                    <t:DeleteItems>None</t:DeleteItems>
                    <t:ReadItems>None</t:ReadItems>
                    <t:PermissionLevel>None</t:PermissionLevel>
                  </t:Permission>
                  <t:Permission>
                    <t:UserId>
                      <t:DistinguishedUser>Anonymous</t:DistinguishedUser>
                    </t:UserId>
                    <t:CanCreateItems>false</t:CanCreateItems>
                    <t:CanCreateSubFolders>false</t:CanCreateSubFolders>
                    <t:IsFolderOwner>false</t:IsFolderOwner>
                    <t:IsFolderVisible>false</t:IsFolderVisible>
                    <t:IsFolderContact>false</t:IsFolderContact>
                    <t:EditItems>None</t:EditItems>
                    <t:DeleteItems>None</t:DeleteItems>
                    <t:ReadItems>None</t:ReadItems>
                    <t:PermissionLevel>None</t:PermissionLevel>
                  </t:Permission>
                </t:Permissions>
              </t:PermissionSet>
            </t:Folder>
          </m:Folders>
        </m:GetFolderResponseMessage>
      </m:ResponseMessages>
    </m:GetFolderResponse>
  </s:Body>
</s:Envelope>
```

<span data-ttu-id="1b246-276">Затем используйте операцию **UpdateFolder** для отправки обновленные [PermissionSet](http://msdn.microsoft.com/library/6ac1bd17-a089-46bb-b9e6-f5b1dfe1076d%28Office.15%29.aspx), которая включает в себя [разрешения](http://msdn.microsoft.com/library/b8d0429a-0e58-4480-9847-4901970c7033%28Office.15%29.aspx) для нового пользователя.</span><span class="sxs-lookup"><span data-stu-id="1b246-276">Next, use the **UpdateFolder** operation to send the updated [PermissionSet](http://msdn.microsoft.com/library/6ac1bd17-a089-46bb-b9e6-f5b1dfe1076d%28Office.15%29.aspx), which includes the [Permission](http://msdn.microsoft.com/library/b8d0429a-0e58-4480-9847-4901970c7033%28Office.15%29.aspx) for the new user.</span></span> <span data-ttu-id="1b246-277">Обратите внимание на то, что включение элемент [SetFolderField](http://msdn.microsoft.com/library/8c69db7b-54b5-4ae2-abca-4d6e0937a790%28Office.15%29.aspx) для соответствующей папке в операции [UpdateFolder](http://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx) перезапишет все параметры разрешений на папку.</span><span class="sxs-lookup"><span data-stu-id="1b246-277">Note that including the [SetFolderField](http://msdn.microsoft.com/library/8c69db7b-54b5-4ae2-abca-4d6e0937a790%28Office.15%29.aspx) element for the respective folder in the [UpdateFolder](http://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx) operation will overwrite all the permission settings on the folder.</span></span> <span data-ttu-id="1b246-278">Аналогичным образом включая параметр [DeleteFolderField](http://msdn.microsoft.com/library/f9c2187b-4c60-4358-b4b4-ede50eadae48%28Office.15%29.aspx) **UpdateFolder** операции приведет к удалению всех параметров разрешений на папку.</span><span class="sxs-lookup"><span data-stu-id="1b246-278">Likewise, including the [DeleteFolderField](http://msdn.microsoft.com/library/f9c2187b-4c60-4358-b4b4-ede50eadae48%28Office.15%29.aspx) option of the **UpdateFolder** operation will also delete all the permission settings on the folder.</span></span> 
  
<span data-ttu-id="1b246-279">Это также XML-запрос, который отправляет управляемый API EWS при вызове метода **Update** для [добавления разрешений для папки](#bk_enableewsma).</span><span class="sxs-lookup"><span data-stu-id="1b246-279">This is also the XML request that the EWS Managed API sends when you call the **Update** method to [add folder permissions](#bk_enableewsma).</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
  </soap:Header>
  <soap:Body>
    <m:UpdateFolder>
      <m:FolderChanges>
        <t:FolderChange>
          <t:FolderId Id="CgAAAA=="
                      ChangeKey="AQAAABYAAADOilbYa8KaT7ZgMoTz2P+hAAABiRd1" />
          <t:Updates>
            <t:SetFolderField>
              <t:FieldURI FieldURI="folder:PermissionSet" />
              <t:Folder>
                <t:PermissionSet>
                  <t:Permissions>
                    <t:Permission>
                      <t:UserId>
                        <t:DistinguishedUser>Default</t:DistinguishedUser>
                      </t:UserId>
                      <t:PermissionLevel>None</t:PermissionLevel>
                    </t:Permission>
                    <t:Permission>
                      <t:UserId>
                        <t:DistinguishedUser>Anonymous</t:DistinguishedUser>
                      </t:UserId>
                      <t:PermissionLevel>None</t:PermissionLevel>
                    </t:Permission>
                    <t:Permission>
                      <t:UserId>
                        <t:PrimarySmtpAddress>sadie@contoso.com</t:PrimarySmtpAddress>
                      </t:UserId>
                      <t:PermissionLevel>Editor</t:PermissionLevel>
                    </t:Permission>
                  </t:Permissions>
                </t:PermissionSet>
              </t:Folder>
            </t:SetFolderField>
          </t:Updates>
        </t:FolderChange>
      </m:FolderChanges>
    </m:UpdateFolder>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="1b246-280">Следующая строка кода указывает уровень разрешений.</span><span class="sxs-lookup"><span data-stu-id="1b246-280">The following line of code specifies the permission level.</span></span>
  
```xml
<t:Permission>
    <t:UserId>
        <t:PrimarySmtpAddress>sadie@contoso.com</t:PrimarySmtpAddress>
    </t:UserId>
    <t:PermissionLevel>Editor</t:PermissionLevel>
</t:Permission>
```

<span data-ttu-id="1b246-281">Если вы хотите использовать пользовательский уровень разрешений, используйте следующий код.</span><span class="sxs-lookup"><span data-stu-id="1b246-281">If you want to use the custom permission level, use this code instead.</span></span>
  
```xml
<t:Permission>
    <t:UserId>
        <t:PrimarySmtpAddress> sadie@contoso.com </t:PrimarySmtpAddress>
    </t:UserId>
    <t:CanCreateItems>true</t:CanCreateItems>
    <t:CanCreateSubFolders>true</t:CanCreateSubFolders>
    <t:IsFolderOwner>false</t:IsFolderOwner>
    <t:IsFolderVisible>false</t:IsFolderVisible>
    <t:IsFolderContact>false</t:IsFolderContact>
    <t:EditItems>None</t:EditItems>
    <t:DeleteItems>None</t:DeleteItems>
    <t:ReadItems>None</t:ReadItems>
    <t:PermissionLevel>Custom</t:PermissionLevel>
</t:Permission>
```

<span data-ttu-id="1b246-282">Сервер отвечает на запрос **UpdateFolder** с [UpdateFolderResponse](http://msdn.microsoft.com/library/31f47739-dc9c-46ba-9e3f-cce25dc85e6e%28Office.15%29.aspx) сообщения, которое содержит значение элемента [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) **NoError**, это означает, что папка успешно обновлены.</span><span class="sxs-lookup"><span data-stu-id="1b246-282">The server responds to the **UpdateFolder** request with an [UpdateFolderResponse](http://msdn.microsoft.com/library/31f47739-dc9c-46ba-9e3f-cce25dc85e6e%28Office.15%29.aspx) message that includes a [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) element value of **NoError**, which indicates that the folder was updated successfully.</span></span>
  
## <a name="removing-folder-permissions-by-using-the-ews-managed-api"></a><span data-ttu-id="1b246-283">Удаление разрешений для папки с помощью управляемого интерфейса API веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="1b246-283">Removing folder permissions by using the EWS Managed API</span></span>
<span data-ttu-id="1b246-284"><a name="bk_removeewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="1b246-284"></span></span>

<span data-ttu-id="1b246-285">В следующем примере кода показано, как использовать управляемый API веб-служб Exchange для удаления всех разрешений на доступ пользователей указанной папки, за исключением разрешения анонимного доступа и по умолчанию с:</span><span class="sxs-lookup"><span data-stu-id="1b246-285">The following code example shows how to use the EWS Managed API to remove all user permissions on a specific folder, except for the default and anonymous permissions, by:</span></span>
  
1. <span data-ttu-id="1b246-286">Получение текущих разрешений для папки с помощью метода **привязки** .</span><span class="sxs-lookup"><span data-stu-id="1b246-286">Getting the current permissions for a folder by using the **Bind** method.</span></span> 
    
2. <span data-ttu-id="1b246-287">Итерации по коллекции **разрешения** и удаление разрешений для отдельных пользователей.</span><span class="sxs-lookup"><span data-stu-id="1b246-287">Iterating through the **Permissions** collection and removing permissions for individual users.</span></span> 
    
3. <span data-ttu-id="1b246-288">Вызов метода **обновления** , чтобы сохранить изменения.</span><span class="sxs-lookup"><span data-stu-id="1b246-288">Calling the **Update** method to save the changes.</span></span> 
    
<span data-ttu-id="1b246-289">В этом примере удаляются все разрешения на папку пользователя.</span><span class="sxs-lookup"><span data-stu-id="1b246-289">This example removes all user permissions on a folder.</span></span> <span data-ttu-id="1b246-290">Если требуется внести изменения в этом примере для удаления разрешений только для определенного пользователя, измените следующую строку кода для идентификации либо отображаемое имя или адрес SMTP пользователя.</span><span class="sxs-lookup"><span data-stu-id="1b246-290">If you want to modify this example to remove permissions only for a specific user, change the following line of code to identify either the display name or SMTP address of the user.</span></span>
  
```cs
if (sentItemsFolder.Permissions[t].UserId.DisplayName != null || sentItemsFolder.Permissions[t].UserId.PrimarySmtpAddress != null)
```

<span data-ttu-id="1b246-291">В этом примере предполагается, что эта **Служба** является допустимым объектом [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) владельца почтового ящика, который пользователь прошел проверку подлинности на сервере Exchange.</span><span class="sxs-lookup"><span data-stu-id="1b246-291">This example assumes that **service** is a valid [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object for the mailbox owner and that the user has been authenticated to an Exchange server.</span></span> 
  
```cs
static void RemoveFolderPermissions(ExchangeService service)
{
    // Create a property set to use for folder binding.
    PropertySet propSet = new PropertySet(BasePropertySet.FirstClassProperties, FolderSchema.Permissions);
    // Bind to the folder and get the current permissions. 
    // This call results in a GetFolder call to EWS.
    Folder sentItemsFolder = Folder.Bind(service, new FolderId(WellKnownFolderName.SentItems, "primary@contoso.com"), propSet);
    // Iterate through the collection of permissions and remove permissions for any 
    // user with a display name or SMTP address. This leaves the anonymous and 
    // default user permissions unchanged. 
    if (sentItemsFolder.Permissions.Count != 0)
    {
        for (int t = 0; t < sentItemsFolder.Permissions.Count; t++)
        {
            // Find any permissions associated with the specified user and remove them from the DACL
            if (sentItemsFolder.Permissions[t].UserId.DisplayName != null || sentItemsFolder.Permissions[t].UserId.PrimarySmtpAddress != null)
            {
                sentItemsFolder.Permissions.Remove(sentItemsFolder.Permissions[t]);
            }
        }
    }
    // This call results in an UpdateFolder call to EWS.
    sentItemsFolder.Update();
}
```

## <a name="removing-folder-permissions-by-using-ews"></a><span data-ttu-id="1b246-292">Удаление разрешений для папки с помощью веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="1b246-292">Removing folder permissions by using EWS</span></span>
<span data-ttu-id="1b246-293"><a name="bk_removeews"> </a></span><span class="sxs-lookup"><span data-stu-id="1b246-293"></span></span>

<span data-ttu-id="1b246-294">В следующих примерах кода веб-служб Exchange показано, как удалить все разрешения пользователя на определенную папку, за исключением по умолчанию и разрешения для анонимных пользователей.</span><span class="sxs-lookup"><span data-stu-id="1b246-294">The following EWS code examples show how to remove all user permissions on a specific folder, except for the default and anonymous permissions.</span></span>
  
<span data-ttu-id="1b246-295">Во-первых отправьте запрос [GetFolder](http://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) , где значение [DistinguishedFolderId](http://msdn.microsoft.com/library/50018162-2941-4227-8a5b-d6b4686bb32f%28Office.15%29.aspx) указывает папку, в которой для удаления разрешений (папка Отправленные в данном примере), а значение [FieldURI](http://msdn.microsoft.com/library/24af8e3b-3074-4c8c-8d0a-52446508d044%28Office.15%29.aspx) включает в себя папки: PermissionSet.</span><span class="sxs-lookup"><span data-stu-id="1b246-295">First, send a [GetFolder](http://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) request where the [DistinguishedFolderId](http://msdn.microsoft.com/library/50018162-2941-4227-8a5b-d6b4686bb32f%28Office.15%29.aspx) value specifies the folder in which to remove permissions (the Sent Items folder in this example) and the [FieldURI](http://msdn.microsoft.com/library/24af8e3b-3074-4c8c-8d0a-52446508d044%28Office.15%29.aspx) value includes folder:PermissionSet.</span></span> <span data-ttu-id="1b246-296">Этот запрос будет извлекать [PermissionSet](http://msdn.microsoft.com/library/6ac1bd17-a089-46bb-b9e6-f5b1dfe1076d%28Office.15%29.aspx) для указанной папки.</span><span class="sxs-lookup"><span data-stu-id="1b246-296">This request will retrieve the [PermissionSet](http://msdn.microsoft.com/library/6ac1bd17-a089-46bb-b9e6-f5b1dfe1076d%28Office.15%29.aspx) for the folder specified.</span></span> 
  
<span data-ttu-id="1b246-297">Это также XML-запрос, который отправляет управляемый API EWS при вызове метода **привязки** для [удаления разрешений для папки](#bk_removeewsma).</span><span class="sxs-lookup"><span data-stu-id="1b246-297">This is also the XML request that the EWS Managed API sends when you call the **Bind** method to [remove folder permissions](#bk_removeewsma).</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
  </soap:Header>
  <soap:Body>
    <m:GetFolder>
      <m:FolderShape>
        <t:BaseShape>AllProperties</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="folder:PermissionSet" />
        </t:AdditionalProperties>
      </m:FolderShape>
      <m:FolderIds>
        <t:DistinguishedFolderId Id="drafts">
          <t:Mailbox>
            <t:EmailAddress>primary@contoso.com</t:EmailAddress>
          </t:Mailbox>
        </t:DistinguishedFolderId>
      </m:FolderIds>
    </m:GetFolder>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="1b246-298">Сервер отвечает на запрос **GetFolder** [GetFolderResponse](http://msdn.microsoft.com/library/47abeec8-78dd-4297-8525-099174ec880d%28Office.15%29.aspx) сообщение, которое содержит значение элемента [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) **NoError**, это означает, что папка был успешно извлечен.</span><span class="sxs-lookup"><span data-stu-id="1b246-298">The server responds to the **GetFolder** request with a [GetFolderResponse](http://msdn.microsoft.com/library/47abeec8-78dd-4297-8525-099174ec880d%28Office.15%29.aspx) message that includes a [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) element value of **NoError**, which indicates that the folder was retrieved successfully.</span></span> <span data-ttu-id="1b246-299">Значения элементов **FolderId** и **ParentFolderId** URL-были сокращены для удобства чтения.</span><span class="sxs-lookup"><span data-stu-id="1b246-299">The values of the **FolderId** and **ParentFolderId** elements have been shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="893"
                         MinorBuildNumber="17"
                         Version="V2_10"
                         xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:GetFolderResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:GetFolderResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Folders>
            <t:Folder>
              <t:FolderId Id="EAAAAA=="
                          ChangeKey="AQAAABYAAADOilbYa8KaT7ZgMoTz2P+hAAABiRd5" />
              <t:ParentFolderId Id="CQAAAA=="
                                ChangeKey="AQAAAA==" />
              <t:FolderClass>IPF.Note</t:FolderClass>
              <t:DisplayName>Drafts</t:DisplayName>
              <t:TotalCount>0</t:TotalCount>
              <t:ChildFolderCount>0</t:ChildFolderCount>
              <t:EffectiveRights>
                <t:CreateAssociated>true</t:CreateAssociated>
                <t:CreateContents>true</t:CreateContents>
                <t:CreateHierarchy>true</t:CreateHierarchy>
                <t:Delete>true</t:Delete>
                <t:Modify>true</t:Modify>
                <t:Read>true</t:Read>
                <t:ViewPrivateItems>true</t:ViewPrivateItems>
              </t:EffectiveRights>
              <t:PermissionSet>
                <t:Permissions>
                  <t:Permission>
                    <t:UserId>
                      <t:DistinguishedUser>Default</t:DistinguishedUser>
                    </t:UserId>
                    <t:CanCreateItems>false</t:CanCreateItems>
                    <t:CanCreateSubFolders>false</t:CanCreateSubFolders>
                    <t:IsFolderOwner>false</t:IsFolderOwner>
                    <t:IsFolderVisible>false</t:IsFolderVisible>
                    <t:IsFolderContact>false</t:IsFolderContact>
                    <t:EditItems>None</t:EditItems>
                    <t:DeleteItems>None</t:DeleteItems>
                    <t:ReadItems>None</t:ReadItems>
                    <t:PermissionLevel>None</t:PermissionLevel>
                  </t:Permission>
                  <t:Permission>
                    <t:UserId>
                      <t:DistinguishedUser>Anonymous</t:DistinguishedUser>
                    </t:UserId>
                    <t:CanCreateItems>false</t:CanCreateItems>
                    <t:CanCreateSubFolders>false</t:CanCreateSubFolders>
                    <t:IsFolderOwner>false</t:IsFolderOwner>
                    <t:IsFolderVisible>false</t:IsFolderVisible>
                    <t:IsFolderContact>false</t:IsFolderContact>
                    <t:EditItems>None</t:EditItems>
                    <t:DeleteItems>None</t:DeleteItems>
                    <t:ReadItems>None</t:ReadItems>
                    <t:PermissionLevel>None</t:PermissionLevel>
                  </t:Permission>
                  <t:Permission>
                    <t:UserId>
                      <t:SID>S-1-5-21-1337771579-694202782-848329751-1535223</t:SID>
                      <t:PrimarySmtpAddress>sadie@Contoso.com</t:PrimarySmtpAddress>
                      <t:DisplayName>Sadie Daniels</t:DisplayName>
                    </t:UserId>
                    <t:CanCreateItems>true</t:CanCreateItems>
                    <t:CanCreateSubFolders>false</t:CanCreateSubFolders>
                    <t:IsFolderOwner>false</t:IsFolderOwner>
                    <t:IsFolderVisible>true</t:IsFolderVisible>
                    <t:IsFolderContact>false</t:IsFolderContact>
                    <t:EditItems>All</t:EditItems>
                    <t:DeleteItems>All</t:DeleteItems>
                    <t:ReadItems>FullDetails</t:ReadItems>
                    <t:PermissionLevel>Editor</t:PermissionLevel>
                  </t:Permission>
                </t:Permissions>
              </t:PermissionSet>
              <t:UnreadCount>0</t:UnreadCount>
            </t:Folder>
          </m:Folders>
        </m:GetFolderResponseMessage>
      </m:ResponseMessages>
    </m:GetFolderResponse>
  </s:Body>
</s:Envelope>
```

<span data-ttu-id="1b246-300">Затем используйте операцию **UpdateFolder** для отправки обновленные **PermissionSet**, которая не включает **разрешения** для удаленных пользователей.</span><span class="sxs-lookup"><span data-stu-id="1b246-300">Next, use the **UpdateFolder** operation to send the updated **PermissionSet**, which does not include the **Permission** for the removed user.</span></span> 
  
<span data-ttu-id="1b246-301">Это также XML-запрос, который отправляет управляемый API EWS при вызове метода **Update** для [удаления разрешений для папки](#bk_removeewsma).</span><span class="sxs-lookup"><span data-stu-id="1b246-301">This is also the XML request that the EWS Managed API sends when you call the **Update** method to [remove folder permissions](#bk_removeewsma).</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
  </soap:Header>
  <soap:Body>
    <m:UpdateFolder>
      <m:FolderChanges>
        <t:FolderChange>
          <t:FolderId Id="EAAAAA=="
                      ChangeKey="AQAAABYAAADOilbYa8KaT7ZgMoTz2P+hAAABiRd5" />
          <t:Updates>
            <t:SetFolderField>
              <t:FieldURI FieldURI="folder:PermissionSet" />
              <t:Folder>
                <t:PermissionSet>
                  <t:Permissions>
                    <t:Permission>
                      <t:UserId>
                        <t:DistinguishedUser>Default</t:DistinguishedUser>
                      </t:UserId>
                      <t:PermissionLevel>None</t:PermissionLevel>
                    </t:Permission>
                    <t:Permission>
                      <t:UserId>
                        <t:DistinguishedUser>Anonymous</t:DistinguishedUser>
                      </t:UserId>
                      <t:PermissionLevel>None</t:PermissionLevel>
                    </t:Permission>
                  </t:Permissions>
                </t:PermissionSet>
              </t:Folder>
            </t:SetFolderField>
          </t:Updates>
        </t:FolderChange>
      </m:FolderChanges>
    </m:UpdateFolder>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="1b246-302">Сервер отвечает на запрос **UpdateFolder** с **UpdateFolderResponse** сообщения, которое содержит значение элемента [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) **NoError**, это означает, что обновление выполнено успешно.</span><span class="sxs-lookup"><span data-stu-id="1b246-302">The server responds to the **UpdateFolder** request with an **UpdateFolderResponse** message that includes a [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) element value of **NoError**, which indicates that the update was successful.</span></span>
  
## <a name="updating-folder-permissions-by-using-the-ews-managed-api"></a><span data-ttu-id="1b246-303">Обновление разрешений для папки с помощью управляемого интерфейса API веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="1b246-303">Updating folder permissions by using the EWS Managed API</span></span>
<span data-ttu-id="1b246-304"><a name="bk_updateewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="1b246-304"></span></span>

<span data-ttu-id="1b246-305">Также можно обновить разрешения для папки для указанной папки с помощью управляемого интерфейса API веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="1b246-305">You can also update folder permissions for a specific folder by using the EWS Managed API.</span></span> <span data-ttu-id="1b246-306">Чтобы обновить разрешения:</span><span class="sxs-lookup"><span data-stu-id="1b246-306">To update the permissions:</span></span> 
  
1. <span data-ttu-id="1b246-307">[Удаление разрешений папки](#bk_removeewsma) для устаревших разрешений, но не вызовите метод **Update** (пока).</span><span class="sxs-lookup"><span data-stu-id="1b246-307">[Remove the folder permissions](#bk_removeewsma) for the outdated permissions, but do not call the **Update** method (yet).</span></span> 
    
2. <span data-ttu-id="1b246-308">[Добавление разрешений для пользователей новые или измененные папки](#bk_enableewsma).</span><span class="sxs-lookup"><span data-stu-id="1b246-308">[Add folder permissions for the new or changed users](#bk_enableewsma).</span></span>
    
3. <span data-ttu-id="1b246-309">Вызовите метод **Update** для сохранения изменений.</span><span class="sxs-lookup"><span data-stu-id="1b246-309">Call the **Update** method to save the changes.</span></span> 
    
<span data-ttu-id="1b246-310">При попытке добавить два набора разрешений для одного пользователя, появится сообщение об ошибке **ServiceResponseException** с следующее описание: «набор указанное разрешение содержит повторяющиеся UserIds».</span><span class="sxs-lookup"><span data-stu-id="1b246-310">If you try to add two sets of permissions for the same user, you will receive a **ServiceResponseException** error with the following description: "The specified permission set contains duplicate UserIds".</span></span> <span data-ttu-id="1b246-311">В этом случае удалить текущие разрешения из набора **разрешений** , а затем добавить новые разрешения в коллекцию **разрешений** .</span><span class="sxs-lookup"><span data-stu-id="1b246-311">In that case, remove the current permissions from the **Permission** collection, then add the new permissions to the **Permission** collection.</span></span> 
  
## <a name="updating-folder-permissions-by-using-ews"></a><span data-ttu-id="1b246-312">Обновление разрешений для папки с помощью веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="1b246-312">Updating folder permissions by using EWS</span></span>
<span data-ttu-id="1b246-313"><a name="bk_updateews"> </a></span><span class="sxs-lookup"><span data-stu-id="1b246-313"></span></span>

<span data-ttu-id="1b246-314">Можно также обновить разрешения папок для конкретных папок с помощью веб-служб Exchange, объединяя в процессе удаления и добавления.</span><span class="sxs-lookup"><span data-stu-id="1b246-314">You can also update folder permissions for specific folders by using EWS by combining the removal and addition process.</span></span> <span data-ttu-id="1b246-315">Чтобы обновить разрешения:</span><span class="sxs-lookup"><span data-stu-id="1b246-315">To update the permissions:</span></span> 
  
1. <span data-ttu-id="1b246-316">Получение разрешений текущей папки с помощью операции **GetFolder** .</span><span class="sxs-lookup"><span data-stu-id="1b246-316">Retrieve the folder's current permissions by using the **GetFolder** operation.</span></span> 
    
2. <span data-ttu-id="1b246-317">Отправьте обновленный список разрешений с помощью операции **UpdateFolder** .</span><span class="sxs-lookup"><span data-stu-id="1b246-317">Send an updated list of permissions by using the **UpdateFolder** operation.</span></span> 
    
<span data-ttu-id="1b246-318">Далее представлены два такие же операции, используемые для [включения](#bk_enableews) или [удаления доступа](#bk_removeews) с помощью веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="1b246-318">These are the same two operations you use to [enable](#bk_enableews) or [remove access](#bk_removeews) by using EWS.</span></span> <span data-ttu-id="1b246-319">Единственное отличие заключается в том, что при получении ответа **GetFolder** она будет содержать **разрешений** для пользователя.</span><span class="sxs-lookup"><span data-stu-id="1b246-319">The only difference is that when you receive the **GetFolder** response, it will contain a **Permission** set for user.</span></span> <span data-ttu-id="1b246-320">Просто заменить существующий элемент **разрешение** новый элемент **разрешения** , а затем отправьте **UpdateFolder** операции с новое значение **разрешения** или значения.</span><span class="sxs-lookup"><span data-stu-id="1b246-320">Simply replace that existing **Permission** element with the new **Permission** element, and then send the **UpdateFolder** operation with the new **Permission** value or values.</span></span> 
  
<span data-ttu-id="1b246-321">При попытке добавить два набора разрешений для одного пользователя, вы получите значение **ResponseCode** **ErrorDuplicateUserIdsSpecified**.</span><span class="sxs-lookup"><span data-stu-id="1b246-321">If you try to add two sets of permissions for the same user, you will receive a **ResponseCode** value of **ErrorDuplicateUserIdsSpecified**.</span></span> <span data-ttu-id="1b246-322">В этом случае удалите значение устаревшие разрешения для пользователя из запроса и повторите попытку запроса.</span><span class="sxs-lookup"><span data-stu-id="1b246-322">In that case, remove the outdated Permission value for the user from the request and then retry the request.</span></span>

## <a name="next-steps"></a><span data-ttu-id="1b246-323">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="1b246-323">Next steps</span></span>

<span data-ttu-id="1b246-324">После предоставить пользователю разрешения в указанную папку, пользователь может получить доступ папку роли представителя.</span><span class="sxs-lookup"><span data-stu-id="1b246-324">After you give a user permission to a specific folder, the user can access the folder as a delegate.</span></span> <span data-ttu-id="1b246-325">Для получения дополнительных сведений см.</span><span class="sxs-lookup"><span data-stu-id="1b246-325">For more information, see:</span></span>
  
- [<span data-ttu-id="1b246-326">Доступ к электронной почте в качестве делегата с помощью веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="1b246-326">Access email as a delegate by using EWS in Exchange</span></span>](how-to-access-email-as-a-delegate-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="1b246-327">Доступ к календарю в качестве делегата с помощью веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="1b246-327">Access a calendar as a delegate by using EWS in Exchange</span></span>](how-to-access-a-calendar-as-a-delegate-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="1b246-328">Контакты доступа роли представителя с помощью веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="1b246-328">Access contacts as a delegate by using EWS in Exchange</span></span>](how-to-access-contacts-as-a-delegate-by-using-ews-in-exchange.md)
    
## <a name="see-also"></a><span data-ttu-id="1b246-329">См. также</span><span class="sxs-lookup"><span data-stu-id="1b246-329">See also</span></span>

- [<span data-ttu-id="1b246-330">Передача прав доступа и EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="1b246-330">Delegate access and EWS in Exchange</span></span>](delegate-access-and-ews-in-exchange.md)   
- [<span data-ttu-id="1b246-331">Добавление и удаление делегаты с помощью веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="1b246-331">Add and remove delegates by using EWS in Exchange</span></span>](how-to-add-and-remove-delegates-by-using-ews-in-exchange.md)    
- [<span data-ttu-id="1b246-332">Папки и элементы в веб-службах Exchange</span><span class="sxs-lookup"><span data-stu-id="1b246-332">Folders and items in EWS in Exchange</span></span>](folders-and-items-in-ews-in-exchange.md)
    

