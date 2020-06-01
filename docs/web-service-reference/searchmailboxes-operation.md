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
ms.openlocfilehash: 9ec7e9dd4ef17f22f236e64ca1fdbeb65e6e56fe
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44456776"
---
# <a name="searchmailboxes-operation"></a><span data-ttu-id="5943e-103">Операция SearchMailboxes</span><span class="sxs-lookup"><span data-stu-id="5943e-103">SearchMailboxes operation</span></span>

> [!NOTE]
> <span data-ttu-id="5943e-104">Эта операция устарела и больше не поддерживается корпорацией Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="5943e-104">This operation is deprecated, and no longer supported by Microsoft.</span></span>  <span data-ttu-id="5943e-105">В качестве замены используйте операцию [FindItem](finditem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="5943e-105">As a replacement, please use the [FindItem](finditem-operation.md) operation.</span></span>

<span data-ttu-id="5943e-106">Поиск сведений о **SearchMailboxesной** операции EWS.</span><span class="sxs-lookup"><span data-stu-id="5943e-106">Find information about the **SearchMailboxes** EWS operation.</span></span> 
  
<span data-ttu-id="5943e-107">Операция **SearchMailboxes** выполняет поиск в почтовых ящиках вхождений терминов в элементах почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="5943e-107">The **SearchMailboxes** operation searches mailboxes for occurrences of terms in mailbox items.</span></span> 
  
<span data-ttu-id="5943e-108">Эта операция появилась в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="5943e-108">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-searchmailboxes-operation"></a><span data-ttu-id="5943e-109">Использование операции SearchMailboxes</span><span class="sxs-lookup"><span data-stu-id="5943e-109">Using the SearchMailboxes operation</span></span>

<span data-ttu-id="5943e-110">Для выполнения поиска в нескольких почтовых ящиках с помощью операции **SearchMailboxes** можно использовать несколько одновременных запросов поиска.</span><span class="sxs-lookup"><span data-stu-id="5943e-110">The **SearchMailboxes** operation can use many simultaneous search queries to perform discovery search on multiple mailboxes.</span></span> <span data-ttu-id="5943e-111">Результаты могут представлять собой статистическую информацию о количестве выполняемых условий поиска или предварительном просмотре элементов, содержащих условия поиска.</span><span class="sxs-lookup"><span data-stu-id="5943e-111">The results can be either statistical information about the number of times search terms occur, or a preview of the items that contain the search terms.</span></span> 
  
### <a name="searchmailboxes-operation-soap-headers"></a><span data-ttu-id="5943e-112">Заголовки SOAP операции SearchMailboxes</span><span class="sxs-lookup"><span data-stu-id="5943e-112">SearchMailboxes operation SOAP headers</span></span>

<span data-ttu-id="5943e-113">Операция **SearchMailboxes** может использовать заголовки SOAP, указанные в приведенной ниже таблице.</span><span class="sxs-lookup"><span data-stu-id="5943e-113">The **SearchMailboxes** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="5943e-114">**Имя заголовка**</span><span class="sxs-lookup"><span data-stu-id="5943e-114">**Header name**</span></span>|<span data-ttu-id="5943e-115">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="5943e-115">**Element**</span></span>|<span data-ttu-id="5943e-116">**Описание**</span><span class="sxs-lookup"><span data-stu-id="5943e-116">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="5943e-117">**ManagementRole**</span><span class="sxs-lookup"><span data-stu-id="5943e-117">**ManagementRole**</span></span> <br/> |[<span data-ttu-id="5943e-118">ManagementRole</span><span class="sxs-lookup"><span data-stu-id="5943e-118">ManagementRole</span></span>](managementrole.md) <br/> |<span data-ttu-id="5943e-119">Определяет роли сервера, необходимые для того, чтобы вызывающий абонент мог выполнить запрос.</span><span class="sxs-lookup"><span data-stu-id="5943e-119">Identifies the server roles that are necessary in order for the caller to make the request.</span></span> <span data-ttu-id="5943e-120">Этот заголовок является применимым для запроса.</span><span class="sxs-lookup"><span data-stu-id="5943e-120">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="5943e-121">**рекуестверсион**</span><span class="sxs-lookup"><span data-stu-id="5943e-121">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="5943e-122">рекуестсерверверсион</span><span class="sxs-lookup"><span data-stu-id="5943e-122">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="5943e-123">Определяет версию схемы для запроса операции.</span><span class="sxs-lookup"><span data-stu-id="5943e-123">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="5943e-124">Этот заголовок является применимым для запроса.</span><span class="sxs-lookup"><span data-stu-id="5943e-124">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="5943e-125">**серверверсион**</span><span class="sxs-lookup"><span data-stu-id="5943e-125">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="5943e-126">серверверсионинфо</span><span class="sxs-lookup"><span data-stu-id="5943e-126">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="5943e-127">Определяет версию сервера, который ответил на запрос.</span><span class="sxs-lookup"><span data-stu-id="5943e-127">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="5943e-128">Этот заголовок является применимым для отклика.</span><span class="sxs-lookup"><span data-stu-id="5943e-128">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="searchmailboxes-operation-request-example-search-mailboxes-for-number-of-search-term-hits"></a><span data-ttu-id="5943e-129">Пример запроса операции SearchMailboxes: почтовые ящики поиска для количества совпадений со словами поиска</span><span class="sxs-lookup"><span data-stu-id="5943e-129">SearchMailboxes operation request example: Search mailboxes for number of search term hits</span></span>

<span data-ttu-id="5943e-130">В приведенном ниже примере запроса операции **SearchMailboxes** показано, как использовать два разных запроса для поиска в трех разных почтовых ящиках статистические сведения о том, сколько раз термин отображается в каждом почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="5943e-130">The following example of a **SearchMailboxes** operation request shows how to use two different queries to search three different mailboxes for statistical information about how many times a term appears in each mailbox.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="5943e-131">В этом примере элемент [Query](query.md) является пустым.</span><span class="sxs-lookup"><span data-stu-id="5943e-131">In this example, the [Query](query.md) element is intentionaly left blank.</span></span> <span data-ttu-id="5943e-132">В этом примере показано, как успешный запрос может содержать условия ошибки для каждой базы для поиска почтовых ящиков.</span><span class="sxs-lookup"><span data-stu-id="5943e-132">This shows how a successful request can contain error conditions on a per mailbox search basis.</span></span> 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
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

<span data-ttu-id="5943e-133">Текст SOAP Request содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="5943e-133">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="5943e-134">SearchMailboxes</span><span class="sxs-lookup"><span data-stu-id="5943e-134">SearchMailboxes</span></span>](searchmailboxes.md)
    
- [<span data-ttu-id="5943e-135">сеарчкуериес</span><span class="sxs-lookup"><span data-stu-id="5943e-135">SearchQueries</span></span>](searchqueries.md)
    
- [<span data-ttu-id="5943e-136">маилбокскуери</span><span class="sxs-lookup"><span data-stu-id="5943e-136">MailboxQuery</span></span>](mailboxquery.md)
    
- [<span data-ttu-id="5943e-137">Query</span><span class="sxs-lookup"><span data-stu-id="5943e-137">Query</span></span>](query.md)
    
- [<span data-ttu-id="5943e-138">маилбокссеарчскопес</span><span class="sxs-lookup"><span data-stu-id="5943e-138">MailboxSearchScopes</span></span>](mailboxsearchscopes.md)
    
- [<span data-ttu-id="5943e-139">маилбокссеарчскопе</span><span class="sxs-lookup"><span data-stu-id="5943e-139">MailboxSearchScope</span></span>](mailboxsearchscope.md)
    
- [<span data-ttu-id="5943e-140">Mailbox (строка)</span><span class="sxs-lookup"><span data-stu-id="5943e-140">Mailbox (string)</span></span>](mailbox-string.md)
    
- [<span data-ttu-id="5943e-141">SearchScope</span><span class="sxs-lookup"><span data-stu-id="5943e-141">SearchScope</span></span>](searchscope.md)
    
- [<span data-ttu-id="5943e-142">Тип</span><span class="sxs-lookup"><span data-stu-id="5943e-142">ResultType</span></span>](resulttype.md)
    
## <a name="successful-searchmailboxes-operation-response"></a><span data-ttu-id="5943e-143">Успешный отклик операции SearchMailboxes</span><span class="sxs-lookup"><span data-stu-id="5943e-143">Successful SearchMailboxes operation response</span></span>

<span data-ttu-id="5943e-144">В следующем примере показан успешный ответ на запрос операции **SearchMailboxes** для получения статистической информации о количестве найденных терминов поиска в целевых почтовых ящиках.</span><span class="sxs-lookup"><span data-stu-id="5943e-144">The following example shows a successful response to a **SearchMailboxes** operation request to get statistical information about the number of times search terms are found in the target mailboxes.</span></span> <span data-ttu-id="5943e-145">Последний запрос содержит пустой элемент **запроса** , в котором отображается неудачный Поиск в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="5943e-145">The last query contains an empty **Query** element, which shows a failed mailbox search.</span></span> 
  
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
      <m:SearchMailboxesResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                                 xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
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

<span data-ttu-id="5943e-146">Тело SOAP отклика содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="5943e-146">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="5943e-147">сеарчмаилбоксесреспонсе</span><span class="sxs-lookup"><span data-stu-id="5943e-147">SearchMailboxesResponse</span></span>](searchmailboxesresponse.md)
    
- [<span data-ttu-id="5943e-148">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="5943e-148">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="5943e-149">сеарчмаилбоксесреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="5943e-149">SearchMailboxesResponseMessage</span></span>](searchmailboxesresponsemessage.md)
    
- [<span data-ttu-id="5943e-150">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="5943e-150">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="5943e-151">сеарчмаилбоксесресулт</span><span class="sxs-lookup"><span data-stu-id="5943e-151">SearchMailboxesResult</span></span>](searchmailboxesresult.md)
    
- [<span data-ttu-id="5943e-152">сеарчкуериес</span><span class="sxs-lookup"><span data-stu-id="5943e-152">SearchQueries</span></span>](searchqueries.md)
    
- [<span data-ttu-id="5943e-153">маилбокскуери</span><span class="sxs-lookup"><span data-stu-id="5943e-153">MailboxQuery</span></span>](mailboxquery.md)
    
- [<span data-ttu-id="5943e-154">Query</span><span class="sxs-lookup"><span data-stu-id="5943e-154">Query</span></span>](query.md)
    
- [<span data-ttu-id="5943e-155">маилбокссеарчскопес</span><span class="sxs-lookup"><span data-stu-id="5943e-155">MailboxSearchScopes</span></span>](mailboxsearchscopes.md)
    
- [<span data-ttu-id="5943e-156">маилбокссеарчскопе</span><span class="sxs-lookup"><span data-stu-id="5943e-156">MailboxSearchScope</span></span>](mailboxsearchscope.md)
    
- [<span data-ttu-id="5943e-157">Mailbox (строка)</span><span class="sxs-lookup"><span data-stu-id="5943e-157">Mailbox (string)</span></span>](mailbox-string.md)
    
- [<span data-ttu-id="5943e-158">SearchScope</span><span class="sxs-lookup"><span data-stu-id="5943e-158">SearchScope</span></span>](searchscope.md)
    
- [<span data-ttu-id="5943e-159">Тип</span><span class="sxs-lookup"><span data-stu-id="5943e-159">ResultType</span></span>](resulttype.md)
    
- [<span data-ttu-id="5943e-160">ItemCount</span><span class="sxs-lookup"><span data-stu-id="5943e-160">ItemCount</span></span>](itemcount.md)
    
- [<span data-ttu-id="5943e-161">Размер (длинный)</span><span class="sxs-lookup"><span data-stu-id="5943e-161">Size (long)</span></span>](size-long.md)
    
- [<span data-ttu-id="5943e-162">пажеитемкаунт</span><span class="sxs-lookup"><span data-stu-id="5943e-162">PageItemCount</span></span>](pageitemcount.md)
    
- [<span data-ttu-id="5943e-163">кэйвордстатс</span><span class="sxs-lookup"><span data-stu-id="5943e-163">KeywordStats</span></span>](keywordstats.md)
    
- [<span data-ttu-id="5943e-164">кэйвордстат</span><span class="sxs-lookup"><span data-stu-id="5943e-164">KeywordStat</span></span>](keywordstat.md)
    
- [<span data-ttu-id="5943e-165">Недопустим</span><span class="sxs-lookup"><span data-stu-id="5943e-165">Keyword</span></span>](keyword.md)
    
- [<span data-ttu-id="5943e-166">итемхитс</span><span class="sxs-lookup"><span data-stu-id="5943e-166">ItemHits</span></span>](itemhits.md)
    
- [<span data-ttu-id="5943e-167">фаиледмаилбоксес</span><span class="sxs-lookup"><span data-stu-id="5943e-167">FailedMailboxes</span></span>](failedmailboxes.md)
    
- [<span data-ttu-id="5943e-168">фаиледмаилбокс</span><span class="sxs-lookup"><span data-stu-id="5943e-168">FailedMailbox</span></span>](failedmailbox.md)
    
- [<span data-ttu-id="5943e-169">Mailbox (строка)</span><span class="sxs-lookup"><span data-stu-id="5943e-169">Mailbox (string)</span></span>](mailbox-string.md)
    
- [<span data-ttu-id="5943e-170">ErrorCode (int)</span><span class="sxs-lookup"><span data-stu-id="5943e-170">ErrorCode (int)</span></span>](errorcode-int.md)
    
- [<span data-ttu-id="5943e-171">ErrorMessage</span><span class="sxs-lookup"><span data-stu-id="5943e-171">ErrorMessage</span></span>](errormessage.md)
    
- [<span data-ttu-id="5943e-172">IsArchive</span><span class="sxs-lookup"><span data-stu-id="5943e-172">IsArchive</span></span>](isarchive.md)
    
## <a name="searchmailboxes-operation-error-response"></a><span data-ttu-id="5943e-173">Ответ об ошибке операции SearchMailboxes</span><span class="sxs-lookup"><span data-stu-id="5943e-173">SearchMailboxes operation error response</span></span>

<span data-ttu-id="5943e-174">В следующем примере показан ответ об ошибке для запроса операции **SearchMailboxes** .</span><span class="sxs-lookup"><span data-stu-id="5943e-174">The following example shows an error response to a **SearchMailboxes** operation request.</span></span> <span data-ttu-id="5943e-175">Это ответ на запрос поиска в почтовом ящике при неправильном идентификаторе почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="5943e-175">This is a response to a request to search a mailbox when the mailbox identifier is incorrect.</span></span> 
  
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
      <m:SearchMailboxesResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                                 xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
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

<span data-ttu-id="5943e-176">Основной текст сообщения об ошибке SOAP содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="5943e-176">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="5943e-177">сеарчмаилбоксесреспонсе</span><span class="sxs-lookup"><span data-stu-id="5943e-177">SearchMailboxesResponse</span></span>](searchmailboxesresponse.md)
    
- [<span data-ttu-id="5943e-178">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="5943e-178">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="5943e-179">сеарчмаилбоксесреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="5943e-179">SearchMailboxesResponseMessage</span></span>](searchmailboxesresponsemessage.md)
    
- [<span data-ttu-id="5943e-180">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="5943e-180">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="5943e-181">сеарчмаилбоксесресулт</span><span class="sxs-lookup"><span data-stu-id="5943e-181">SearchMailboxesResult</span></span>](searchmailboxesresult.md)
    
- [<span data-ttu-id="5943e-182">сеарчкуериес</span><span class="sxs-lookup"><span data-stu-id="5943e-182">SearchQueries</span></span>](searchqueries.md)
    
- [<span data-ttu-id="5943e-183">маилбокскуери</span><span class="sxs-lookup"><span data-stu-id="5943e-183">MailboxQuery</span></span>](mailboxquery.md)
    
- [<span data-ttu-id="5943e-184">Query</span><span class="sxs-lookup"><span data-stu-id="5943e-184">Query</span></span>](query.md)
    
- [<span data-ttu-id="5943e-185">маилбокссеарчскопес</span><span class="sxs-lookup"><span data-stu-id="5943e-185">MailboxSearchScopes</span></span>](mailboxsearchscopes.md)
    
- [<span data-ttu-id="5943e-186">маилбокссеарчскопе</span><span class="sxs-lookup"><span data-stu-id="5943e-186">MailboxSearchScope</span></span>](mailboxsearchscope.md)
    
- [<span data-ttu-id="5943e-187">Mailbox (строка)</span><span class="sxs-lookup"><span data-stu-id="5943e-187">Mailbox (string)</span></span>](mailbox-string.md)
    
- [<span data-ttu-id="5943e-188">SearchScope</span><span class="sxs-lookup"><span data-stu-id="5943e-188">SearchScope</span></span>](searchscope.md)
    
- [<span data-ttu-id="5943e-189">Тип</span><span class="sxs-lookup"><span data-stu-id="5943e-189">ResultType</span></span>](resulttype.md)
    
- [<span data-ttu-id="5943e-190">ItemCount</span><span class="sxs-lookup"><span data-stu-id="5943e-190">ItemCount</span></span>](itemcount.md)
    
- [<span data-ttu-id="5943e-191">Размер (длинный)</span><span class="sxs-lookup"><span data-stu-id="5943e-191">Size (long)</span></span>](size-long.md)
    
- [<span data-ttu-id="5943e-192">пажеитемкаунт</span><span class="sxs-lookup"><span data-stu-id="5943e-192">PageItemCount</span></span>](pageitemcount.md)
    
- [<span data-ttu-id="5943e-193">пажеитемсизе</span><span class="sxs-lookup"><span data-stu-id="5943e-193">PageItemSize</span></span>](pageitemsize.md)
    
- [<span data-ttu-id="5943e-194">фаиледмаилбоксес</span><span class="sxs-lookup"><span data-stu-id="5943e-194">FailedMailboxes</span></span>](failedmailboxes.md)
    
- [<span data-ttu-id="5943e-195">фаиледмаилбокс</span><span class="sxs-lookup"><span data-stu-id="5943e-195">FailedMailbox</span></span>](failedmailbox.md)
    
- [<span data-ttu-id="5943e-196">Mailbox (строка)</span><span class="sxs-lookup"><span data-stu-id="5943e-196">Mailbox (string)</span></span>](mailbox-string.md)
    
- [<span data-ttu-id="5943e-197">ErrorCode (int)</span><span class="sxs-lookup"><span data-stu-id="5943e-197">ErrorCode (int)</span></span>](errorcode-int.md)
    
- [<span data-ttu-id="5943e-198">ErrorMessage</span><span class="sxs-lookup"><span data-stu-id="5943e-198">ErrorMessage</span></span>](errormessage.md)
    
- [<span data-ttu-id="5943e-199">IsArchive</span><span class="sxs-lookup"><span data-stu-id="5943e-199">IsArchive</span></span>](isarchive.md)
    
<span data-ttu-id="5943e-200">Дополнительные коды ошибок, которые являются общими для EWS и специфичными для этой операции, можно найти в разделе [респонсекоде](responsecode.md).</span><span class="sxs-lookup"><span data-stu-id="5943e-200">For additional error codes that are generic to EWS and specific to this operation, see [ResponseCode](responsecode.md).</span></span>
  
## <a name="see-also"></a><span data-ttu-id="5943e-201">См. также</span><span class="sxs-lookup"><span data-stu-id="5943e-201">See also</span></span>

- [<span data-ttu-id="5943e-202">Операции EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="5943e-202">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
    
- [<span data-ttu-id="5943e-203">Операция GetSearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="5943e-203">GetSearchableMailboxes operation</span></span>](getsearchablemailboxes-operation.md)
    
- [<span data-ttu-id="5943e-204">Операция SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="5943e-204">SetHoldOnMailboxes operation</span></span>](setholdonmailboxes-operation.md)
    
- [<span data-ttu-id="5943e-205">Операция GetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="5943e-205">GetHoldOnMailboxes operation</span></span>](getholdonmailboxes-operation.md)
    
- [<span data-ttu-id="5943e-206">Операция GetDiscoverySearchConfiguration</span><span class="sxs-lookup"><span data-stu-id="5943e-206">GetDiscoverySearchConfiguration operation</span></span>](getdiscoverysearchconfiguration-operation.md)
    
- [<span data-ttu-id="5943e-207">Операция GetNonIndexableItemDetails</span><span class="sxs-lookup"><span data-stu-id="5943e-207">GetNonIndexableItemDetails operation</span></span>](getnonindexableitemdetails-operation.md)
    
- [<span data-ttu-id="5943e-208">Операция GetNonIndexableItemStatistics</span><span class="sxs-lookup"><span data-stu-id="5943e-208">GetNonIndexableItemStatistics operation</span></span>](getnonindexableitemstatistics-operation.md)
    

