---
title: Операция MarkAllItemsAsRead
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: ea5b1cb6-6998-46fb-a99c-a6d3da77591f
description: Найдите сведения о веб-служб Exchange MarkAllItemsAsRead операции.
ms.openlocfilehash: 995a6219f0a3b41bddb0d65c875d981322e1ce78
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19834354"
---
# <a name="markallitemsasread-operation"></a><span data-ttu-id="a9435-103">Операция MarkAllItemsAsRead</span><span class="sxs-lookup"><span data-stu-id="a9435-103">MarkAllItemsAsRead operation</span></span>

<span data-ttu-id="a9435-104">Найдите сведения о **MarkAllItemsAsRead** операции веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="a9435-104">Find information about the **MarkAllItemsAsRead** EWS operation.</span></span> 
  
<span data-ttu-id="a9435-105">Операция **MarkAllItemsAsRead** задает свойство [IsRead](isread.md) на все элементы в одной или нескольких папок, чтобы указать, что все элементы являются чтения или непрочитанные сообщения.</span><span class="sxs-lookup"><span data-stu-id="a9435-105">The **MarkAllItemsAsRead** operation sets the [IsRead](isread.md) property on all items, in one or more folders, to indicate that all items are either read or unread.</span></span> 
  
<span data-ttu-id="a9435-106">Эта операция появилась в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="a9435-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-markallitemsasread-operation"></a><span data-ttu-id="a9435-107">С помощью операции MarkAllItemsAsRead</span><span class="sxs-lookup"><span data-stu-id="a9435-107">Using the MarkAllItemsAsRead operation</span></span>

<span data-ttu-id="a9435-108">Операция **MarkAllItemsAsRead** можно задать свойство [IsRead](isread.md) для всех элементов в папках, определяемую средством идентификатор папки веб-служб Exchange (EWS) или имя папки Exchange по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="a9435-108">The **MarkAllItemsAsRead** operation can set the [IsRead](isread.md) property on all items in folders identified by either the Exchange Web Services (EWS) folder identifier or the default Exchange folder name.</span></span> <span data-ttu-id="a9435-109">Операция **MarkAllItemsAsRead** также можно отключить отправку прочтении для элементов, помеченных как прочтенные.</span><span class="sxs-lookup"><span data-stu-id="a9435-109">The **MarkAllItemsAsRead** operation can also suppress the sending of read receipts for items marked as read.</span></span> 
  
### <a name="markallitemsasread-operation-soap-headers"></a><span data-ttu-id="a9435-110">Заголовки SOAP MarkAllItemsAsRead операции</span><span class="sxs-lookup"><span data-stu-id="a9435-110">MarkAllItemsAsRead operation SOAP headers</span></span>

<span data-ttu-id="a9435-111">Операция **MarkAllItemsAsRead** можно использовать заголовки SOAP, которые перечислены в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="a9435-111">The **MarkAllItemsAsRead** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="a9435-112">**Имя заголовка**</span><span class="sxs-lookup"><span data-stu-id="a9435-112">**Header name**</span></span>|<span data-ttu-id="a9435-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="a9435-113">**Element**</span></span>|<span data-ttu-id="a9435-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="a9435-114">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="a9435-115">**Олицетворение**</span><span class="sxs-lookup"><span data-stu-id="a9435-115">**Impersonation**</span></span> <br/> |[<span data-ttu-id="a9435-116">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="a9435-116">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="a9435-117">Идентифицирует пользователя, которого олицетворения в клиентском приложении.</span><span class="sxs-lookup"><span data-stu-id="a9435-117">Identifies the user whom the client application is impersonating.</span></span> <span data-ttu-id="a9435-118">Этот заголовок можно применять к запросу.</span><span class="sxs-lookup"><span data-stu-id="a9435-118">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="a9435-119">**MailboxCulture**</span><span class="sxs-lookup"><span data-stu-id="a9435-119">**MailboxCulture**</span></span> <br/> |[<span data-ttu-id="a9435-120">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="a9435-120">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="a9435-121">Определяет язык и региональные параметры, как определено в RFC 3066, «Теги для идентификации языков», который будет использоваться для доступа к почтовому ящику.</span><span class="sxs-lookup"><span data-stu-id="a9435-121">Identifies the culture, as defined in RFC 3066, "Tags for the Identification of Languages", to be used to access the mailbox.</span></span> <span data-ttu-id="a9435-122">Этот заголовок можно применять к запросу.</span><span class="sxs-lookup"><span data-stu-id="a9435-122">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="a9435-123">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="a9435-123">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="a9435-124">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="a9435-124">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="a9435-125">Определяет версию схемы для операции запроса.</span><span class="sxs-lookup"><span data-stu-id="a9435-125">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="a9435-126">Этот заголовок можно применять к запросу.</span><span class="sxs-lookup"><span data-stu-id="a9435-126">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="a9435-127">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="a9435-127">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="a9435-128">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="a9435-128">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="a9435-129">Определяет версию сервера, ответившего на запрос.</span><span class="sxs-lookup"><span data-stu-id="a9435-129">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="a9435-130">Этот заголовок можно применять, чтобы получить ответ.</span><span class="sxs-lookup"><span data-stu-id="a9435-130">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="markallitemsasread-operation-request-example-mark-all-items-in-a-folder-as-read"></a><span data-ttu-id="a9435-131">Пример запроса MarkAllItemsAsRead операции: Пометка всех элементов в папке как прочтенные</span><span class="sxs-lookup"><span data-stu-id="a9435-131">MarkAllItemsAsRead operation request example: Mark all items in a folder as read</span></span>

<span data-ttu-id="a9435-132">В следующем примере запрос операции **MarkAllItemsAsRead** показано, как задать свойство [IsRead](isread.md) , которая также называется чтения флаг, значение **true** для всех элементов в папке.</span><span class="sxs-lookup"><span data-stu-id="a9435-132">The following example of a **MarkAllItemsAsRead** operation request shows how to set the [IsRead](isread.md) property, which is also called the read flag, to **true** on all items in a folder.</span></span> <span data-ttu-id="a9435-133">В этом примере также показано, что чтения, уведомления не отправляются в ответ на все запросы на уведомление.</span><span class="sxs-lookup"><span data-stu-id="a9435-133">This example also shows that read receipts are not sent in response to any read receipt requests.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="a9435-134">Все идентификаторы элементов и ключей изменения в этой статье URL были сокращены, чтобы сохранить удобочитаемость.</span><span class="sxs-lookup"><span data-stu-id="a9435-134">All item identifiers and change keys in this article have been shortened to preserve readability.</span></span> <span data-ttu-id="a9435-135">Изменение ключей не являются обязательными для этой операции.</span><span class="sxs-lookup"><span data-stu-id="a9435-135">Change keys are not required for this operation.</span></span> 
  
```XML
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013" />
   </soap:Header>
   <soap:Body>
      <m:MarkAllItemsAsRead>
         <m:ReadFlag>true</m:ReadFlag>
         <m:SuppressReadReceipts>true</m:SuppressReadReceipts>
         <m:FolderIds>
            <t:FolderId Id="AAMkADEzOTExYZRAAA=" 
                        ChangeKey="AQAAAAA3vA==" />
         </m:FolderIds>
      </m:MarkAllItemsAsRead>
   </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="a9435-136">Запрос SOAP body содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="a9435-136">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="a9435-137">MarkAllItemsAsRead</span><span class="sxs-lookup"><span data-stu-id="a9435-137">MarkAllItemsAsRead</span></span>](markallitemsasread.md)
    
- [<span data-ttu-id="a9435-138">ReadFlag</span><span class="sxs-lookup"><span data-stu-id="a9435-138">ReadFlag</span></span>](readflag.md)
    
- [<span data-ttu-id="a9435-139">SuppressReadReceipts</span><span class="sxs-lookup"><span data-stu-id="a9435-139">SuppressReadReceipts</span></span>](suppressreadreceipts.md)
    
- [<span data-ttu-id="a9435-140">FolderIds</span><span class="sxs-lookup"><span data-stu-id="a9435-140">FolderIds</span></span>](folderids.md)
    
- [<span data-ttu-id="a9435-141">FolderId</span><span class="sxs-lookup"><span data-stu-id="a9435-141">FolderId</span></span>](folderid.md)
    
## <a name="successful-markallitemsasread-operation-response"></a><span data-ttu-id="a9435-142">Успешные операции ответа MarkAllItemsAsRead</span><span class="sxs-lookup"><span data-stu-id="a9435-142">Successful MarkAllItemsAsRead operation response</span></span>

<span data-ttu-id="a9435-143">В следующем примере показано успешного ответа на запрос операции **MarkAllItemsAsRead** , чтобы пометить все элементы в папке как прочтенные.</span><span class="sxs-lookup"><span data-stu-id="a9435-143">The following example shows a successful response to a **MarkAllItemsAsRead** operation request to mark all items in a folder as read.</span></span> 
  
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
      <m:MarkAllItemsAsReadResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                                    xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
         <m:ResponseMessages>
            <m:MarkAllItemsAsReadResponseMessage ResponseClass="Success">
               <m:ResponseCode>NoError</m:ResponseCode>
            </m:MarkAllItemsAsReadResponseMessage>
         </m:ResponseMessages>
      </m:MarkAllItemsAsReadResponse>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="a9435-144">Ответ SOAP body содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="a9435-144">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="a9435-145">MarkAllItemsAsReadResponse</span><span class="sxs-lookup"><span data-stu-id="a9435-145">MarkAllItemsAsReadResponse</span></span>](markallitemsasreadresponse.md)
    
- [<span data-ttu-id="a9435-146">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="a9435-146">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="a9435-147">MarkAllItemsAsReadResponseMessage</span><span class="sxs-lookup"><span data-stu-id="a9435-147">MarkAllItemsAsReadResponseMessage</span></span>](markallitemsasreadresponsemessage.md)
    
- [<span data-ttu-id="a9435-148">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="a9435-148">ResponseCode</span></span>](responsecode.md)
    
## <a name="markallitemsasread-operation-request-example-mark-all-items-in-a-folder-as-unread"></a><span data-ttu-id="a9435-149">Пример запроса MarkAllItemsAsRead операции: Пометка всех элементов в папке как непрочтенные</span><span class="sxs-lookup"><span data-stu-id="a9435-149">MarkAllItemsAsRead operation request example: Mark all items in a folder as unread</span></span>

<span data-ttu-id="a9435-150">В следующем примере запрос операции **MarkAllItemsAsRead** показано, как для свойства [IsRead](isread.md) значение **false** для всех элементов в папке.</span><span class="sxs-lookup"><span data-stu-id="a9435-150">The following example of a **MarkAllItemsAsRead** operation request shows how to set the [IsRead](isread.md) property to **false** on all items in a folder.</span></span> <span data-ttu-id="a9435-151">В этом примере также показано, что чтения, уведомления не отправляются в ответ на все запросы на уведомление.</span><span class="sxs-lookup"><span data-stu-id="a9435-151">This example also shows that read receipts are not sent in response to any read receipt requests.</span></span> 
  
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
      <m:MarkAllItemsAsRead>
         <m:ReadFlag>false</m:ReadFlag>
         <m:SuppressReadReceipts>true</m:SuppressReadReceipts>
         <m:FolderIds>
            <t:FolderId Id="AAMkADEzOTExYZRAAA=" 
                        ChangeKey="AQAAAAA3vA==" />
         </m:FolderIds>
      </m:MarkAllItemsAsRead>
   </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="a9435-152">Успешного ответа на запрос, чтобы пометить все элементы как прочитанные — это то же, что ответ на запрос, чтобы пометить все элементы как непрочтенные.</span><span class="sxs-lookup"><span data-stu-id="a9435-152">A successful response to a request to mark all items as read is the same as the response to a request to mark all items as unread.</span></span>
  
<span data-ttu-id="a9435-153">Запрос SOAP body содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="a9435-153">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="a9435-154">MarkAllItemsAsRead</span><span class="sxs-lookup"><span data-stu-id="a9435-154">MarkAllItemsAsRead</span></span>](markallitemsasread.md)
    
- [<span data-ttu-id="a9435-155">ReadFlag</span><span class="sxs-lookup"><span data-stu-id="a9435-155">ReadFlag</span></span>](readflag.md)
    
- [<span data-ttu-id="a9435-156">SuppressReadReceipts</span><span class="sxs-lookup"><span data-stu-id="a9435-156">SuppressReadReceipts</span></span>](suppressreadreceipts.md)
    
- [<span data-ttu-id="a9435-157">FolderIds</span><span class="sxs-lookup"><span data-stu-id="a9435-157">FolderIds</span></span>](folderids.md)
    
- [<span data-ttu-id="a9435-158">FolderId</span><span class="sxs-lookup"><span data-stu-id="a9435-158">FolderId</span></span>](folderid.md)
    
## <a name="markallitemsasread-operation-error-response"></a><span data-ttu-id="a9435-159">Ошибка операции MarkAllItemsAsRead ответа</span><span class="sxs-lookup"><span data-stu-id="a9435-159">MarkAllItemsAsRead operation error response</span></span>

<span data-ttu-id="a9435-160">В следующем примере показано возврату ошибки на запрос операции **MarkAllItemsAsRead** Пометка всех элементов в папке прочитан или не прочитан при папка не существует в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="a9435-160">The following example shows an error response to a **MarkAllItemsAsRead** operation request to mark all items in a folder as read or unread when the folder does not exist in the mailbox.</span></span> 
  
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
      <m:MarkAllItemsAsReadResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                                    xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
         <m:ResponseMessages>
            <m:MarkAllItemsAsReadResponseMessage ResponseClass="Error">
               <m:MessageText>The specified object was not found in the store.</m:MessageText>
               <m:ResponseCode>ErrorItemNotFound</m:ResponseCode>
               <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
            </m:MarkAllItemsAsReadResponseMessage>
         </m:ResponseMessages>
      </m:MarkAllItemsAsReadResponse>
   </s:Body>
</s:Envelope>

```

<span data-ttu-id="a9435-161">Ошибка ответ SOAP body содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="a9435-161">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="a9435-162">MarkAllItemsAsReadResponse</span><span class="sxs-lookup"><span data-stu-id="a9435-162">MarkAllItemsAsReadResponse</span></span>](markallitemsasreadresponse.md)
    
- [<span data-ttu-id="a9435-163">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="a9435-163">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="a9435-164">MarkAllItemsAsReadResponseMessage</span><span class="sxs-lookup"><span data-stu-id="a9435-164">MarkAllItemsAsReadResponseMessage</span></span>](markallitemsasreadresponsemessage.md)
    
- [<span data-ttu-id="a9435-165">MessageText</span><span class="sxs-lookup"><span data-stu-id="a9435-165">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="a9435-166">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="a9435-166">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="a9435-167">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="a9435-167">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
## <a name="see-also"></a><span data-ttu-id="a9435-168">См. также</span><span class="sxs-lookup"><span data-stu-id="a9435-168">See also</span></span>

- [<span data-ttu-id="a9435-169">Операции EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="a9435-169">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
    
- [<span data-ttu-id="a9435-170">FindFolder Operation</span><span class="sxs-lookup"><span data-stu-id="a9435-170">FindFolder operation</span></span>](findfolder-operation.md)
    

