---
title: Операция SetHoldOnMailboxes
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 9015a0d8-3495-461b-aa79-797d23169585
description: Поиск сведений о SetHoldOnMailboxesной операции EWS.
ms.openlocfilehash: 1091ed14ceb25dfd275499b9db47ae4e41b5f1a0
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835412"
---
# <a name="setholdonmailboxes-operation"></a><span data-ttu-id="79b18-103">Операция SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="79b18-103">SetHoldOnMailboxes operation</span></span>

<span data-ttu-id="79b18-104">Поиск сведений о **SetHoldOnMailboxesной** операции EWS.</span><span class="sxs-lookup"><span data-stu-id="79b18-104">Find information about the **SetHoldOnMailboxes** EWS operation.</span></span> 
  
<span data-ttu-id="79b18-105">Операция **SetHoldOnMailboxes** задает политику хранения почтовых ящиков в почтовых ящиках.</span><span class="sxs-lookup"><span data-stu-id="79b18-105">The **SetHoldOnMailboxes** operation sets a mailbox hold policy on mailboxes.</span></span> 
  
<span data-ttu-id="79b18-106">Эта операция появилась в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="79b18-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-setholdonmailboxes-operation"></a><span data-ttu-id="79b18-107">Использование операции SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="79b18-107">Using the SetHoldOnMailboxes operation</span></span>

<span data-ttu-id="79b18-108">Операция **SetHoldOnMailboxes** устанавливает для почтового ящика один или несколько почтовых ящиков.</span><span class="sxs-lookup"><span data-stu-id="79b18-108">The **SetHoldOnMailboxes** operation sets a mailbox hold on to one or more mailboxes.</span></span> 
  
### <a name="setholdonmailboxes-operation-soap-headers"></a><span data-ttu-id="79b18-109">Заголовки SOAP операции SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="79b18-109">SetHoldOnMailboxes operation SOAP headers</span></span>

<span data-ttu-id="79b18-110">Операция **SetHoldOnMailboxes** может использовать заголовки SOAP, указанные в приведенной ниже таблице.</span><span class="sxs-lookup"><span data-stu-id="79b18-110">The **SetHoldOnMailboxes** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="79b18-111">**Имя заголовка**</span><span class="sxs-lookup"><span data-stu-id="79b18-111">**Header name**</span></span>|<span data-ttu-id="79b18-112">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="79b18-112">**Element**</span></span>|<span data-ttu-id="79b18-113">**Описание**</span><span class="sxs-lookup"><span data-stu-id="79b18-113">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="79b18-114">**ManagementRole**</span><span class="sxs-lookup"><span data-stu-id="79b18-114">**ManagementRole**</span></span> <br/> |[<span data-ttu-id="79b18-115">ManagementRole</span><span class="sxs-lookup"><span data-stu-id="79b18-115">ManagementRole</span></span>](managementrole.md) <br/> |<span data-ttu-id="79b18-116">Определяет роли сервера, необходимые для того, чтобы вызывающий абонент мог выполнить запрос.</span><span class="sxs-lookup"><span data-stu-id="79b18-116">Identifies the server roles that are necessary in order for the caller to make the request.</span></span> <span data-ttu-id="79b18-117">Этот заголовок является применимым для запроса.</span><span class="sxs-lookup"><span data-stu-id="79b18-117">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="79b18-118">**рекуестверсион**</span><span class="sxs-lookup"><span data-stu-id="79b18-118">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="79b18-119">рекуестсерверверсион</span><span class="sxs-lookup"><span data-stu-id="79b18-119">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="79b18-120">Определяет версию схемы для запроса операции.</span><span class="sxs-lookup"><span data-stu-id="79b18-120">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="79b18-121">Этот заголовок является применимым для запроса.</span><span class="sxs-lookup"><span data-stu-id="79b18-121">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="79b18-122">**серверверсион**</span><span class="sxs-lookup"><span data-stu-id="79b18-122">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="79b18-123">серверверсионинфо</span><span class="sxs-lookup"><span data-stu-id="79b18-123">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="79b18-124">Определяет версию сервера, который ответил на запрос.</span><span class="sxs-lookup"><span data-stu-id="79b18-124">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="79b18-125">Этот заголовок является применимым для отклика.</span><span class="sxs-lookup"><span data-stu-id="79b18-125">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="setholdonmailboxes-operation-request-example-apply-a-hold-on-a-mailbox"></a><span data-ttu-id="79b18-126">Пример запроса операции SetHoldOnMailboxes: применение удержания для почтового ящика</span><span class="sxs-lookup"><span data-stu-id="79b18-126">SetHoldOnMailboxes operation request example: Apply a hold on a mailbox</span></span>

<span data-ttu-id="79b18-127">В приведенном ниже примере запроса операции **SetHoldOnMailboxes** показано, как применить удержание к двум почтовым ящикам.</span><span class="sxs-lookup"><span data-stu-id="79b18-127">The following example of a **SetHoldOnMailboxes** operation request shows how to apply a hold on two mailboxes.</span></span> <span data-ttu-id="79b18-128">Удержание почтовых ящиков создано с помощью команды [New – MailboxSearch](http://technet.microsoft.com/en-us/library/dd298064.aspx) .</span><span class="sxs-lookup"><span data-stu-id="79b18-128">The mailbox hold was created by using the [New-MailboxSearch](http://technet.microsoft.com/en-us/library/dd298064.aspx) command.</span></span> 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013" />
   </soap:Header>
   <soap:Body >
      <m:SetHoldOnMailboxes>
         <m:ActionType>Create</m:ActionType>
         <m:HoldId>HoldId2</m:HoldId>
         <m:Query>test</m:Query>
         <m:Mailboxes>
            <t:String>/o=First/ou=Exchange(DLT)/cn=Recipients/cn=1fa441ff5e4749ba43ecc0fd94c21adf-Willi</t:String>
            <t:String>/o=First/ou=Exchange(DLT)/cn=Recipients/cn=aed2346adaa34ffc9f0f339917e8de95-Micha</t:String>
         </m:Mailboxes>
         <m:Language>English</m:Language>
         <m:IncludeNonIndexableItems>false</m:IncludeNonIndexableItems>
         <m:Deduplication>true</m:Deduplication>
      </m:SetHoldOnMailboxes>
   </soap:Body>
</soap:Envelope>

```

<span data-ttu-id="79b18-129">Текст SOAP Request содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="79b18-129">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="79b18-130">SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="79b18-130">SetHoldOnMailboxes</span></span>](setholdonmailboxes.md)
    
- [<span data-ttu-id="79b18-131">Себя (Холдактионтипе)</span><span class="sxs-lookup"><span data-stu-id="79b18-131">ActionType (HoldActionType)</span></span>](actiontype-holdactiontype.md)
    
- [<span data-ttu-id="79b18-132">холдид</span><span class="sxs-lookup"><span data-stu-id="79b18-132">HoldId</span></span>](holdid.md)
    
- [<span data-ttu-id="79b18-133">Query</span><span class="sxs-lookup"><span data-stu-id="79b18-133">Query</span></span>](query.md)
    
- [<span data-ttu-id="79b18-134">Почтовые ящики (Аррайофстрингстипе)</span><span class="sxs-lookup"><span data-stu-id="79b18-134">Mailboxes (ArrayOfStringsType)</span></span>](mailboxes-arrayofstringstype.md)
    
- [<span data-ttu-id="79b18-135">String</span><span class="sxs-lookup"><span data-stu-id="79b18-135">String</span></span>](string.md)
    
- [<span data-ttu-id="79b18-136">Язык</span><span class="sxs-lookup"><span data-stu-id="79b18-136">Language</span></span>](language.md)
    
- [<span data-ttu-id="79b18-137">инклуденониндексаблеитемс</span><span class="sxs-lookup"><span data-stu-id="79b18-137">IncludeNonIndexableItems</span></span>](includenonindexableitems.md)
    
- [<span data-ttu-id="79b18-138">Дедупликацию</span><span class="sxs-lookup"><span data-stu-id="79b18-138">Deduplication</span></span>](deduplication.md)
    
## <a name="successful-setholdonmailboxes-operation-response"></a><span data-ttu-id="79b18-139">Успешный отклик операции SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="79b18-139">Successful SetHoldOnMailboxes operation response</span></span>

<span data-ttu-id="79b18-140">В следующем примере показан успешный ответ на запрос операции **SetHoldOnMailboxes** для размещения двух почтовых ящиков на удержании.</span><span class="sxs-lookup"><span data-stu-id="79b18-140">The following example shows a successful response to a **SetHoldOnMailboxes** operation request to put two mailboxes on hold.</span></span> 
  
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
      <SetHoldOnMailboxesResponse ResponseClass="Success" 
                                  xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
         <MailboxHoldResult>
            <HoldId xmlns="http://schemas.microsoft.com/exchange/services/2006/types">HoldId2</HoldId>
            <Query xmlns="http://schemas.microsoft.com/exchange/services/2006/types">test</Query>
            <MailboxHoldStatuses xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
               <MailboxHoldStatus>
                  <Mailbox>o=First/ou=Exchange(DLT)/cn=Recipients/cn=1fa441ff5e4749ba43ecc0fd94c21adf-Willi</Mailbox>
                  <Status>Pending</Status>
                  <AdditionalInfo/>
               </MailboxHoldStatus>
               <MailboxHoldStatus>
                  <Mailbox>/o=First/ou=Exchange(DLT)/cn=Recipients/cn=aed2346adaa34ffc9f0f339917e8de95-Micha</Mailbox>
                  <Status>Pending</Status>
                  <AdditionalInfo/>
               </MailboxHoldStatus>
            </MailboxHoldStatuses>
         </MailboxHoldResult>
      </SetHoldOnMailboxesResponse>
   </s:Body>
</s:Envelope>

```

<span data-ttu-id="79b18-141">Тело SOAP отклика содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="79b18-141">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="79b18-142">сесолдонмаилбоксесреспонсе</span><span class="sxs-lookup"><span data-stu-id="79b18-142">SetHoldOnMailboxesResponse</span></span>](setholdonmailboxesresponse.md)
    
- [<span data-ttu-id="79b18-143">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="79b18-143">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="79b18-144">маилбоксхолдресулт</span><span class="sxs-lookup"><span data-stu-id="79b18-144">MailboxHoldResult</span></span>](mailboxholdresult.md)
    
- [<span data-ttu-id="79b18-145">холдид</span><span class="sxs-lookup"><span data-stu-id="79b18-145">HoldId</span></span>](holdid.md)
    
- [<span data-ttu-id="79b18-146">Query</span><span class="sxs-lookup"><span data-stu-id="79b18-146">Query</span></span>](query.md)
    
- [<span data-ttu-id="79b18-147">маилбоксхолдстатусес</span><span class="sxs-lookup"><span data-stu-id="79b18-147">MailboxHoldStatuses</span></span>](mailboxholdstatuses.md)
    
- [<span data-ttu-id="79b18-148">маилбоксхолдстатус</span><span class="sxs-lookup"><span data-stu-id="79b18-148">MailboxHoldStatus</span></span>](mailboxholdstatus.md)
    
- [<span data-ttu-id="79b18-149">Mailbox (строка)</span><span class="sxs-lookup"><span data-stu-id="79b18-149">Mailbox (string)</span></span>](mailbox-string.md)
    
- [<span data-ttu-id="79b18-150">Состояние (Холдстатустипе)</span><span class="sxs-lookup"><span data-stu-id="79b18-150">Status (HoldStatusType)</span></span>](status-holdstatustype.md)
    
- [<span data-ttu-id="79b18-151">аддитионалинфо</span><span class="sxs-lookup"><span data-stu-id="79b18-151">AdditionalInfo</span></span>](additionalinfo.md)
    
## <a name="setholdonmailboxes-operation-error-response"></a><span data-ttu-id="79b18-152">Ответ об ошибке операции SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="79b18-152">SetHoldOnMailboxes operation error response</span></span>

<span data-ttu-id="79b18-153">В следующем примере показан ответ об ошибке для запроса операции **SetHoldOnMailboxes** .</span><span class="sxs-lookup"><span data-stu-id="79b18-153">The following example shows an error response to a **SetHoldOnMailboxes** operation request.</span></span> <span data-ttu-id="79b18-154">Это ответ на запрос, который содержит неправильно указанный идентификатор почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="79b18-154">This is a response to a request that contains an incorrectly specified mailbox identifier.</span></span> 
  
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
      <SetHoldOnMailboxesResponse ResponseClass="Error" 
                                  xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>No mailbox is specified for hold operation. If specified in the request, then it could be the object does not exist in AD or is a Distribution Group.</MessageText>
         <ResponseCode>ErrorInvalidOperation</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
      </SetHoldOnMailboxesResponse>
   </s:Body>
</s:Envelope>

```

<span data-ttu-id="79b18-155">Основной текст сообщения об ошибке SOAP содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="79b18-155">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="79b18-156">сесолдонмаилбоксесреспонсе</span><span class="sxs-lookup"><span data-stu-id="79b18-156">SetHoldOnMailboxesResponse</span></span>](setholdonmailboxesresponse.md)
    
- [<span data-ttu-id="79b18-157">мессажетекст</span><span class="sxs-lookup"><span data-stu-id="79b18-157">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="79b18-158">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="79b18-158">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="79b18-159">дескриптивелинккэй</span><span class="sxs-lookup"><span data-stu-id="79b18-159">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
<span data-ttu-id="79b18-160">Дополнительные коды ошибок, которые являются общими для EWS и специфичными для этой операции, можно найти в разделе [респонсекоде](responsecode.md).</span><span class="sxs-lookup"><span data-stu-id="79b18-160">For additional error codes that are generic to EWS and specific to this operation, see [ResponseCode](responsecode.md).</span></span>
  
## <a name="see-also"></a><span data-ttu-id="79b18-161">См. также</span><span class="sxs-lookup"><span data-stu-id="79b18-161">See also</span></span>

- [<span data-ttu-id="79b18-162">Операции EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="79b18-162">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
    
- [<span data-ttu-id="79b18-163">Операция GetSearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="79b18-163">GetSearchableMailboxes operation</span></span>](getsearchablemailboxes-operation.md)
    
- [<span data-ttu-id="79b18-164">Операция SearchMailboxes</span><span class="sxs-lookup"><span data-stu-id="79b18-164">SearchMailboxes operation</span></span>](searchmailboxes-operation.md)
    
- [<span data-ttu-id="79b18-165">Операция GetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="79b18-165">GetHoldOnMailboxes operation</span></span>](getholdonmailboxes-operation.md)
    
- [<span data-ttu-id="79b18-166">Операция GetDiscoverySearchConfiguration</span><span class="sxs-lookup"><span data-stu-id="79b18-166">GetDiscoverySearchConfiguration operation</span></span>](getdiscoverysearchconfiguration-operation.md)
    
- [<span data-ttu-id="79b18-167">Операция GetNonIndexableItemDetails</span><span class="sxs-lookup"><span data-stu-id="79b18-167">GetNonIndexableItemDetails operation</span></span>](getnonindexableitemdetails-operation.md)
    
- [<span data-ttu-id="79b18-168">Операция GetNonIndexableItemStatistics</span><span class="sxs-lookup"><span data-stu-id="79b18-168">GetNonIndexableItemStatistics operation</span></span>](getnonindexableitemstatistics-operation.md)
    

