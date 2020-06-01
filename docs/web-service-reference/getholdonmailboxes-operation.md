---
title: Операция GetHoldOnMailboxes
manager: sethgros
ms.date: 01/24/2020
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 9157f329-80b4-4cd0-a158-378064966ae6
description: Поиск сведений о GetHoldOnMailboxesной операции EWS.
ms.openlocfilehash: 867f38be87e60af8708eeb0b9d0e3ac8eee6ff64
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457734"
---
# <a name="getholdonmailboxes-operation"></a><span data-ttu-id="37f6a-103">Операция GetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="37f6a-103">GetHoldOnMailboxes operation</span></span>

> [!IMPORTANT]
> <span data-ttu-id="37f6a-104">Начиная с 1 апреля 2020, операция GetHoldOnMailboxes больше не будет доступна в Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="37f6a-104">Starting on April 1, 2020, the GetHoldOnMailboxes operation will no longer be available in Exchange Online.</span></span> <span data-ttu-id="37f6a-105">Эта операция не будет затронута в локальных версиях Exchange Server.</span><span class="sxs-lookup"><span data-stu-id="37f6a-105">This operation won't be affected in on-premises versions of Exchange Server.</span></span> <span data-ttu-id="37f6a-106">Дополнительные сведения см. [в статье выбытие средств прежних версий электронных данных в Exchange Online](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#getsearchablemailboxes-setholdonmailboxes-and-getholdonmailboxes-operations-in-the-ews-api).</span><span class="sxs-lookup"><span data-stu-id="37f6a-106">For more information, see [Retirement of legacy eDiscovery tools in Exchange Online](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#getsearchablemailboxes-setholdonmailboxes-and-getholdonmailboxes-operations-in-the-ews-api).</span></span>

<span data-ttu-id="37f6a-107">Поиск сведений о **GetHoldOnMailboxesной** операции EWS.</span><span class="sxs-lookup"><span data-stu-id="37f6a-107">Find information about the **GetHoldOnMailboxes** EWS operation.</span></span> 
  
<span data-ttu-id="37f6a-108">Операция **GetHoldOnMailboxes** получает почтовые ящики, которые находятся в определенном удержании и связанном запросе удержания.</span><span class="sxs-lookup"><span data-stu-id="37f6a-108">The **GetHoldOnMailboxes** operation gets the mailboxes that are under a specific hold and the associated hold query.</span></span> 
  
<span data-ttu-id="37f6a-109">Эта операция появилась в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="37f6a-109">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-getholdonmailboxes-operation"></a><span data-ttu-id="37f6a-110">Использование операции GetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="37f6a-110">Using the GetHoldOnMailboxes operation</span></span>

<span data-ttu-id="37f6a-111">Операция **GetHoldOnMailboxes** предоставляет клиенту сведения о том, какие почтовые ящики помещаются в конкретное удержание, сведения о запросе удержания, связанном с каждым удержанием, если это необходимо, и сведения о состоянии удержания для каждого почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="37f6a-111">The **GetHoldOnMailboxes** operation gives the client information about which mailboxes are placed under a specific hold, information about the hold query associated with each hold, if applicable, and information about the hold status for each mailbox.</span></span> <span data-ttu-id="37f6a-112">Дополнительные сведения о удержаниях почтовых ящиков, в том числе о удержаниях на основе запросов, можно найти [в статье удержание на месте](https://technet.microsoft.com/library/ff637980%28v=exchg.150%29) на сайте TechNet.</span><span class="sxs-lookup"><span data-stu-id="37f6a-112">For more information about mailbox holds, including query-based holds, see [In-Place Hold](https://technet.microsoft.com/library/ff637980%28v=exchg.150%29) on TechNet.</span></span> 
  
### <a name="getholdonmailboxes-operation-soap-headers"></a><span data-ttu-id="37f6a-113">Заголовки SOAP операции GetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="37f6a-113">GetHoldOnMailboxes operation SOAP headers</span></span>

<span data-ttu-id="37f6a-114">Операция **GetHoldOnMailboxes** может использовать заголовки SOAP, указанные в приведенной ниже таблице.</span><span class="sxs-lookup"><span data-stu-id="37f6a-114">The **GetHoldOnMailboxes** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="37f6a-115">**Имя заголовка**</span><span class="sxs-lookup"><span data-stu-id="37f6a-115">**Header name**</span></span>|<span data-ttu-id="37f6a-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="37f6a-116">**Element**</span></span>|<span data-ttu-id="37f6a-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="37f6a-117">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="37f6a-118">**ManagementRole**</span><span class="sxs-lookup"><span data-stu-id="37f6a-118">**ManagementRole**</span></span> <br/> |[<span data-ttu-id="37f6a-119">ManagementRole</span><span class="sxs-lookup"><span data-stu-id="37f6a-119">ManagementRole</span></span>](managementrole.md) <br/> |<span data-ttu-id="37f6a-120">Определяет роли сервера, необходимые для того, чтобы вызывающий абонент мог выполнить запрос.</span><span class="sxs-lookup"><span data-stu-id="37f6a-120">Identifies the server roles that are necessary in order for the caller to make the request.</span></span> <span data-ttu-id="37f6a-121">Этот заголовок является применимым для запроса.</span><span class="sxs-lookup"><span data-stu-id="37f6a-121">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="37f6a-122">**рекуестверсион**</span><span class="sxs-lookup"><span data-stu-id="37f6a-122">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="37f6a-123">рекуестсерверверсион</span><span class="sxs-lookup"><span data-stu-id="37f6a-123">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="37f6a-124">Определяет версию схемы для запроса операции.</span><span class="sxs-lookup"><span data-stu-id="37f6a-124">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="37f6a-125">Этот заголовок является применимым для запроса.</span><span class="sxs-lookup"><span data-stu-id="37f6a-125">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="37f6a-126">**серверверсион**</span><span class="sxs-lookup"><span data-stu-id="37f6a-126">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="37f6a-127">серверверсионинфо</span><span class="sxs-lookup"><span data-stu-id="37f6a-127">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="37f6a-128">Определяет версию сервера, который ответил на запрос.</span><span class="sxs-lookup"><span data-stu-id="37f6a-128">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="37f6a-129">Этот заголовок является применимым для отклика.</span><span class="sxs-lookup"><span data-stu-id="37f6a-129">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="getholdonmailboxes-operation-request-example-get-mailbox-hold-information"></a><span data-ttu-id="37f6a-130">Пример запроса операции GetHoldOnMailboxes: получение сведений о удержании почтовых ящиков</span><span class="sxs-lookup"><span data-stu-id="37f6a-130">GetHoldOnMailboxes operation request example: Get mailbox hold information</span></span>

<span data-ttu-id="37f6a-131">В следующем примере запроса операции **GetHoldOnMailboxes** показано, как получить сведения о удержании почтовых ящиков для хранения почтовых ящиков HoldId2.</span><span class="sxs-lookup"><span data-stu-id="37f6a-131">The following example of a **GetHoldOnMailboxes** operation request shows how to get the mailbox hold information for the HoldId2 mailbox hold.</span></span> 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
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

<span data-ttu-id="37f6a-132">Текст SOAP Request содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="37f6a-132">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="37f6a-133">GetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="37f6a-133">GetHoldOnMailboxes</span></span>](getholdonmailboxes.md)
    
- [<span data-ttu-id="37f6a-134">холдид</span><span class="sxs-lookup"><span data-stu-id="37f6a-134">HoldId</span></span>](holdid.md)
    
## <a name="successful-getholdonmailboxes-operation-response"></a><span data-ttu-id="37f6a-135">Успешный отклик операции GetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="37f6a-135">Successful GetHoldOnMailboxes operation response</span></span>

<span data-ttu-id="37f6a-136">В следующем примере показан успешный ответ на запрос операции **GetHoldOnMailboxes** для получения сведений о удержании почтовых ящиков для хранения почтовых ящиков HoldId2.</span><span class="sxs-lookup"><span data-stu-id="37f6a-136">The following example shows a successful response to a **GetHoldOnMailboxes** operation request to get the mailbox hold information for the HoldId2 mailbox hold.</span></span> 
  
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
      <GetHoldOnMailboxesResponse ResponseClass="Success" 
                                  xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
         <MailboxHoldResult>
            <HoldId xmlns="https://schemas.microsoft.com/exchange/services/2006/types">HoldId2</HoldId>
            <Query xmlns="https://schemas.microsoft.com/exchange/services/2006/types">test</Query>
            <MailboxHoldStatuses xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
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

<span data-ttu-id="37f6a-137">Тело SOAP отклика содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="37f6a-137">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="37f6a-138">жесолдонмаилбоксесреспонсе</span><span class="sxs-lookup"><span data-stu-id="37f6a-138">GetHoldOnMailboxesResponse</span></span>](getholdonmailboxesresponse.md)
    
- [<span data-ttu-id="37f6a-139">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="37f6a-139">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="37f6a-140">маилбоксхолдресулт</span><span class="sxs-lookup"><span data-stu-id="37f6a-140">MailboxHoldResult</span></span>](mailboxholdresult.md)
    
- [<span data-ttu-id="37f6a-141">холдид</span><span class="sxs-lookup"><span data-stu-id="37f6a-141">HoldId</span></span>](holdid.md)
    
- [<span data-ttu-id="37f6a-142">Query</span><span class="sxs-lookup"><span data-stu-id="37f6a-142">Query</span></span>](query.md)
    
- [<span data-ttu-id="37f6a-143">маилбоксхолдстатусес</span><span class="sxs-lookup"><span data-stu-id="37f6a-143">MailboxHoldStatuses</span></span>](mailboxholdstatuses.md)
    
- [<span data-ttu-id="37f6a-144">маилбоксхолдстатус</span><span class="sxs-lookup"><span data-stu-id="37f6a-144">MailboxHoldStatus</span></span>](mailboxholdstatus.md)
    
- [<span data-ttu-id="37f6a-145">Mailbox (строка)</span><span class="sxs-lookup"><span data-stu-id="37f6a-145">Mailbox (string)</span></span>](mailbox-string.md)
    
- [<span data-ttu-id="37f6a-146">Состояние (Холдстатустипе)</span><span class="sxs-lookup"><span data-stu-id="37f6a-146">Status (HoldStatusType)</span></span>](status-holdstatustype.md)
    
- [<span data-ttu-id="37f6a-147">аддитионалинфо</span><span class="sxs-lookup"><span data-stu-id="37f6a-147">AdditionalInfo</span></span>](additionalinfo.md)
    
## <a name="getholdonmailboxes-operation-error-response"></a><span data-ttu-id="37f6a-148">Ответ об ошибке операции GetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="37f6a-148">GetHoldOnMailboxes operation error response</span></span>

<span data-ttu-id="37f6a-149">В следующем примере показан ответ об ошибке для запроса операции **GetHoldOnMailboxes** .</span><span class="sxs-lookup"><span data-stu-id="37f6a-149">The following example shows an error response to a **GetHoldOnMailboxes** operation request.</span></span> <span data-ttu-id="37f6a-150">Это ответ на запрос на получение удержания, которое было удалено.</span><span class="sxs-lookup"><span data-stu-id="37f6a-150">This is a response to a request to get a hold that has been deleted.</span></span> 
  
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
      <GetHoldOnMailboxesResponse ResponseClass="Error" 
                                  xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>The specific query-based hold is not found.</MessageText>
         <ResponseCode>ErrorMailboxHoldNotFound</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
      </GetHoldOnMailboxesResponse>
   </s:Body>
</s:Envelope>

```

<span data-ttu-id="37f6a-151">Основной текст сообщения об ошибке SOAP содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="37f6a-151">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="37f6a-152">жесолдонмаилбоксесреспонсе</span><span class="sxs-lookup"><span data-stu-id="37f6a-152">GetHoldOnMailboxesResponse</span></span>](getholdonmailboxesresponse.md)
    
- [<span data-ttu-id="37f6a-153">мессажетекст</span><span class="sxs-lookup"><span data-stu-id="37f6a-153">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="37f6a-154">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="37f6a-154">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="37f6a-155">дескриптивелинккэй</span><span class="sxs-lookup"><span data-stu-id="37f6a-155">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
<span data-ttu-id="37f6a-156">Дополнительные коды ошибок, которые являются общими для EWS и специфичными для этой операции, можно найти в разделе [респонсекоде](responsecode.md).</span><span class="sxs-lookup"><span data-stu-id="37f6a-156">For additional error codes that are generic to EWS and specific to this operation, see [ResponseCode](responsecode.md).</span></span>
  
## <a name="see-also"></a><span data-ttu-id="37f6a-157">См. также</span><span class="sxs-lookup"><span data-stu-id="37f6a-157">See also</span></span>

- [<span data-ttu-id="37f6a-158">Операции EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="37f6a-158">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
    
- [<span data-ttu-id="37f6a-159">Операция GetSearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="37f6a-159">GetSearchableMailboxes operation</span></span>](getsearchablemailboxes-operation.md)
    
- [<span data-ttu-id="37f6a-160">Операция SearchMailboxes</span><span class="sxs-lookup"><span data-stu-id="37f6a-160">SearchMailboxes operation</span></span>](searchmailboxes-operation.md)
    
- [<span data-ttu-id="37f6a-161">Операция SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="37f6a-161">SetHoldOnMailboxes operation</span></span>](setholdonmailboxes-operation.md)
    
- [<span data-ttu-id="37f6a-162">Операция GetDiscoverySearchConfiguration</span><span class="sxs-lookup"><span data-stu-id="37f6a-162">GetDiscoverySearchConfiguration operation</span></span>](getdiscoverysearchconfiguration-operation.md)
    
- [<span data-ttu-id="37f6a-163">Операция GetNonIndexableItemDetails</span><span class="sxs-lookup"><span data-stu-id="37f6a-163">GetNonIndexableItemDetails operation</span></span>](getnonindexableitemdetails-operation.md)
    
- [<span data-ttu-id="37f6a-164">Операция GetNonIndexableItemStatistics</span><span class="sxs-lookup"><span data-stu-id="37f6a-164">GetNonIndexableItemStatistics operation</span></span>](getnonindexableitemstatistics-operation.md)
    

