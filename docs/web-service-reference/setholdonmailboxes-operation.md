---
title: Операция SetHoldOnMailboxes
manager: sethgros
ms.date: 01/24/2020
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 9015a0d8-3495-461b-aa79-797d23169585
description: Поиск сведений о SetHoldOnMailboxesной операции EWS.
ms.openlocfilehash: 4d79ba9f616974b9415ae9eae23b8f5fdb0ab205
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44448396"
---
# <a name="setholdonmailboxes-operation"></a><span data-ttu-id="7265f-103">Операция SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="7265f-103">SetHoldOnMailboxes operation</span></span>

> [!IMPORTANT]
> <span data-ttu-id="7265f-104">Начиная с 1 апреля 2020, операция SetHoldOnMailboxes больше не будет доступна в Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="7265f-104">Starting on April 1, 2020, the SetHoldOnMailboxes operation will no longer be available in Exchange Online.</span></span> <span data-ttu-id="7265f-105">Эта операция не будет затронута в локальных версиях Exchange Server.</span><span class="sxs-lookup"><span data-stu-id="7265f-105">This operation won't be affected in on-premises versions of Exchange Server.</span></span> <span data-ttu-id="7265f-106">Дополнительные сведения см. [в статье выбытие средств прежних версий электронных данных в Exchange Online](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#getsearchablemailboxes-setholdonmailboxes-and-getholdonmailboxes-operations-in-the-ews-api).</span><span class="sxs-lookup"><span data-stu-id="7265f-106">For more information, see [Retirement of legacy eDiscovery tools in Exchange Online](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#getsearchablemailboxes-setholdonmailboxes-and-getholdonmailboxes-operations-in-the-ews-api).</span></span>

<span data-ttu-id="7265f-107">Поиск сведений о **SetHoldOnMailboxesной** операции EWS.</span><span class="sxs-lookup"><span data-stu-id="7265f-107">Find information about the **SetHoldOnMailboxes** EWS operation.</span></span> 
  
<span data-ttu-id="7265f-108">Операция **SetHoldOnMailboxes** задает политику хранения почтовых ящиков в почтовых ящиках.</span><span class="sxs-lookup"><span data-stu-id="7265f-108">The **SetHoldOnMailboxes** operation sets a mailbox hold policy on mailboxes.</span></span> 
  
<span data-ttu-id="7265f-109">Эта операция появилась в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="7265f-109">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-setholdonmailboxes-operation"></a><span data-ttu-id="7265f-110">Использование операции SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="7265f-110">Using the SetHoldOnMailboxes operation</span></span>

<span data-ttu-id="7265f-111">Операция **SetHoldOnMailboxes** устанавливает для почтового ящика один или несколько почтовых ящиков.</span><span class="sxs-lookup"><span data-stu-id="7265f-111">The **SetHoldOnMailboxes** operation sets a mailbox hold on to one or more mailboxes.</span></span> 
  
### <a name="setholdonmailboxes-operation-soap-headers"></a><span data-ttu-id="7265f-112">Заголовки SOAP операции SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="7265f-112">SetHoldOnMailboxes operation SOAP headers</span></span>

<span data-ttu-id="7265f-113">Операция **SetHoldOnMailboxes** может использовать заголовки SOAP, указанные в приведенной ниже таблице.</span><span class="sxs-lookup"><span data-stu-id="7265f-113">The **SetHoldOnMailboxes** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="7265f-114">**Имя заголовка**</span><span class="sxs-lookup"><span data-stu-id="7265f-114">**Header name**</span></span>|<span data-ttu-id="7265f-115">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="7265f-115">**Element**</span></span>|<span data-ttu-id="7265f-116">**Описание**</span><span class="sxs-lookup"><span data-stu-id="7265f-116">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="7265f-117">**ManagementRole**</span><span class="sxs-lookup"><span data-stu-id="7265f-117">**ManagementRole**</span></span> <br/> |[<span data-ttu-id="7265f-118">ManagementRole</span><span class="sxs-lookup"><span data-stu-id="7265f-118">ManagementRole</span></span>](managementrole.md) <br/> |<span data-ttu-id="7265f-119">Определяет роли сервера, необходимые для того, чтобы вызывающий абонент мог выполнить запрос.</span><span class="sxs-lookup"><span data-stu-id="7265f-119">Identifies the server roles that are necessary in order for the caller to make the request.</span></span> <span data-ttu-id="7265f-120">Этот заголовок является применимым для запроса.</span><span class="sxs-lookup"><span data-stu-id="7265f-120">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="7265f-121">**рекуестверсион**</span><span class="sxs-lookup"><span data-stu-id="7265f-121">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="7265f-122">рекуестсерверверсион</span><span class="sxs-lookup"><span data-stu-id="7265f-122">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="7265f-123">Определяет версию схемы для запроса операции.</span><span class="sxs-lookup"><span data-stu-id="7265f-123">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="7265f-124">Этот заголовок является применимым для запроса.</span><span class="sxs-lookup"><span data-stu-id="7265f-124">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="7265f-125">**серверверсион**</span><span class="sxs-lookup"><span data-stu-id="7265f-125">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="7265f-126">серверверсионинфо</span><span class="sxs-lookup"><span data-stu-id="7265f-126">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="7265f-127">Определяет версию сервера, который ответил на запрос.</span><span class="sxs-lookup"><span data-stu-id="7265f-127">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="7265f-128">Этот заголовок является применимым для отклика.</span><span class="sxs-lookup"><span data-stu-id="7265f-128">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="setholdonmailboxes-operation-request-example-apply-a-hold-on-a-mailbox"></a><span data-ttu-id="7265f-129">Пример запроса операции SetHoldOnMailboxes: применение удержания для почтового ящика</span><span class="sxs-lookup"><span data-stu-id="7265f-129">SetHoldOnMailboxes operation request example: Apply a hold on a mailbox</span></span>

<span data-ttu-id="7265f-130">В приведенном ниже примере запроса операции **SetHoldOnMailboxes** показано, как применить удержание к двум почтовым ящикам.</span><span class="sxs-lookup"><span data-stu-id="7265f-130">The following example of a **SetHoldOnMailboxes** operation request shows how to apply a hold on two mailboxes.</span></span> <span data-ttu-id="7265f-131">Удержание почтовых ящиков создано с помощью команды [New – MailboxSearch](https://technet.microsoft.com/library/dd298064.aspx) .</span><span class="sxs-lookup"><span data-stu-id="7265f-131">The mailbox hold was created by using the [New-MailboxSearch](https://technet.microsoft.com/library/dd298064.aspx) command.</span></span> 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
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

<span data-ttu-id="7265f-132">Текст SOAP Request содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="7265f-132">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="7265f-133">SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="7265f-133">SetHoldOnMailboxes</span></span>](setholdonmailboxes.md)
    
- [<span data-ttu-id="7265f-134">Себя (Холдактионтипе)</span><span class="sxs-lookup"><span data-stu-id="7265f-134">ActionType (HoldActionType)</span></span>](actiontype-holdactiontype.md)
    
- [<span data-ttu-id="7265f-135">холдид</span><span class="sxs-lookup"><span data-stu-id="7265f-135">HoldId</span></span>](holdid.md)
    
- [<span data-ttu-id="7265f-136">Query</span><span class="sxs-lookup"><span data-stu-id="7265f-136">Query</span></span>](query.md)
    
- [<span data-ttu-id="7265f-137">Почтовые ящики (Аррайофстрингстипе)</span><span class="sxs-lookup"><span data-stu-id="7265f-137">Mailboxes (ArrayOfStringsType)</span></span>](mailboxes-arrayofstringstype.md)
    
- [<span data-ttu-id="7265f-138">String</span><span class="sxs-lookup"><span data-stu-id="7265f-138">String</span></span>](string.md)
    
- [<span data-ttu-id="7265f-139">Language</span><span class="sxs-lookup"><span data-stu-id="7265f-139">Language</span></span>](language.md)
    
- [<span data-ttu-id="7265f-140">инклуденониндексаблеитемс</span><span class="sxs-lookup"><span data-stu-id="7265f-140">IncludeNonIndexableItems</span></span>](includenonindexableitems.md)
    
- [<span data-ttu-id="7265f-141">Дедупликацию</span><span class="sxs-lookup"><span data-stu-id="7265f-141">Deduplication</span></span>](deduplication.md)
    
## <a name="successful-setholdonmailboxes-operation-response"></a><span data-ttu-id="7265f-142">Успешный отклик операции SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="7265f-142">Successful SetHoldOnMailboxes operation response</span></span>

<span data-ttu-id="7265f-143">В следующем примере показан успешный ответ на запрос операции **SetHoldOnMailboxes** для размещения двух почтовых ящиков на удержании.</span><span class="sxs-lookup"><span data-stu-id="7265f-143">The following example shows a successful response to a **SetHoldOnMailboxes** operation request to put two mailboxes on hold.</span></span> 
  
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
      <SetHoldOnMailboxesResponse ResponseClass="Success" 
                                  xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
         <MailboxHoldResult>
            <HoldId xmlns="https://schemas.microsoft.com/exchange/services/2006/types">HoldId2</HoldId>
            <Query xmlns="https://schemas.microsoft.com/exchange/services/2006/types">test</Query>
            <MailboxHoldStatuses xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
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

<span data-ttu-id="7265f-144">Тело SOAP отклика содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="7265f-144">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="7265f-145">сесолдонмаилбоксесреспонсе</span><span class="sxs-lookup"><span data-stu-id="7265f-145">SetHoldOnMailboxesResponse</span></span>](setholdonmailboxesresponse.md)
    
- [<span data-ttu-id="7265f-146">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="7265f-146">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="7265f-147">маилбоксхолдресулт</span><span class="sxs-lookup"><span data-stu-id="7265f-147">MailboxHoldResult</span></span>](mailboxholdresult.md)
    
- [<span data-ttu-id="7265f-148">холдид</span><span class="sxs-lookup"><span data-stu-id="7265f-148">HoldId</span></span>](holdid.md)
    
- [<span data-ttu-id="7265f-149">Query</span><span class="sxs-lookup"><span data-stu-id="7265f-149">Query</span></span>](query.md)
    
- [<span data-ttu-id="7265f-150">маилбоксхолдстатусес</span><span class="sxs-lookup"><span data-stu-id="7265f-150">MailboxHoldStatuses</span></span>](mailboxholdstatuses.md)
    
- [<span data-ttu-id="7265f-151">маилбоксхолдстатус</span><span class="sxs-lookup"><span data-stu-id="7265f-151">MailboxHoldStatus</span></span>](mailboxholdstatus.md)
    
- [<span data-ttu-id="7265f-152">Mailbox (строка)</span><span class="sxs-lookup"><span data-stu-id="7265f-152">Mailbox (string)</span></span>](mailbox-string.md)
    
- [<span data-ttu-id="7265f-153">Состояние (Холдстатустипе)</span><span class="sxs-lookup"><span data-stu-id="7265f-153">Status (HoldStatusType)</span></span>](status-holdstatustype.md)
    
- [<span data-ttu-id="7265f-154">аддитионалинфо</span><span class="sxs-lookup"><span data-stu-id="7265f-154">AdditionalInfo</span></span>](additionalinfo.md)
    
## <a name="setholdonmailboxes-operation-error-response"></a><span data-ttu-id="7265f-155">Ответ об ошибке операции SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="7265f-155">SetHoldOnMailboxes operation error response</span></span>

<span data-ttu-id="7265f-156">В следующем примере показан ответ об ошибке для запроса операции **SetHoldOnMailboxes** .</span><span class="sxs-lookup"><span data-stu-id="7265f-156">The following example shows an error response to a **SetHoldOnMailboxes** operation request.</span></span> <span data-ttu-id="7265f-157">Это ответ на запрос, который содержит неправильно указанный идентификатор почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="7265f-157">This is a response to a request that contains an incorrectly specified mailbox identifier.</span></span> 
  
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
      <SetHoldOnMailboxesResponse ResponseClass="Error" 
                                  xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>No mailbox is specified for hold operation. If specified in the request, then it could be the object does not exist in AD or is a Distribution Group.</MessageText>
         <ResponseCode>ErrorInvalidOperation</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
      </SetHoldOnMailboxesResponse>
   </s:Body>
</s:Envelope>

```

<span data-ttu-id="7265f-158">Основной текст сообщения об ошибке SOAP содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="7265f-158">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="7265f-159">сесолдонмаилбоксесреспонсе</span><span class="sxs-lookup"><span data-stu-id="7265f-159">SetHoldOnMailboxesResponse</span></span>](setholdonmailboxesresponse.md)
    
- [<span data-ttu-id="7265f-160">мессажетекст</span><span class="sxs-lookup"><span data-stu-id="7265f-160">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="7265f-161">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="7265f-161">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="7265f-162">дескриптивелинккэй</span><span class="sxs-lookup"><span data-stu-id="7265f-162">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
<span data-ttu-id="7265f-163">Дополнительные коды ошибок, которые являются общими для EWS и специфичными для этой операции, можно найти в разделе [респонсекоде](responsecode.md).</span><span class="sxs-lookup"><span data-stu-id="7265f-163">For additional error codes that are generic to EWS and specific to this operation, see [ResponseCode](responsecode.md).</span></span>
  
## <a name="see-also"></a><span data-ttu-id="7265f-164">См. также</span><span class="sxs-lookup"><span data-stu-id="7265f-164">See also</span></span>

- [<span data-ttu-id="7265f-165">Операции EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="7265f-165">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
    
- [<span data-ttu-id="7265f-166">Операция GetSearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="7265f-166">GetSearchableMailboxes operation</span></span>](getsearchablemailboxes-operation.md)
    
- [<span data-ttu-id="7265f-167">Операция SearchMailboxes</span><span class="sxs-lookup"><span data-stu-id="7265f-167">SearchMailboxes operation</span></span>](searchmailboxes-operation.md)
    
- [<span data-ttu-id="7265f-168">Операция GetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="7265f-168">GetHoldOnMailboxes operation</span></span>](getholdonmailboxes-operation.md)
    
- [<span data-ttu-id="7265f-169">Операция GetDiscoverySearchConfiguration</span><span class="sxs-lookup"><span data-stu-id="7265f-169">GetDiscoverySearchConfiguration operation</span></span>](getdiscoverysearchconfiguration-operation.md)
    
- [<span data-ttu-id="7265f-170">Операция GetNonIndexableItemDetails</span><span class="sxs-lookup"><span data-stu-id="7265f-170">GetNonIndexableItemDetails operation</span></span>](getnonindexableitemdetails-operation.md)
    
- [<span data-ttu-id="7265f-171">Операция GetNonIndexableItemStatistics</span><span class="sxs-lookup"><span data-stu-id="7265f-171">GetNonIndexableItemStatistics operation</span></span>](getnonindexableitemstatistics-operation.md)
    

