---
title: Операция GetNonIndexableItemStatistics
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: ed077877-9d98-4434-b8b6-a4a905e7f7a6
description: Поиск сведений о GetNonIndexableItemStatisticsной операции EWS.
ms.openlocfilehash: c7d49f9e0d7b4191c7403cb4d1a20e70a96c3882
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44452820"
---
# <a name="getnonindexableitemstatistics-operation"></a><span data-ttu-id="0dd39-103">Операция GetNonIndexableItemStatistics</span><span class="sxs-lookup"><span data-stu-id="0dd39-103">GetNonIndexableItemStatistics operation</span></span>

<span data-ttu-id="0dd39-104">Поиск сведений о **GetNonIndexableItemStatisticsной** операции EWS.</span><span class="sxs-lookup"><span data-stu-id="0dd39-104">Find information about the **GetNonIndexableItemStatistics** EWS operation.</span></span> 
  
<span data-ttu-id="0dd39-105">Операция **GetNonIndexableItemStatistics** получает количество элементов, которые не удается индексировать в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="0dd39-105">The **GetNonIndexableItemStatistics** operation retrieves the count of items that cannot be indexed in a mailbox.</span></span> 
  
<span data-ttu-id="0dd39-106">Эта операция появилась в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="0dd39-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-getnonindexableitemstatistics-operation"></a><span data-ttu-id="0dd39-107">Использование операции GetNonIndexableItemStatistics</span><span class="sxs-lookup"><span data-stu-id="0dd39-107">Using the GetNonIndexableItemStatistics operation</span></span>

<span data-ttu-id="0dd39-108">Операция **GetNonIndexableItemStatistics** учитывает элементы почтового ящика, которые не удается индексировать.</span><span class="sxs-lookup"><span data-stu-id="0dd39-108">The **GetNonIndexableItemStatistics** operation counts mailbox items that cannot be indexed.</span></span> <span data-ttu-id="0dd39-109">Элементы, которые не могут индексироваться, не ищутся во время поиска обнаружения.</span><span class="sxs-lookup"><span data-stu-id="0dd39-109">Items that cannot be indexed are not searched during a discovery search.</span></span> 
  
### <a name="getnonindexableitemstatistics-operation-soap-headers"></a><span data-ttu-id="0dd39-110">Заголовки SOAP операции GetNonIndexableItemStatistics</span><span class="sxs-lookup"><span data-stu-id="0dd39-110">GetNonIndexableItemStatistics operation SOAP headers</span></span>

<span data-ttu-id="0dd39-111">Операция **GetNonIndexableItemStatistics** может использовать заголовки SOAP, указанные в приведенной ниже таблице.</span><span class="sxs-lookup"><span data-stu-id="0dd39-111">The **GetNonIndexableItemStatistics** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="0dd39-112">**Имя заголовка**</span><span class="sxs-lookup"><span data-stu-id="0dd39-112">**Header name**</span></span>|<span data-ttu-id="0dd39-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="0dd39-113">**Element**</span></span>|<span data-ttu-id="0dd39-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="0dd39-114">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="0dd39-115">**ManagementRole**</span><span class="sxs-lookup"><span data-stu-id="0dd39-115">**ManagementRole**</span></span> <br/> |[<span data-ttu-id="0dd39-116">ManagementRole</span><span class="sxs-lookup"><span data-stu-id="0dd39-116">ManagementRole</span></span>](managementrole.md) <br/> |<span data-ttu-id="0dd39-117">Определяет роли сервера, необходимые для того, чтобы вызывающий абонент мог выполнить запрос.</span><span class="sxs-lookup"><span data-stu-id="0dd39-117">Identifies the server roles that are necessary in order for the caller to make the request.</span></span> <span data-ttu-id="0dd39-118">Этот заголовок является применимым для запроса.</span><span class="sxs-lookup"><span data-stu-id="0dd39-118">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="0dd39-119">**рекуестверсион**</span><span class="sxs-lookup"><span data-stu-id="0dd39-119">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="0dd39-120">рекуестсерверверсион</span><span class="sxs-lookup"><span data-stu-id="0dd39-120">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="0dd39-121">Определяет версию схемы для запроса операции.</span><span class="sxs-lookup"><span data-stu-id="0dd39-121">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="0dd39-122">Этот заголовок является применимым для запроса.</span><span class="sxs-lookup"><span data-stu-id="0dd39-122">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="0dd39-123">**серверверсион**</span><span class="sxs-lookup"><span data-stu-id="0dd39-123">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="0dd39-124">серверверсионинфо</span><span class="sxs-lookup"><span data-stu-id="0dd39-124">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="0dd39-125">Определяет версию сервера, который ответил на запрос.</span><span class="sxs-lookup"><span data-stu-id="0dd39-125">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="0dd39-126">Этот заголовок является применимым для отклика.</span><span class="sxs-lookup"><span data-stu-id="0dd39-126">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="getnonindexableitemstatistics-operation-request-example-get-the-count-of-items-that-cannot-be-indexed-in-a-mailbox"></a><span data-ttu-id="0dd39-127">Пример запроса операции GetNonIndexableItemStatistics: получение числа элементов, которые не удается индексировать в почтовом ящике</span><span class="sxs-lookup"><span data-stu-id="0dd39-127">GetNonIndexableItemStatistics operation request example: Get the count of items that cannot be indexed in a mailbox</span></span>

<span data-ttu-id="0dd39-128">В следующем примере запроса операции **GetNonIndexableItemStatistics** показано, как запросить количество элементов, которые не удается индексировать в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="0dd39-128">The following example of a **GetNonIndexableItemStatistics** operation request shows how to request the count of items that cannot be indexed in a mailbox.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="0dd39-129">Все устаревшие доменные имена в этом примере сокращены, чтобы сохранить удобочитаемость.</span><span class="sxs-lookup"><span data-stu-id="0dd39-129">All legacy domain names in this example have be shortened to preserve readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
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

<span data-ttu-id="0dd39-130">Текст SOAP Request содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="0dd39-130">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="0dd39-131">GetNonIndexableItemStatistics</span><span class="sxs-lookup"><span data-stu-id="0dd39-131">GetNonIndexableItemStatistics</span></span>](getnonindexableitemstatistics.md)
    
- [<span data-ttu-id="0dd39-132">Почтовые ящики (Нонемптяррайофлегациднстипе)</span><span class="sxs-lookup"><span data-stu-id="0dd39-132">Mailboxes (NonEmptyArrayOfLegacyDNsType)</span></span>](mailboxes-nonemptyarrayoflegacydnstype.md)
    
- [<span data-ttu-id="0dd39-133">LegacyDN</span><span class="sxs-lookup"><span data-stu-id="0dd39-133">LegacyDN</span></span>](legacydn.md)
    
- [<span data-ttu-id="0dd39-134">сеарчарчивеонли</span><span class="sxs-lookup"><span data-stu-id="0dd39-134">SearchArchiveOnly</span></span>](searcharchiveonly.md)
    
## <a name="successful-getnonindexableitemstatistics-operation-response"></a><span data-ttu-id="0dd39-135">Успешный отклик операции GetNonIndexableItemStatistics</span><span class="sxs-lookup"><span data-stu-id="0dd39-135">Successful GetNonIndexableItemStatistics operation response</span></span>

<span data-ttu-id="0dd39-136">В следующем примере показан успешный ответ на запрос операции **GetNonIndexableItemStatistics** для получения количества элементов, которые не удается индексировать в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="0dd39-136">The following example shows a successful response to a **GetNonIndexableItemStatistics** operation request to get the count of items that cannot be indexed in a mailbox.</span></span> 
  
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
      <GetNonIndexableItemStatisticsResponse ResponseClass="Success" 
                                             xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
         <NonIndexableItemStatistics>
            <NonIndexableItemStatistic xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
               <Mailbox>/o=First Organization/ou=Exchange Administrative Group (FYT)/cn=Recipients/cn=35181acf-Steve</Mailbox>
               <ItemCount>2</ItemCount>
            </NonIndexableItemStatistic>
         </NonIndexableItemStatistics>
      </GetNonIndexableItemStatisticsResponse>
   </s:Body>
</s:Envelope>

```

<span data-ttu-id="0dd39-137">Тело SOAP отклика содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="0dd39-137">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="0dd39-138">жетнониндексаблеитемстатистиксреспонсе</span><span class="sxs-lookup"><span data-stu-id="0dd39-138">GetNonIndexableItemStatisticsResponse</span></span>](getnonindexableitemstatisticsresponse.md)
    
- [<span data-ttu-id="0dd39-139">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="0dd39-139">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="0dd39-140">нониндексаблеитемстатистикс</span><span class="sxs-lookup"><span data-stu-id="0dd39-140">NonIndexableItemStatistics</span></span>](nonindexableitemstatistics.md)
    
- [<span data-ttu-id="0dd39-141">нониндексаблеитемстатистик</span><span class="sxs-lookup"><span data-stu-id="0dd39-141">NonIndexableItemStatistic</span></span>](nonindexableitemstatistic.md)
    
- [<span data-ttu-id="0dd39-142">Mailbox (строка)</span><span class="sxs-lookup"><span data-stu-id="0dd39-142">Mailbox (string)</span></span>](mailbox-string.md)
    
- [<span data-ttu-id="0dd39-143">ItemCount</span><span class="sxs-lookup"><span data-stu-id="0dd39-143">ItemCount</span></span>](itemcount.md)
    
## <a name="getnonindexableitemstatistics-operation-error-response"></a><span data-ttu-id="0dd39-144">Ответ об ошибке операции GetNonIndexableItemStatistics</span><span class="sxs-lookup"><span data-stu-id="0dd39-144">GetNonIndexableItemStatistics operation error response</span></span>

<span data-ttu-id="0dd39-145">В следующем примере показан ответ об ошибке для запроса операции **GetNonIndexableItemStatistics** .</span><span class="sxs-lookup"><span data-stu-id="0dd39-145">The following example shows an error response to a **GetNonIndexableItemStatistics** operation request.</span></span> <span data-ttu-id="0dd39-146">Это ответ на запрос на получение количества элементов, которые не удается индексировать из нескольких почтовых ящиков.</span><span class="sxs-lookup"><span data-stu-id="0dd39-146">This is a response to a request to get the count of items that cannot be indexed from more than one mailbox.</span></span> 
  
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
      <GetNonIndexableItemStatisticsResponse ResponseClass="Error" 
                                             xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>Multiple mailboxes is currently not supported, only single mailbox is supported.</MessageText>
         <ResponseCode>ErrorInvalidArgument</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
      </GetNonIndexableItemStatisticsResponse>
   </s:Body>
</s:Envelope>

```

<span data-ttu-id="0dd39-147">Основной текст сообщения об ошибке SOAP содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="0dd39-147">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="0dd39-148">жетнониндексаблеитемстатистиксреспонсе</span><span class="sxs-lookup"><span data-stu-id="0dd39-148">GetNonIndexableItemStatisticsResponse</span></span>](getnonindexableitemstatisticsresponse.md)
    
- [<span data-ttu-id="0dd39-149">мессажетекст</span><span class="sxs-lookup"><span data-stu-id="0dd39-149">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="0dd39-150">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="0dd39-150">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="0dd39-151">дескриптивелинккэй</span><span class="sxs-lookup"><span data-stu-id="0dd39-151">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
<span data-ttu-id="0dd39-152">Дополнительные коды ошибок, которые являются общими для EWS и специфичными для этой операции, можно найти в разделе [респонсекоде](responsecode.md).</span><span class="sxs-lookup"><span data-stu-id="0dd39-152">For additional error codes that are generic to EWS and specific to this operation, see [ResponseCode](responsecode.md).</span></span>
  
## <a name="see-also"></a><span data-ttu-id="0dd39-153">См. также</span><span class="sxs-lookup"><span data-stu-id="0dd39-153">See also</span></span>

- [<span data-ttu-id="0dd39-154">Операции EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="0dd39-154">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
    
- [<span data-ttu-id="0dd39-155">Операция GetSearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="0dd39-155">GetSearchableMailboxes operation</span></span>](getsearchablemailboxes-operation.md)
    
- [<span data-ttu-id="0dd39-156">Операция SearchMailboxes</span><span class="sxs-lookup"><span data-stu-id="0dd39-156">SearchMailboxes operation</span></span>](searchmailboxes-operation.md)
    
- [<span data-ttu-id="0dd39-157">Операция GetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="0dd39-157">GetHoldOnMailboxes operation</span></span>](getholdonmailboxes-operation.md)
    
- [<span data-ttu-id="0dd39-158">Операция SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="0dd39-158">SetHoldOnMailboxes operation</span></span>](setholdonmailboxes-operation.md)
    
- [<span data-ttu-id="0dd39-159">Операция GetDiscoverySearchConfiguration</span><span class="sxs-lookup"><span data-stu-id="0dd39-159">GetDiscoverySearchConfiguration operation</span></span>](getdiscoverysearchconfiguration-operation.md)
    
- [<span data-ttu-id="0dd39-160">Операция GetNonIndexableItemDetails</span><span class="sxs-lookup"><span data-stu-id="0dd39-160">GetNonIndexableItemDetails operation</span></span>](getnonindexableitemdetails-operation.md)
    

