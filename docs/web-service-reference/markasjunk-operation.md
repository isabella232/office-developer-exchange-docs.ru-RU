---
title: MarkAsJunk Operation
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 1f71f04d-56a9-4fee-a4e7-d1034438329e
description: Найдите сведения о веб-служб Exchange MarkAsJunk операции.
ms.openlocfilehash: b9d79e6fbec87ce41030b4981f3c16f2f9ce9507
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834353"
---
# <a name="markasjunk-operation"></a><span data-ttu-id="626c6-103">MarkAsJunk Operation</span><span class="sxs-lookup"><span data-stu-id="626c6-103">MarkAsJunk operation</span></span>

<span data-ttu-id="626c6-104">Найдите сведения о **MarkAsJunk** операции веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="626c6-104">Find information about the **MarkAsJunk** EWS operation.</span></span> 
  
<span data-ttu-id="626c6-105">Операция **MarkAsJunk** добавляет и удаление пользователей из списка заблокированных электронной почты и перемещает сообщения электронной почты в папку нежелательной почты.</span><span class="sxs-lookup"><span data-stu-id="626c6-105">The **MarkAsJunk** operation adds and removes users from the blocked email list and moves email messages to the Junk Email folder.</span></span> 
  
<span data-ttu-id="626c6-106">Эта операция появилась в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="626c6-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-markasjunk-operation"></a><span data-ttu-id="626c6-107">С помощью операции MarkAsJunk</span><span class="sxs-lookup"><span data-stu-id="626c6-107">Using the MarkAsJunk operation</span></span>

<span data-ttu-id="626c6-108">Операция **MarkAsJunk** содержит два типа Boolean вариантов, чтобы указать ли будет добавлен в список заблокированных отправителей электронной почты отправителя и является ли целевой для сообщения электронной почты необходимо переместить папку нежелательной почты по умолчанию или к папке "Входящие".</span><span class="sxs-lookup"><span data-stu-id="626c6-108">The **MarkAsJunk** operation contains two Boolean options to indicate whether an email sender should be added to the blocked sender list and whether the target email message should be moved to the default Junk Email folder or the Inbox folder.</span></span> <span data-ttu-id="626c6-109">Действия определяются по значениям **IsJunk** и **MoveItem** атрибуты.</span><span class="sxs-lookup"><span data-stu-id="626c6-109">The actions are determined by the values of the **IsJunk** and **MoveItem** attributes.</span></span> <span data-ttu-id="626c6-110">Ниже приведены возможные действия в зависимости от комбинации значений атрибутов **IsJunk** и **MoveItem** .</span><span class="sxs-lookup"><span data-stu-id="626c6-110">The following are the possible actions based on the value combinations for the **IsJunk** and **MoveItem** attributes:</span></span> 
  
- <span data-ttu-id="626c6-111">Если атрибут **IsJunk** имеет значение **true**, а атрибут **MoveItem** имеет значение **true**, отправителя сообщения электронной почты конечного добавляется в список заблокированных отправителей, и сообщение электронной почты перемещается в папку нежелательной Dmail.</span><span class="sxs-lookup"><span data-stu-id="626c6-111">If the **IsJunk** attribute is set to **true**, and the **MoveItem** attribute is set to **true**, the sender of the target email message is added to the blocked sender list and the email message is moved to the Junk Dmail folder.</span></span>
    
- <span data-ttu-id="626c6-112">Если атрибут **IsJunk** имеет значение **true**, а атрибут **MoveItem** присвоено **значение false**, отправителя сообщения электронной почты конечного добавляется в список заблокированных отправителей, и сообщение электронной почты не перемещается из папки.</span><span class="sxs-lookup"><span data-stu-id="626c6-112">If the **IsJunk** attribute is set to **true**, and the **MoveItem** attribute is set to **false**, the sender of the target email message is added to the blocked sender list and the email message is not moved from the folder.</span></span>
    
- <span data-ttu-id="626c6-113">Если атрибут **IsJunk** имеет значение **false**, а **MoveItem** атрибут имеет значение **true**, отправителя конечного messageis электронной почты, удаляется из списка заблокированных отправителей, и сообщение электронной почты перемещается в папку "Входящие".</span><span class="sxs-lookup"><span data-stu-id="626c6-113">If the **IsJunk** attribute is set to **false**, and the **MoveItem** attribute is set to **true**, the sender of the target email messageis removed from the blocked sender list and the email message is moved to the Inbox folder.</span></span>
    
- <span data-ttu-id="626c6-114">Если атрибут **IsJunk** имеет значение **false**, а атрибут **MoveItem** присвоено **значение false**, отправителя сообщения электронной почты конечного удаляется из списка заблокированных отправителей, и сообщение электронной почты не перемещается из папки.</span><span class="sxs-lookup"><span data-stu-id="626c6-114">If the **IsJunk** attribute is set to **false**, and the **MoveItem** attribute is set to **false**, the sender of the target email message is removed from the blocked sender list and the email message is not moved from the folder.</span></span>
    
> [!IMPORTANT]
> <span data-ttu-id="626c6-115">Содержимое списка заблокированных отправителей не доступные из веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="626c6-115">The contents of the blocked sender list are not discoverable from EWS.</span></span> <span data-ttu-id="626c6-116">Если отправитель добавляется в список заблокированных отправителей, необходимо сохранить копию сообщения электронной почты, отправленные с заблокированных отправителей разблокирование отправителя в будущем.</span><span class="sxs-lookup"><span data-stu-id="626c6-116">If a sender is added to the blocked sender list, you need to keep a copy of an email message sent by the blocked sender to unblock the sender in the future.</span></span> 
  
### <a name="markasjunk-operation-soap-headers"></a><span data-ttu-id="626c6-117">Заголовки SOAP MarkAsJunk операции</span><span class="sxs-lookup"><span data-stu-id="626c6-117">MarkAsJunk operation SOAP headers</span></span>

<span data-ttu-id="626c6-118">Операция **MarkAsJunk** можно использовать заголовки SOAP, которые перечислены в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="626c6-118">The **MarkAsJunk** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="626c6-119">**Имя заголовка**</span><span class="sxs-lookup"><span data-stu-id="626c6-119">**Header name**</span></span>|<span data-ttu-id="626c6-120">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="626c6-120">**Element**</span></span>|<span data-ttu-id="626c6-121">**Описание**</span><span class="sxs-lookup"><span data-stu-id="626c6-121">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="626c6-122">**Олицетворение**</span><span class="sxs-lookup"><span data-stu-id="626c6-122">**Impersonation**</span></span> <br/> |[<span data-ttu-id="626c6-123">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="626c6-123">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="626c6-124">Идентифицирует пользователя, которого олицетворения в клиентском приложении.</span><span class="sxs-lookup"><span data-stu-id="626c6-124">Identifies the user whom the client application is impersonating.</span></span> <span data-ttu-id="626c6-125">Этот заголовок можно применять к запросу.</span><span class="sxs-lookup"><span data-stu-id="626c6-125">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="626c6-126">**MailboxCulture**</span><span class="sxs-lookup"><span data-stu-id="626c6-126">**MailboxCulture**</span></span> <br/> |[<span data-ttu-id="626c6-127">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="626c6-127">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="626c6-128">Определяет язык и региональные параметры, как определено в RFC 3066, «Теги для идентификации языков», который будет использоваться для доступа к почтовому ящику.</span><span class="sxs-lookup"><span data-stu-id="626c6-128">Identifies the culture, as defined in RFC 3066, "Tags for the Identification of Languages", to be used to access the mailbox.</span></span> <span data-ttu-id="626c6-129">Этот заголовок можно применять к запросу.</span><span class="sxs-lookup"><span data-stu-id="626c6-129">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="626c6-130">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="626c6-130">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="626c6-131">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="626c6-131">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="626c6-132">Определяет версию схемы для операции запроса.</span><span class="sxs-lookup"><span data-stu-id="626c6-132">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="626c6-133">Этот заголовок можно применять к запросу.</span><span class="sxs-lookup"><span data-stu-id="626c6-133">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="626c6-134">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="626c6-134">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="626c6-135">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="626c6-135">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="626c6-136">Определяет версию сервера, ответившего на запрос.</span><span class="sxs-lookup"><span data-stu-id="626c6-136">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="626c6-137">Этот заголовок можно применять, чтобы получить ответ.</span><span class="sxs-lookup"><span data-stu-id="626c6-137">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="markasjunk-operation-request-example-add-a-sender-to-the-blocked-sender-list"></a><span data-ttu-id="626c6-138">Пример запроса MarkAsJunk операции: Добавление отправителя в список заблокированных отправителей</span><span class="sxs-lookup"><span data-stu-id="626c6-138">MarkAsJunk operation request example: Add a sender to the blocked sender list</span></span>

<span data-ttu-id="626c6-139">В следующем примере запрос операции **MarkAsJunk** показано, как добавить отправителя сообщения электронной почты в список заблокированных отправителей и перемещать сообщения электронной почты в папку нежелательной почты.</span><span class="sxs-lookup"><span data-stu-id="626c6-139">The following example of a **MarkAsJunk** operation request shows how to add the sender of an email to the blocked sender list and move the email to the junk mail folder.</span></span> <span data-ttu-id="626c6-140">Операция **MarkAsJunk** принимает идентификатор сообщения уникальные электронной почты для идентификации электронной почты, который используется для ссылки отправителя, который добавляется в список заблокированных отправителей.</span><span class="sxs-lookup"><span data-stu-id="626c6-140">The **MarkAsJunk** operation accepts the unique email message identifier to identify the email that is used to reference the sender that is added to the blocked sender list.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="626c6-141">Все идентификаторы элементов и ключей изменения в этой статье URL были сокращены, чтобы сохранить удобочитаемость.</span><span class="sxs-lookup"><span data-stu-id="626c6-141">All item identifiers and change keys in this article have been shortened to preserve readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
    <soap:Header>
        <t:RequestServerVersion Version="Exchange2013" />
    </soap:Header>
    <soap:Body>
        <m:MarkAsJunk IsJunk="true" MoveItem="true">
            <m:ItemIds>
                <t:ItemId Id="AAMkAD=" ChangeKey="CQAAABYA" />
            </m:ItemIds>
        </m:MarkAsJunk>
    </soap:Body>
</soap:Envelope>

```

<span data-ttu-id="626c6-142">Запрос SOAP body содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="626c6-142">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="626c6-143">MarkAsJunk</span><span class="sxs-lookup"><span data-stu-id="626c6-143">MarkAsJunk</span></span>](markasjunk.md)
    
- [<span data-ttu-id="626c6-144">Что ItemID</span><span class="sxs-lookup"><span data-stu-id="626c6-144">ItemIds</span></span>](itemids.md)
    
- [<span data-ttu-id="626c6-145">Идентификатор элемента</span><span class="sxs-lookup"><span data-stu-id="626c6-145">ItemId</span></span>](itemid.md)
    
## <a name="successful-markasjunk-operation-response"></a><span data-ttu-id="626c6-146">Успешные операции ответа MarkAsJunk</span><span class="sxs-lookup"><span data-stu-id="626c6-146">Successful MarkAsJunk operation response</span></span>

<span data-ttu-id="626c6-147">В следующем примере показано успешного ответа на запрос операции **MarkAsJunk** добавить отправителя в список заблокированных отправителей и перемещение сообщений электронной почты в папку нежелательной почты.</span><span class="sxs-lookup"><span data-stu-id="626c6-147">The following example shows a successful response to a **MarkAsJunk** operation request to add a sender to the blocked sender list and move the email message to the Junk Email folder.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
    <s:Header>
        <h:ServerVersionInfo MajorVersion="15" 
                             MinorVersion="0" 
                             MajorBuildNumber="545" 
                             MinorBuildNumber="11" 
                             Version="Exchange2013" 
                             xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                             xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                             xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                             xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
    </s:Header>
    <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
            xmlns:xsd="http://www.w3.org/2001/XMLSchema">
        <m:MarkAsJunkResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                              xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
           <m:ResponseMessages>
               <m:MarkAsJunkResponseMessage ResponseClass="Success">
                  <m:ResponseCode>NoError</m:ResponseCode>
                 <m:MovedItemId Id="AAMkAD=" ChangeKey="CQAAABYu" />
               </m:MarkAsJunkResponseMessage>
           </m:ResponseMessages>
        </m:MarkAsJunkResponse>
    </s:Body>
</s:Envelope>
```

<span data-ttu-id="626c6-148">Ответ SOAP body содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="626c6-148">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="626c6-149">MarkAsJunkResponse</span><span class="sxs-lookup"><span data-stu-id="626c6-149">MarkAsJunkResponse</span></span>](markasjunkresponse.md)
    
- [<span data-ttu-id="626c6-150">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="626c6-150">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="626c6-151">MarkAsJunkResponseMessage</span><span class="sxs-lookup"><span data-stu-id="626c6-151">MarkAsJunkResponseMessage</span></span>](markasjunkresponsemessage.md)
    
- [<span data-ttu-id="626c6-152">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="626c6-152">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="626c6-153">MovedItemId</span><span class="sxs-lookup"><span data-stu-id="626c6-153">MovedItemId</span></span>](moveditemid.md)
    
## <a name="markasjunk-operation-request-example-remove-a-sender-from-the-blocked-sender-list"></a><span data-ttu-id="626c6-154">Пример запроса MarkAsJunk операции: удаление отправителя в список заблокированных отправителей</span><span class="sxs-lookup"><span data-stu-id="626c6-154">MarkAsJunk operation request example: Remove a sender from the blocked sender list</span></span>

<span data-ttu-id="626c6-155">В следующем примере запрос операции **MarkAsJunk** показано, как удалить отправителя сообщения электронной почты из списка заблокированных отправителей и перемещение сообщений электронной почты в папке "Входящие".</span><span class="sxs-lookup"><span data-stu-id="626c6-155">The following example of a **MarkAsJunk** operation request shows how to remove the sender of an email message from the blocked sender list and move the email message to the Inbox folder.</span></span> <span data-ttu-id="626c6-156">Необходимо хранить сообщения электронной почты, отправленные с заблокированных отправителей, чтобы удалить отправителя из списка заблокированных отправителей.</span><span class="sxs-lookup"><span data-stu-id="626c6-156">You need to keep an email message sent by the blocked sender to remove the sender from the blocked sender list.</span></span> <span data-ttu-id="626c6-157">Адрес электронной почты отправителя связан с сообщениями электронной почты, отправленные отправителем.</span><span class="sxs-lookup"><span data-stu-id="626c6-157">The sender's email address is associated with email messages that have been sent by the sender.</span></span> <span data-ttu-id="626c6-158">Удаление отправителя в список заблокированных отправителей не выполняется, если сообщение электронной почты ссылку больше не существует в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="626c6-158">Removing a sender from the blocked sender list will not succeed if the reference email message no longer exists in the user's mailbox.</span></span> <span data-ttu-id="626c6-159">Идентификатор элемента, который используется для связи с его отправителю сообщения электронной почты должен быть связан с элементом, который существует в почтовом ящике Exchange.</span><span class="sxs-lookup"><span data-stu-id="626c6-159">The item identifier used to associate an email message with its sender must be associated with an item that exists in the Exchange mailbox.</span></span> <span data-ttu-id="626c6-160">Рекомендуется создать скрытые папки для хранения элементов, отправленных ранее заблокированных отправителей, чтобы отправители может быть заблокирован из клиентского приложения.</span><span class="sxs-lookup"><span data-stu-id="626c6-160">We recommend that you create a hidden folder to store items sent by previously blocked senders so that the senders can be unblocked from the client application.</span></span> <span data-ttu-id="626c6-161">В случае, если элемент был удален из почтового ящика Exchange, администратор должен использовать консоль управления Exchange для доступа к списку заблокированных отправителей для удаления отправителя из списка.</span><span class="sxs-lookup"><span data-stu-id="626c6-161">In the event that an item has been removed from the Exchange mailbox, an administrator has to use the Exchange Management Console to access the blocked sender list to remove a sender from the list.</span></span> <span data-ttu-id="626c6-162">Сведения о том, как разблокировать пользователя с помощью консоли управления Exchange, в [Настройка надежных отправителей и заблокированных отправителей параметры в Office 365](http://support.microsoft.com/kb/2545137).</span><span class="sxs-lookup"><span data-stu-id="626c6-162">For information about how to unblock a user by using the Exchange Management Console, see [How to configure the safe senders and blocked senders settings in Office 365](http://support.microsoft.com/kb/2545137).</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
    <soap:Header>
      <t:RequestServerVersion Version="Exchange2013" />
    </soap:Header>
    <soap:Body>
      <m:MarkAsJunk IsJunk="false" MoveItem="true">
        <m:ItemIds>
          <t:ItemId Id="AAMkAD=" ChangeKey="CQAAABYu" />
        </m:ItemIds>
      </m:MarkAsJunk>
    </soap:Body>
 </soap:Envelope>

```

<span data-ttu-id="626c6-163">Успешного ответа для удаления отправителя в список заблокированных отправителей — это то же, что ответ на добавление отправителя в список заблокированных отправителей.</span><span class="sxs-lookup"><span data-stu-id="626c6-163">A successful response for removing a sender from the blocked sender list is the same as the response for adding a sender to the blocked sender list.</span></span>
  
<span data-ttu-id="626c6-164">Запрос SOAP body содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="626c6-164">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="626c6-165">MarkAsJunk</span><span class="sxs-lookup"><span data-stu-id="626c6-165">MarkAsJunk</span></span>](markasjunk.md)
    
- [<span data-ttu-id="626c6-166">Что ItemID</span><span class="sxs-lookup"><span data-stu-id="626c6-166">ItemIds</span></span>](itemids.md)
    
- [<span data-ttu-id="626c6-167">Идентификатор элемента</span><span class="sxs-lookup"><span data-stu-id="626c6-167">ItemId</span></span>](itemid.md)
    
## <a name="markasjunk-operation-error-response"></a><span data-ttu-id="626c6-168">Ошибка операции MarkAsJunk ответа</span><span class="sxs-lookup"><span data-stu-id="626c6-168">MarkAsJunk operation error response</span></span>

<span data-ttu-id="626c6-169">В следующем примере показано ошибочный ответ на запрос операции **MarkAsJunk** .</span><span class="sxs-lookup"><span data-stu-id="626c6-169">The following example shows an error response to a **MarkAsJunk** operation request.</span></span> <span data-ttu-id="626c6-170">Это ответ на запрос для добавления или удаления отправителя в списке заблокированных отправителей, когда сообщение электронной почты, указанного идентификатором идентификатор элемента больше не существует в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="626c6-170">This is a response to a request to add or remove a sender from the blocked sender list when the email message specified by the item identifier no longer exists in the mailbox.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" 
                         MinorVersion="0" 
                         MajorBuildNumber="545" 
                         MinorBuildNumber="11" 
                         Version="Exchange2013" 
                         xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:MarkAsJunkResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                          xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:MarkAsJunkResponseMessage ResponseClass="Error">
          <m:MessageText>The specified object was not found in the store.</m:MessageText>
          <m:ResponseCode>ErrorItemNotFound</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
        </m:MarkAsJunkResponseMessage>
      </m:ResponseMessages>
    </m:MarkAsJunkResponse>
  </s:Body>
</s:Envelope>
```

<span data-ttu-id="626c6-171">Ошибка ответ SOAP body содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="626c6-171">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="626c6-172">MarkAsJunkResponse</span><span class="sxs-lookup"><span data-stu-id="626c6-172">MarkAsJunkResponse</span></span>](markasjunkresponse.md)
    
- [<span data-ttu-id="626c6-173">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="626c6-173">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="626c6-174">MarkAsJunkResponseMessage</span><span class="sxs-lookup"><span data-stu-id="626c6-174">MarkAsJunkResponseMessage</span></span>](markasjunkresponsemessage.md)
    
- [<span data-ttu-id="626c6-175">MessageText</span><span class="sxs-lookup"><span data-stu-id="626c6-175">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="626c6-176">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="626c6-176">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="626c6-177">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="626c6-177">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
## <a name="see-also"></a><span data-ttu-id="626c6-178">См. также</span><span class="sxs-lookup"><span data-stu-id="626c6-178">See also</span></span>

- [<span data-ttu-id="626c6-179">Операции EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="626c6-179">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
    
- <span data-ttu-id="626c6-180">[Операции GetItem](getitem-operation.md) Операции GetItem</span><span class="sxs-lookup"><span data-stu-id="626c6-180">[GetItem operation](getitem-operation.md) GetItem operation</span></span> 
    
- [<span data-ttu-id="626c6-181">FindItem Operation</span><span class="sxs-lookup"><span data-stu-id="626c6-181">FindItem operation</span></span>](finditem-operation.md)
    

