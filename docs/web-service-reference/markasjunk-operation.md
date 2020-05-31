---
title: Операция MarkAsJunk
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 1f71f04d-56a9-4fee-a4e7-d1034438329e
description: Поиск сведений о MarkAsJunkной операции EWS.
ms.openlocfilehash: b9d79e6fbec87ce41030b4981f3c16f2f9ce9507
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834353"
---
# <a name="markasjunk-operation"></a><span data-ttu-id="2ce34-103">Операция MarkAsJunk</span><span class="sxs-lookup"><span data-stu-id="2ce34-103">MarkAsJunk operation</span></span>

<span data-ttu-id="2ce34-104">Поиск сведений о **MarkAsJunkной** операции EWS.</span><span class="sxs-lookup"><span data-stu-id="2ce34-104">Find information about the **MarkAsJunk** EWS operation.</span></span> 
  
<span data-ttu-id="2ce34-105">Операция **MarkAsJunk** добавляет и удаляет пользователей из списка заблокированных сообщений электронной почты и перемещает сообщения электронной почты в папку "Нежелательная почта".</span><span class="sxs-lookup"><span data-stu-id="2ce34-105">The **MarkAsJunk** operation adds and removes users from the blocked email list and moves email messages to the Junk Email folder.</span></span> 
  
<span data-ttu-id="2ce34-106">Эта операция появилась в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="2ce34-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-markasjunk-operation"></a><span data-ttu-id="2ce34-107">Использование операции MarkAsJunk</span><span class="sxs-lookup"><span data-stu-id="2ce34-107">Using the MarkAsJunk operation</span></span>

<span data-ttu-id="2ce34-108">Операция **MarkAsJunk** содержит два логических параметра, указывающие, следует ли добавить отправителя электронной почты в список заблокированных отправителей и следует ли переместить целевое сообщение электронной почты в папку нежелательной почты по умолчанию или папку "Входящие".</span><span class="sxs-lookup"><span data-stu-id="2ce34-108">The **MarkAsJunk** operation contains two Boolean options to indicate whether an email sender should be added to the blocked sender list and whether the target email message should be moved to the default Junk Email folder or the Inbox folder.</span></span> <span data-ttu-id="2ce34-109">Действия определяются значениями атрибутов **MoveItem** и **нежелательной почты** .</span><span class="sxs-lookup"><span data-stu-id="2ce34-109">The actions are determined by the values of the **IsJunk** and **MoveItem** attributes.</span></span> <span data-ttu-id="2ce34-110">Ниже приведены возможные действия, основанные на комбинациях значений для атрибутов **MoveItem** и **нежелательной почты** :</span><span class="sxs-lookup"><span data-stu-id="2ce34-110">The following are the possible actions based on the value combinations for the **IsJunk** and **MoveItem** attributes:</span></span> 
  
- <span data-ttu-id="2ce34-111">Если атрибуту InAttribute присвоено значение **true**, **а атрибуту** **MoveItem** присвоено значение **true**, отправитель целевого сообщения электронной почты добавляется в список заблокированных отправителей и сообщение электронной почты перемещается в папку "Нежелательная дмаил".</span><span class="sxs-lookup"><span data-stu-id="2ce34-111">If the **IsJunk** attribute is set to **true**, and the **MoveItem** attribute is set to **true**, the sender of the target email message is added to the blocked sender list and the email message is moved to the Junk Dmail folder.</span></span>
    
- <span data-ttu-id="2ce34-112">Если атрибуту InAttribute присвоено значение **true**, **а атрибуту** **MoveItem** присвоено значение **false**, отправитель целевого сообщения электронной почты добавляется в список заблокированных отправителей, а сообщение электронной почты не перемещается из нее.</span><span class="sxs-lookup"><span data-stu-id="2ce34-112">If the **IsJunk** attribute is set to **true**, and the **MoveItem** attribute is set to **false**, the sender of the target email message is added to the blocked sender list and the email message is not moved from the folder.</span></span>
    
- <span data-ttu-id="2ce34-113">Если атрибуту InAttribute присвоено значение **false**, **а атрибуту** **MoveItem** присвоено значение **true**, то отправитель целевого сообщения электронной почты удален из списка заблокированных отправителей, а сообщение электронной почты перемещается в папку "Входящие".</span><span class="sxs-lookup"><span data-stu-id="2ce34-113">If the **IsJunk** attribute is set to **false**, and the **MoveItem** attribute is set to **true**, the sender of the target email messageis removed from the blocked sender list and the email message is moved to the Inbox folder.</span></span>
    
- <span data-ttu-id="2ce34-114">Если атрибуту InAttribute присвоено значение **false**, **а атрибуту** **MoveItem** присвоено значение **false**, то отправитель целевого сообщения электронной почты удаляется из списка заблокированных отправителей, а сообщение электронной почты не перемещается из папки.</span><span class="sxs-lookup"><span data-stu-id="2ce34-114">If the **IsJunk** attribute is set to **false**, and the **MoveItem** attribute is set to **false**, the sender of the target email message is removed from the blocked sender list and the email message is not moved from the folder.</span></span>
    
> [!IMPORTANT]
> <span data-ttu-id="2ce34-115">Содержимое списка заблокированных отправителей не обнаруживается в EWS.</span><span class="sxs-lookup"><span data-stu-id="2ce34-115">The contents of the blocked sender list are not discoverable from EWS.</span></span> <span data-ttu-id="2ce34-116">Если отправитель добавляется в список заблокированных отправителей, необходимо сохранить копию сообщения электронной почты, отправленного заблокированным отправителем, чтобы разблокировать отправителя в будущем.</span><span class="sxs-lookup"><span data-stu-id="2ce34-116">If a sender is added to the blocked sender list, you need to keep a copy of an email message sent by the blocked sender to unblock the sender in the future.</span></span> 
  
### <a name="markasjunk-operation-soap-headers"></a><span data-ttu-id="2ce34-117">Заголовки SOAP операции MarkAsJunk</span><span class="sxs-lookup"><span data-stu-id="2ce34-117">MarkAsJunk operation SOAP headers</span></span>

<span data-ttu-id="2ce34-118">Операция **MarkAsJunk** может использовать заголовки SOAP, указанные в приведенной ниже таблице.</span><span class="sxs-lookup"><span data-stu-id="2ce34-118">The **MarkAsJunk** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="2ce34-119">**Имя заголовка**</span><span class="sxs-lookup"><span data-stu-id="2ce34-119">**Header name**</span></span>|<span data-ttu-id="2ce34-120">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="2ce34-120">**Element**</span></span>|<span data-ttu-id="2ce34-121">**Описание**</span><span class="sxs-lookup"><span data-stu-id="2ce34-121">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="2ce34-122">**Олицетворение**</span><span class="sxs-lookup"><span data-stu-id="2ce34-122">**Impersonation**</span></span> <br/> |[<span data-ttu-id="2ce34-123">ексчанжеимперсонатион</span><span class="sxs-lookup"><span data-stu-id="2ce34-123">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="2ce34-124">Идентифицирует пользователя, который олицетворяет клиентское приложение.</span><span class="sxs-lookup"><span data-stu-id="2ce34-124">Identifies the user whom the client application is impersonating.</span></span> <span data-ttu-id="2ce34-125">Этот заголовок является применимым для запроса.</span><span class="sxs-lookup"><span data-stu-id="2ce34-125">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="2ce34-126">**маилбокскултуре**</span><span class="sxs-lookup"><span data-stu-id="2ce34-126">**MailboxCulture**</span></span> <br/> |[<span data-ttu-id="2ce34-127">маилбокскултуре</span><span class="sxs-lookup"><span data-stu-id="2ce34-127">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="2ce34-128">Определяет язык и региональные параметры, определенные в документе RFC 3066 "Теги для идентификации языков", которые будут использоваться для доступа к почтовому ящику.</span><span class="sxs-lookup"><span data-stu-id="2ce34-128">Identifies the culture, as defined in RFC 3066, "Tags for the Identification of Languages", to be used to access the mailbox.</span></span> <span data-ttu-id="2ce34-129">Этот заголовок является применимым для запроса.</span><span class="sxs-lookup"><span data-stu-id="2ce34-129">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="2ce34-130">**рекуестверсион**</span><span class="sxs-lookup"><span data-stu-id="2ce34-130">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="2ce34-131">рекуестсерверверсион</span><span class="sxs-lookup"><span data-stu-id="2ce34-131">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="2ce34-132">Определяет версию схемы для запроса операции.</span><span class="sxs-lookup"><span data-stu-id="2ce34-132">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="2ce34-133">Этот заголовок является применимым для запроса.</span><span class="sxs-lookup"><span data-stu-id="2ce34-133">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="2ce34-134">**серверверсион**</span><span class="sxs-lookup"><span data-stu-id="2ce34-134">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="2ce34-135">серверверсионинфо</span><span class="sxs-lookup"><span data-stu-id="2ce34-135">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="2ce34-136">Определяет версию сервера, который ответил на запрос.</span><span class="sxs-lookup"><span data-stu-id="2ce34-136">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="2ce34-137">Этот заголовок является применимым для отклика.</span><span class="sxs-lookup"><span data-stu-id="2ce34-137">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="markasjunk-operation-request-example-add-a-sender-to-the-blocked-sender-list"></a><span data-ttu-id="2ce34-138">Пример запроса операции MarkAsJunk: Добавление отправителя в список заблокированных отправителей</span><span class="sxs-lookup"><span data-stu-id="2ce34-138">MarkAsJunk operation request example: Add a sender to the blocked sender list</span></span>

<span data-ttu-id="2ce34-139">В следующем примере запроса операции **MarkAsJunk** показано, как добавить отправителя электронного письма в список заблокированных отправителей и переместить сообщение в папку нежелательной почты.</span><span class="sxs-lookup"><span data-stu-id="2ce34-139">The following example of a **MarkAsJunk** operation request shows how to add the sender of an email to the blocked sender list and move the email to the junk mail folder.</span></span> <span data-ttu-id="2ce34-140">Операция **MarkAsJunk** принимает уникальный идентификатор электронного сообщения, чтобы определить адрес электронной почты, который используется для ссылки на отправителя, добавляемого в список заблокированных отправителей.</span><span class="sxs-lookup"><span data-stu-id="2ce34-140">The **MarkAsJunk** operation accepts the unique email message identifier to identify the email that is used to reference the sender that is added to the blocked sender list.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="2ce34-141">Все идентификаторы элементов и изменения ключей в этой статье были сокращены, чтобы сохранить удобочитаемость.</span><span class="sxs-lookup"><span data-stu-id="2ce34-141">All item identifiers and change keys in this article have been shortened to preserve readability.</span></span> 
  
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

<span data-ttu-id="2ce34-142">Текст SOAP Request содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="2ce34-142">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="2ce34-143">MarkAsJunk</span><span class="sxs-lookup"><span data-stu-id="2ce34-143">MarkAsJunk</span></span>](markasjunk.md)
    
- [<span data-ttu-id="2ce34-144">итемидс</span><span class="sxs-lookup"><span data-stu-id="2ce34-144">ItemIds</span></span>](itemids.md)
    
- [<span data-ttu-id="2ce34-145">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="2ce34-145">ItemId</span></span>](itemid.md)
    
## <a name="successful-markasjunk-operation-response"></a><span data-ttu-id="2ce34-146">Успешный отклик операции MarkAsJunk</span><span class="sxs-lookup"><span data-stu-id="2ce34-146">Successful MarkAsJunk operation response</span></span>

<span data-ttu-id="2ce34-147">В следующем примере показан успешный ответ на запрос операции **MarkAsJunk** для добавления отправителя в список заблокированных отправителей и перемещения сообщения электронной почты в папку нежелательной почты.</span><span class="sxs-lookup"><span data-stu-id="2ce34-147">The following example shows a successful response to a **MarkAsJunk** operation request to add a sender to the blocked sender list and move the email message to the Junk Email folder.</span></span> 
  
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

<span data-ttu-id="2ce34-148">Тело SOAP отклика содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="2ce34-148">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="2ce34-149">маркасжункреспонсе</span><span class="sxs-lookup"><span data-stu-id="2ce34-149">MarkAsJunkResponse</span></span>](markasjunkresponse.md)
    
- [<span data-ttu-id="2ce34-150">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="2ce34-150">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="2ce34-151">маркасжункреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="2ce34-151">MarkAsJunkResponseMessage</span></span>](markasjunkresponsemessage.md)
    
- [<span data-ttu-id="2ce34-152">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="2ce34-152">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="2ce34-153">моведитемид</span><span class="sxs-lookup"><span data-stu-id="2ce34-153">MovedItemId</span></span>](moveditemid.md)
    
## <a name="markasjunk-operation-request-example-remove-a-sender-from-the-blocked-sender-list"></a><span data-ttu-id="2ce34-154">Пример запроса операции MarkAsJunk: Удаление отправителя из списка заблокированных отправителей</span><span class="sxs-lookup"><span data-stu-id="2ce34-154">MarkAsJunk operation request example: Remove a sender from the blocked sender list</span></span>

<span data-ttu-id="2ce34-155">В приведенном ниже примере запроса операции **MarkAsJunk** показано, как удалить отправителя сообщения электронной почты из списка заблокированных отправителей и переместить сообщение в папку "Входящие".</span><span class="sxs-lookup"><span data-stu-id="2ce34-155">The following example of a **MarkAsJunk** operation request shows how to remove the sender of an email message from the blocked sender list and move the email message to the Inbox folder.</span></span> <span data-ttu-id="2ce34-156">Чтобы удалить отправителя из списка заблокированных отправителей, необходимо оставить сообщение электронной почты, отправленное заблокированным отправителем.</span><span class="sxs-lookup"><span data-stu-id="2ce34-156">You need to keep an email message sent by the blocked sender to remove the sender from the blocked sender list.</span></span> <span data-ttu-id="2ce34-157">Адрес электронной почты отправителя связан с сообщениями электронной почты, отправленными отправителями.</span><span class="sxs-lookup"><span data-stu-id="2ce34-157">The sender's email address is associated with email messages that have been sent by the sender.</span></span> <span data-ttu-id="2ce34-158">Удаление отправителя из списка заблокированных отправителей не будет успешным, если справочное сообщение электронной почты больше не существует в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="2ce34-158">Removing a sender from the blocked sender list will not succeed if the reference email message no longer exists in the user's mailbox.</span></span> <span data-ttu-id="2ce34-159">Идентификатор элемента, используемый для связи с сообщением электронной почты с отправителями, должен быть связан с элементом, который существует в почтовом ящике Exchange.</span><span class="sxs-lookup"><span data-stu-id="2ce34-159">The item identifier used to associate an email message with its sender must be associated with an item that exists in the Exchange mailbox.</span></span> <span data-ttu-id="2ce34-160">Рекомендуется создать скрытую папку для хранения элементов, отправленных ранее заблокированными отправителями, чтобы отправители можно было разблокировать из клиентского приложения.</span><span class="sxs-lookup"><span data-stu-id="2ce34-160">We recommend that you create a hidden folder to store items sent by previously blocked senders so that the senders can be unblocked from the client application.</span></span> <span data-ttu-id="2ce34-161">В случае, если элемент удален из почтового ящика Exchange, администратору необходимо использовать консоль управления Exchange для доступа к списку заблокированных отправителей, чтобы удалить отправителя из списка.</span><span class="sxs-lookup"><span data-stu-id="2ce34-161">In the event that an item has been removed from the Exchange mailbox, an administrator has to use the Exchange Management Console to access the blocked sender list to remove a sender from the list.</span></span> <span data-ttu-id="2ce34-162">Сведения о том, как разблокировать пользователя с помощью консоли управления Exchange, можно узнать в статье [Настройка параметров надежных отправителей и заблокированных отправителей в Office 365](http://support.microsoft.com/kb/2545137).</span><span class="sxs-lookup"><span data-stu-id="2ce34-162">For information about how to unblock a user by using the Exchange Management Console, see [How to configure the safe senders and blocked senders settings in Office 365](http://support.microsoft.com/kb/2545137).</span></span>
  
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

<span data-ttu-id="2ce34-163">Успешный ответ на удаление отправителя из списка заблокированных отправителей совпадает с ответом на Добавление отправителя в список заблокированных отправителей.</span><span class="sxs-lookup"><span data-stu-id="2ce34-163">A successful response for removing a sender from the blocked sender list is the same as the response for adding a sender to the blocked sender list.</span></span>
  
<span data-ttu-id="2ce34-164">Текст SOAP Request содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="2ce34-164">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="2ce34-165">MarkAsJunk</span><span class="sxs-lookup"><span data-stu-id="2ce34-165">MarkAsJunk</span></span>](markasjunk.md)
    
- [<span data-ttu-id="2ce34-166">итемидс</span><span class="sxs-lookup"><span data-stu-id="2ce34-166">ItemIds</span></span>](itemids.md)
    
- [<span data-ttu-id="2ce34-167">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="2ce34-167">ItemId</span></span>](itemid.md)
    
## <a name="markasjunk-operation-error-response"></a><span data-ttu-id="2ce34-168">Ответ об ошибке операции MarkAsJunk</span><span class="sxs-lookup"><span data-stu-id="2ce34-168">MarkAsJunk operation error response</span></span>

<span data-ttu-id="2ce34-169">В следующем примере показан ответ об ошибке для запроса операции **MarkAsJunk** .</span><span class="sxs-lookup"><span data-stu-id="2ce34-169">The following example shows an error response to a **MarkAsJunk** operation request.</span></span> <span data-ttu-id="2ce34-170">Это ответ на запрос на добавление или удаление отправителя из списка заблокированных отправителей, если сообщение электронной почты, заданное идентификатором элемента, больше не существует в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="2ce34-170">This is a response to a request to add or remove a sender from the blocked sender list when the email message specified by the item identifier no longer exists in the mailbox.</span></span> 
  
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

<span data-ttu-id="2ce34-171">Основной текст сообщения об ошибке SOAP содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="2ce34-171">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="2ce34-172">маркасжункреспонсе</span><span class="sxs-lookup"><span data-stu-id="2ce34-172">MarkAsJunkResponse</span></span>](markasjunkresponse.md)
    
- [<span data-ttu-id="2ce34-173">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="2ce34-173">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="2ce34-174">маркасжункреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="2ce34-174">MarkAsJunkResponseMessage</span></span>](markasjunkresponsemessage.md)
    
- [<span data-ttu-id="2ce34-175">мессажетекст</span><span class="sxs-lookup"><span data-stu-id="2ce34-175">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="2ce34-176">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="2ce34-176">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="2ce34-177">дескриптивелинккэй</span><span class="sxs-lookup"><span data-stu-id="2ce34-177">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
## <a name="see-also"></a><span data-ttu-id="2ce34-178">См. также</span><span class="sxs-lookup"><span data-stu-id="2ce34-178">See also</span></span>

- [<span data-ttu-id="2ce34-179">Операции EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="2ce34-179">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
    
- <span data-ttu-id="2ce34-180">[Операция GetItem](getitem-operation.md) Операция GetItem</span><span class="sxs-lookup"><span data-stu-id="2ce34-180">[GetItem operation](getitem-operation.md) GetItem operation</span></span> 
    
- [<span data-ttu-id="2ce34-181">Операция FindItem</span><span class="sxs-lookup"><span data-stu-id="2ce34-181">FindItem operation</span></span>](finditem-operation.md)
    

