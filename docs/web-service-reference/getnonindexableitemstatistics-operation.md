---
title: Операция GetNonIndexableItemStatistics
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: ed077877-9d98-4434-b8b6-a4a905e7f7a6
description: Найдите сведения о веб-служб Exchange GetNonIndexableItemStatistics операции.
ms.openlocfilehash: 35c2d3321c6e1a3154c88307d0e875cd6997e7fb
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762858"
---
# <a name="getnonindexableitemstatistics-operation"></a><span data-ttu-id="36831-103">Операция GetNonIndexableItemStatistics</span><span class="sxs-lookup"><span data-stu-id="36831-103">GetNonIndexableItemStatistics operation</span></span>

<span data-ttu-id="36831-104">Найдите сведения о **GetNonIndexableItemStatistics** операции веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="36831-104">Find information about the **GetNonIndexableItemStatistics** EWS operation.</span></span> 
  
<span data-ttu-id="36831-105">Операция **GetNonIndexableItemStatistics** извлекает число элементов, которые не могут быть индексированы в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="36831-105">The **GetNonIndexableItemStatistics** operation retrieves the count of items that cannot be indexed in a mailbox.</span></span> 
  
<span data-ttu-id="36831-106">Эта операция появилась в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="36831-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-getnonindexableitemstatistics-operation"></a><span data-ttu-id="36831-107">С помощью операции GetNonIndexableItemStatistics</span><span class="sxs-lookup"><span data-stu-id="36831-107">Using the GetNonIndexableItemStatistics operation</span></span>

<span data-ttu-id="36831-108">Операция **GetNonIndexableItemStatistics** подсчитывает элементы почтовых ящиков, которые не могут быть индексированы.</span><span class="sxs-lookup"><span data-stu-id="36831-108">The **GetNonIndexableItemStatistics** operation counts mailbox items that cannot be indexed.</span></span> <span data-ttu-id="36831-109">Во время поиска обнаружения не поиска элементов, которые не могут быть индексированы.</span><span class="sxs-lookup"><span data-stu-id="36831-109">Items that cannot be indexed are not searched during a discovery search.</span></span> 
  
### <a name="getnonindexableitemstatistics-operation-soap-headers"></a><span data-ttu-id="36831-110">Заголовки SOAP GetNonIndexableItemStatistics операции</span><span class="sxs-lookup"><span data-stu-id="36831-110">GetNonIndexableItemStatistics operation SOAP headers</span></span>

<span data-ttu-id="36831-111">Операция **GetNonIndexableItemStatistics** можно использовать заголовки SOAP, которые перечислены в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="36831-111">The **GetNonIndexableItemStatistics** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="36831-112">**Имя заголовка**</span><span class="sxs-lookup"><span data-stu-id="36831-112">**Header name**</span></span>|<span data-ttu-id="36831-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="36831-113">**Element**</span></span>|<span data-ttu-id="36831-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="36831-114">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="36831-115">**ManagementRole**</span><span class="sxs-lookup"><span data-stu-id="36831-115">**ManagementRole**</span></span> <br/> |[<span data-ttu-id="36831-116">ManagementRole</span><span class="sxs-lookup"><span data-stu-id="36831-116">ManagementRole</span></span>](managementrole.md) <br/> |<span data-ttu-id="36831-117">Идентифицирует ролей сервера, необходимых в порядке для абонентов для запроса.</span><span class="sxs-lookup"><span data-stu-id="36831-117">Identifies the server roles that are necessary in order for the caller to make the request.</span></span> <span data-ttu-id="36831-118">Этот заголовок можно применять к запросу.</span><span class="sxs-lookup"><span data-stu-id="36831-118">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="36831-119">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="36831-119">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="36831-120">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="36831-120">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="36831-121">Определяет версию схемы для операции запроса.</span><span class="sxs-lookup"><span data-stu-id="36831-121">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="36831-122">Этот заголовок можно применять к запросу.</span><span class="sxs-lookup"><span data-stu-id="36831-122">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="36831-123">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="36831-123">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="36831-124">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="36831-124">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="36831-125">Определяет версию сервера, ответившего на запрос.</span><span class="sxs-lookup"><span data-stu-id="36831-125">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="36831-126">Этот заголовок можно применять, чтобы получить ответ.</span><span class="sxs-lookup"><span data-stu-id="36831-126">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="getnonindexableitemstatistics-operation-request-example-get-the-count-of-items-that-cannot-be-indexed-in-a-mailbox"></a><span data-ttu-id="36831-127">Пример запроса GetNonIndexableItemStatistics операции: получение числа элементов, которые не могут быть индексированы в почтовом ящике</span><span class="sxs-lookup"><span data-stu-id="36831-127">GetNonIndexableItemStatistics operation request example: Get the count of items that cannot be indexed in a mailbox</span></span>

<span data-ttu-id="36831-128">В следующем примере запрос операции **GetNonIndexableItemStatistics** показано, как запросить число элементов, которые не могут быть индексированы в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="36831-128">The following example of a **GetNonIndexableItemStatistics** operation request shows how to request the count of items that cannot be indexed in a mailbox.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="36831-129">Все устаревшие доменных имен в этом примере имеют сокращение, чтобы сохранить удобочитаемость.</span><span class="sxs-lookup"><span data-stu-id="36831-129">All legacy domain names in this example have be shortened to preserve readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013" />
   </soap:Header>
   <soap:Body >
      <m:GetNonIndexableItemStatistics>
         <m:Mailboxes>
            <t:LegacyDN>/o=First Organization/ou=Exchange Administrative Group (FYDIDLT)/cn=Recipients/cn=3518cf-Steve</t:LegacyDN>
         </m:Mailboxes>
         <m:SearchArchiveOnly>false</m:SearchArchiveOnly>
      </m:GetNonIndexableItemStatistics>
   </soap:Body>
</soap:Envelope>

```

<span data-ttu-id="36831-130">Запрос SOAP body содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="36831-130">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="36831-131">GetNonIndexableItemStatistics</span><span class="sxs-lookup"><span data-stu-id="36831-131">GetNonIndexableItemStatistics</span></span>](getnonindexableitemstatistics.md)
    
- [<span data-ttu-id="36831-132">Почтовые ящики (NonEmptyArrayOfLegacyDNsType)</span><span class="sxs-lookup"><span data-stu-id="36831-132">Mailboxes (NonEmptyArrayOfLegacyDNsType)</span></span>](mailboxes-nonemptyarrayoflegacydnstype.md)
    
- [<span data-ttu-id="36831-133">LegacyDN</span><span class="sxs-lookup"><span data-stu-id="36831-133">LegacyDN</span></span>](legacydn.md)
    
- [<span data-ttu-id="36831-134">SearchArchiveOnly</span><span class="sxs-lookup"><span data-stu-id="36831-134">SearchArchiveOnly</span></span>](searcharchiveonly.md)
    
## <a name="successful-getnonindexableitemstatistics-operation-response"></a><span data-ttu-id="36831-135">Успешные операции ответа GetNonIndexableItemStatistics</span><span class="sxs-lookup"><span data-stu-id="36831-135">Successful GetNonIndexableItemStatistics operation response</span></span>

<span data-ttu-id="36831-136">В следующем примере показано успешного ответа на запрос операции **GetNonIndexableItemStatistics** для получения количества элементов, которые не могут быть индексированы в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="36831-136">The following example shows a successful response to a **GetNonIndexableItemStatistics** operation request to get the count of items that cannot be indexed in a mailbox.</span></span> 
  
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
      <GetNonIndexableItemStatisticsResponse ResponseClass="Success" 
                                             xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
         <NonIndexableItemStatistics>
            <NonIndexableItemStatistic xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
               <Mailbox>/o=First Organization/ou=Exchange Administrative Group (FYT)/cn=Recipients/cn=35181acf-Steve</Mailbox>
               <ItemCount>2</ItemCount>
            </NonIndexableItemStatistic>
         </NonIndexableItemStatistics>
      </GetNonIndexableItemStatisticsResponse>
   </s:Body>
</s:Envelope>

```

<span data-ttu-id="36831-137">Ответ SOAP body содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="36831-137">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="36831-138">GetNonIndexableItemStatisticsResponse</span><span class="sxs-lookup"><span data-stu-id="36831-138">GetNonIndexableItemStatisticsResponse</span></span>](getnonindexableitemstatisticsresponse.md)
    
- [<span data-ttu-id="36831-139">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="36831-139">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="36831-140">NonIndexableItemStatistics</span><span class="sxs-lookup"><span data-stu-id="36831-140">NonIndexableItemStatistics</span></span>](nonindexableitemstatistics.md)
    
- [<span data-ttu-id="36831-141">NonIndexableItemStatistic</span><span class="sxs-lookup"><span data-stu-id="36831-141">NonIndexableItemStatistic</span></span>](nonindexableitemstatistic.md)
    
- [<span data-ttu-id="36831-142">Почтовый ящик (строка)</span><span class="sxs-lookup"><span data-stu-id="36831-142">Mailbox (string)</span></span>](mailbox-string.md)
    
- [<span data-ttu-id="36831-143">ItemCount</span><span class="sxs-lookup"><span data-stu-id="36831-143">ItemCount</span></span>](itemcount.md)
    
## <a name="getnonindexableitemstatistics-operation-error-response"></a><span data-ttu-id="36831-144">Ошибка операции GetNonIndexableItemStatistics ответа</span><span class="sxs-lookup"><span data-stu-id="36831-144">GetNonIndexableItemStatistics operation error response</span></span>

<span data-ttu-id="36831-145">В следующем примере показано ошибочный ответ на запрос операции **GetNonIndexableItemStatistics** .</span><span class="sxs-lookup"><span data-stu-id="36831-145">The following example shows an error response to a **GetNonIndexableItemStatistics** operation request.</span></span> <span data-ttu-id="36831-146">Это ответ на запрос для получения количества элементов, которые не могут быть индексированы из более одного почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="36831-146">This is a response to a request to get the count of items that cannot be indexed from more than one mailbox.</span></span> 
  
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
      <GetNonIndexableItemStatisticsResponse ResponseClass="Error" 
                                             xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>Multiple mailboxes is currently not supported, only single mailbox is supported.</MessageText>
         <ResponseCode>ErrorInvalidArgument</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
      </GetNonIndexableItemStatisticsResponse>
   </s:Body>
</s:Envelope>

```

<span data-ttu-id="36831-147">Ошибка ответ SOAP body содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="36831-147">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="36831-148">GetNonIndexableItemStatisticsResponse</span><span class="sxs-lookup"><span data-stu-id="36831-148">GetNonIndexableItemStatisticsResponse</span></span>](getnonindexableitemstatisticsresponse.md)
    
- [<span data-ttu-id="36831-149">MessageText</span><span class="sxs-lookup"><span data-stu-id="36831-149">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="36831-150">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="36831-150">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="36831-151">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="36831-151">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
<span data-ttu-id="36831-152">Дополнительные коды ошибок, которые являются общими для веб-служб Exchange и специально для этой операции в разделе [ResponseCode](responsecode.md).</span><span class="sxs-lookup"><span data-stu-id="36831-152">For additional error codes that are generic to EWS and specific to this operation, see [ResponseCode](responsecode.md).</span></span>
  
## <a name="see-also"></a><span data-ttu-id="36831-153">См. также</span><span class="sxs-lookup"><span data-stu-id="36831-153">See also</span></span>

- [<span data-ttu-id="36831-154">Операции EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="36831-154">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
    
- [<span data-ttu-id="36831-155">Операция GetSearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="36831-155">GetSearchableMailboxes operation</span></span>](getsearchablemailboxes-operation.md)
    
- [<span data-ttu-id="36831-156">Операция SearchMailboxes</span><span class="sxs-lookup"><span data-stu-id="36831-156">SearchMailboxes operation</span></span>](searchmailboxes-operation.md)
    
- [<span data-ttu-id="36831-157">Операция GetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="36831-157">GetHoldOnMailboxes operation</span></span>](getholdonmailboxes-operation.md)
    
- [<span data-ttu-id="36831-158">Операция SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="36831-158">SetHoldOnMailboxes operation</span></span>](setholdonmailboxes-operation.md)
    
- [<span data-ttu-id="36831-159">Операция GetDiscoverySearchConfiguration</span><span class="sxs-lookup"><span data-stu-id="36831-159">GetDiscoverySearchConfiguration operation</span></span>](getdiscoverysearchconfiguration-operation.md)
    
- [<span data-ttu-id="36831-160">Операция GetNonIndexableItemDetails</span><span class="sxs-lookup"><span data-stu-id="36831-160">GetNonIndexableItemDetails operation</span></span>](getnonindexableitemdetails-operation.md)
    

