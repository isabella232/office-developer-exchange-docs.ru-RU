---
title: Операция ArchiveItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 1af216b3-13ea-498e-b4fc-23513755d731
description: Найдите сведения о веб-служб Exchange ArchiveItem операции.
ms.openlocfilehash: 954943acefef8da61e92de5f8857ca023ca4fc9f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761491"
---
# <a name="archiveitem-operation"></a><span data-ttu-id="ce1e0-103">Операция ArchiveItem</span><span class="sxs-lookup"><span data-stu-id="ce1e0-103">ArchiveItem operation</span></span>

<span data-ttu-id="ce1e0-104">Найдите сведения о **ArchiveItem** операции веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="ce1e0-104">Find information about the **ArchiveItem** EWS operation.</span></span> 
  
<span data-ttu-id="ce1e0-105">Операция **ArchiveItem** Перемещение элемента в архивный почтовый ящик пользователя почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="ce1e0-105">The **ArchiveItem** operation moves an item into the mailbox user's archive mailbox.</span></span> 
  
<span data-ttu-id="ce1e0-106">Эта операция появилась в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="ce1e0-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-archiveitem-operation"></a><span data-ttu-id="ce1e0-107">С помощью операции ArchiveItem</span><span class="sxs-lookup"><span data-stu-id="ce1e0-107">Using the ArchiveItem operation</span></span>

<span data-ttu-id="ce1e0-108">Операция **ArchiveItem** принимает два аргумента в запросе, определите, какие элементы для перемещения архивного почтового ящика и конечной папки для этих элементов.</span><span class="sxs-lookup"><span data-stu-id="ce1e0-108">The **ArchiveItem** operation takes two arguments in the request that identify the items to move to the archive mailbox and the destination folder for those items.</span></span> <span data-ttu-id="ce1e0-109">Архивный почтовый ящик должна быть включена в порядке, для успешного выполнения этой операции.</span><span class="sxs-lookup"><span data-stu-id="ce1e0-109">An archive mailbox must be enabled in order for this operation to work.</span></span> <span data-ttu-id="ce1e0-110">Сведения о включении архивного почтового ящика можно [Управление архивами на месте](http://technet.microsoft.com/en-us/library/jj651146.aspx).</span><span class="sxs-lookup"><span data-stu-id="ce1e0-110">For information about how to enable an archive mailbox, see [Manage In-Place Archives](http://technet.microsoft.com/en-us/library/jj651146.aspx).</span></span>
  
### <a name="archiveitem-operation-soap-headers"></a><span data-ttu-id="ce1e0-111">Заголовки SOAP ArchiveItem операции</span><span class="sxs-lookup"><span data-stu-id="ce1e0-111">ArchiveItem operation SOAP headers</span></span>

<span data-ttu-id="ce1e0-112">Операция **ArchiveItem** можно использовать заголовки SOAP, которые перечислены в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="ce1e0-112">The **ArchiveItem** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="ce1e0-113">**Имя заголовка**</span><span class="sxs-lookup"><span data-stu-id="ce1e0-113">**Header name**</span></span>|<span data-ttu-id="ce1e0-114">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="ce1e0-114">**Element**</span></span>|<span data-ttu-id="ce1e0-115">**Описание**</span><span class="sxs-lookup"><span data-stu-id="ce1e0-115">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="ce1e0-116">**Олицетворение**</span><span class="sxs-lookup"><span data-stu-id="ce1e0-116">**Impersonation**</span></span> <br/> |[<span data-ttu-id="ce1e0-117">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="ce1e0-117">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="ce1e0-118">Идентифицирует пользователя, которого олицетворения в клиентском приложении.</span><span class="sxs-lookup"><span data-stu-id="ce1e0-118">Identifies the user whom the client application is impersonating.</span></span> <span data-ttu-id="ce1e0-119">Этот заголовок можно применять к запросу.</span><span class="sxs-lookup"><span data-stu-id="ce1e0-119">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="ce1e0-120">**MailboxCulture**</span><span class="sxs-lookup"><span data-stu-id="ce1e0-120">**MailboxCulture**</span></span> <br/> |[<span data-ttu-id="ce1e0-121">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="ce1e0-121">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="ce1e0-122">Определяет язык и региональные параметры, как определено в RFC 3066, **теги для идентификации языков**, которые будут использоваться для доступа к почтовому ящику.</span><span class="sxs-lookup"><span data-stu-id="ce1e0-122">Identifies the culture, as defined in RFC 3066, **Tags for the Identification of Languages**, to be used to access the mailbox.</span></span> <span data-ttu-id="ce1e0-123">Этот заголовок можно применять к запросу.</span><span class="sxs-lookup"><span data-stu-id="ce1e0-123">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="ce1e0-124">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="ce1e0-124">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="ce1e0-125">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="ce1e0-125">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="ce1e0-126">Определяет версию схемы для операции запроса.</span><span class="sxs-lookup"><span data-stu-id="ce1e0-126">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="ce1e0-127">Этот заголовок можно применять к запросу.</span><span class="sxs-lookup"><span data-stu-id="ce1e0-127">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="ce1e0-128">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="ce1e0-128">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="ce1e0-129">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="ce1e0-129">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="ce1e0-130">Определяет версию сервера, ответившего на запрос.</span><span class="sxs-lookup"><span data-stu-id="ce1e0-130">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="ce1e0-131">Этот заголовок можно применять, чтобы получить ответ.</span><span class="sxs-lookup"><span data-stu-id="ce1e0-131">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="archiveitem-operation-request-example-move-an-item-to-the-archive-inbox-folder"></a><span data-ttu-id="ce1e0-132">Пример запроса ArchiveItem операции: перемещение элемента в папке "Входящие" архив</span><span class="sxs-lookup"><span data-stu-id="ce1e0-132">ArchiveItem operation request example: Move an item to the archive inbox folder</span></span>

<span data-ttu-id="ce1e0-133">В следующем примере запрос операции **ArchiveItem** показано, как перемещение элемента в архив папки "Входящие".</span><span class="sxs-lookup"><span data-stu-id="ce1e0-133">The following example of an **ArchiveItem** operation request shows how to move an item to the archive Inbox folder.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="ce1e0-134">Все идентификаторы элементов и ключей изменения в этой статье URL были сокращены, чтобы сохранить удобочитаемость.</span><span class="sxs-lookup"><span data-stu-id="ce1e0-134">All item identifiers and change keys in this article have been shortened to preserve readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013"/>
   </soap:Header>
   <soap:Body>
      <m:ArchiveItem>
         <m:ArchiveSourceFolderId>
            <t:DistinguishedFolderId Id="inbox"/>
         </m:ArchiveSourceFolderId>
         <m:ItemIds>
            <t:ItemId Id="AQMkG5BBwrQAAAxoAAAA=" ChangeKey="CQAAAHCtAAAAAAB7"/>
         </m:ItemIds>
      </m:ArchiveItem>
   </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="ce1e0-135">Запрос SOAP body содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="ce1e0-135">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="ce1e0-136">ArchiveItem</span><span class="sxs-lookup"><span data-stu-id="ce1e0-136">ArchiveItem</span></span>](archiveitem.md)    
- [<span data-ttu-id="ce1e0-137">ArchiveSourceFolderId</span><span class="sxs-lookup"><span data-stu-id="ce1e0-137">ArchiveSourceFolderId</span></span>](archivesourcefolderid.md)    
- [<span data-ttu-id="ce1e0-138">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="ce1e0-138">DistinguishedFolderId</span></span>](distinguishedfolderid.md)    
- [<span data-ttu-id="ce1e0-139">Что ItemID</span><span class="sxs-lookup"><span data-stu-id="ce1e0-139">ItemIds</span></span>](itemids.md)   
- [<span data-ttu-id="ce1e0-140">Идентификатор элемента</span><span class="sxs-lookup"><span data-stu-id="ce1e0-140">ItemId</span></span>](itemid.md)
    
## <a name="successful-archiveitem-operation-response"></a><span data-ttu-id="ce1e0-141">Успешные операции ответа ArchiveItem</span><span class="sxs-lookup"><span data-stu-id="ce1e0-141">Successful ArchiveItem operation response</span></span>

<span data-ttu-id="ce1e0-142">В следующем примере показано успешного ответа на запрос операции **ArchiveItem** для перемещения элемента архивного почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="ce1e0-142">The following example shows a successful response to an **ArchiveItem** operation request to move an item to an archive mailbox.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="526" 
                           MinorBuildNumber="0" 
                           Version="Exchange2013" 
                           xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <m:ArchiveItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                             xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
         <m:ResponseMessages>
            <m:ArchiveItemResponseMessage ResponseClass="Success">
               <m:ResponseCode>NoError</m:ResponseCode>
               <m:Items/>
            </m:ArchiveItemResponseMessage>
         </m:ResponseMessages>
      </m:ArchiveItemResponse>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="ce1e0-143">Ответ SOAP body содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="ce1e0-143">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="ce1e0-144">ArchiveItemResponse</span><span class="sxs-lookup"><span data-stu-id="ce1e0-144">ArchiveItemResponse</span></span>](archiveitemresponse.md)    
- [<span data-ttu-id="ce1e0-145">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="ce1e0-145">ResponseMessages</span></span>](responsemessages.md)   
- [<span data-ttu-id="ce1e0-146">ArchiveItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="ce1e0-146">ArchiveItemResponseMessage</span></span>](archiveitemresponsemessage.md)    
- [<span data-ttu-id="ce1e0-147">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="ce1e0-147">ResponseCode</span></span>](responsecode.md)    
- [<span data-ttu-id="ce1e0-148">Элементы</span><span class="sxs-lookup"><span data-stu-id="ce1e0-148">Items</span></span>](items.md)
    
## <a name="archiveitem-operation-error-response"></a><span data-ttu-id="ce1e0-149">Ошибка операции ArchiveItem ответа</span><span class="sxs-lookup"><span data-stu-id="ce1e0-149">ArchiveItem operation error response</span></span>

<span data-ttu-id="ce1e0-150">В следующем примере показано ошибочный ответ на запрос операции **ArchiveItem** .</span><span class="sxs-lookup"><span data-stu-id="ce1e0-150">The following example shows an error response to an **ArchiveItem** operation request.</span></span> <span data-ttu-id="ce1e0-151">Это ответ на допустимый запрос в архив элемента при архивного почтового ящика не включен для пользователя.</span><span class="sxs-lookup"><span data-stu-id="ce1e0-151">This is a response to a valid request to archive an item when an archive mailbox is not enabled for a user.</span></span> 
  
```xml
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="556" 
                           MinorBuildNumber="8" 
                           Version="Exchange2013" 
                           xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <m:ArchiveItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                             xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
         <m:ResponseMessages>
            <m:ArchiveItemResponseMessage ResponseClass="Error">
               <m:MessageText>Archive mailbox is not enabled for this user.</m:MessageText>
               <m:ResponseCode>ErrorInvalidOperation</m:ResponseCode>
               <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
               <m:Items/>
            </m:ArchiveItemResponseMessage>
         </m:ResponseMessages>
      </m:ArchiveItemResponse>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="ce1e0-152">Ошибка ответ SOAP body содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="ce1e0-152">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="ce1e0-153">ArchiveItemResponse</span><span class="sxs-lookup"><span data-stu-id="ce1e0-153">ArchiveItemResponse</span></span>](archiveitemresponse.md)    
- [<span data-ttu-id="ce1e0-154">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="ce1e0-154">ResponseMessages</span></span>](responsemessages.md)    
- [<span data-ttu-id="ce1e0-155">ArchiveItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="ce1e0-155">ArchiveItemResponseMessage</span></span>](archiveitemresponsemessage.md)    
- [<span data-ttu-id="ce1e0-156">MessageText</span><span class="sxs-lookup"><span data-stu-id="ce1e0-156">MessageText</span></span>](messagetext.md)    
- [<span data-ttu-id="ce1e0-157">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="ce1e0-157">ResponseCode</span></span>](responsecode.md)    
- [<span data-ttu-id="ce1e0-158">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="ce1e0-158">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)    
- [<span data-ttu-id="ce1e0-159">Элементы</span><span class="sxs-lookup"><span data-stu-id="ce1e0-159">Items</span></span>](items.md)
    
<span data-ttu-id="ce1e0-160">Дополнительные коды ошибок, которые являются общими для веб-служб Exchange и специально для этой операции в разделе [ResponseCode](responsecode.md).</span><span class="sxs-lookup"><span data-stu-id="ce1e0-160">For additional error codes that are generic to EWS and specific to this operation, see [ResponseCode](responsecode.md).</span></span>
  
## <a name="see-also"></a><span data-ttu-id="ce1e0-161">См. также</span><span class="sxs-lookup"><span data-stu-id="ce1e0-161">See also</span></span>

- [<span data-ttu-id="ce1e0-162">Операции EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="ce1e0-162">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md) 
- [<span data-ttu-id="ce1e0-163">Архивация в веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="ce1e0-163">Archiving in EWS in Exchange</span></span>](http://msdn.microsoft.com/library/78ae179b-ae4f-4f64-911a-e0c70e0fa314%28Office.15%29.aspx)
    

