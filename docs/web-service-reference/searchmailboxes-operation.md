---
title: Операция SearchMailboxes
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 8a67c1d8-d021-4e68-aa62-35f7d9c2edc7
description: Найдите сведения о веб-служб Exchange SearchMailboxes операции.
ms.openlocfilehash: 141ea466a24f3cb400a8e0b63e2162c1eae5d7f8
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835296"
---
# <a name="searchmailboxes-operation"></a><span data-ttu-id="accd0-103">Операция SearchMailboxes</span><span class="sxs-lookup"><span data-stu-id="accd0-103">SearchMailboxes operation</span></span>

<span data-ttu-id="accd0-104">Найдите сведения о **SearchMailboxes** операции веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="accd0-104">Find information about the **SearchMailboxes** EWS operation.</span></span> 
  
<span data-ttu-id="accd0-105">Операция **SearchMailboxes** осуществляет поиск почтовых ящиков для вхождения термины в элементы почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="accd0-105">The **SearchMailboxes** operation searches mailboxes for occurrences of terms in mailbox items.</span></span> 
  
<span data-ttu-id="accd0-106">Эта операция появилась в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="accd0-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-searchmailboxes-operation"></a><span data-ttu-id="accd0-107">С помощью операции SearchMailboxes</span><span class="sxs-lookup"><span data-stu-id="accd0-107">Using the SearchMailboxes operation</span></span>

<span data-ttu-id="accd0-108">Операция **SearchMailboxes** можно использовать множество одновременных поисковых запросов для выполнения поиска на обнаружение для нескольких почтовых ящиков.</span><span class="sxs-lookup"><span data-stu-id="accd0-108">The **SearchMailboxes** operation can use many simultaneous search queries to perform discovery search on multiple mailboxes.</span></span> <span data-ttu-id="accd0-109">Результаты можно либо статистические сведения о число попыток возникают условия поиска, или Предварительный просмотр элементов, которые содержат условия поиска.</span><span class="sxs-lookup"><span data-stu-id="accd0-109">The results can be either statistical information about the number of times search terms occur, or a preview of the items that contain the search terms.</span></span> 
  
### <a name="searchmailboxes-operation-soap-headers"></a><span data-ttu-id="accd0-110">Заголовки SOAP SearchMailboxes операции</span><span class="sxs-lookup"><span data-stu-id="accd0-110">SearchMailboxes operation SOAP headers</span></span>

<span data-ttu-id="accd0-111">Операция **SearchMailboxes** можно использовать заголовки SOAP, которые перечислены в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="accd0-111">The **SearchMailboxes** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="accd0-112">**Имя заголовка**</span><span class="sxs-lookup"><span data-stu-id="accd0-112">**Header name**</span></span>|<span data-ttu-id="accd0-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="accd0-113">**Element**</span></span>|<span data-ttu-id="accd0-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="accd0-114">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="accd0-115">**ManagementRole**</span><span class="sxs-lookup"><span data-stu-id="accd0-115">**ManagementRole**</span></span> <br/> |[<span data-ttu-id="accd0-116">ManagementRole</span><span class="sxs-lookup"><span data-stu-id="accd0-116">ManagementRole</span></span>](managementrole.md) <br/> |<span data-ttu-id="accd0-117">Идентифицирует ролей сервера, необходимых в порядке для абонентов для запроса.</span><span class="sxs-lookup"><span data-stu-id="accd0-117">Identifies the server roles that are necessary in order for the caller to make the request.</span></span> <span data-ttu-id="accd0-118">Этот заголовок можно применять к запросу.</span><span class="sxs-lookup"><span data-stu-id="accd0-118">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="accd0-119">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="accd0-119">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="accd0-120">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="accd0-120">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="accd0-121">Определяет версию схемы для операции запроса.</span><span class="sxs-lookup"><span data-stu-id="accd0-121">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="accd0-122">Этот заголовок можно применять к запросу.</span><span class="sxs-lookup"><span data-stu-id="accd0-122">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="accd0-123">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="accd0-123">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="accd0-124">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="accd0-124">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="accd0-125">Определяет версию сервера, ответившего на запрос.</span><span class="sxs-lookup"><span data-stu-id="accd0-125">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="accd0-126">Этот заголовок можно применять, чтобы получить ответ.</span><span class="sxs-lookup"><span data-stu-id="accd0-126">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="searchmailboxes-operation-request-example-search-mailboxes-for-number-of-search-term-hits"></a><span data-ttu-id="accd0-127">Пример запроса SearchMailboxes операции: поиск почтовых ящиков для число найденных терминов</span><span class="sxs-lookup"><span data-stu-id="accd0-127">SearchMailboxes operation request example: Search mailboxes for number of search term hits</span></span>

<span data-ttu-id="accd0-128">В следующем примере запрос операции **SearchMailboxes** показано, как использовать два разных запросах для поиска три разных почтовых ящиков статистические сведения о сколько раз в каждом почтовом ящике отображается терминов.</span><span class="sxs-lookup"><span data-stu-id="accd0-128">The following example of a **SearchMailboxes** operation request shows how to use two different queries to search three different mailboxes for statistical information about how many times a term appears in each mailbox.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="accd0-129">В следующем примере элемент [Query](query.md) — intentionaly остаться пустым.</span><span class="sxs-lookup"><span data-stu-id="accd0-129">In this example, the [Query](query.md) element is intentionaly left blank.</span></span> <span data-ttu-id="accd0-130">Показано, как успешный запрос может содержать ошибок на каждой поиска почтовых ящиков.</span><span class="sxs-lookup"><span data-stu-id="accd0-130">This shows how a successful request can contain error conditions on a per mailbox search basis.</span></span> 
  
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

<span data-ttu-id="accd0-131">Запрос SOAP body содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="accd0-131">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="accd0-132">SearchMailboxes</span><span class="sxs-lookup"><span data-stu-id="accd0-132">SearchMailboxes</span></span>](searchmailboxes.md)
    
- [<span data-ttu-id="accd0-133">SearchQueries</span><span class="sxs-lookup"><span data-stu-id="accd0-133">SearchQueries</span></span>](searchqueries.md)
    
- [<span data-ttu-id="accd0-134">MailboxQuery</span><span class="sxs-lookup"><span data-stu-id="accd0-134">MailboxQuery</span></span>](mailboxquery.md)
    
- [<span data-ttu-id="accd0-135">Query</span><span class="sxs-lookup"><span data-stu-id="accd0-135">Query</span></span>](query.md)
    
- [<span data-ttu-id="accd0-136">MailboxSearchScopes</span><span class="sxs-lookup"><span data-stu-id="accd0-136">MailboxSearchScopes</span></span>](mailboxsearchscopes.md)
    
- [<span data-ttu-id="accd0-137">MailboxSearchScope</span><span class="sxs-lookup"><span data-stu-id="accd0-137">MailboxSearchScope</span></span>](mailboxsearchscope.md)
    
- [<span data-ttu-id="accd0-138">Почтовый ящик (строка)</span><span class="sxs-lookup"><span data-stu-id="accd0-138">Mailbox (string)</span></span>](mailbox-string.md)
    
- [<span data-ttu-id="accd0-139">Область поиска</span><span class="sxs-lookup"><span data-stu-id="accd0-139">SearchScope</span></span>](searchscope.md)
    
- [<span data-ttu-id="accd0-140">ResultType</span><span class="sxs-lookup"><span data-stu-id="accd0-140">ResultType</span></span>](resulttype.md)
    
## <a name="successful-searchmailboxes-operation-response"></a><span data-ttu-id="accd0-141">Успешные операции ответа SearchMailboxes</span><span class="sxs-lookup"><span data-stu-id="accd0-141">Successful SearchMailboxes operation response</span></span>

<span data-ttu-id="accd0-142">В следующем примере показано успешного ответа на запрос операции **SearchMailboxes** для получения статистические данные о количестве условий поиска находятся в почтовые ящики конечного времени.</span><span class="sxs-lookup"><span data-stu-id="accd0-142">The following example shows a successful response to a **SearchMailboxes** operation request to get statistical information about the number of times search terms are found in the target mailboxes.</span></span> <span data-ttu-id="accd0-143">Последний запрос содержит пустой элемент **запроса** , который показывает поиска в почтовом ящике неудачных.</span><span class="sxs-lookup"><span data-stu-id="accd0-143">The last query contains an empty **Query** element, which shows a failed mailbox search.</span></span> 
  
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

<span data-ttu-id="accd0-144">Ответ SOAP body содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="accd0-144">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="accd0-145">SearchMailboxesResponse</span><span class="sxs-lookup"><span data-stu-id="accd0-145">SearchMailboxesResponse</span></span>](searchmailboxesresponse.md)
    
- [<span data-ttu-id="accd0-146">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="accd0-146">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="accd0-147">SearchMailboxesResponseMessage</span><span class="sxs-lookup"><span data-stu-id="accd0-147">SearchMailboxesResponseMessage</span></span>](searchmailboxesresponsemessage.md)
    
- [<span data-ttu-id="accd0-148">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="accd0-148">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="accd0-149">SearchMailboxesResult</span><span class="sxs-lookup"><span data-stu-id="accd0-149">SearchMailboxesResult</span></span>](searchmailboxesresult.md)
    
- [<span data-ttu-id="accd0-150">SearchQueries</span><span class="sxs-lookup"><span data-stu-id="accd0-150">SearchQueries</span></span>](searchqueries.md)
    
- [<span data-ttu-id="accd0-151">MailboxQuery</span><span class="sxs-lookup"><span data-stu-id="accd0-151">MailboxQuery</span></span>](mailboxquery.md)
    
- [<span data-ttu-id="accd0-152">Query</span><span class="sxs-lookup"><span data-stu-id="accd0-152">Query</span></span>](query.md)
    
- [<span data-ttu-id="accd0-153">MailboxSearchScopes</span><span class="sxs-lookup"><span data-stu-id="accd0-153">MailboxSearchScopes</span></span>](mailboxsearchscopes.md)
    
- [<span data-ttu-id="accd0-154">MailboxSearchScope</span><span class="sxs-lookup"><span data-stu-id="accd0-154">MailboxSearchScope</span></span>](mailboxsearchscope.md)
    
- [<span data-ttu-id="accd0-155">Почтовый ящик (строка)</span><span class="sxs-lookup"><span data-stu-id="accd0-155">Mailbox (string)</span></span>](mailbox-string.md)
    
- [<span data-ttu-id="accd0-156">Область поиска</span><span class="sxs-lookup"><span data-stu-id="accd0-156">SearchScope</span></span>](searchscope.md)
    
- [<span data-ttu-id="accd0-157">ResultType</span><span class="sxs-lookup"><span data-stu-id="accd0-157">ResultType</span></span>](resulttype.md)
    
- [<span data-ttu-id="accd0-158">ItemCount</span><span class="sxs-lookup"><span data-stu-id="accd0-158">ItemCount</span></span>](itemcount.md)
    
- [<span data-ttu-id="accd0-159">Размер (long)</span><span class="sxs-lookup"><span data-stu-id="accd0-159">Size (long)</span></span>](size-long.md)
    
- [<span data-ttu-id="accd0-160">PageItemCount</span><span class="sxs-lookup"><span data-stu-id="accd0-160">PageItemCount</span></span>](pageitemcount.md)
    
- [<span data-ttu-id="accd0-161">KeywordStats</span><span class="sxs-lookup"><span data-stu-id="accd0-161">KeywordStats</span></span>](keywordstats.md)
    
- [<span data-ttu-id="accd0-162">KeywordStat</span><span class="sxs-lookup"><span data-stu-id="accd0-162">KeywordStat</span></span>](keywordstat.md)
    
- [<span data-ttu-id="accd0-163">Ключевое слово</span><span class="sxs-lookup"><span data-stu-id="accd0-163">Keyword</span></span>](keyword.md)
    
- [<span data-ttu-id="accd0-164">ItemHits</span><span class="sxs-lookup"><span data-stu-id="accd0-164">ItemHits</span></span>](itemhits.md)
    
- [<span data-ttu-id="accd0-165">FailedMailboxes</span><span class="sxs-lookup"><span data-stu-id="accd0-165">FailedMailboxes</span></span>](failedmailboxes.md)
    
- [<span data-ttu-id="accd0-166">FailedMailbox</span><span class="sxs-lookup"><span data-stu-id="accd0-166">FailedMailbox</span></span>](failedmailbox.md)
    
- [<span data-ttu-id="accd0-167">Почтовый ящик (строка)</span><span class="sxs-lookup"><span data-stu-id="accd0-167">Mailbox (string)</span></span>](mailbox-string.md)
    
- [<span data-ttu-id="accd0-168">Код ошибки (int)</span><span class="sxs-lookup"><span data-stu-id="accd0-168">ErrorCode (int)</span></span>](errorcode-int.md)
    
- [<span data-ttu-id="accd0-169">Сообщение об ошибке</span><span class="sxs-lookup"><span data-stu-id="accd0-169">ErrorMessage</span></span>](errormessage.md)
    
- [<span data-ttu-id="accd0-170">IsArchive</span><span class="sxs-lookup"><span data-stu-id="accd0-170">IsArchive</span></span>](isarchive.md)
    
## <a name="searchmailboxes-operation-error-response"></a><span data-ttu-id="accd0-171">Ошибка операции SearchMailboxes ответа</span><span class="sxs-lookup"><span data-stu-id="accd0-171">SearchMailboxes operation error response</span></span>

<span data-ttu-id="accd0-172">В следующем примере показано ошибочный ответ на запрос операции **SearchMailboxes** .</span><span class="sxs-lookup"><span data-stu-id="accd0-172">The following example shows an error response to a **SearchMailboxes** operation request.</span></span> <span data-ttu-id="accd0-173">Это ответ на запрос для поиска в почтовом ящике при неправильный идентификатор почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="accd0-173">This is a response to a request to search a mailbox when the mailbox identifier is incorrect.</span></span> 
  
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

<span data-ttu-id="accd0-174">Ошибка ответ SOAP body содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="accd0-174">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="accd0-175">SearchMailboxesResponse</span><span class="sxs-lookup"><span data-stu-id="accd0-175">SearchMailboxesResponse</span></span>](searchmailboxesresponse.md)
    
- [<span data-ttu-id="accd0-176">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="accd0-176">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="accd0-177">SearchMailboxesResponseMessage</span><span class="sxs-lookup"><span data-stu-id="accd0-177">SearchMailboxesResponseMessage</span></span>](searchmailboxesresponsemessage.md)
    
- [<span data-ttu-id="accd0-178">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="accd0-178">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="accd0-179">SearchMailboxesResult</span><span class="sxs-lookup"><span data-stu-id="accd0-179">SearchMailboxesResult</span></span>](searchmailboxesresult.md)
    
- [<span data-ttu-id="accd0-180">SearchQueries</span><span class="sxs-lookup"><span data-stu-id="accd0-180">SearchQueries</span></span>](searchqueries.md)
    
- [<span data-ttu-id="accd0-181">MailboxQuery</span><span class="sxs-lookup"><span data-stu-id="accd0-181">MailboxQuery</span></span>](mailboxquery.md)
    
- [<span data-ttu-id="accd0-182">Query</span><span class="sxs-lookup"><span data-stu-id="accd0-182">Query</span></span>](query.md)
    
- [<span data-ttu-id="accd0-183">MailboxSearchScopes</span><span class="sxs-lookup"><span data-stu-id="accd0-183">MailboxSearchScopes</span></span>](mailboxsearchscopes.md)
    
- [<span data-ttu-id="accd0-184">MailboxSearchScope</span><span class="sxs-lookup"><span data-stu-id="accd0-184">MailboxSearchScope</span></span>](mailboxsearchscope.md)
    
- [<span data-ttu-id="accd0-185">Почтовый ящик (строка)</span><span class="sxs-lookup"><span data-stu-id="accd0-185">Mailbox (string)</span></span>](mailbox-string.md)
    
- [<span data-ttu-id="accd0-186">Область поиска</span><span class="sxs-lookup"><span data-stu-id="accd0-186">SearchScope</span></span>](searchscope.md)
    
- [<span data-ttu-id="accd0-187">ResultType</span><span class="sxs-lookup"><span data-stu-id="accd0-187">ResultType</span></span>](resulttype.md)
    
- [<span data-ttu-id="accd0-188">ItemCount</span><span class="sxs-lookup"><span data-stu-id="accd0-188">ItemCount</span></span>](itemcount.md)
    
- [<span data-ttu-id="accd0-189">Размер (long)</span><span class="sxs-lookup"><span data-stu-id="accd0-189">Size (long)</span></span>](size-long.md)
    
- [<span data-ttu-id="accd0-190">PageItemCount</span><span class="sxs-lookup"><span data-stu-id="accd0-190">PageItemCount</span></span>](pageitemcount.md)
    
- [<span data-ttu-id="accd0-191">PageItemSize</span><span class="sxs-lookup"><span data-stu-id="accd0-191">PageItemSize</span></span>](pageitemsize.md)
    
- [<span data-ttu-id="accd0-192">FailedMailboxes</span><span class="sxs-lookup"><span data-stu-id="accd0-192">FailedMailboxes</span></span>](failedmailboxes.md)
    
- [<span data-ttu-id="accd0-193">FailedMailbox</span><span class="sxs-lookup"><span data-stu-id="accd0-193">FailedMailbox</span></span>](failedmailbox.md)
    
- [<span data-ttu-id="accd0-194">Почтовый ящик (строка)</span><span class="sxs-lookup"><span data-stu-id="accd0-194">Mailbox (string)</span></span>](mailbox-string.md)
    
- [<span data-ttu-id="accd0-195">Код ошибки (int)</span><span class="sxs-lookup"><span data-stu-id="accd0-195">ErrorCode (int)</span></span>](errorcode-int.md)
    
- [<span data-ttu-id="accd0-196">Сообщение об ошибке</span><span class="sxs-lookup"><span data-stu-id="accd0-196">ErrorMessage</span></span>](errormessage.md)
    
- [<span data-ttu-id="accd0-197">IsArchive</span><span class="sxs-lookup"><span data-stu-id="accd0-197">IsArchive</span></span>](isarchive.md)
    
<span data-ttu-id="accd0-198">Дополнительные коды ошибок, которые являются общими для веб-служб Exchange и специально для этой операции в разделе [ResponseCode](responsecode.md).</span><span class="sxs-lookup"><span data-stu-id="accd0-198">For additional error codes that are generic to EWS and specific to this operation, see [ResponseCode](responsecode.md).</span></span>
  
## <a name="see-also"></a><span data-ttu-id="accd0-199">См. также</span><span class="sxs-lookup"><span data-stu-id="accd0-199">See also</span></span>

- [<span data-ttu-id="accd0-200">Операции EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="accd0-200">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
    
- [<span data-ttu-id="accd0-201">Операция GetSearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="accd0-201">GetSearchableMailboxes operation</span></span>](getsearchablemailboxes-operation.md)
    
- [<span data-ttu-id="accd0-202">Операция SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="accd0-202">SetHoldOnMailboxes operation</span></span>](setholdonmailboxes-operation.md)
    
- [<span data-ttu-id="accd0-203">Операция GetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="accd0-203">GetHoldOnMailboxes operation</span></span>](getholdonmailboxes-operation.md)
    
- [<span data-ttu-id="accd0-204">Операция GetDiscoverySearchConfiguration</span><span class="sxs-lookup"><span data-stu-id="accd0-204">GetDiscoverySearchConfiguration operation</span></span>](getdiscoverysearchconfiguration-operation.md)
    
- [<span data-ttu-id="accd0-205">Операция GetNonIndexableItemDetails</span><span class="sxs-lookup"><span data-stu-id="accd0-205">GetNonIndexableItemDetails operation</span></span>](getnonindexableitemdetails-operation.md)
    
- [<span data-ttu-id="accd0-206">Операция GetNonIndexableItemStatistics</span><span class="sxs-lookup"><span data-stu-id="accd0-206">GetNonIndexableItemStatistics operation</span></span>](getnonindexableitemstatistics-operation.md)
    

