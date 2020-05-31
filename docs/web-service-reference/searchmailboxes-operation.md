---
title: Операция SearchMailboxes
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 8a67c1d8-d021-4e68-aa62-35f7d9c2edc7
description: Поиск сведений о SearchMailboxesной операции EWS.
ms.openlocfilehash: 141ea466a24f3cb400a8e0b63e2162c1eae5d7f8
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835296"
---
# <a name="searchmailboxes-operation"></a><span data-ttu-id="bff68-103">Операция SearchMailboxes</span><span class="sxs-lookup"><span data-stu-id="bff68-103">SearchMailboxes operation</span></span>

<span data-ttu-id="bff68-104">Поиск сведений о **SearchMailboxesной** операции EWS.</span><span class="sxs-lookup"><span data-stu-id="bff68-104">Find information about the **SearchMailboxes** EWS operation.</span></span> 
  
<span data-ttu-id="bff68-105">Операция **SearchMailboxes** выполняет поиск в почтовых ящиках вхождений терминов в элементах почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="bff68-105">The **SearchMailboxes** operation searches mailboxes for occurrences of terms in mailbox items.</span></span> 
  
<span data-ttu-id="bff68-106">Эта операция появилась в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="bff68-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-searchmailboxes-operation"></a><span data-ttu-id="bff68-107">Использование операции SearchMailboxes</span><span class="sxs-lookup"><span data-stu-id="bff68-107">Using the SearchMailboxes operation</span></span>

<span data-ttu-id="bff68-108">Для выполнения поиска в нескольких почтовых ящиках с помощью операции **SearchMailboxes** можно использовать несколько одновременных запросов поиска.</span><span class="sxs-lookup"><span data-stu-id="bff68-108">The **SearchMailboxes** operation can use many simultaneous search queries to perform discovery search on multiple mailboxes.</span></span> <span data-ttu-id="bff68-109">Результаты могут представлять собой статистическую информацию о количестве выполняемых условий поиска или предварительном просмотре элементов, содержащих условия поиска.</span><span class="sxs-lookup"><span data-stu-id="bff68-109">The results can be either statistical information about the number of times search terms occur, or a preview of the items that contain the search terms.</span></span> 
  
### <a name="searchmailboxes-operation-soap-headers"></a><span data-ttu-id="bff68-110">Заголовки SOAP операции SearchMailboxes</span><span class="sxs-lookup"><span data-stu-id="bff68-110">SearchMailboxes operation SOAP headers</span></span>

<span data-ttu-id="bff68-111">Операция **SearchMailboxes** может использовать заголовки SOAP, указанные в приведенной ниже таблице.</span><span class="sxs-lookup"><span data-stu-id="bff68-111">The **SearchMailboxes** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="bff68-112">**Имя заголовка**</span><span class="sxs-lookup"><span data-stu-id="bff68-112">**Header name**</span></span>|<span data-ttu-id="bff68-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="bff68-113">**Element**</span></span>|<span data-ttu-id="bff68-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="bff68-114">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="bff68-115">**ManagementRole**</span><span class="sxs-lookup"><span data-stu-id="bff68-115">**ManagementRole**</span></span> <br/> |[<span data-ttu-id="bff68-116">ManagementRole</span><span class="sxs-lookup"><span data-stu-id="bff68-116">ManagementRole</span></span>](managementrole.md) <br/> |<span data-ttu-id="bff68-117">Определяет роли сервера, необходимые для того, чтобы вызывающий абонент мог выполнить запрос.</span><span class="sxs-lookup"><span data-stu-id="bff68-117">Identifies the server roles that are necessary in order for the caller to make the request.</span></span> <span data-ttu-id="bff68-118">Этот заголовок является применимым для запроса.</span><span class="sxs-lookup"><span data-stu-id="bff68-118">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="bff68-119">**рекуестверсион**</span><span class="sxs-lookup"><span data-stu-id="bff68-119">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="bff68-120">рекуестсерверверсион</span><span class="sxs-lookup"><span data-stu-id="bff68-120">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="bff68-121">Определяет версию схемы для запроса операции.</span><span class="sxs-lookup"><span data-stu-id="bff68-121">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="bff68-122">Этот заголовок является применимым для запроса.</span><span class="sxs-lookup"><span data-stu-id="bff68-122">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="bff68-123">**серверверсион**</span><span class="sxs-lookup"><span data-stu-id="bff68-123">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="bff68-124">серверверсионинфо</span><span class="sxs-lookup"><span data-stu-id="bff68-124">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="bff68-125">Определяет версию сервера, который ответил на запрос.</span><span class="sxs-lookup"><span data-stu-id="bff68-125">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="bff68-126">Этот заголовок является применимым для отклика.</span><span class="sxs-lookup"><span data-stu-id="bff68-126">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="searchmailboxes-operation-request-example-search-mailboxes-for-number-of-search-term-hits"></a><span data-ttu-id="bff68-127">Пример запроса операции SearchMailboxes: почтовые ящики поиска для количества совпадений со словами поиска</span><span class="sxs-lookup"><span data-stu-id="bff68-127">SearchMailboxes operation request example: Search mailboxes for number of search term hits</span></span>

<span data-ttu-id="bff68-128">В приведенном ниже примере запроса операции **SearchMailboxes** показано, как использовать два разных запроса для поиска в трех разных почтовых ящиках статистические сведения о том, сколько раз термин отображается в каждом почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="bff68-128">The following example of a **SearchMailboxes** operation request shows how to use two different queries to search three different mailboxes for statistical information about how many times a term appears in each mailbox.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="bff68-129">В этом примере элемент [Query](query.md) является пустым.</span><span class="sxs-lookup"><span data-stu-id="bff68-129">In this example, the [Query](query.md) element is intentionaly left blank.</span></span> <span data-ttu-id="bff68-130">В этом примере показано, как успешный запрос может содержать условия ошибки для каждой базы для поиска почтовых ящиков.</span><span class="sxs-lookup"><span data-stu-id="bff68-130">This shows how a successful request can contain error conditions on a per mailbox search basis.</span></span> 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013" />
   </soap:Header>
   <soap:Body >
      <m:SearchMailboxes>
         <m:SearchQueries>
            <t:MailboxQuery>
               <t:Query>Test Item</t:Query>
               <t:MailboxSearchScopes>
                  <t:MailboxSearchScope>
                     <t:Mailbox>/o=First Organization/ou=Exchange Administrative Group (FYDLT)/cn=Recipients/cn=12311a742f0e47e392c8201a60d13ecf-Steve</t:Mailbox>
                     <t:SearchScope>All</t:SearchScope>
                  </t:MailboxSearchScope>
                  <t:MailboxSearchScope>
                     <t:Mailbox>/o=First Organization/ou=Exchange Administrative Group (FYDLT)/cn=Recipients/cn=f00c9f70539844beb52341d8f40c572e-Antho</t:Mailbox>
                     <t:SearchScope>PrimaryOnly</t:SearchScope>
                  </t:MailboxSearchScope>
               </t:MailboxSearchScopes>
            </t:MailboxQuery>
            <t:MailboxQuery>
               <t:Query></t:Query>
               <t:MailboxSearchScopes>
                  <t:MailboxSearchScope>
                     <t:Mailbox>/o=First Organization/ou=Exchange Administrative Group (FYDLT)/cn=Recipients/cn=accba4fd5ddf12214a0e82ce1645f4e-Danie</t:Mailbox>
                     <t:SearchScope>ArchiveOnly</t:SearchScope>
                  </t:MailboxSearchScope>
               </t:MailboxSearchScopes>
            </t:MailboxQuery>
         </m:SearchQueries>
         <m:ResultType>StatisticsOnly</m:ResultType>
      </m:SearchMailboxes>
   </soap:Body>
</soap:Envelope>

```

<span data-ttu-id="bff68-131">Текст SOAP Request содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="bff68-131">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="bff68-132">SearchMailboxes</span><span class="sxs-lookup"><span data-stu-id="bff68-132">SearchMailboxes</span></span>](searchmailboxes.md)
    
- [<span data-ttu-id="bff68-133">сеарчкуериес</span><span class="sxs-lookup"><span data-stu-id="bff68-133">SearchQueries</span></span>](searchqueries.md)
    
- [<span data-ttu-id="bff68-134">маилбокскуери</span><span class="sxs-lookup"><span data-stu-id="bff68-134">MailboxQuery</span></span>](mailboxquery.md)
    
- [<span data-ttu-id="bff68-135">Query</span><span class="sxs-lookup"><span data-stu-id="bff68-135">Query</span></span>](query.md)
    
- [<span data-ttu-id="bff68-136">маилбокссеарчскопес</span><span class="sxs-lookup"><span data-stu-id="bff68-136">MailboxSearchScopes</span></span>](mailboxsearchscopes.md)
    
- [<span data-ttu-id="bff68-137">маилбокссеарчскопе</span><span class="sxs-lookup"><span data-stu-id="bff68-137">MailboxSearchScope</span></span>](mailboxsearchscope.md)
    
- [<span data-ttu-id="bff68-138">Mailbox (строка)</span><span class="sxs-lookup"><span data-stu-id="bff68-138">Mailbox (string)</span></span>](mailbox-string.md)
    
- [<span data-ttu-id="bff68-139">SearchScope</span><span class="sxs-lookup"><span data-stu-id="bff68-139">SearchScope</span></span>](searchscope.md)
    
- [<span data-ttu-id="bff68-140">Тип</span><span class="sxs-lookup"><span data-stu-id="bff68-140">ResultType</span></span>](resulttype.md)
    
## <a name="successful-searchmailboxes-operation-response"></a><span data-ttu-id="bff68-141">Успешный отклик операции SearchMailboxes</span><span class="sxs-lookup"><span data-stu-id="bff68-141">Successful SearchMailboxes operation response</span></span>

<span data-ttu-id="bff68-142">В следующем примере показан успешный ответ на запрос операции **SearchMailboxes** для получения статистической информации о количестве найденных терминов поиска в целевых почтовых ящиках.</span><span class="sxs-lookup"><span data-stu-id="bff68-142">The following example shows a successful response to a **SearchMailboxes** operation request to get statistical information about the number of times search terms are found in the target mailboxes.</span></span> <span data-ttu-id="bff68-143">Последний запрос содержит пустой элемент **запроса** , в котором отображается неудачный Поиск в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="bff68-143">The last query contains an empty **Query** element, which shows a failed mailbox search.</span></span> 
  
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
      <m:SearchMailboxesResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                                 xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
         <m:ResponseMessages>
            <m:SearchMailboxesResponseMessage ResponseClass="Success">
               <m:ResponseCode>NoError</m:ResponseCode>
               <m:SearchMailboxesResult>
                  <t:SearchQueries>
                     <t:MailboxQuery>
                        <t:Query>Test Item</t:Query>
                        <t:MailboxSearchScopes>
                           <t:MailboxSearchScope>
                              <t:Mailbox>/o=First Organization/ou=Exchange Administrative Group (FYPDLT)/cn=Recipients/cn=35181a94327e392c8201a60d13ecf-Steve</t:Mailbox>
                              <t:SearchScope>All</t:SearchScope>
                           </t:MailboxSearchScope>
                           <t:MailboxSearchScope>
                              <t:Mailbox>/o=First Organization/ou=Exchange Administrative Group (FYPDLT)/cn=Recipients/cn=f00c9f789572-beb04001d8f40c572e-Antho</t:Mailbox>
                              <t:SearchScope>PrimaryOnly</t:SearchScope>
                           </t:MailboxSearchScope>
                        </t:MailboxSearchScopes>
                     </t:MailboxQuery>
                  </t:SearchQueries>
                  <t:ResultType>StatisticsOnly</t:ResultType>
                  <t:ItemCount>2</t:ItemCount>
                  <t:Size>20206</t:Size>
                  <t:PageItemCount>0</t:PageItemCount>
                  <t:PageItemSize>0</t:PageItemSize>
                  <t:KeywordStats>
                     <t:KeywordStat>
                        <t:Keyword>Test Item</t:Keyword>
                        <t:ItemHits>2</t:ItemHits>
                        <t:Size>20206</t:Size>
                     </t:KeywordStat>
                  </t:KeywordStats>
                  <t:FailedMailboxes>
                     <t:FailedMailbox>
                        <t:Mailbox>/o=First Organization/ou=Exchange Administrative Group (FYPDLT)/cn=Recipients/cn=accba4as3df234234a0e82ce1645f4e-Danie</t:Mailbox>
                        <t:ErrorCode>0</t:ErrorCode>
                        <t:ErrorMessage>The search query can't be empty.</t:ErrorMessage>
                        <t:IsArchive>true</t:IsArchive>
                     </t:FailedMailbox>
                  </t:FailedMailboxes>
               </m:SearchMailboxesResult>
            </m:SearchMailboxesResponseMessage>
         </m:ResponseMessages>
      </m:SearchMailboxesResponse>
   </s:Body>
</s:Envelope>

```

<span data-ttu-id="bff68-144">Тело SOAP отклика содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="bff68-144">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="bff68-145">сеарчмаилбоксесреспонсе</span><span class="sxs-lookup"><span data-stu-id="bff68-145">SearchMailboxesResponse</span></span>](searchmailboxesresponse.md)
    
- [<span data-ttu-id="bff68-146">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="bff68-146">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="bff68-147">сеарчмаилбоксесреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="bff68-147">SearchMailboxesResponseMessage</span></span>](searchmailboxesresponsemessage.md)
    
- [<span data-ttu-id="bff68-148">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="bff68-148">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="bff68-149">сеарчмаилбоксесресулт</span><span class="sxs-lookup"><span data-stu-id="bff68-149">SearchMailboxesResult</span></span>](searchmailboxesresult.md)
    
- [<span data-ttu-id="bff68-150">сеарчкуериес</span><span class="sxs-lookup"><span data-stu-id="bff68-150">SearchQueries</span></span>](searchqueries.md)
    
- [<span data-ttu-id="bff68-151">маилбокскуери</span><span class="sxs-lookup"><span data-stu-id="bff68-151">MailboxQuery</span></span>](mailboxquery.md)
    
- [<span data-ttu-id="bff68-152">Query</span><span class="sxs-lookup"><span data-stu-id="bff68-152">Query</span></span>](query.md)
    
- [<span data-ttu-id="bff68-153">маилбокссеарчскопес</span><span class="sxs-lookup"><span data-stu-id="bff68-153">MailboxSearchScopes</span></span>](mailboxsearchscopes.md)
    
- [<span data-ttu-id="bff68-154">маилбокссеарчскопе</span><span class="sxs-lookup"><span data-stu-id="bff68-154">MailboxSearchScope</span></span>](mailboxsearchscope.md)
    
- [<span data-ttu-id="bff68-155">Mailbox (строка)</span><span class="sxs-lookup"><span data-stu-id="bff68-155">Mailbox (string)</span></span>](mailbox-string.md)
    
- [<span data-ttu-id="bff68-156">SearchScope</span><span class="sxs-lookup"><span data-stu-id="bff68-156">SearchScope</span></span>](searchscope.md)
    
- [<span data-ttu-id="bff68-157">Тип</span><span class="sxs-lookup"><span data-stu-id="bff68-157">ResultType</span></span>](resulttype.md)
    
- [<span data-ttu-id="bff68-158">ItemCount</span><span class="sxs-lookup"><span data-stu-id="bff68-158">ItemCount</span></span>](itemcount.md)
    
- [<span data-ttu-id="bff68-159">Размер (длинный)</span><span class="sxs-lookup"><span data-stu-id="bff68-159">Size (long)</span></span>](size-long.md)
    
- [<span data-ttu-id="bff68-160">пажеитемкаунт</span><span class="sxs-lookup"><span data-stu-id="bff68-160">PageItemCount</span></span>](pageitemcount.md)
    
- [<span data-ttu-id="bff68-161">кэйвордстатс</span><span class="sxs-lookup"><span data-stu-id="bff68-161">KeywordStats</span></span>](keywordstats.md)
    
- [<span data-ttu-id="bff68-162">кэйвордстат</span><span class="sxs-lookup"><span data-stu-id="bff68-162">KeywordStat</span></span>](keywordstat.md)
    
- [<span data-ttu-id="bff68-163">Недопустим</span><span class="sxs-lookup"><span data-stu-id="bff68-163">Keyword</span></span>](keyword.md)
    
- [<span data-ttu-id="bff68-164">итемхитс</span><span class="sxs-lookup"><span data-stu-id="bff68-164">ItemHits</span></span>](itemhits.md)
    
- [<span data-ttu-id="bff68-165">фаиледмаилбоксес</span><span class="sxs-lookup"><span data-stu-id="bff68-165">FailedMailboxes</span></span>](failedmailboxes.md)
    
- [<span data-ttu-id="bff68-166">фаиледмаилбокс</span><span class="sxs-lookup"><span data-stu-id="bff68-166">FailedMailbox</span></span>](failedmailbox.md)
    
- [<span data-ttu-id="bff68-167">Mailbox (строка)</span><span class="sxs-lookup"><span data-stu-id="bff68-167">Mailbox (string)</span></span>](mailbox-string.md)
    
- [<span data-ttu-id="bff68-168">ErrorCode (int)</span><span class="sxs-lookup"><span data-stu-id="bff68-168">ErrorCode (int)</span></span>](errorcode-int.md)
    
- [<span data-ttu-id="bff68-169">ErrorMessage</span><span class="sxs-lookup"><span data-stu-id="bff68-169">ErrorMessage</span></span>](errormessage.md)
    
- [<span data-ttu-id="bff68-170">IsArchive</span><span class="sxs-lookup"><span data-stu-id="bff68-170">IsArchive</span></span>](isarchive.md)
    
## <a name="searchmailboxes-operation-error-response"></a><span data-ttu-id="bff68-171">Ответ об ошибке операции SearchMailboxes</span><span class="sxs-lookup"><span data-stu-id="bff68-171">SearchMailboxes operation error response</span></span>

<span data-ttu-id="bff68-172">В следующем примере показан ответ об ошибке для запроса операции **SearchMailboxes** .</span><span class="sxs-lookup"><span data-stu-id="bff68-172">The following example shows an error response to a **SearchMailboxes** operation request.</span></span> <span data-ttu-id="bff68-173">Это ответ на запрос поиска в почтовом ящике при неправильном идентификаторе почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="bff68-173">This is a response to a request to search a mailbox when the mailbox identifier is incorrect.</span></span> 
  
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
      <m:SearchMailboxesResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                                 xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
         <m:ResponseMessages>
            <m:SearchMailboxesResponseMessage ResponseClass="Error">
               <m:MessageText>No mailbox is specified for search operation. If specified in the request, 
               then it could be due to permission issue.</m:MessageText>
               <m:ResponseCode>ErrorInvalidOperation</m:ResponseCode>
               <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
               <m:SearchMailboxesResult>
                  <t:SearchQueries>
                     <t:MailboxQuery>
                        <t:Query>subject:Test Item</t:Query>
                        <t:MailboxSearchScopes>
                           <t:MailboxSearchScope>
                              <t:Mailbox>sbrown@contoso.com</t:Mailbox>
                              <t:SearchScope>All</t:SearchScope>
                           </t:MailboxSearchScope>
                        </t:MailboxSearchScopes>
                     </t:MailboxQuery>
                  </t:SearchQueries>
                  <t:ResultType>StatisticsOnly</t:ResultType>
                  <t:ItemCount>0</t:ItemCount>
                  <t:Size>0</t:Size>
                  <t:PageItemCount>0</t:PageItemCount>
                  <t:PageItemSize>0</t:PageItemSize>
                  <t:FailedMailboxes>
                     <t:FailedMailbox>
                        <t:Mailbox>sbrown@contoso.com</t:Mailbox>
                        <t:ErrorCode>0</t:ErrorCode>
                        <t:ErrorMessage>No mailbox is specified for search operation. If specified in the request, 
                        then it could be due to permission issue.</t:ErrorMessage>
                        <t:IsArchive>false</t:IsArchive>
                     </t:FailedMailbox>
                  </t:FailedMailboxes>
               </m:SearchMailboxesResult>
            </m:SearchMailboxesResponseMessage>
         </m:ResponseMessages>
      </m:SearchMailboxesResponse>
   </s:Body>
</s:Envelope>

```

<span data-ttu-id="bff68-174">Основной текст сообщения об ошибке SOAP содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="bff68-174">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="bff68-175">сеарчмаилбоксесреспонсе</span><span class="sxs-lookup"><span data-stu-id="bff68-175">SearchMailboxesResponse</span></span>](searchmailboxesresponse.md)
    
- [<span data-ttu-id="bff68-176">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="bff68-176">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="bff68-177">сеарчмаилбоксесреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="bff68-177">SearchMailboxesResponseMessage</span></span>](searchmailboxesresponsemessage.md)
    
- [<span data-ttu-id="bff68-178">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="bff68-178">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="bff68-179">сеарчмаилбоксесресулт</span><span class="sxs-lookup"><span data-stu-id="bff68-179">SearchMailboxesResult</span></span>](searchmailboxesresult.md)
    
- [<span data-ttu-id="bff68-180">сеарчкуериес</span><span class="sxs-lookup"><span data-stu-id="bff68-180">SearchQueries</span></span>](searchqueries.md)
    
- [<span data-ttu-id="bff68-181">маилбокскуери</span><span class="sxs-lookup"><span data-stu-id="bff68-181">MailboxQuery</span></span>](mailboxquery.md)
    
- [<span data-ttu-id="bff68-182">Query</span><span class="sxs-lookup"><span data-stu-id="bff68-182">Query</span></span>](query.md)
    
- [<span data-ttu-id="bff68-183">маилбокссеарчскопес</span><span class="sxs-lookup"><span data-stu-id="bff68-183">MailboxSearchScopes</span></span>](mailboxsearchscopes.md)
    
- [<span data-ttu-id="bff68-184">маилбокссеарчскопе</span><span class="sxs-lookup"><span data-stu-id="bff68-184">MailboxSearchScope</span></span>](mailboxsearchscope.md)
    
- [<span data-ttu-id="bff68-185">Mailbox (строка)</span><span class="sxs-lookup"><span data-stu-id="bff68-185">Mailbox (string)</span></span>](mailbox-string.md)
    
- [<span data-ttu-id="bff68-186">SearchScope</span><span class="sxs-lookup"><span data-stu-id="bff68-186">SearchScope</span></span>](searchscope.md)
    
- [<span data-ttu-id="bff68-187">Тип</span><span class="sxs-lookup"><span data-stu-id="bff68-187">ResultType</span></span>](resulttype.md)
    
- [<span data-ttu-id="bff68-188">ItemCount</span><span class="sxs-lookup"><span data-stu-id="bff68-188">ItemCount</span></span>](itemcount.md)
    
- [<span data-ttu-id="bff68-189">Размер (длинный)</span><span class="sxs-lookup"><span data-stu-id="bff68-189">Size (long)</span></span>](size-long.md)
    
- [<span data-ttu-id="bff68-190">пажеитемкаунт</span><span class="sxs-lookup"><span data-stu-id="bff68-190">PageItemCount</span></span>](pageitemcount.md)
    
- [<span data-ttu-id="bff68-191">пажеитемсизе</span><span class="sxs-lookup"><span data-stu-id="bff68-191">PageItemSize</span></span>](pageitemsize.md)
    
- [<span data-ttu-id="bff68-192">фаиледмаилбоксес</span><span class="sxs-lookup"><span data-stu-id="bff68-192">FailedMailboxes</span></span>](failedmailboxes.md)
    
- [<span data-ttu-id="bff68-193">фаиледмаилбокс</span><span class="sxs-lookup"><span data-stu-id="bff68-193">FailedMailbox</span></span>](failedmailbox.md)
    
- [<span data-ttu-id="bff68-194">Mailbox (строка)</span><span class="sxs-lookup"><span data-stu-id="bff68-194">Mailbox (string)</span></span>](mailbox-string.md)
    
- [<span data-ttu-id="bff68-195">ErrorCode (int)</span><span class="sxs-lookup"><span data-stu-id="bff68-195">ErrorCode (int)</span></span>](errorcode-int.md)
    
- [<span data-ttu-id="bff68-196">ErrorMessage</span><span class="sxs-lookup"><span data-stu-id="bff68-196">ErrorMessage</span></span>](errormessage.md)
    
- [<span data-ttu-id="bff68-197">IsArchive</span><span class="sxs-lookup"><span data-stu-id="bff68-197">IsArchive</span></span>](isarchive.md)
    
<span data-ttu-id="bff68-198">Дополнительные коды ошибок, которые являются общими для EWS и специфичными для этой операции, можно найти в разделе [респонсекоде](responsecode.md).</span><span class="sxs-lookup"><span data-stu-id="bff68-198">For additional error codes that are generic to EWS and specific to this operation, see [ResponseCode](responsecode.md).</span></span>
  
## <a name="see-also"></a><span data-ttu-id="bff68-199">См. также</span><span class="sxs-lookup"><span data-stu-id="bff68-199">See also</span></span>

- [<span data-ttu-id="bff68-200">Операции EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="bff68-200">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
    
- [<span data-ttu-id="bff68-201">Операция GetSearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="bff68-201">GetSearchableMailboxes operation</span></span>](getsearchablemailboxes-operation.md)
    
- [<span data-ttu-id="bff68-202">Операция SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="bff68-202">SetHoldOnMailboxes operation</span></span>](setholdonmailboxes-operation.md)
    
- [<span data-ttu-id="bff68-203">Операция GetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="bff68-203">GetHoldOnMailboxes operation</span></span>](getholdonmailboxes-operation.md)
    
- [<span data-ttu-id="bff68-204">Операция GetDiscoverySearchConfiguration</span><span class="sxs-lookup"><span data-stu-id="bff68-204">GetDiscoverySearchConfiguration operation</span></span>](getdiscoverysearchconfiguration-operation.md)
    
- [<span data-ttu-id="bff68-205">Операция GetNonIndexableItemDetails</span><span class="sxs-lookup"><span data-stu-id="bff68-205">GetNonIndexableItemDetails operation</span></span>](getnonindexableitemdetails-operation.md)
    
- [<span data-ttu-id="bff68-206">Операция GetNonIndexableItemStatistics</span><span class="sxs-lookup"><span data-stu-id="bff68-206">GetNonIndexableItemStatistics operation</span></span>](getnonindexableitemstatistics-operation.md)
    

