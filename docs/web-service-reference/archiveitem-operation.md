---
title: Операция ArchiveItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 1af216b3-13ea-498e-b4fc-23513755d731
description: Поиск сведений о ArchiveItemной операции EWS.
ms.openlocfilehash: d1e18122e67c36babbc8bf01d305309e2b17b568
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463435"
---
# <a name="archiveitem-operation"></a><span data-ttu-id="73dc8-103">Операция ArchiveItem</span><span class="sxs-lookup"><span data-stu-id="73dc8-103">ArchiveItem operation</span></span>

<span data-ttu-id="73dc8-104">Поиск сведений о **ArchiveItemной** операции EWS.</span><span class="sxs-lookup"><span data-stu-id="73dc8-104">Find information about the **ArchiveItem** EWS operation.</span></span> 
  
<span data-ttu-id="73dc8-105">Операция **ArchiveItem** перемещает элемент в архивный почтовый ящик пользователя почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="73dc8-105">The **ArchiveItem** operation moves an item into the mailbox user's archive mailbox.</span></span> 
  
<span data-ttu-id="73dc8-106">Эта операция появилась в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="73dc8-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-archiveitem-operation"></a><span data-ttu-id="73dc8-107">Использование операции ArchiveItem</span><span class="sxs-lookup"><span data-stu-id="73dc8-107">Using the ArchiveItem operation</span></span>

<span data-ttu-id="73dc8-108">Операция **ArchiveItem** использует в запросе два аргумента, которые определяют элементы для перемещения в архивный почтовый ящик и конечную папку для этих элементов.</span><span class="sxs-lookup"><span data-stu-id="73dc8-108">The **ArchiveItem** operation takes two arguments in the request that identify the items to move to the archive mailbox and the destination folder for those items.</span></span> <span data-ttu-id="73dc8-109">Чтобы эта операция работала, необходимо включить архивный почтовый ящик.</span><span class="sxs-lookup"><span data-stu-id="73dc8-109">An archive mailbox must be enabled in order for this operation to work.</span></span> <span data-ttu-id="73dc8-110">Сведения о том, как включить архивный почтовый ящик, можно найти [в разделе Управление архивами на месте](https://technet.microsoft.com/library/jj651146.aspx).</span><span class="sxs-lookup"><span data-stu-id="73dc8-110">For information about how to enable an archive mailbox, see [Manage In-Place Archives](https://technet.microsoft.com/library/jj651146.aspx).</span></span>
  
### <a name="archiveitem-operation-soap-headers"></a><span data-ttu-id="73dc8-111">Заголовки SOAP операции ArchiveItem</span><span class="sxs-lookup"><span data-stu-id="73dc8-111">ArchiveItem operation SOAP headers</span></span>

<span data-ttu-id="73dc8-112">Операция **ArchiveItem** может использовать заголовки SOAP, указанные в приведенной ниже таблице.</span><span class="sxs-lookup"><span data-stu-id="73dc8-112">The **ArchiveItem** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="73dc8-113">**Имя заголовка**</span><span class="sxs-lookup"><span data-stu-id="73dc8-113">**Header name**</span></span>|<span data-ttu-id="73dc8-114">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="73dc8-114">**Element**</span></span>|<span data-ttu-id="73dc8-115">**Описание**</span><span class="sxs-lookup"><span data-stu-id="73dc8-115">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="73dc8-116">**Олицетворение**</span><span class="sxs-lookup"><span data-stu-id="73dc8-116">**Impersonation**</span></span> <br/> |[<span data-ttu-id="73dc8-117">ексчанжеимперсонатион</span><span class="sxs-lookup"><span data-stu-id="73dc8-117">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="73dc8-118">Идентифицирует пользователя, который олицетворяет клиентское приложение.</span><span class="sxs-lookup"><span data-stu-id="73dc8-118">Identifies the user whom the client application is impersonating.</span></span> <span data-ttu-id="73dc8-119">Этот заголовок является применимым для запроса.</span><span class="sxs-lookup"><span data-stu-id="73dc8-119">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="73dc8-120">**маилбокскултуре**</span><span class="sxs-lookup"><span data-stu-id="73dc8-120">**MailboxCulture**</span></span> <br/> |[<span data-ttu-id="73dc8-121">маилбокскултуре</span><span class="sxs-lookup"><span data-stu-id="73dc8-121">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="73dc8-122">Определяет язык и региональные параметры, как определено в RFC 3066 **теги для идентификации языков**, которые будут использоваться для доступа к почтовому ящику.</span><span class="sxs-lookup"><span data-stu-id="73dc8-122">Identifies the culture, as defined in RFC 3066, **Tags for the Identification of Languages**, to be used to access the mailbox.</span></span> <span data-ttu-id="73dc8-123">Этот заголовок является применимым для запроса.</span><span class="sxs-lookup"><span data-stu-id="73dc8-123">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="73dc8-124">**рекуестверсион**</span><span class="sxs-lookup"><span data-stu-id="73dc8-124">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="73dc8-125">рекуестсерверверсион</span><span class="sxs-lookup"><span data-stu-id="73dc8-125">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="73dc8-126">Определяет версию схемы для запроса операции.</span><span class="sxs-lookup"><span data-stu-id="73dc8-126">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="73dc8-127">Этот заголовок является применимым для запроса.</span><span class="sxs-lookup"><span data-stu-id="73dc8-127">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="73dc8-128">**серверверсион**</span><span class="sxs-lookup"><span data-stu-id="73dc8-128">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="73dc8-129">серверверсионинфо</span><span class="sxs-lookup"><span data-stu-id="73dc8-129">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="73dc8-130">Определяет версию сервера, который ответил на запрос.</span><span class="sxs-lookup"><span data-stu-id="73dc8-130">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="73dc8-131">Этот заголовок является применимым для отклика.</span><span class="sxs-lookup"><span data-stu-id="73dc8-131">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="archiveitem-operation-request-example-move-an-item-to-the-archive-inbox-folder"></a><span data-ttu-id="73dc8-132">Пример запроса операции ArchiveItem: перемещение элемента в архивную папку "Входящие"</span><span class="sxs-lookup"><span data-stu-id="73dc8-132">ArchiveItem operation request example: Move an item to the archive inbox folder</span></span>

<span data-ttu-id="73dc8-133">В следующем примере запроса операции **ArchiveItem** показано, как переместить элемент в архивную папку "Входящие".</span><span class="sxs-lookup"><span data-stu-id="73dc8-133">The following example of an **ArchiveItem** operation request shows how to move an item to the archive Inbox folder.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="73dc8-134">Все идентификаторы элементов и изменения ключей в этой статье были сокращены, чтобы сохранить удобочитаемость.</span><span class="sxs-lookup"><span data-stu-id="73dc8-134">All item identifiers and change keys in this article have been shortened to preserve readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
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

<span data-ttu-id="73dc8-135">Текст SOAP Request содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="73dc8-135">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="73dc8-136">ArchiveItem</span><span class="sxs-lookup"><span data-stu-id="73dc8-136">ArchiveItem</span></span>](archiveitem.md)    
- [<span data-ttu-id="73dc8-137">арчивесаурцефолдерид</span><span class="sxs-lookup"><span data-stu-id="73dc8-137">ArchiveSourceFolderId</span></span>](archivesourcefolderid.md)    
- [<span data-ttu-id="73dc8-138">дистингуишедфолдерид</span><span class="sxs-lookup"><span data-stu-id="73dc8-138">DistinguishedFolderId</span></span>](distinguishedfolderid.md)    
- [<span data-ttu-id="73dc8-139">итемидс</span><span class="sxs-lookup"><span data-stu-id="73dc8-139">ItemIds</span></span>](itemids.md)   
- [<span data-ttu-id="73dc8-140">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="73dc8-140">ItemId</span></span>](itemid.md)
    
## <a name="successful-archiveitem-operation-response"></a><span data-ttu-id="73dc8-141">Успешный отклик операции ArchiveItem</span><span class="sxs-lookup"><span data-stu-id="73dc8-141">Successful ArchiveItem operation response</span></span>

<span data-ttu-id="73dc8-142">В следующем примере показан успешный ответ на запрос операции **ArchiveItem** для перемещения элемента в архивный почтовый ящик.</span><span class="sxs-lookup"><span data-stu-id="73dc8-142">The following example shows a successful response to an **ArchiveItem** operation request to move an item to an archive mailbox.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="526" 
                           MinorBuildNumber="0" 
                           Version="Exchange2013" 
                           xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <m:ArchiveItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                             xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
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

<span data-ttu-id="73dc8-143">Тело SOAP отклика содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="73dc8-143">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="73dc8-144">арчивеитемреспонсе</span><span class="sxs-lookup"><span data-stu-id="73dc8-144">ArchiveItemResponse</span></span>](archiveitemresponse.md)    
- [<span data-ttu-id="73dc8-145">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="73dc8-145">ResponseMessages</span></span>](responsemessages.md)   
- [<span data-ttu-id="73dc8-146">арчивеитемреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="73dc8-146">ArchiveItemResponseMessage</span></span>](archiveitemresponsemessage.md)    
- [<span data-ttu-id="73dc8-147">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="73dc8-147">ResponseCode</span></span>](responsecode.md)    
- [<span data-ttu-id="73dc8-148">Items</span><span class="sxs-lookup"><span data-stu-id="73dc8-148">Items</span></span>](items.md)
    
## <a name="archiveitem-operation-error-response"></a><span data-ttu-id="73dc8-149">Ответ об ошибке операции ArchiveItem</span><span class="sxs-lookup"><span data-stu-id="73dc8-149">ArchiveItem operation error response</span></span>

<span data-ttu-id="73dc8-150">В следующем примере показан ответ об ошибке для запроса операции **ArchiveItem** .</span><span class="sxs-lookup"><span data-stu-id="73dc8-150">The following example shows an error response to an **ArchiveItem** operation request.</span></span> <span data-ttu-id="73dc8-151">Это ответ на действительный запрос на архивацию элемента, когда архивный почтовый ящик не включен для пользователя.</span><span class="sxs-lookup"><span data-stu-id="73dc8-151">This is a response to a valid request to archive an item when an archive mailbox is not enabled for a user.</span></span> 
  
```xml
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="556" 
                           MinorBuildNumber="8" 
                           Version="Exchange2013" 
                           xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <m:ArchiveItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                             xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
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

<span data-ttu-id="73dc8-152">Основной текст сообщения об ошибке SOAP содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="73dc8-152">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="73dc8-153">арчивеитемреспонсе</span><span class="sxs-lookup"><span data-stu-id="73dc8-153">ArchiveItemResponse</span></span>](archiveitemresponse.md)    
- [<span data-ttu-id="73dc8-154">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="73dc8-154">ResponseMessages</span></span>](responsemessages.md)    
- [<span data-ttu-id="73dc8-155">арчивеитемреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="73dc8-155">ArchiveItemResponseMessage</span></span>](archiveitemresponsemessage.md)    
- [<span data-ttu-id="73dc8-156">мессажетекст</span><span class="sxs-lookup"><span data-stu-id="73dc8-156">MessageText</span></span>](messagetext.md)    
- [<span data-ttu-id="73dc8-157">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="73dc8-157">ResponseCode</span></span>](responsecode.md)    
- [<span data-ttu-id="73dc8-158">дескриптивелинккэй</span><span class="sxs-lookup"><span data-stu-id="73dc8-158">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)    
- [<span data-ttu-id="73dc8-159">Items</span><span class="sxs-lookup"><span data-stu-id="73dc8-159">Items</span></span>](items.md)
    
<span data-ttu-id="73dc8-160">Дополнительные коды ошибок, которые являются общими для EWS и специфичными для этой операции, можно найти в разделе [респонсекоде](responsecode.md).</span><span class="sxs-lookup"><span data-stu-id="73dc8-160">For additional error codes that are generic to EWS and specific to this operation, see [ResponseCode](responsecode.md).</span></span>
  
## <a name="see-also"></a><span data-ttu-id="73dc8-161">См. также</span><span class="sxs-lookup"><span data-stu-id="73dc8-161">See also</span></span>

- [<span data-ttu-id="73dc8-162">Операции EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="73dc8-162">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md) 
- [<span data-ttu-id="73dc8-163">Архивация в веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="73dc8-163">Archiving in EWS in Exchange</span></span>](https://msdn.microsoft.com/library/78ae179b-ae4f-4f64-911a-e0c70e0fa314%28Office.15%29.aspx)
    

