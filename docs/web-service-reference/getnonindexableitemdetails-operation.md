---
title: Операция GetNonIndexableItemDetails
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 9279c3ad-f7c8-4bbc-b0a7-2c78416cb39a
description: Поиск сведений о GetNonIndexableItemDetailsной операции EWS.
ms.openlocfilehash: 6b0c5afd54ac98f89bc6c5199300c20862c6f207
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762857"
---
# <a name="getnonindexableitemdetails-operation"></a><span data-ttu-id="bc15d-103">Операция GetNonIndexableItemDetails</span><span class="sxs-lookup"><span data-stu-id="bc15d-103">GetNonIndexableItemDetails operation</span></span>

<span data-ttu-id="bc15d-104">Поиск сведений о **GetNonIndexableItemDetailsной** операции EWS.</span><span class="sxs-lookup"><span data-stu-id="bc15d-104">Find information about the **GetNonIndexableItemDetails** EWS operation.</span></span> 
  
<span data-ttu-id="bc15d-105">Операция **GetNonIndexableItemDetails** получает сведения об элементах, которые не удается индексировать.</span><span class="sxs-lookup"><span data-stu-id="bc15d-105">The **GetNonIndexableItemDetails** operation retrieves details about items that cannot be indexed.</span></span> <span data-ttu-id="bc15d-106">Это относится только к идентификатору элемента, к коду ошибки, описанию ошибки, при попытке индексирования элемента и дополнительной информации о файле.</span><span class="sxs-lookup"><span data-stu-id="bc15d-106">This includes, but is not limited to, the item identifier, an error code, an error description, when an attempt was made to index the item, and additional information about the file.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="bc15d-107">Несмотря на то что схема указывает на то, что можно выполнять поиск в нескольких почтовых ящиках, в исходной версии Exchange 2013 служба поддерживает только извлечение сведений об элементах для неиндексируемых элементов в одном почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="bc15d-107">Although the schema indicates that more than one mailbox can be searched, in the initial release version of Exchange 2013, the service only supports getting item details for nonindexable items in a single mailbox.</span></span> 
  
<span data-ttu-id="bc15d-108">Эта операция появилась в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="bc15d-108">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-getnonindexableitemdetails-operation"></a><span data-ttu-id="bc15d-109">Использование операции GetNonIndexableItemDetails</span><span class="sxs-lookup"><span data-stu-id="bc15d-109">Using the GetNonIndexableItemDetails operation</span></span>

<span data-ttu-id="bc15d-110">Операция **GetNonIndexableItemDetails** определяет элементы почтового ящика, которые не удается индексировать, и предоставляет сведения о причинах, по которым не удается индексировать элементы.</span><span class="sxs-lookup"><span data-stu-id="bc15d-110">The **GetNonIndexableItemDetails** operation identifies mailbox items that cannot be indexed and provides information about why the items cannot be indexed.</span></span> <span data-ttu-id="bc15d-111">Элементы, которые не могут индексироваться, не ищутся во время поиска обнаружения.</span><span class="sxs-lookup"><span data-stu-id="bc15d-111">Items that cannot be indexed are not searched during a discovery search.</span></span> 
  
### <a name="getnonindexableitemdetails-operation-soap-headers"></a><span data-ttu-id="bc15d-112">Заголовки SOAP операции GetNonIndexableItemDetails</span><span class="sxs-lookup"><span data-stu-id="bc15d-112">GetNonIndexableItemDetails operation SOAP headers</span></span>

<span data-ttu-id="bc15d-113">Операция **GetNonIndexableItemDetails** может использовать заголовки SOAP, указанные в приведенной ниже таблице.</span><span class="sxs-lookup"><span data-stu-id="bc15d-113">The **GetNonIndexableItemDetails** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="bc15d-114">**Имя заголовка**</span><span class="sxs-lookup"><span data-stu-id="bc15d-114">**Header name**</span></span>|<span data-ttu-id="bc15d-115">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="bc15d-115">**Element**</span></span>|<span data-ttu-id="bc15d-116">**Описание**</span><span class="sxs-lookup"><span data-stu-id="bc15d-116">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="bc15d-117">**ManagementRole**</span><span class="sxs-lookup"><span data-stu-id="bc15d-117">**ManagementRole**</span></span> <br/> |[<span data-ttu-id="bc15d-118">ManagementRole</span><span class="sxs-lookup"><span data-stu-id="bc15d-118">ManagementRole</span></span>](managementrole.md) <br/> |<span data-ttu-id="bc15d-119">Определяет роли сервера, необходимые для того, чтобы вызывающий абонент мог выполнить запрос.</span><span class="sxs-lookup"><span data-stu-id="bc15d-119">Identifies the server roles that are necessary in order for the caller to make the request.</span></span> <span data-ttu-id="bc15d-120">Этот заголовок является применимым для запроса.</span><span class="sxs-lookup"><span data-stu-id="bc15d-120">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="bc15d-121">**рекуестверсион**</span><span class="sxs-lookup"><span data-stu-id="bc15d-121">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="bc15d-122">рекуестсерверверсион</span><span class="sxs-lookup"><span data-stu-id="bc15d-122">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="bc15d-123">Определяет версию схемы для запроса операции.</span><span class="sxs-lookup"><span data-stu-id="bc15d-123">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="bc15d-124">Этот заголовок является применимым для запроса.</span><span class="sxs-lookup"><span data-stu-id="bc15d-124">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="bc15d-125">**серверверсион**</span><span class="sxs-lookup"><span data-stu-id="bc15d-125">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="bc15d-126">серверверсионинфо</span><span class="sxs-lookup"><span data-stu-id="bc15d-126">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="bc15d-127">Определяет версию сервера, который ответил на запрос.</span><span class="sxs-lookup"><span data-stu-id="bc15d-127">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="bc15d-128">Этот заголовок является применимым для отклика.</span><span class="sxs-lookup"><span data-stu-id="bc15d-128">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="getnonindexableitemdetails-operation-request-example-get-the-details-of-an-item-that-cannot-be-indexed"></a><span data-ttu-id="bc15d-129">Пример запроса операции GetNonIndexableItemDetails: получение сведений о элементе, который не удается индексировать</span><span class="sxs-lookup"><span data-stu-id="bc15d-129">GetNonIndexableItemDetails operation request example: Get the details of an item that cannot be indexed</span></span>

<span data-ttu-id="bc15d-130">В приведенном ниже примере запроса операции **GetNonIndexableItemDetails** показано, как запросить сведения для элементов, которые не удается индексировать для одного почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="bc15d-130">The following example of a **GetNonIndexableItemDetails** operation request shows how to request the details for items that cannot be indexed for a single mailbox.</span></span> <span data-ttu-id="bc15d-131">Поиск выполняется как в основном, так и в архивных почтовых ящиках.</span><span class="sxs-lookup"><span data-stu-id="bc15d-131">The search is performed across both primary and archive mailboxes.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="bc15d-132">Все устаревшие доменные имена в этом примере сокращены, чтобы сохранить удобочитаемость.</span><span class="sxs-lookup"><span data-stu-id="bc15d-132">All legacy domain names in this example have be shortened to preserve readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013" />
   </soap:Header>
   <soap:Body >
      <m:GetNonIndexableItemDetails>
         <m:Mailboxes>
            <t:LegacyDN>/o=First Organization/ou=Exchange Administrative Group (FYT)/cn=Recipients/cn=35-Steve</t:LegacyDN>
         </m:Mailboxes>
         <m:SearchArchiveOnly>false</m:SearchArchiveOnly>
      </m:GetNonIndexableItemDetails>
   </soap:Body>
</soap:Envelope>

```

<span data-ttu-id="bc15d-133">Текст SOAP Request содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="bc15d-133">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="bc15d-134">GetNonIndexableItemDetails</span><span class="sxs-lookup"><span data-stu-id="bc15d-134">GetNonIndexableItemDetails</span></span>](getnonindexableitemdetails.md)
    
- [<span data-ttu-id="bc15d-135">Почтовые ящики (Нонемптяррайофлегациднстипе)</span><span class="sxs-lookup"><span data-stu-id="bc15d-135">Mailboxes (NonEmptyArrayOfLegacyDNsType)</span></span>](mailboxes-nonemptyarrayoflegacydnstype.md)
    
- [<span data-ttu-id="bc15d-136">LegacyDN</span><span class="sxs-lookup"><span data-stu-id="bc15d-136">LegacyDN</span></span>](legacydn.md)
    
- [<span data-ttu-id="bc15d-137">сеарчарчивеонли</span><span class="sxs-lookup"><span data-stu-id="bc15d-137">SearchArchiveOnly</span></span>](searcharchiveonly.md)
    
## <a name="successful-getnonindexableitemdetails-operation-response"></a><span data-ttu-id="bc15d-138">Успешный отклик операции GetNonIndexableItemDetails</span><span class="sxs-lookup"><span data-stu-id="bc15d-138">Successful GetNonIndexableItemDetails operation response</span></span>

<span data-ttu-id="bc15d-139">В следующем примере показан успешный ответ на запрос операции **GetNonIndexableItemDetails** для получения элементов, которые не удается индексировать для одного почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="bc15d-139">The following example shows a successful response to a **GetNonIndexableItemDetails** operation request to get items that cannot be indexed for a single mailbox.</span></span> <span data-ttu-id="bc15d-140">В этом примере элемент, который не удается индексировать, — это файл бинарифиле. ABC, который имеет неизвестный формат.</span><span class="sxs-lookup"><span data-stu-id="bc15d-140">The item in this example that cannot be indexed is the binaryfile.abc file, which is of an unknown format.</span></span> 
  
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
      <GetNonIndexableItemDetailsResponse ResponseClass="Success" 
                                          xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
         <NonIndexableItemDetailsResult>
            <Items xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
               <NonIndexableItemDetail>
                  <ItemId Id="AQMkAGVmNDAyOQAAAY2fUAAAAA==" ChangeKey="CQAAAA=="/>
                  <ErrorCode>DocumentParserFailure</ErrorCode>
                  <ErrorDescription>The document parser encountered a processing error.</ErrorDescription>
                  <IsPartiallyIndexed>false</IsPartiallyIndexed>
                  <IsPermanentFailure>true</IsPermanentFailure>
                  <SortValue>502511175756</SortValue>
                  <AttemptCount>0</AttemptCount>
                  <LastAttemptTime>2012-11-15T01:56:11Z</LastAttemptTime>
                  <AdditionalInfo> 301002 Error parsing document 'exchange://localhost/Attachment/d987b1f4-9aa7-42b3-aa8c-9515a35dfa1a/1f3047d4-c287-41e4-910c-feb70c1a59f0/ef402830-3d33-4a0d-a4e9-d8576900060d/85b83861-0026-418f-8464-be2036696333/502511175756.0/binaryfile.abc'. Document has an undetectable format and will not be parsed.</AdditionalInfo>
               </NonIndexableItemDetail>
            </Items>
         </NonIndexableItemDetailsResult>
      </GetNonIndexableItemDetailsResponse>
   </s:Body>
</s:Envelope>

```

<span data-ttu-id="bc15d-141">Тело SOAP отклика содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="bc15d-141">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="bc15d-142">жетнониндексаблеитемдетаилсреспонсе</span><span class="sxs-lookup"><span data-stu-id="bc15d-142">GetNonIndexableItemDetailsResponse</span></span>](getnonindexableitemdetailsresponse.md)
    
- [<span data-ttu-id="bc15d-143">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="bc15d-143">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="bc15d-144">нониндексаблеитемдетаилсресулт</span><span class="sxs-lookup"><span data-stu-id="bc15d-144">NonIndexableItemDetailsResult</span></span>](nonindexableitemdetailsresult.md)
    
- [<span data-ttu-id="bc15d-145">нониндексаблеитемдетаил</span><span class="sxs-lookup"><span data-stu-id="bc15d-145">NonIndexableItemDetail</span></span>](nonindexableitemdetail.md)
    
- [<span data-ttu-id="bc15d-146">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="bc15d-146">ItemId</span></span>](itemid.md)
    
- [<span data-ttu-id="bc15d-147">ErrorCode (Итеминдексеррортипе)</span><span class="sxs-lookup"><span data-stu-id="bc15d-147">ErrorCode (ItemIndexErrorType)</span></span>](errorcode-itemindexerrortype.md)
    
- [<span data-ttu-id="bc15d-148">еррордескриптион</span><span class="sxs-lookup"><span data-stu-id="bc15d-148">ErrorDescription</span></span>](errordescription.md)
    
- [<span data-ttu-id="bc15d-149">испартиаллиндексед</span><span class="sxs-lookup"><span data-stu-id="bc15d-149">IsPartiallyIndexed</span></span>](ispartiallyindexed.md)
    
- [<span data-ttu-id="bc15d-150">исперманентфаилуре</span><span class="sxs-lookup"><span data-stu-id="bc15d-150">IsPermanentFailure</span></span>](ispermanentfailure.md)
    
- [<span data-ttu-id="bc15d-151">сортвалуе</span><span class="sxs-lookup"><span data-stu-id="bc15d-151">SortValue</span></span>](sortvalue.md)
    
- [<span data-ttu-id="bc15d-152">аттемпткаунт</span><span class="sxs-lookup"><span data-stu-id="bc15d-152">AttemptCount</span></span>](attemptcount.md)
    
- [<span data-ttu-id="bc15d-153">ластаттемпттиме</span><span class="sxs-lookup"><span data-stu-id="bc15d-153">LastAttemptTime</span></span>](lastattempttime.md)
    
- [<span data-ttu-id="bc15d-154">аддитионалинфо</span><span class="sxs-lookup"><span data-stu-id="bc15d-154">AdditionalInfo</span></span>](additionalinfo.md)
    
## <a name="getnonindexableitemdetails-operation-error-response"></a><span data-ttu-id="bc15d-155">Ответ об ошибке операции GetNonIndexableItemDetails</span><span class="sxs-lookup"><span data-stu-id="bc15d-155">GetNonIndexableItemDetails operation error response</span></span>

<span data-ttu-id="bc15d-156">В следующем примере показан ответ об ошибке для запроса операции **GetNonIndexableItemDetails** .</span><span class="sxs-lookup"><span data-stu-id="bc15d-156">The following example shows an error response to a **GetNonIndexableItemDetails** operation request.</span></span> <span data-ttu-id="bc15d-157">Это ответ на запрос получения сведений об элементах, которые не удается индексировать из нескольких почтовых ящиков.</span><span class="sxs-lookup"><span data-stu-id="bc15d-157">This is a response to a request to get item details for items that cannot be indexed from more than one mailbox.</span></span> 
  
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
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <GetNonIndexableItemDetailsResponse ResponseClass="Error" xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>Multiple mailboxes is currently not supported, only single mailbox is supported.</MessageText>
         <ResponseCode>ErrorInvalidArgument</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
      </GetNonIndexableItemDetailsResponse>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="bc15d-158">Основной текст сообщения об ошибке SOAP содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="bc15d-158">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="bc15d-159">жетнониндексаблеитемдетаилсреспонсе</span><span class="sxs-lookup"><span data-stu-id="bc15d-159">GetNonIndexableItemDetailsResponse</span></span>](getnonindexableitemdetailsresponse.md)
    
- [<span data-ttu-id="bc15d-160">мессажетекст</span><span class="sxs-lookup"><span data-stu-id="bc15d-160">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="bc15d-161">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="bc15d-161">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="bc15d-162">дескриптивелинккэй</span><span class="sxs-lookup"><span data-stu-id="bc15d-162">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
<span data-ttu-id="bc15d-163">Дополнительные коды ошибок, которые являются общими для EWS и специфичными для этой операции, можно найти в разделе [респонсекоде](responsecode.md).</span><span class="sxs-lookup"><span data-stu-id="bc15d-163">For additional error codes that are generic to EWS and specific to this operation, see [ResponseCode](responsecode.md).</span></span>
  
## <a name="see-also"></a><span data-ttu-id="bc15d-164">См. также</span><span class="sxs-lookup"><span data-stu-id="bc15d-164">See also</span></span>

- [<span data-ttu-id="bc15d-165">Операции EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="bc15d-165">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
    
- [<span data-ttu-id="bc15d-166">Операция GetSearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="bc15d-166">GetSearchableMailboxes operation</span></span>](getsearchablemailboxes-operation.md)
    
- [<span data-ttu-id="bc15d-167">Операция SearchMailboxes</span><span class="sxs-lookup"><span data-stu-id="bc15d-167">SearchMailboxes operation</span></span>](searchmailboxes-operation.md)
    
- [<span data-ttu-id="bc15d-168">Операция GetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="bc15d-168">GetHoldOnMailboxes operation</span></span>](getholdonmailboxes-operation.md)
    
- [<span data-ttu-id="bc15d-169">Операция SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="bc15d-169">SetHoldOnMailboxes operation</span></span>](setholdonmailboxes-operation.md)
    
- [<span data-ttu-id="bc15d-170">Операция GetDiscoverySearchConfiguration</span><span class="sxs-lookup"><span data-stu-id="bc15d-170">GetDiscoverySearchConfiguration operation</span></span>](getdiscoverysearchconfiguration-operation.md)
    
- [<span data-ttu-id="bc15d-171">Операция GetNonIndexableItemStatistics</span><span class="sxs-lookup"><span data-stu-id="bc15d-171">GetNonIndexableItemStatistics operation</span></span>](getnonindexableitemstatistics-operation.md)
    

