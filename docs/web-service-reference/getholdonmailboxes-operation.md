---
title: Операция GetHoldOnMailboxes
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 9157f329-80b4-4cd0-a158-378064966ae6
description: Поиск сведений о GetHoldOnMailboxesной операции EWS.
ms.openlocfilehash: 1d0bc2f9d26e11d8d2710693d67843ad2f339a5d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762806"
---
# <a name="getholdonmailboxes-operation"></a><span data-ttu-id="b93d8-103">Операция GetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="b93d8-103">GetHoldOnMailboxes operation</span></span>

<span data-ttu-id="b93d8-104">Поиск сведений о **GetHoldOnMailboxesной** операции EWS.</span><span class="sxs-lookup"><span data-stu-id="b93d8-104">Find information about the **GetHoldOnMailboxes** EWS operation.</span></span> 
  
<span data-ttu-id="b93d8-105">Операция **GetHoldOnMailboxes** получает почтовые ящики, которые находятся в определенном удержании и связанном запросе удержания.</span><span class="sxs-lookup"><span data-stu-id="b93d8-105">The **GetHoldOnMailboxes** operation gets the mailboxes that are under a specific hold and the associated hold query.</span></span> 
  
<span data-ttu-id="b93d8-106">Эта операция появилась в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="b93d8-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-getholdonmailboxes-operation"></a><span data-ttu-id="b93d8-107">Использование операции GetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="b93d8-107">Using the GetHoldOnMailboxes operation</span></span>

<span data-ttu-id="b93d8-108">Операция **GetHoldOnMailboxes** предоставляет клиенту сведения о том, какие почтовые ящики помещаются в конкретное удержание, сведения о запросе удержания, связанном с каждым удержанием, если это необходимо, и сведения о состоянии удержания для каждого почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="b93d8-108">The **GetHoldOnMailboxes** operation gives the client information about which mailboxes are placed under a specific hold, information about the hold query associated with each hold, if applicable, and information about the hold status for each mailbox.</span></span> <span data-ttu-id="b93d8-109">Дополнительные сведения о удержаниях почтовых ящиков, в том числе о удержаниях на основе запросов, можно найти [в статье удержание на месте](http://technet.microsoft.com/en-us/library/ff637980%28v=exchg.150%29) на сайте TechNet.</span><span class="sxs-lookup"><span data-stu-id="b93d8-109">For more information about mailbox holds, including query-based holds, see [In-Place Hold](http://technet.microsoft.com/en-us/library/ff637980%28v=exchg.150%29) on TechNet.</span></span> 
  
### <a name="getholdonmailboxes-operation-soap-headers"></a><span data-ttu-id="b93d8-110">Заголовки SOAP операции GetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="b93d8-110">GetHoldOnMailboxes operation SOAP headers</span></span>

<span data-ttu-id="b93d8-111">Операция **GetHoldOnMailboxes** может использовать заголовки SOAP, указанные в приведенной ниже таблице.</span><span class="sxs-lookup"><span data-stu-id="b93d8-111">The **GetHoldOnMailboxes** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="b93d8-112">**Имя заголовка**</span><span class="sxs-lookup"><span data-stu-id="b93d8-112">**Header name**</span></span>|<span data-ttu-id="b93d8-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="b93d8-113">**Element**</span></span>|<span data-ttu-id="b93d8-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="b93d8-114">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="b93d8-115">**ManagementRole**</span><span class="sxs-lookup"><span data-stu-id="b93d8-115">**ManagementRole**</span></span> <br/> |[<span data-ttu-id="b93d8-116">ManagementRole</span><span class="sxs-lookup"><span data-stu-id="b93d8-116">ManagementRole</span></span>](managementrole.md) <br/> |<span data-ttu-id="b93d8-117">Определяет роли сервера, необходимые для того, чтобы вызывающий абонент мог выполнить запрос.</span><span class="sxs-lookup"><span data-stu-id="b93d8-117">Identifies the server roles that are necessary in order for the caller to make the request.</span></span> <span data-ttu-id="b93d8-118">Этот заголовок является применимым для запроса.</span><span class="sxs-lookup"><span data-stu-id="b93d8-118">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="b93d8-119">**рекуестверсион**</span><span class="sxs-lookup"><span data-stu-id="b93d8-119">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="b93d8-120">рекуестсерверверсион</span><span class="sxs-lookup"><span data-stu-id="b93d8-120">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="b93d8-121">Определяет версию схемы для запроса операции.</span><span class="sxs-lookup"><span data-stu-id="b93d8-121">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="b93d8-122">Этот заголовок является применимым для запроса.</span><span class="sxs-lookup"><span data-stu-id="b93d8-122">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="b93d8-123">**серверверсион**</span><span class="sxs-lookup"><span data-stu-id="b93d8-123">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="b93d8-124">серверверсионинфо</span><span class="sxs-lookup"><span data-stu-id="b93d8-124">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="b93d8-125">Определяет версию сервера, который ответил на запрос.</span><span class="sxs-lookup"><span data-stu-id="b93d8-125">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="b93d8-126">Этот заголовок является применимым для отклика.</span><span class="sxs-lookup"><span data-stu-id="b93d8-126">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="getholdonmailboxes-operation-request-example-get-mailbox-hold-information"></a><span data-ttu-id="b93d8-127">Пример запроса операции GetHoldOnMailboxes: получение сведений о удержании почтовых ящиков</span><span class="sxs-lookup"><span data-stu-id="b93d8-127">GetHoldOnMailboxes operation request example: Get mailbox hold information</span></span>

<span data-ttu-id="b93d8-128">В следующем примере запроса операции **GetHoldOnMailboxes** показано, как получить сведения о удержании почтовых ящиков для хранения почтовых ящиков HoldId2.</span><span class="sxs-lookup"><span data-stu-id="b93d8-128">The following example of a **GetHoldOnMailboxes** operation request shows how to get the mailbox hold information for the HoldId2 mailbox hold.</span></span> 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013" />
   </soap:Header>
   <soap:Body >
      <m:GetHoldOnMailboxes>
         <m:HoldId>HoldId2</m:HoldId>
      </m:GetHoldOnMailboxes>
   </soap:Body>
</soap:Envelope>

```

<span data-ttu-id="b93d8-129">Текст SOAP Request содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="b93d8-129">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="b93d8-130">GetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="b93d8-130">GetHoldOnMailboxes</span></span>](getholdonmailboxes.md)
    
- [<span data-ttu-id="b93d8-131">холдид</span><span class="sxs-lookup"><span data-stu-id="b93d8-131">HoldId</span></span>](holdid.md)
    
## <a name="successful-getholdonmailboxes-operation-response"></a><span data-ttu-id="b93d8-132">Успешный отклик операции GetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="b93d8-132">Successful GetHoldOnMailboxes operation response</span></span>

<span data-ttu-id="b93d8-133">В следующем примере показан успешный ответ на запрос операции **GetHoldOnMailboxes** для получения сведений о удержании почтовых ящиков для хранения почтовых ящиков HoldId2.</span><span class="sxs-lookup"><span data-stu-id="b93d8-133">The following example shows a successful response to a **GetHoldOnMailboxes** operation request to get the mailbox hold information for the HoldId2 mailbox hold.</span></span> 
  
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
      <GetHoldOnMailboxesResponse ResponseClass="Success" 
                                  xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
         <MailboxHoldResult>
            <HoldId xmlns="http://schemas.microsoft.com/exchange/services/2006/types">HoldId2</HoldId>
            <Query xmlns="http://schemas.microsoft.com/exchange/services/2006/types">test</Query>
            <MailboxHoldStatuses xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
               <MailboxHoldStatus>
                  <Mailbox>/o=First Organization/ou=Exchange Administrative Group (FYDIBPDLT)/cn=Recipients/cn=ecc0fd98c2cadf-Willi</Mailbox>
                  <Status>OnHold</Status>
                  <AdditionalInfo/>
               </MailboxHoldStatus>
               <MailboxHoldStatus>
                  <Mailbox>/o=First Organization/ou=Exchange Administrative Group (FYDIBPDLT)/cn=Recipients/cn=dasdat341q8de95-Micha</Mailbox>
                  <Status>OnHold</Status>
                  <AdditionalInfo/>
               </MailboxHoldStatus>
            </MailboxHoldStatuses>
         </MailboxHoldResult>
      </GetHoldOnMailboxesResponse>
   </s:Body>
</s:Envelope>

```

<span data-ttu-id="b93d8-134">Тело SOAP отклика содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="b93d8-134">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="b93d8-135">жесолдонмаилбоксесреспонсе</span><span class="sxs-lookup"><span data-stu-id="b93d8-135">GetHoldOnMailboxesResponse</span></span>](getholdonmailboxesresponse.md)
    
- [<span data-ttu-id="b93d8-136">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="b93d8-136">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="b93d8-137">маилбоксхолдресулт</span><span class="sxs-lookup"><span data-stu-id="b93d8-137">MailboxHoldResult</span></span>](mailboxholdresult.md)
    
- [<span data-ttu-id="b93d8-138">холдид</span><span class="sxs-lookup"><span data-stu-id="b93d8-138">HoldId</span></span>](holdid.md)
    
- [<span data-ttu-id="b93d8-139">Query</span><span class="sxs-lookup"><span data-stu-id="b93d8-139">Query</span></span>](query.md)
    
- [<span data-ttu-id="b93d8-140">маилбоксхолдстатусес</span><span class="sxs-lookup"><span data-stu-id="b93d8-140">MailboxHoldStatuses</span></span>](mailboxholdstatuses.md)
    
- [<span data-ttu-id="b93d8-141">маилбоксхолдстатус</span><span class="sxs-lookup"><span data-stu-id="b93d8-141">MailboxHoldStatus</span></span>](mailboxholdstatus.md)
    
- [<span data-ttu-id="b93d8-142">Mailbox (строка)</span><span class="sxs-lookup"><span data-stu-id="b93d8-142">Mailbox (string)</span></span>](mailbox-string.md)
    
- [<span data-ttu-id="b93d8-143">Состояние (Холдстатустипе)</span><span class="sxs-lookup"><span data-stu-id="b93d8-143">Status (HoldStatusType)</span></span>](status-holdstatustype.md)
    
- [<span data-ttu-id="b93d8-144">аддитионалинфо</span><span class="sxs-lookup"><span data-stu-id="b93d8-144">AdditionalInfo</span></span>](additionalinfo.md)
    
## <a name="getholdonmailboxes-operation-error-response"></a><span data-ttu-id="b93d8-145">Ответ об ошибке операции GetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="b93d8-145">GetHoldOnMailboxes operation error response</span></span>

<span data-ttu-id="b93d8-146">В следующем примере показан ответ об ошибке для запроса операции **GetHoldOnMailboxes** .</span><span class="sxs-lookup"><span data-stu-id="b93d8-146">The following example shows an error response to a **GetHoldOnMailboxes** operation request.</span></span> <span data-ttu-id="b93d8-147">Это ответ на запрос на получение удержания, которое было удалено.</span><span class="sxs-lookup"><span data-stu-id="b93d8-147">This is a response to a request to get a hold that has been deleted.</span></span> 
  
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
      <GetHoldOnMailboxesResponse ResponseClass="Error" 
                                  xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>The specific query-based hold is not found.</MessageText>
         <ResponseCode>ErrorMailboxHoldNotFound</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
      </GetHoldOnMailboxesResponse>
   </s:Body>
</s:Envelope>

```

<span data-ttu-id="b93d8-148">Основной текст сообщения об ошибке SOAP содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="b93d8-148">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="b93d8-149">жесолдонмаилбоксесреспонсе</span><span class="sxs-lookup"><span data-stu-id="b93d8-149">GetHoldOnMailboxesResponse</span></span>](getholdonmailboxesresponse.md)
    
- [<span data-ttu-id="b93d8-150">мессажетекст</span><span class="sxs-lookup"><span data-stu-id="b93d8-150">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="b93d8-151">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="b93d8-151">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="b93d8-152">дескриптивелинккэй</span><span class="sxs-lookup"><span data-stu-id="b93d8-152">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
<span data-ttu-id="b93d8-153">Дополнительные коды ошибок, которые являются общими для EWS и специфичными для этой операции, можно найти в разделе [респонсекоде](responsecode.md).</span><span class="sxs-lookup"><span data-stu-id="b93d8-153">For additional error codes that are generic to EWS and specific to this operation, see [ResponseCode](responsecode.md).</span></span>
  
## <a name="see-also"></a><span data-ttu-id="b93d8-154">См. также</span><span class="sxs-lookup"><span data-stu-id="b93d8-154">See also</span></span>

- [<span data-ttu-id="b93d8-155">Операции EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="b93d8-155">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
    
- [<span data-ttu-id="b93d8-156">Операция GetSearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="b93d8-156">GetSearchableMailboxes operation</span></span>](getsearchablemailboxes-operation.md)
    
- [<span data-ttu-id="b93d8-157">Операция SearchMailboxes</span><span class="sxs-lookup"><span data-stu-id="b93d8-157">SearchMailboxes operation</span></span>](searchmailboxes-operation.md)
    
- [<span data-ttu-id="b93d8-158">Операция SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="b93d8-158">SetHoldOnMailboxes operation</span></span>](setholdonmailboxes-operation.md)
    
- [<span data-ttu-id="b93d8-159">Операция GetDiscoverySearchConfiguration</span><span class="sxs-lookup"><span data-stu-id="b93d8-159">GetDiscoverySearchConfiguration operation</span></span>](getdiscoverysearchconfiguration-operation.md)
    
- [<span data-ttu-id="b93d8-160">Операция GetNonIndexableItemDetails</span><span class="sxs-lookup"><span data-stu-id="b93d8-160">GetNonIndexableItemDetails operation</span></span>](getnonindexableitemdetails-operation.md)
    
- [<span data-ttu-id="b93d8-161">Операция GetNonIndexableItemStatistics</span><span class="sxs-lookup"><span data-stu-id="b93d8-161">GetNonIndexableItemStatistics operation</span></span>](getnonindexableitemstatistics-operation.md)
    

