---
title: Операция GetHoldOnMailboxes
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 9157f329-80b4-4cd0-a158-378064966ae6
description: Найдите сведения о веб-служб Exchange GetHoldOnMailboxes операции.
ms.openlocfilehash: 1d0bc2f9d26e11d8d2710693d67843ad2f339a5d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762806"
---
# <a name="getholdonmailboxes-operation"></a><span data-ttu-id="f79c3-103">Операция GetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="f79c3-103">GetHoldOnMailboxes operation</span></span>

<span data-ttu-id="f79c3-104">Найдите сведения о **GetHoldOnMailboxes** операции веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="f79c3-104">Find information about the **GetHoldOnMailboxes** EWS operation.</span></span> 
  
<span data-ttu-id="f79c3-105">Операция **GetHoldOnMailboxes** возвращает почтовые ящики, которые находятся под конкретного удержания и связанный с ним удерживайте запроса.</span><span class="sxs-lookup"><span data-stu-id="f79c3-105">The **GetHoldOnMailboxes** operation gets the mailboxes that are under a specific hold and the associated hold query.</span></span> 
  
<span data-ttu-id="f79c3-106">Эта операция появилась в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="f79c3-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-getholdonmailboxes-operation"></a><span data-ttu-id="f79c3-107">С помощью операции GetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="f79c3-107">Using the GetHoldOnMailboxes operation</span></span>

<span data-ttu-id="f79c3-108">Операция **GetHoldOnMailboxes** предоставляет сведения о клиенте, о том, какие почтовые ящики размещаются в разделе конкретного удержания, сведения о запросе удержания, связанные с каждой удержание, если это возможно и сведения о состоянии удержания для каждого почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="f79c3-108">The **GetHoldOnMailboxes** operation gives the client information about which mailboxes are placed under a specific hold, information about the hold query associated with each hold, if applicable, and information about the hold status for each mailbox.</span></span> <span data-ttu-id="f79c3-109">Дополнительные сведения об удержаниях почтового ящика, включая запроса на удержание можно [Хранения на месте](http://technet.microsoft.com/ru-ru/library/ff637980%28v=exchg.150%29) на сайте TechNet.</span><span class="sxs-lookup"><span data-stu-id="f79c3-109">For more information about mailbox holds, including query-based holds, see [In-Place Hold](http://technet.microsoft.com/ru-ru/library/ff637980%28v=exchg.150%29) on TechNet.</span></span> 
  
### <a name="getholdonmailboxes-operation-soap-headers"></a><span data-ttu-id="f79c3-110">Заголовки SOAP GetHoldOnMailboxes операции</span><span class="sxs-lookup"><span data-stu-id="f79c3-110">GetHoldOnMailboxes operation SOAP headers</span></span>

<span data-ttu-id="f79c3-111">Операция **GetHoldOnMailboxes** можно использовать заголовки SOAP, которые перечислены в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="f79c3-111">The **GetHoldOnMailboxes** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="f79c3-112">**Имя заголовка**</span><span class="sxs-lookup"><span data-stu-id="f79c3-112">**Header name**</span></span>|<span data-ttu-id="f79c3-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="f79c3-113">**Element**</span></span>|<span data-ttu-id="f79c3-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="f79c3-114">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="f79c3-115">**ManagementRole**</span><span class="sxs-lookup"><span data-stu-id="f79c3-115">**ManagementRole**</span></span> <br/> |[<span data-ttu-id="f79c3-116">ManagementRole</span><span class="sxs-lookup"><span data-stu-id="f79c3-116">ManagementRole</span></span>](managementrole.md) <br/> |<span data-ttu-id="f79c3-117">Идентифицирует ролей сервера, необходимых в порядке для абонентов для запроса.</span><span class="sxs-lookup"><span data-stu-id="f79c3-117">Identifies the server roles that are necessary in order for the caller to make the request.</span></span> <span data-ttu-id="f79c3-118">Этот заголовок можно применять к запросу.</span><span class="sxs-lookup"><span data-stu-id="f79c3-118">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="f79c3-119">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="f79c3-119">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="f79c3-120">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="f79c3-120">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="f79c3-121">Определяет версию схемы для операции запроса.</span><span class="sxs-lookup"><span data-stu-id="f79c3-121">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="f79c3-122">Этот заголовок можно применять к запросу.</span><span class="sxs-lookup"><span data-stu-id="f79c3-122">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="f79c3-123">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="f79c3-123">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="f79c3-124">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="f79c3-124">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="f79c3-125">Определяет версию сервера, ответившего на запрос.</span><span class="sxs-lookup"><span data-stu-id="f79c3-125">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="f79c3-126">Этот заголовок можно применять, чтобы получить ответ.</span><span class="sxs-lookup"><span data-stu-id="f79c3-126">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="getholdonmailboxes-operation-request-example-get-mailbox-hold-information"></a><span data-ttu-id="f79c3-127">Пример запроса GetHoldOnMailboxes операции: получение сведений о почтовых ящиках удержания</span><span class="sxs-lookup"><span data-stu-id="f79c3-127">GetHoldOnMailboxes operation request example: Get mailbox hold information</span></span>

<span data-ttu-id="f79c3-128">В следующем примере запрос операции **GetHoldOnMailboxes** показано, как получить сведения об удержаниях почтового ящика для удержания HoldId2 почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="f79c3-128">The following example of a **GetHoldOnMailboxes** operation request shows how to get the mailbox hold information for the HoldId2 mailbox hold.</span></span> 
  
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

<span data-ttu-id="f79c3-129">Запрос SOAP body содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="f79c3-129">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="f79c3-130">GetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="f79c3-130">GetHoldOnMailboxes</span></span>](getholdonmailboxes.md)
    
- [<span data-ttu-id="f79c3-131">HoldId</span><span class="sxs-lookup"><span data-stu-id="f79c3-131">HoldId</span></span>](holdid.md)
    
## <a name="successful-getholdonmailboxes-operation-response"></a><span data-ttu-id="f79c3-132">Успешные операции ответа GetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="f79c3-132">Successful GetHoldOnMailboxes operation response</span></span>

<span data-ttu-id="f79c3-133">В следующем примере показано успешные ответ на операцию **GetHoldOnMailboxes** запрос на получение почтового ящика хранения сведений для удержания HoldId2 почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="f79c3-133">The following example shows a successful response to a **GetHoldOnMailboxes** operation request to get the mailbox hold information for the HoldId2 mailbox hold.</span></span> 
  
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

<span data-ttu-id="f79c3-134">Ответ SOAP body содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="f79c3-134">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="f79c3-135">GetHoldOnMailboxesResponse</span><span class="sxs-lookup"><span data-stu-id="f79c3-135">GetHoldOnMailboxesResponse</span></span>](getholdonmailboxesresponse.md)
    
- [<span data-ttu-id="f79c3-136">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="f79c3-136">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="f79c3-137">MailboxHoldResult</span><span class="sxs-lookup"><span data-stu-id="f79c3-137">MailboxHoldResult</span></span>](mailboxholdresult.md)
    
- [<span data-ttu-id="f79c3-138">HoldId</span><span class="sxs-lookup"><span data-stu-id="f79c3-138">HoldId</span></span>](holdid.md)
    
- [<span data-ttu-id="f79c3-139">Query</span><span class="sxs-lookup"><span data-stu-id="f79c3-139">Query</span></span>](query.md)
    
- [<span data-ttu-id="f79c3-140">MailboxHoldStatuses</span><span class="sxs-lookup"><span data-stu-id="f79c3-140">MailboxHoldStatuses</span></span>](mailboxholdstatuses.md)
    
- [<span data-ttu-id="f79c3-141">MailboxHoldStatus</span><span class="sxs-lookup"><span data-stu-id="f79c3-141">MailboxHoldStatus</span></span>](mailboxholdstatus.md)
    
- [<span data-ttu-id="f79c3-142">Почтовый ящик (строка)</span><span class="sxs-lookup"><span data-stu-id="f79c3-142">Mailbox (string)</span></span>](mailbox-string.md)
    
- [<span data-ttu-id="f79c3-143">Состояние (HoldStatusType)</span><span class="sxs-lookup"><span data-stu-id="f79c3-143">Status (HoldStatusType)</span></span>](status-holdstatustype.md)
    
- [<span data-ttu-id="f79c3-144">AdditionalInfo</span><span class="sxs-lookup"><span data-stu-id="f79c3-144">AdditionalInfo</span></span>](additionalinfo.md)
    
## <a name="getholdonmailboxes-operation-error-response"></a><span data-ttu-id="f79c3-145">Ошибка операции GetHoldOnMailboxes ответа</span><span class="sxs-lookup"><span data-stu-id="f79c3-145">GetHoldOnMailboxes operation error response</span></span>

<span data-ttu-id="f79c3-146">В следующем примере показано ошибочный ответ на запрос операции **GetHoldOnMailboxes** .</span><span class="sxs-lookup"><span data-stu-id="f79c3-146">The following example shows an error response to a **GetHoldOnMailboxes** operation request.</span></span> <span data-ttu-id="f79c3-147">Это ответ на запрос для получения удержания, который был удален.</span><span class="sxs-lookup"><span data-stu-id="f79c3-147">This is a response to a request to get a hold that has been deleted.</span></span> 
  
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

<span data-ttu-id="f79c3-148">Ошибка ответ SOAP body содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="f79c3-148">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="f79c3-149">GetHoldOnMailboxesResponse</span><span class="sxs-lookup"><span data-stu-id="f79c3-149">GetHoldOnMailboxesResponse</span></span>](getholdonmailboxesresponse.md)
    
- [<span data-ttu-id="f79c3-150">MessageText</span><span class="sxs-lookup"><span data-stu-id="f79c3-150">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="f79c3-151">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="f79c3-151">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="f79c3-152">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="f79c3-152">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
<span data-ttu-id="f79c3-153">Дополнительные коды ошибок, которые являются общими для веб-служб Exchange и специально для этой операции в разделе [ResponseCode](responsecode.md).</span><span class="sxs-lookup"><span data-stu-id="f79c3-153">For additional error codes that are generic to EWS and specific to this operation, see [ResponseCode](responsecode.md).</span></span>
  
## <a name="see-also"></a><span data-ttu-id="f79c3-154">См. также</span><span class="sxs-lookup"><span data-stu-id="f79c3-154">See also</span></span>

- [<span data-ttu-id="f79c3-155">Операции EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="f79c3-155">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
    
- [<span data-ttu-id="f79c3-156">Операция GetSearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="f79c3-156">GetSearchableMailboxes operation</span></span>](getsearchablemailboxes-operation.md)
    
- [<span data-ttu-id="f79c3-157">Операция SearchMailboxes</span><span class="sxs-lookup"><span data-stu-id="f79c3-157">SearchMailboxes operation</span></span>](searchmailboxes-operation.md)
    
- [<span data-ttu-id="f79c3-158">Операция SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="f79c3-158">SetHoldOnMailboxes operation</span></span>](setholdonmailboxes-operation.md)
    
- [<span data-ttu-id="f79c3-159">Операция GetDiscoverySearchConfiguration</span><span class="sxs-lookup"><span data-stu-id="f79c3-159">GetDiscoverySearchConfiguration operation</span></span>](getdiscoverysearchconfiguration-operation.md)
    
- [<span data-ttu-id="f79c3-160">Операция GetNonIndexableItemDetails</span><span class="sxs-lookup"><span data-stu-id="f79c3-160">GetNonIndexableItemDetails operation</span></span>](getnonindexableitemdetails-operation.md)
    
- [<span data-ttu-id="f79c3-161">Операция GetNonIndexableItemStatistics</span><span class="sxs-lookup"><span data-stu-id="f79c3-161">GetNonIndexableItemStatistics operation</span></span>](getnonindexableitemstatistics-operation.md)
    

