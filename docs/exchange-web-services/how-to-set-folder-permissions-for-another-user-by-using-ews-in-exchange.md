---
title: Задание разрешений для папки другого пользователя с помощью EWS в Exchange
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 7eb81676-a780-4c56-b4f2-c4ed2697107d
description: Узнайте, как задать уровни разрешений для папки с помощью управляемого API EWS или EWS в Exchange.
ms.openlocfilehash: e25f1a49a430e8c95829d404fa53451b76cab167
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44455872"
---
# <a name="set-folder-permissions-for-another-user-by-using-ews-in-exchange"></a><span data-ttu-id="5de13-103">Задание разрешений для папки другого пользователя с помощью EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="5de13-103">Set folder permissions for another user by using EWS in Exchange</span></span>

<span data-ttu-id="5de13-104">Узнайте, как задать уровни разрешений для папки с помощью управляемого API EWS или EWS в Exchange.</span><span class="sxs-lookup"><span data-stu-id="5de13-104">Learn how to set permission levels on a folder by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="5de13-105">Разрешения уровня папки позволяют пользователям получать доступ к одной или нескольким папкам в почтовом ящике другого пользователя.</span><span class="sxs-lookup"><span data-stu-id="5de13-105">Folder-level permissions enable users to access one or more folders in another user's mailbox.</span></span> <span data-ttu-id="5de13-106">Разрешения для папок аналогичны Делегированному доступу, но они отличаются следующими особенностями:</span><span class="sxs-lookup"><span data-stu-id="5de13-106">Folder permissions are similar to delegate access, but they differ in the following ways:</span></span> 
  
- <span data-ttu-id="5de13-107">Разрешения для папок не позволяют пользователю "Отправить от имени" или "Отправить как" другого пользователя.</span><span class="sxs-lookup"><span data-stu-id="5de13-107">Folder permissions do not enable a user to "send on behalf of" or "send as" another user.</span></span> <span data-ttu-id="5de13-108">Они позволяют получать доступ только к папкам.</span><span class="sxs-lookup"><span data-stu-id="5de13-108">They only enable access to folders.</span></span> <span data-ttu-id="5de13-109">Пользователи могут создавать элементы в этих папках, но не могут их отправлять.</span><span class="sxs-lookup"><span data-stu-id="5de13-109">Users can create items in those folders, but they can't send them.</span></span>
    
- <span data-ttu-id="5de13-110">Вы можете задать разрешения для папки в любой папке почтового ящика, но вы можете добавить делегата в папки "Календарь", "Контакты", "Входящие", "журнал", "Заметки" и "задачи".</span><span class="sxs-lookup"><span data-stu-id="5de13-110">You can set folder permissions on any folder in the mailbox, but you can only add a delegate to the Calendar, Contacts, Inbox, Journal, Notes, and Tasks folders.</span></span>
    
- <span data-ttu-id="5de13-111">Вы можете задать ряд [разрешений для конкретной папки](#bk_folderperms).</span><span class="sxs-lookup"><span data-stu-id="5de13-111">You can set a number of [permissions on a specific folder](#bk_folderperms).</span></span> <span data-ttu-id="5de13-112">При добавлении делегата можно назначить один из [пяти уровней разрешений](delegate-access-and-ews-in-exchange.md#bk_delegateperms).</span><span class="sxs-lookup"><span data-stu-id="5de13-112">When you add a delegate, you can assign one of only [five permission levels](delegate-access-and-ews-in-exchange.md#bk_delegateperms).</span></span>
    
- <span data-ttu-id="5de13-113">Вы можете задать разрешения для папок анонимных пользователей и пользователей по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="5de13-113">You can set folder permissions for anonymous and default users.</span></span> <span data-ttu-id="5de13-114">Вы можете предоставить представителю доступ только к учетной записи с включенной поддержкой почты.</span><span class="sxs-lookup"><span data-stu-id="5de13-114">You can only grant delegate access to a mail-enabled account.</span></span>
    
<span data-ttu-id="5de13-115">Если вы знакомы с записями управления доступом и избирательными списками управления доступом (DACL), то вы знаете, что у пользователя может быть только один набор разрешений для каждой папки.</span><span class="sxs-lookup"><span data-stu-id="5de13-115">If you're familiar with Access Control Entries (ACEs) and Discretionary Access Control Lists (DACLs), you know that a user can only have one set of permissions for each folder.</span></span> <span data-ttu-id="5de13-116">Если вы попытаетесь добавить набор разрешений для пользователя и у него уже есть набор разрешений, возникнет ошибка.</span><span class="sxs-lookup"><span data-stu-id="5de13-116">If you try to add a set of permissions for a user and they already have a set of permissions, you'll get an error.</span></span> <span data-ttu-id="5de13-117">При добавлении, удалении или обновлении разрешений для папки вы получаете текущий список DACL, добавляете или удаляете все записи управления доступом, а затем отправляете обновленный список DACL.</span><span class="sxs-lookup"><span data-stu-id="5de13-117">When you add, remove, or update permissions on a folder, you get the current DACL, add or remove any ACEs, and then send the updated DACL.</span></span> <span data-ttu-id="5de13-118">Вы не можете добавить несколько элементов управления доступом для одного и того же пользователя.</span><span class="sxs-lookup"><span data-stu-id="5de13-118">You cannot add multiple ACEs for the same user.</span></span> <span data-ttu-id="5de13-119">При обновлении разрешений с помощью управляемого API EWS необходимо удалить текущую запись ACE пользователя, а затем добавить в нее новый элемент управления доступом.</span><span class="sxs-lookup"><span data-stu-id="5de13-119">When you update permissions by using the EWS Managed API, you need to remove the user's current ACE and then add their new ACE to the collection.</span></span> <span data-ttu-id="5de13-120">Если вы используете EWS, вы просто замените предыдущий набор записей ACE на новые.</span><span class="sxs-lookup"><span data-stu-id="5de13-120">If you're using EWS, you just replace the previous set of ACEs with the new ones.</span></span>
  
<span data-ttu-id="5de13-121">Если вы вносите несколько изменений разрешений в одну папку, вы можете пакетным добавлением, удалением или обновлениям, просто обратите внимание на то, что вы не можете выполнять пакетное обновление для нескольких папок.</span><span class="sxs-lookup"><span data-stu-id="5de13-121">If you're making multiple permission changes to a single folder, you can batch additions, removals, or updates —just note that you cannot batch user updates on multiple folders.</span></span> <span data-ttu-id="5de13-122">Один вызов необходим для получения разрешений для одной папки, а второй вызов необходим для обновления разрешений для этой папки.</span><span class="sxs-lookup"><span data-stu-id="5de13-122">One call is required to get the permissions on a single folder, and a second call is required to update the permissions on that folder.</span></span> <span data-ttu-id="5de13-123">При добавлении, удалении или обновлении разрешений пользователя используются одинаковые два вызова метода или операции для каждой задачи.</span><span class="sxs-lookup"><span data-stu-id="5de13-123">When you add, remove, or update user permissions, you use the same two method calls or operations for each task.</span></span>
  
<span data-ttu-id="5de13-124">**Таблица 1. Методы управляемого API EWS и операции EWS для установки разрешений для папки**</span><span class="sxs-lookup"><span data-stu-id="5de13-124">**Table 1. EWS Managed API methods and EWS operations for setting folder permissions**</span></span>

|<span data-ttu-id="5de13-125">Что требуется сделать</span><span class="sxs-lookup"><span data-stu-id="5de13-125">If you want to…</span></span>|<span data-ttu-id="5de13-126">Используйте этот метод управляемого API EWS...</span><span class="sxs-lookup"><span data-stu-id="5de13-126">Use this EWS Managed API method…</span></span>|<span data-ttu-id="5de13-127">Используйте эту операцию EWS...</span><span class="sxs-lookup"><span data-stu-id="5de13-127">Use this EWS operation…</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="5de13-128">Включение, удаление и обновление разрешений для папки</span><span class="sxs-lookup"><span data-stu-id="5de13-128">Enable, remove, or update folder permissions</span></span>  <br/> |<span data-ttu-id="5de13-129">[Folder. Bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) , за которым следует [Папка. Update](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage.reply%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="5de13-129">[Folder.Bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) followed by [Folder.Update](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage.reply%28v=exchg.80%29.aspx)</span></span> <br/> |<span data-ttu-id="5de13-130">[Папка](https://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) , за которой следует [операцию UpdateFolder](https://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="5de13-130">[GetFolder](https://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) followed by [UpdateFolder](https://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx)</span></span> <br/> |
|<span data-ttu-id="5de13-131">Создание папки и определение разрешений для папки</span><span class="sxs-lookup"><span data-stu-id="5de13-131">Create a folder and define folder permissions</span></span>  <br/> |[<span data-ttu-id="5de13-132">Folder. Save</span><span class="sxs-lookup"><span data-stu-id="5de13-132">Folder.Save</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.save%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="5de13-133">CreateFolder</span><span class="sxs-lookup"><span data-stu-id="5de13-133">CreateFolder</span></span>](https://msdn.microsoft.com/library/6f6c334c-b190-4e55-8f0a-38f2a018d1b3%28Office.15%29.aspx) <br/> |
   
## <a name="folder-permissions"></a><span data-ttu-id="5de13-134">Разрешения для папок</span><span class="sxs-lookup"><span data-stu-id="5de13-134">Folder permissions</span></span>
<span data-ttu-id="5de13-135"><a name="bk_folderperms"> </a></span><span class="sxs-lookup"><span data-stu-id="5de13-135"><a name="bk_folderperms"> </a></span></span>

<span data-ttu-id="5de13-136">При настройке разрешений для папки в определенной папке есть несколько вариантов.</span><span class="sxs-lookup"><span data-stu-id="5de13-136">You have quite a few options when it comes to setting folder permissions on a specific folder.</span></span> <span data-ttu-id="5de13-137">Вы можете задать уровень разрешений для папки для каждого пользователя, который добавляет набор предварительно определенных разрешений в список DACL или устанавливает индивидуальные разрешения для папки, но не позволяет смешивать и сопоставлять их.</span><span class="sxs-lookup"><span data-stu-id="5de13-137">You can set a permission level on a folder for each user, which adds a set of predefined individual permissions to the DACL, or you can set individual permissions on a folder — but you can't mix and match.</span></span>
  
<span data-ttu-id="5de13-138">Доступны следующие отдельные разрешения:</span><span class="sxs-lookup"><span data-stu-id="5de13-138">The following individual permissions are available:</span></span>
  
- <span data-ttu-id="5de13-139">Могут создавать</span><span class="sxs-lookup"><span data-stu-id="5de13-139">Can create</span></span>
- <span data-ttu-id="5de13-140">Может создавать вложенные папки</span><span class="sxs-lookup"><span data-stu-id="5de13-140">Can create subfolders</span></span>    
- <span data-ttu-id="5de13-141">Является владельцем папки</span><span class="sxs-lookup"><span data-stu-id="5de13-141">Is folder owner</span></span>    
- <span data-ttu-id="5de13-142">Является видимой папкой</span><span class="sxs-lookup"><span data-stu-id="5de13-142">Is folder visible</span></span>    
- <span data-ttu-id="5de13-143">Является контактом папки</span><span class="sxs-lookup"><span data-stu-id="5de13-143">Is folder contact</span></span>    
- <span data-ttu-id="5de13-144">Изменение элементов</span><span class="sxs-lookup"><span data-stu-id="5de13-144">Edit items</span></span>    
- <span data-ttu-id="5de13-145">удалять элементы.</span><span class="sxs-lookup"><span data-stu-id="5de13-145">Delete items</span></span>    
- <span data-ttu-id="5de13-146">Чтение элементов</span><span class="sxs-lookup"><span data-stu-id="5de13-146">Read items</span></span>
    
<span data-ttu-id="5de13-147">Кроме того, доступны следующие уровни разрешений, которые определяют подмножество отдельных разрешений и значений, как показано в таблице 2:</span><span class="sxs-lookup"><span data-stu-id="5de13-147">In addition, the following permission levels are available, which define a subset of individual permissions and values, as shown in Table 2:</span></span>
  
- <span data-ttu-id="5de13-148">Нет</span><span class="sxs-lookup"><span data-stu-id="5de13-148">None</span></span>    
- <span data-ttu-id="5de13-149">Владелец</span><span class="sxs-lookup"><span data-stu-id="5de13-149">Owner</span></span>    
- <span data-ttu-id="5de13-150">PublishingEditor</span><span class="sxs-lookup"><span data-stu-id="5de13-150">PublishingEditor</span></span>    
- <span data-ttu-id="5de13-151">Корректор</span><span class="sxs-lookup"><span data-stu-id="5de13-151">Editor</span></span>    
- <span data-ttu-id="5de13-152">PublishingAuthor</span><span class="sxs-lookup"><span data-stu-id="5de13-152">PublishingAuthor</span></span>    
- <span data-ttu-id="5de13-153">Автор</span><span class="sxs-lookup"><span data-stu-id="5de13-153">Author</span></span>    
- <span data-ttu-id="5de13-154">Noneditingauthorcreateitems</span><span class="sxs-lookup"><span data-stu-id="5de13-154">NoneditingAuthor</span></span>    
- <span data-ttu-id="5de13-155">Reviewer</span><span class="sxs-lookup"><span data-stu-id="5de13-155">Reviewer</span></span>    
- <span data-ttu-id="5de13-156">Участник</span><span class="sxs-lookup"><span data-stu-id="5de13-156">Contributor</span></span>   
- <span data-ttu-id="5de13-157">Custom — это значение не может быть задано приложением.</span><span class="sxs-lookup"><span data-stu-id="5de13-157">Custom - This value cannot be set by the application.</span></span> <span data-ttu-id="5de13-158">Сервер задает это значение, если приложение включает настраиваемую коллекцию отдельных разрешений.</span><span class="sxs-lookup"><span data-stu-id="5de13-158">The server sets this value if the application includes a custom collection of individual permissions.</span></span>    
- <span data-ttu-id="5de13-159">Фрибуситимеонли — можно задать только для папок календаря.</span><span class="sxs-lookup"><span data-stu-id="5de13-159">FreeBusyTimeOnly - This can only be set on Calendar folders.</span></span>   
- <span data-ttu-id="5de13-160">Фрибуситимеандсубжектандлокатион — можно задать только для папок календаря.</span><span class="sxs-lookup"><span data-stu-id="5de13-160">FreeBusyTimeAndSubjectAndLocation - This can only be set on Calendar folders.</span></span>
    
<span data-ttu-id="5de13-161">В следующей таблице показано, какие индивидуальные разрешения применяются по умолчанию на основе уровня разрешений.</span><span class="sxs-lookup"><span data-stu-id="5de13-161">The following table shows which individual permissions are applied by default based on permission level.</span></span>
  
<span data-ttu-id="5de13-162">**Таблица 2. Индивидуальные разрешения по уровню разрешений**</span><span class="sxs-lookup"><span data-stu-id="5de13-162">**Table 2. Individual permissions by permission level**</span></span>

|<span data-ttu-id="5de13-163">Уровень разрешений</span><span class="sxs-lookup"><span data-stu-id="5de13-163">Permission level</span></span>|<span data-ttu-id="5de13-164">Может создавать элементы</span><span class="sxs-lookup"><span data-stu-id="5de13-164">Can create items</span></span>|<span data-ttu-id="5de13-165">Может создавать вложенные папки</span><span class="sxs-lookup"><span data-stu-id="5de13-165">Can create sub folders</span></span>|<span data-ttu-id="5de13-166">Является владельцем папки</span><span class="sxs-lookup"><span data-stu-id="5de13-166">Is folder owner</span></span>|<span data-ttu-id="5de13-167">Является видимой папкой</span><span class="sxs-lookup"><span data-stu-id="5de13-167">Is folder visible</span></span>|<span data-ttu-id="5de13-168">Является контактом папки</span><span class="sxs-lookup"><span data-stu-id="5de13-168">Is folder contact</span></span>|<span data-ttu-id="5de13-169">Изменение элементов</span><span class="sxs-lookup"><span data-stu-id="5de13-169">Edit items</span></span>|<span data-ttu-id="5de13-170">удалять элементы.</span><span class="sxs-lookup"><span data-stu-id="5de13-170">Delete items</span></span>|<span data-ttu-id="5de13-171">Возможность чтения элементов</span><span class="sxs-lookup"><span data-stu-id="5de13-171">Can read items</span></span>|
|:-----|:-----|:-----|:-----|:-----|:-----|:-----|:-----|:-----|
|<span data-ttu-id="5de13-172">Нет</span><span class="sxs-lookup"><span data-stu-id="5de13-172">None</span></span>  <br/> |<span data-ttu-id="5de13-173">False</span><span class="sxs-lookup"><span data-stu-id="5de13-173">False</span></span>  <br/> |<span data-ttu-id="5de13-174">False</span><span class="sxs-lookup"><span data-stu-id="5de13-174">False</span></span>  <br/> |<span data-ttu-id="5de13-175">False</span><span class="sxs-lookup"><span data-stu-id="5de13-175">False</span></span>  <br/> |<span data-ttu-id="5de13-176">False</span><span class="sxs-lookup"><span data-stu-id="5de13-176">False</span></span>  <br/> |<span data-ttu-id="5de13-177">False</span><span class="sxs-lookup"><span data-stu-id="5de13-177">False</span></span>  <br/> |<span data-ttu-id="5de13-178">Нет</span><span class="sxs-lookup"><span data-stu-id="5de13-178">None</span></span>  <br/> |<span data-ttu-id="5de13-179">Нет</span><span class="sxs-lookup"><span data-stu-id="5de13-179">None</span></span>  <br/> |<span data-ttu-id="5de13-180">Нет</span><span class="sxs-lookup"><span data-stu-id="5de13-180">None</span></span>  <br/> |
|<span data-ttu-id="5de13-181">Владелец</span><span class="sxs-lookup"><span data-stu-id="5de13-181">Owner</span></span>  <br/> |<span data-ttu-id="5de13-182">Да</span><span class="sxs-lookup"><span data-stu-id="5de13-182">True</span></span>  <br/> |<span data-ttu-id="5de13-183">Да</span><span class="sxs-lookup"><span data-stu-id="5de13-183">True</span></span>  <br/> |<span data-ttu-id="5de13-184">Да</span><span class="sxs-lookup"><span data-stu-id="5de13-184">True</span></span>  <br/> |<span data-ttu-id="5de13-185">Да</span><span class="sxs-lookup"><span data-stu-id="5de13-185">True</span></span>  <br/> |<span data-ttu-id="5de13-186">Да</span><span class="sxs-lookup"><span data-stu-id="5de13-186">True</span></span>  <br/> |<span data-ttu-id="5de13-187">Все</span><span class="sxs-lookup"><span data-stu-id="5de13-187">All</span></span>  <br/> |<span data-ttu-id="5de13-188">Все</span><span class="sxs-lookup"><span data-stu-id="5de13-188">All</span></span>  <br/> |<span data-ttu-id="5de13-189">фуллдетаилс</span><span class="sxs-lookup"><span data-stu-id="5de13-189">FullDetails</span></span>  <br/> |
|<span data-ttu-id="5de13-190">PublishingEditor</span><span class="sxs-lookup"><span data-stu-id="5de13-190">PublishingEditor</span></span>  <br/> |<span data-ttu-id="5de13-191">Да</span><span class="sxs-lookup"><span data-stu-id="5de13-191">True</span></span>  <br/> |<span data-ttu-id="5de13-192">Да</span><span class="sxs-lookup"><span data-stu-id="5de13-192">True</span></span>  <br/> |<span data-ttu-id="5de13-193">False</span><span class="sxs-lookup"><span data-stu-id="5de13-193">False</span></span>  <br/> |<span data-ttu-id="5de13-194">Верно.</span><span class="sxs-lookup"><span data-stu-id="5de13-194">True</span></span>  <br/> |<span data-ttu-id="5de13-195">False</span><span class="sxs-lookup"><span data-stu-id="5de13-195">False</span></span>  <br/> |<span data-ttu-id="5de13-196">Все</span><span class="sxs-lookup"><span data-stu-id="5de13-196">All</span></span>  <br/> |<span data-ttu-id="5de13-197">Все</span><span class="sxs-lookup"><span data-stu-id="5de13-197">All</span></span>  <br/> |<span data-ttu-id="5de13-198">фуллдетаилс</span><span class="sxs-lookup"><span data-stu-id="5de13-198">FullDetails</span></span>  <br/> |
|<span data-ttu-id="5de13-199">Корректор</span><span class="sxs-lookup"><span data-stu-id="5de13-199">Editor</span></span>  <br/> |<span data-ttu-id="5de13-200">Верно.</span><span class="sxs-lookup"><span data-stu-id="5de13-200">True</span></span>  <br/> |<span data-ttu-id="5de13-201">False</span><span class="sxs-lookup"><span data-stu-id="5de13-201">False</span></span>  <br/> |<span data-ttu-id="5de13-202">False</span><span class="sxs-lookup"><span data-stu-id="5de13-202">False</span></span>  <br/> |<span data-ttu-id="5de13-203">Верно.</span><span class="sxs-lookup"><span data-stu-id="5de13-203">True</span></span>  <br/> |<span data-ttu-id="5de13-204">False</span><span class="sxs-lookup"><span data-stu-id="5de13-204">False</span></span>  <br/> |<span data-ttu-id="5de13-205">Все</span><span class="sxs-lookup"><span data-stu-id="5de13-205">All</span></span>  <br/> |<span data-ttu-id="5de13-206">Все</span><span class="sxs-lookup"><span data-stu-id="5de13-206">All</span></span>  <br/> |<span data-ttu-id="5de13-207">фуллдетаилс</span><span class="sxs-lookup"><span data-stu-id="5de13-207">FullDetails</span></span>  <br/> |
|<span data-ttu-id="5de13-208">PublishingAuthor</span><span class="sxs-lookup"><span data-stu-id="5de13-208">PublishingAuthor</span></span>  <br/> |<span data-ttu-id="5de13-209">Да</span><span class="sxs-lookup"><span data-stu-id="5de13-209">True</span></span>  <br/> |<span data-ttu-id="5de13-210">Да</span><span class="sxs-lookup"><span data-stu-id="5de13-210">True</span></span>  <br/> |<span data-ttu-id="5de13-211">False</span><span class="sxs-lookup"><span data-stu-id="5de13-211">False</span></span>  <br/> |<span data-ttu-id="5de13-212">Верно.</span><span class="sxs-lookup"><span data-stu-id="5de13-212">True</span></span>  <br/> |<span data-ttu-id="5de13-213">False</span><span class="sxs-lookup"><span data-stu-id="5de13-213">False</span></span>  <br/> |<span data-ttu-id="5de13-214">Он</span><span class="sxs-lookup"><span data-stu-id="5de13-214">Owned</span></span>  <br/> |<span data-ttu-id="5de13-215">Он</span><span class="sxs-lookup"><span data-stu-id="5de13-215">Owned</span></span>  <br/> |<span data-ttu-id="5de13-216">фуллдетаилс</span><span class="sxs-lookup"><span data-stu-id="5de13-216">FullDetails</span></span>  <br/> |
|<span data-ttu-id="5de13-217">Автор</span><span class="sxs-lookup"><span data-stu-id="5de13-217">Author</span></span>  <br/> |<span data-ttu-id="5de13-218">Верно.</span><span class="sxs-lookup"><span data-stu-id="5de13-218">True</span></span>  <br/> |<span data-ttu-id="5de13-219">False</span><span class="sxs-lookup"><span data-stu-id="5de13-219">False</span></span>  <br/> |<span data-ttu-id="5de13-220">False</span><span class="sxs-lookup"><span data-stu-id="5de13-220">False</span></span>  <br/> |<span data-ttu-id="5de13-221">Верно.</span><span class="sxs-lookup"><span data-stu-id="5de13-221">True</span></span>  <br/> |<span data-ttu-id="5de13-222">False</span><span class="sxs-lookup"><span data-stu-id="5de13-222">False</span></span>  <br/> |<span data-ttu-id="5de13-223">Он</span><span class="sxs-lookup"><span data-stu-id="5de13-223">Owned</span></span>  <br/> |<span data-ttu-id="5de13-224">Он</span><span class="sxs-lookup"><span data-stu-id="5de13-224">Owned</span></span>  <br/> |<span data-ttu-id="5de13-225">фуллдетаилс</span><span class="sxs-lookup"><span data-stu-id="5de13-225">FullDetails</span></span>  <br/> |
|<span data-ttu-id="5de13-226">Noneditingauthorcreateitems</span><span class="sxs-lookup"><span data-stu-id="5de13-226">NoneditingAuthor</span></span>  <br/> |<span data-ttu-id="5de13-227">Верно.</span><span class="sxs-lookup"><span data-stu-id="5de13-227">True</span></span>  <br/> |<span data-ttu-id="5de13-228">False</span><span class="sxs-lookup"><span data-stu-id="5de13-228">False</span></span>  <br/> |<span data-ttu-id="5de13-229">False</span><span class="sxs-lookup"><span data-stu-id="5de13-229">False</span></span>  <br/> |<span data-ttu-id="5de13-230">Верно.</span><span class="sxs-lookup"><span data-stu-id="5de13-230">True</span></span>  <br/> |<span data-ttu-id="5de13-231">False</span><span class="sxs-lookup"><span data-stu-id="5de13-231">False</span></span>  <br/> |<span data-ttu-id="5de13-232">Нет</span><span class="sxs-lookup"><span data-stu-id="5de13-232">None</span></span>  <br/> |<span data-ttu-id="5de13-233">Он</span><span class="sxs-lookup"><span data-stu-id="5de13-233">Owned</span></span>  <br/> |<span data-ttu-id="5de13-234">фуллдетаилс</span><span class="sxs-lookup"><span data-stu-id="5de13-234">FullDetails</span></span>  <br/> |
|<span data-ttu-id="5de13-235">Reviewer</span><span class="sxs-lookup"><span data-stu-id="5de13-235">Reviewer</span></span>  <br/> |<span data-ttu-id="5de13-236">False</span><span class="sxs-lookup"><span data-stu-id="5de13-236">False</span></span>  <br/> |<span data-ttu-id="5de13-237">False</span><span class="sxs-lookup"><span data-stu-id="5de13-237">False</span></span>  <br/> |<span data-ttu-id="5de13-238">False</span><span class="sxs-lookup"><span data-stu-id="5de13-238">False</span></span>  <br/> |<span data-ttu-id="5de13-239">Верно.</span><span class="sxs-lookup"><span data-stu-id="5de13-239">True</span></span>  <br/> |<span data-ttu-id="5de13-240">False</span><span class="sxs-lookup"><span data-stu-id="5de13-240">False</span></span>  <br/> |<span data-ttu-id="5de13-241">Нет</span><span class="sxs-lookup"><span data-stu-id="5de13-241">None</span></span>  <br/> |<span data-ttu-id="5de13-242">Нет</span><span class="sxs-lookup"><span data-stu-id="5de13-242">None</span></span>  <br/> |<span data-ttu-id="5de13-243">фуллдетаилс</span><span class="sxs-lookup"><span data-stu-id="5de13-243">FullDetails</span></span>  <br/> |
|<span data-ttu-id="5de13-244">Участник</span><span class="sxs-lookup"><span data-stu-id="5de13-244">Contributor</span></span>  <br/> |<span data-ttu-id="5de13-245">Верно.</span><span class="sxs-lookup"><span data-stu-id="5de13-245">True</span></span>  <br/> |<span data-ttu-id="5de13-246">False</span><span class="sxs-lookup"><span data-stu-id="5de13-246">False</span></span>  <br/> |<span data-ttu-id="5de13-247">False</span><span class="sxs-lookup"><span data-stu-id="5de13-247">False</span></span>  <br/> |<span data-ttu-id="5de13-248">Верно.</span><span class="sxs-lookup"><span data-stu-id="5de13-248">True</span></span>  <br/> |<span data-ttu-id="5de13-249">False</span><span class="sxs-lookup"><span data-stu-id="5de13-249">False</span></span>  <br/> |<span data-ttu-id="5de13-250">Нет</span><span class="sxs-lookup"><span data-stu-id="5de13-250">None</span></span>  <br/> |<span data-ttu-id="5de13-251">Нет</span><span class="sxs-lookup"><span data-stu-id="5de13-251">None</span></span>  <br/> |<span data-ttu-id="5de13-252">Нет</span><span class="sxs-lookup"><span data-stu-id="5de13-252">None</span></span>  <br/> |
   
<span data-ttu-id="5de13-253">Если вы укажете ненастраиваемый уровень разрешений в запросе разрешений на уровне папки, вам не нужно указывать индивидуальные параметры разрешений.</span><span class="sxs-lookup"><span data-stu-id="5de13-253">If you specify a non-custom permission level in the folder-level permissions request, you don't need to specify the individual permission settings.</span></span> <span data-ttu-id="5de13-254">Если вы задаете отдельное разрешение, когда вы задаете уровень разрешений, в отклике будет возвращена ошибка **ерроринвалидпермиссионсеттингс** .</span><span class="sxs-lookup"><span data-stu-id="5de13-254">If you do specify an individual permission when you set a permission level, an **ErrorInvalidPermissionSettings** error will be returned in the response.</span></span> 
  
## <a name="adding-folder-permissions-by-using-the-ews-managed-api"></a><span data-ttu-id="5de13-255">Добавление разрешений для папки с помощью управляемого API EWS</span><span class="sxs-lookup"><span data-stu-id="5de13-255">Adding folder permissions by using the EWS Managed API</span></span>
<span data-ttu-id="5de13-256"><a name="bk_enableewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="5de13-256"><a name="bk_enableewsma"> </a></span></span>

<span data-ttu-id="5de13-257">В приведенном ниже примере кода показано, как использовать управляемый API EWS для:</span><span class="sxs-lookup"><span data-stu-id="5de13-257">The following code example shows how to use the EWS Managed API to:</span></span> 
  
- <span data-ttu-id="5de13-258">Создайте новый объект [фолдерпермиссион](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folderpermission%28v=exchg.80%29.aspx) для нового пользователя.</span><span class="sxs-lookup"><span data-stu-id="5de13-258">Create a new [FolderPermission](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folderpermission%28v=exchg.80%29.aspx) object for the new user.</span></span> 
    
- <span data-ttu-id="5de13-259">Получение текущих разрешений для папки с помощью метода [BIND](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="5de13-259">Get the current permissions for a folder by using the [Bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) method.</span></span> 
    
- <span data-ttu-id="5de13-260">Добавьте новый **фолдерпермиссионс** в свойство [Folder. Permissions](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.permissions%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="5de13-260">Add the new **FolderPermissions** to the [Folder.Permissions](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.permissions%28v=exchg.80%29.aspx) property.</span></span> 
    
- <span data-ttu-id="5de13-261">Вызовите метод [Update](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.update%28v=exchg.80%29.aspx) , чтобы сохранить новые разрешения на сервере.</span><span class="sxs-lookup"><span data-stu-id="5de13-261">Call the [Update](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.update%28v=exchg.80%29.aspx) method to save the new permissions to the server.</span></span> 
    
<span data-ttu-id="5de13-262">В этом примере предполагается, что **Служба** является допустимым объектом [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) для владельца почтового ящика, а пользователь прошел проверку подлинности на сервере Exchange.</span><span class="sxs-lookup"><span data-stu-id="5de13-262">This example assumes that **service** is a valid [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object for the mailbox owner and that the user has been authenticated to an Exchange server.</span></span> 
  
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

<span data-ttu-id="5de13-263">В следующей строке кода указывается уровень разрешений.</span><span class="sxs-lookup"><span data-stu-id="5de13-263">The following line of code specifies the permission level.</span></span>
  
```cs
    FolderPermission fldperm = new FolderPermission("sadie@contoso.com", FolderPermissionLevel.Editor);
```

<span data-ttu-id="5de13-264">Если вы хотите использовать пользовательский уровень разрешений, используйте вместо этого этот код.</span><span class="sxs-lookup"><span data-stu-id="5de13-264">If you want to use the custom permission level, use this code instead.</span></span>
  
```cs
FolderPermission fldperm = new FolderPermission();
fldperm.UserId = "sadie@Contoso1000.onmicrosoft.com";
fldperm.CanCreateItems = true;
fldperm.CanCreateSubFolders = true;
…
```

<span data-ttu-id="5de13-265">Вы можете задать любое или все доступные для записи [Свойства фолдерпермиссион](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folderpermission_properties%28v=exchg.80%29.aspx) при создании объекта **фолдерпермиссион** с пользовательским уровнем разрешений.</span><span class="sxs-lookup"><span data-stu-id="5de13-265">You can set any or all of the writable [FolderPermission properties](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folderpermission_properties%28v=exchg.80%29.aspx) when you create a **FolderPermission** object with a custom permission level.</span></span> <span data-ttu-id="5de13-266">Однако обратите внимание, что [фолдерпермиссионлевел](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folderpermissionlevel%28v=exchg.80%29.aspx) не имеет явное значение, **настраиваемое** приложением.</span><span class="sxs-lookup"><span data-stu-id="5de13-266">Note, however, that the [FolderPermissionLevel](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folderpermissionlevel%28v=exchg.80%29.aspx) is never explicitly set to **Custom** by the application.</span></span> <span data-ttu-id="5de13-267">Для **фолдерпермиссионлевел** задано значение Custom только при создании объекта **фолдерпермиссион** и настройке отдельных разрешений.</span><span class="sxs-lookup"><span data-stu-id="5de13-267">The **FolderPermissionLevel** is set to Custom only when you create a **FolderPermission** object and set individual permissions.</span></span> 
  
## <a name="adding-folder-permissions-by-using-ews"></a><span data-ttu-id="5de13-268">Добавление разрешений для папки с помощью EWS</span><span class="sxs-lookup"><span data-stu-id="5de13-268">Adding folder permissions by using EWS</span></span>
<span data-ttu-id="5de13-269"><a name="bk_enableews"> </a></span><span class="sxs-lookup"><span data-stu-id="5de13-269"><a name="bk_enableews"> </a></span></span>

<span data-ttu-id="5de13-270">В следующих примерах кода EWS показано, как добавить разрешения в определенную папку, получая текущие разрешения, а затем отправляя список новых разрешений.</span><span class="sxs-lookup"><span data-stu-id="5de13-270">The following EWS code examples show how to add permissions to a specific folder by retrieving the current permissions and then submitting a list of new permissions.</span></span>
  
<span data-ttu-id="5de13-271">Первый шаг — Отправка запроса на получение [папки](https://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) , где значение [дистингуишедфолдерид](https://msdn.microsoft.com/library/50018162-2941-4227-8a5b-d6b4686bb32f%28Office.15%29.aspx) указывает папку, в которую добавляются разрешения (папка "Отправленные" в этом примере), а значение [фиелдури](https://msdn.microsoft.com/library/24af8e3b-3074-4c8c-8d0a-52446508d044%28Office.15%29.aspx) включает в себя папку: набор разрешений.</span><span class="sxs-lookup"><span data-stu-id="5de13-271">The first step is to send a [GetFolder](https://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) request, where the [DistinguishedFolderId](https://msdn.microsoft.com/library/50018162-2941-4227-8a5b-d6b4686bb32f%28Office.15%29.aspx) value specifies the folder in which to add permissions (the Sent Items folder in this example) and the [FieldURI](https://msdn.microsoft.com/library/24af8e3b-3074-4c8c-8d0a-52446508d044%28Office.15%29.aspx) value includes folder:PermissionSet.</span></span> <span data-ttu-id="5de13-272">Этот запрос получает параметры разрешений для указанной папки.</span><span class="sxs-lookup"><span data-stu-id="5de13-272">This request will retrieve the permission settings for the folder specified.</span></span> 
  
<span data-ttu-id="5de13-273">Это также запрос XML, который отправляет управляемый API EWS при вызове метода **BIND** для [добавления разрешений для папки](#bk_enableewsma).</span><span class="sxs-lookup"><span data-stu-id="5de13-273">This is also the XML request that the EWS Managed API sends when you call the **Bind** method to [add folder permissions](#bk_enableewsma).</span></span>
  
```XML
  <?xml version="1.0" encoding="utf-8"?>
  <soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
                 xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                 xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                 xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
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

<span data-ttu-id="5de13-274">Сервер отвечает на запрос к **папке** жетфолдерреспонсе с сообщением [GetFolderResponse](https://msdn.microsoft.com/library/47abeec8-78dd-4297-8525-099174ec880d%28Office.15%29.aspx) , которое содержит значение **ошибки**элемента [респонсекоде](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) , которое указывает, что папка была получена успешно.</span><span class="sxs-lookup"><span data-stu-id="5de13-274">The server responds to the **GetFolder** request with a [GetFolderResponse](https://msdn.microsoft.com/library/47abeec8-78dd-4297-8525-099174ec880d%28Office.15%29.aspx) message that includes a [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) element value of **NoError**, which indicates that the folder was retrieved successfully.</span></span> <span data-ttu-id="5de13-275">Значения [FolderId](https://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) и [ParentFolderId](https://msdn.microsoft.com/library/258f4b1f-367e-4c7d-9c29-eb775a2398c7%28Office.15%29.aspx) были сокращены для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="5de13-275">The [FolderId](https://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) and [ParentFolderId](https://msdn.microsoft.com/library/258f4b1f-367e-4c7d-9c29-eb775a2398c7%28Office.15%29.aspx) values have been shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="893"
                         MinorBuildNumber="17"
                         Version="V2_10"
                         xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:GetFolderResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
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

<span data-ttu-id="5de13-276">Затем используйте операцию **операцию UpdateFolder** , чтобы отправить обновленный уровень [разрешений](https://msdn.microsoft.com/library/6ac1bd17-a089-46bb-b9e6-f5b1dfe1076d%28Office.15%29.aspx), включающий [разрешение](https://msdn.microsoft.com/library/b8d0429a-0e58-4480-9847-4901970c7033%28Office.15%29.aspx) для нового пользователя.</span><span class="sxs-lookup"><span data-stu-id="5de13-276">Next, use the **UpdateFolder** operation to send the updated [PermissionSet](https://msdn.microsoft.com/library/6ac1bd17-a089-46bb-b9e6-f5b1dfe1076d%28Office.15%29.aspx), which includes the [Permission](https://msdn.microsoft.com/library/b8d0429a-0e58-4480-9847-4901970c7033%28Office.15%29.aspx) for the new user.</span></span> <span data-ttu-id="5de13-277">Обратите внимание, что при включении элемента [сетфолдерфиелд](https://msdn.microsoft.com/library/8c69db7b-54b5-4ae2-abca-4d6e0937a790%28Office.15%29.aspx) для соответствующей папки в операции [операцию UpdateFolder](https://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx) все параметры разрешений для папки будут перезаписаны.</span><span class="sxs-lookup"><span data-stu-id="5de13-277">Note that including the [SetFolderField](https://msdn.microsoft.com/library/8c69db7b-54b5-4ae2-abca-4d6e0937a790%28Office.15%29.aspx) element for the respective folder in the [UpdateFolder](https://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx) operation will overwrite all the permission settings on the folder.</span></span> <span data-ttu-id="5de13-278">Аналогично, при включении параметра [делетефолдерфиелд](https://msdn.microsoft.com/library/f9c2187b-4c60-4358-b4b4-ede50eadae48%28Office.15%29.aspx) операции **операцию UpdateFolder** также будут удалены все параметры разрешений для папки.</span><span class="sxs-lookup"><span data-stu-id="5de13-278">Likewise, including the [DeleteFolderField](https://msdn.microsoft.com/library/f9c2187b-4c60-4358-b4b4-ede50eadae48%28Office.15%29.aspx) option of the **UpdateFolder** operation will also delete all the permission settings on the folder.</span></span> 
  
<span data-ttu-id="5de13-279">Это также запрос XML, который отправляет управляемый API EWS при вызове метода **Update** для [добавления разрешений для папки](#bk_enableewsma).</span><span class="sxs-lookup"><span data-stu-id="5de13-279">This is also the XML request that the EWS Managed API sends when you call the **Update** method to [add folder permissions](#bk_enableewsma).</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
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

<span data-ttu-id="5de13-280">В следующей строке кода указывается уровень разрешений.</span><span class="sxs-lookup"><span data-stu-id="5de13-280">The following line of code specifies the permission level.</span></span>
  
```xml
<t:Permission>
    <t:UserId>
        <t:PrimarySmtpAddress>sadie@contoso.com</t:PrimarySmtpAddress>
    </t:UserId>
    <t:PermissionLevel>Editor</t:PermissionLevel>
</t:Permission>
```

<span data-ttu-id="5de13-281">Если вы хотите использовать пользовательский уровень разрешений, используйте вместо этого этот код.</span><span class="sxs-lookup"><span data-stu-id="5de13-281">If you want to use the custom permission level, use this code instead.</span></span>
  
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

<span data-ttu-id="5de13-282">Сервер отвечает на запрос **операцию UpdateFolder** с сообщением [упдатефолдерреспонсе](https://msdn.microsoft.com/library/31f47739-dc9c-46ba-9e3f-cce25dc85e6e%28Office.15%29.aspx) , которое содержит значение **ошибки**элемента [респонсекоде](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) , которое указывает, что папка обновлена успешно.</span><span class="sxs-lookup"><span data-stu-id="5de13-282">The server responds to the **UpdateFolder** request with an [UpdateFolderResponse](https://msdn.microsoft.com/library/31f47739-dc9c-46ba-9e3f-cce25dc85e6e%28Office.15%29.aspx) message that includes a [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) element value of **NoError**, which indicates that the folder was updated successfully.</span></span>
  
## <a name="removing-folder-permissions-by-using-the-ews-managed-api"></a><span data-ttu-id="5de13-283">Удаление разрешений для папки с помощью управляемого API EWS</span><span class="sxs-lookup"><span data-stu-id="5de13-283">Removing folder permissions by using the EWS Managed API</span></span>
<span data-ttu-id="5de13-284"><a name="bk_removeewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="5de13-284"><a name="bk_removeewsma"> </a></span></span>

<span data-ttu-id="5de13-285">В приведенном ниже примере кода показано, как использовать управляемый API EWS для удаления всех разрешений пользователя в определенной папке, за исключением разрешений по умолчанию и анонимности:</span><span class="sxs-lookup"><span data-stu-id="5de13-285">The following code example shows how to use the EWS Managed API to remove all user permissions on a specific folder, except for the default and anonymous permissions, by:</span></span>
  
1. <span data-ttu-id="5de13-286">Извлечение текущих разрешений для папки с помощью метода **BIND** .</span><span class="sxs-lookup"><span data-stu-id="5de13-286">Getting the current permissions for a folder by using the **Bind** method.</span></span> 
    
2. <span data-ttu-id="5de13-287">Итерация по коллекции **разрешений** и удаление разрешений для отдельных пользователей.</span><span class="sxs-lookup"><span data-stu-id="5de13-287">Iterating through the **Permissions** collection and removing permissions for individual users.</span></span> 
    
3. <span data-ttu-id="5de13-288">Вызов метода **Update** для сохранения изменений.</span><span class="sxs-lookup"><span data-stu-id="5de13-288">Calling the **Update** method to save the changes.</span></span> 
    
<span data-ttu-id="5de13-289">В этом примере удаляются все разрешения пользователя на папку.</span><span class="sxs-lookup"><span data-stu-id="5de13-289">This example removes all user permissions on a folder.</span></span> <span data-ttu-id="5de13-290">Если вы хотите изменить этот пример, чтобы удалить разрешения только для определенного пользователя, измените следующую строку кода, чтобы определить отображаемое имя или SMTP-адрес пользователя.</span><span class="sxs-lookup"><span data-stu-id="5de13-290">If you want to modify this example to remove permissions only for a specific user, change the following line of code to identify either the display name or SMTP address of the user.</span></span>
  
```cs
if (sentItemsFolder.Permissions[t].UserId.DisplayName != null || sentItemsFolder.Permissions[t].UserId.PrimarySmtpAddress != null)
```

<span data-ttu-id="5de13-291">В этом примере предполагается, что **Служба** является допустимым объектом [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) для владельца почтового ящика, а пользователь прошел проверку подлинности на сервере Exchange.</span><span class="sxs-lookup"><span data-stu-id="5de13-291">This example assumes that **service** is a valid [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object for the mailbox owner and that the user has been authenticated to an Exchange server.</span></span> 
  
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

## <a name="removing-folder-permissions-by-using-ews"></a><span data-ttu-id="5de13-292">Удаление разрешений для папки с помощью EWS</span><span class="sxs-lookup"><span data-stu-id="5de13-292">Removing folder permissions by using EWS</span></span>
<span data-ttu-id="5de13-293"><a name="bk_removeews"> </a></span><span class="sxs-lookup"><span data-stu-id="5de13-293"><a name="bk_removeews"> </a></span></span>

<span data-ttu-id="5de13-294">В следующих примерах кода EWS показано, как удалить все разрешения пользователя для конкретной папки, за исключением разрешений по умолчанию и анонимности.</span><span class="sxs-lookup"><span data-stu-id="5de13-294">The following EWS code examples show how to remove all user permissions on a specific folder, except for the default and anonymous permissions.</span></span>
  
<span data-ttu-id="5de13-295">Сначала отправьте запрос на получение [папки](https://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) , где значение [дистингуишедфолдерид](https://msdn.microsoft.com/library/50018162-2941-4227-8a5b-d6b4686bb32f%28Office.15%29.aspx) указывает папку для удаления разрешений (папка "Отправленные" в этом примере), а значение [Фиелдури](https://msdn.microsoft.com/library/24af8e3b-3074-4c8c-8d0a-52446508d044%28Office.15%29.aspx) включает папку: набор разрешений.</span><span class="sxs-lookup"><span data-stu-id="5de13-295">First, send a [GetFolder](https://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) request where the [DistinguishedFolderId](https://msdn.microsoft.com/library/50018162-2941-4227-8a5b-d6b4686bb32f%28Office.15%29.aspx) value specifies the folder in which to remove permissions (the Sent Items folder in this example) and the [FieldURI](https://msdn.microsoft.com/library/24af8e3b-3074-4c8c-8d0a-52446508d044%28Office.15%29.aspx) value includes folder:PermissionSet.</span></span> <span data-ttu-id="5de13-296">Этот запрос получает заданный для папки уровень [разрешений](https://msdn.microsoft.com/library/6ac1bd17-a089-46bb-b9e6-f5b1dfe1076d%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="5de13-296">This request will retrieve the [PermissionSet](https://msdn.microsoft.com/library/6ac1bd17-a089-46bb-b9e6-f5b1dfe1076d%28Office.15%29.aspx) for the folder specified.</span></span> 
  
<span data-ttu-id="5de13-297">Это также запрос XML, который отправляет управляемый API EWS при вызове метода **BIND** для [удаления разрешений для папки](#bk_removeewsma).</span><span class="sxs-lookup"><span data-stu-id="5de13-297">This is also the XML request that the EWS Managed API sends when you call the **Bind** method to [remove folder permissions](#bk_removeewsma).</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
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

<span data-ttu-id="5de13-298">Сервер отвечает на запрос к **папке** жетфолдерреспонсе с сообщением [GetFolderResponse](https://msdn.microsoft.com/library/47abeec8-78dd-4297-8525-099174ec880d%28Office.15%29.aspx) , которое содержит значение **ошибки**элемента [респонсекоде](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) , которое указывает, что папка была получена успешно.</span><span class="sxs-lookup"><span data-stu-id="5de13-298">The server responds to the **GetFolder** request with a [GetFolderResponse](https://msdn.microsoft.com/library/47abeec8-78dd-4297-8525-099174ec880d%28Office.15%29.aspx) message that includes a [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) element value of **NoError**, which indicates that the folder was retrieved successfully.</span></span> <span data-ttu-id="5de13-299">Значения элементов **FolderId** и **ParentFolderId** были сокращены для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="5de13-299">The values of the **FolderId** and **ParentFolderId** elements have been shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="893"
                         MinorBuildNumber="17"
                         Version="V2_10"
                         xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:GetFolderResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
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

<span data-ttu-id="5de13-300">Затем используйте операцию **операцию UpdateFolder** , чтобы отправить обновленный уровень **разрешений**, не включающий в себя **разрешение** для удаленного пользователя.</span><span class="sxs-lookup"><span data-stu-id="5de13-300">Next, use the **UpdateFolder** operation to send the updated **PermissionSet**, which does not include the **Permission** for the removed user.</span></span> 
  
<span data-ttu-id="5de13-301">Это также запрос XML, который отправляет управляемый API EWS при вызове метода **Update** для [удаления разрешений для папки](#bk_removeewsma).</span><span class="sxs-lookup"><span data-stu-id="5de13-301">This is also the XML request that the EWS Managed API sends when you call the **Update** method to [remove folder permissions](#bk_removeewsma).</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
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

<span data-ttu-id="5de13-302">Сервер отвечает на запрос **операцию UpdateFolder** с сообщением **упдатефолдерреспонсе** , которое содержит значение **ошибки**элемента [респонсекоде](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) , которое указывает, что обновление прошло успешно.</span><span class="sxs-lookup"><span data-stu-id="5de13-302">The server responds to the **UpdateFolder** request with an **UpdateFolderResponse** message that includes a [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) element value of **NoError**, which indicates that the update was successful.</span></span>
  
## <a name="updating-folder-permissions-by-using-the-ews-managed-api"></a><span data-ttu-id="5de13-303">Обновление разрешений для папки с помощью управляемого API EWS</span><span class="sxs-lookup"><span data-stu-id="5de13-303">Updating folder permissions by using the EWS Managed API</span></span>
<span data-ttu-id="5de13-304"><a name="bk_updateewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="5de13-304"><a name="bk_updateewsma"> </a></span></span>

<span data-ttu-id="5de13-305">Вы также можете обновить разрешения для папки для определенной папки с помощью управляемого API EWS.</span><span class="sxs-lookup"><span data-stu-id="5de13-305">You can also update folder permissions for a specific folder by using the EWS Managed API.</span></span> <span data-ttu-id="5de13-306">Чтобы обновить разрешения, выполните следующие действия.</span><span class="sxs-lookup"><span data-stu-id="5de13-306">To update the permissions:</span></span> 
  
1. <span data-ttu-id="5de13-307">[Удалите разрешения для папки](#bk_removeewsma) с устаревшими разрешениями, но не вызывайте метод **обновления** (пока).</span><span class="sxs-lookup"><span data-stu-id="5de13-307">[Remove the folder permissions](#bk_removeewsma) for the outdated permissions, but do not call the **Update** method (yet).</span></span> 
    
2. <span data-ttu-id="5de13-308">[Добавление разрешений на доступ к папке для новых или измененных пользователей](#bk_enableewsma).</span><span class="sxs-lookup"><span data-stu-id="5de13-308">[Add folder permissions for the new or changed users](#bk_enableewsma).</span></span>
    
3. <span data-ttu-id="5de13-309">Вызовите метод **Update** , чтобы сохранить изменения.</span><span class="sxs-lookup"><span data-stu-id="5de13-309">Call the **Update** method to save the changes.</span></span> 
    
<span data-ttu-id="5de13-310">Если попытаться добавить два набора разрешений для одного и того же пользователя, появится сообщение об ошибке **сервицереспонсиксцептион** со следующим описанием: "указанный набор разрешений содержит дублирующиеся UserID".</span><span class="sxs-lookup"><span data-stu-id="5de13-310">If you try to add two sets of permissions for the same user, you will receive a **ServiceResponseException** error with the following description: "The specified permission set contains duplicate UserIds".</span></span> <span data-ttu-id="5de13-311">В этом случае удалите текущие разрешения из коллекции **разрешений** , а затем добавьте новые разрешения в коллекцию **разрешений** .</span><span class="sxs-lookup"><span data-stu-id="5de13-311">In that case, remove the current permissions from the **Permission** collection, then add the new permissions to the **Permission** collection.</span></span> 
  
## <a name="updating-folder-permissions-by-using-ews"></a><span data-ttu-id="5de13-312">Обновление разрешений для папки с помощью EWS</span><span class="sxs-lookup"><span data-stu-id="5de13-312">Updating folder permissions by using EWS</span></span>
<span data-ttu-id="5de13-313"><a name="bk_updateews"> </a></span><span class="sxs-lookup"><span data-stu-id="5de13-313"><a name="bk_updateews"> </a></span></span>

<span data-ttu-id="5de13-314">Вы также можете обновить разрешения для папок для определенных папок с помощью EWS, объединив процесс удаления и добавления.</span><span class="sxs-lookup"><span data-stu-id="5de13-314">You can also update folder permissions for specific folders by using EWS by combining the removal and addition process.</span></span> <span data-ttu-id="5de13-315">Чтобы обновить разрешения, выполните следующие действия.</span><span class="sxs-lookup"><span data-stu-id="5de13-315">To update the permissions:</span></span> 
  
1. <span data-ttu-id="5de13-316">Получение текущих разрешений папки с помощью операции "операция с **папкой** ".</span><span class="sxs-lookup"><span data-stu-id="5de13-316">Retrieve the folder's current permissions by using the **GetFolder** operation.</span></span> 
    
2. <span data-ttu-id="5de13-317">Отправьте обновленный список разрешений с помощью операции **операцию UpdateFolder** .</span><span class="sxs-lookup"><span data-stu-id="5de13-317">Send an updated list of permissions by using the **UpdateFolder** operation.</span></span> 
    
<span data-ttu-id="5de13-318">Это те же две операции, которые используются для [включения](#bk_enableews) или [отключения доступа](#bk_removeews) с помощью EWS.</span><span class="sxs-lookup"><span data-stu-id="5de13-318">These are the same two operations you use to [enable](#bk_enableews) or [remove access](#bk_removeews) by using EWS.</span></span> <span data-ttu-id="5de13-319">Единственное отличие заключается в том, что при получении ответа на **папку** он будет содержать набор **разрешений** для пользователя.</span><span class="sxs-lookup"><span data-stu-id="5de13-319">The only difference is that when you receive the **GetFolder** response, it will contain a **Permission** set for user.</span></span> <span data-ttu-id="5de13-320">Просто замените существующий элемент **Permission** на новый элемент **Permission** , а затем отправьте операцию **операцию UpdateFolder** с новым значением или значениями **разрешений** .</span><span class="sxs-lookup"><span data-stu-id="5de13-320">Simply replace that existing **Permission** element with the new **Permission** element, and then send the **UpdateFolder** operation with the new **Permission** value or values.</span></span> 
  
<span data-ttu-id="5de13-321">Если вы попытаетесь добавить два набора разрешений для одного и того же пользователя, вы получите значение **респонсекоде** для **еррордупликатеусеридсспеЦифиед**.</span><span class="sxs-lookup"><span data-stu-id="5de13-321">If you try to add two sets of permissions for the same user, you will receive a **ResponseCode** value of **ErrorDuplicateUserIdsSpecified**.</span></span> <span data-ttu-id="5de13-322">В этом случае удалите устаревшее значение разрешения для пользователя из запроса и повторите запрос.</span><span class="sxs-lookup"><span data-stu-id="5de13-322">In that case, remove the outdated Permission value for the user from the request and then retry the request.</span></span>

## <a name="next-steps"></a><span data-ttu-id="5de13-323">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="5de13-323">Next steps</span></span>

<span data-ttu-id="5de13-324">После предоставления пользователю разрешения на доступ к определенной папке пользователь может получить доступ к папке в качестве делегата.</span><span class="sxs-lookup"><span data-stu-id="5de13-324">After you give a user permission to a specific folder, the user can access the folder as a delegate.</span></span> <span data-ttu-id="5de13-325">Дополнительные сведения см. в указанных ниже статьях.</span><span class="sxs-lookup"><span data-stu-id="5de13-325">For more information, see:</span></span>
  
- [<span data-ttu-id="5de13-326">Доступ к электронной почте как представителю с помощью EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="5de13-326">Access email as a delegate by using EWS in Exchange</span></span>](how-to-access-email-as-a-delegate-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="5de13-327">Доступ к календарю как представителю с помощью EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="5de13-327">Access a calendar as a delegate by using EWS in Exchange</span></span>](how-to-access-a-calendar-as-a-delegate-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="5de13-328">Доступ к контактам как представителю с помощью EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="5de13-328">Access contacts as a delegate by using EWS in Exchange</span></span>](how-to-access-contacts-as-a-delegate-by-using-ews-in-exchange.md)
    
## <a name="see-also"></a><span data-ttu-id="5de13-329">См. также</span><span class="sxs-lookup"><span data-stu-id="5de13-329">See also</span></span>

- [<span data-ttu-id="5de13-330">Передача прав доступа и EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="5de13-330">Delegate access and EWS in Exchange</span></span>](delegate-access-and-ews-in-exchange.md)   
- [<span data-ttu-id="5de13-331">Добавление и удаление делегатов с помощью EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="5de13-331">Add and remove delegates by using EWS in Exchange</span></span>](how-to-add-and-remove-delegates-by-using-ews-in-exchange.md)    
- [<span data-ttu-id="5de13-332">Папки и элементы в веб-службах Exchange</span><span class="sxs-lookup"><span data-stu-id="5de13-332">Folders and items in EWS in Exchange</span></span>](folders-and-items-in-ews-in-exchange.md)
    

