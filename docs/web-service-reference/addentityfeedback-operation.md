---
title: Операция AddEntityFeedback
manager: luken
ms.date: 4/18/2016
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 00e40197-5794-4268-b937-bd65aa044890
description: Операция AddEntityFeedback возвращает сведения об ошибке, соответствующее проблем на сервере.
ms.openlocfilehash: b695806f543827d78aea139ffcbd7e4af58b9fef
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761343"
---
# <a name="addentityfeedback-operation"></a><span data-ttu-id="beb83-103">Операция AddEntityFeedback</span><span class="sxs-lookup"><span data-stu-id="beb83-103">AddEntityFeedback operation</span></span>

<span data-ttu-id="beb83-104">Операция **AddEntityFeedback** возвращает сведения об ошибке, соответствующее проблем на сервере.</span><span class="sxs-lookup"><span data-stu-id="beb83-104">The **AddEntityFeedback** operation returns error information corresponding to server-side issues.</span></span> 
  
<span data-ttu-id="beb83-105">Эта операция зависит от типа ведущих запись в журнал событий.</span><span class="sxs-lookup"><span data-stu-id="beb83-105">This operation relies on the type of event being logged.</span></span> <span data-ttu-id="beb83-106">Одной из самых важных событиях является **EntityAdded**, соответствующий выбранной сущности.</span><span class="sxs-lookup"><span data-stu-id="beb83-106">One of the most important events is **EntityAdded**, which corresponds to an entity being selected.</span></span> <span data-ttu-id="beb83-107">Это пакет, поэтому его можно использовать для записи в журнал пакетов записей в одном запросе.</span><span class="sxs-lookup"><span data-stu-id="beb83-107">This operation is batch, so it can be used to log batches of entries in a single request.</span></span> 
  
## <a name="findpeople-request-examples"></a><span data-ttu-id="beb83-108">Примеры запросов FindPeople</span><span class="sxs-lookup"><span data-stu-id="beb83-108">FindPeople request examples</span></span>

<span data-ttu-id="beb83-109">Операция **AddEntityFeedback** позволяет клиентам входить сведений взаимодействия с сущностями, возвращенных службой.</span><span class="sxs-lookup"><span data-stu-id="beb83-109">The **AddEntityFeedback** operation provides a way for clients to log details of interaction with entities returned by the service.</span></span> <span data-ttu-id="beb83-110">Это можно использовать в качестве сигнала для улучшения релевантности в фоновом режиме для каждого клиента.</span><span class="sxs-lookup"><span data-stu-id="beb83-110">This can be used as a signal to improve relevance behind the scenes for each client.</span></span> <span data-ttu-id="beb83-111">Например клиенты могут использовать эту операцию для оставьте свой отзыв на сущности людей, возвращенный из **FindPeople**.</span><span class="sxs-lookup"><span data-stu-id="beb83-111">E.g., Clients can use this operation to provide feedback on people entities returned from **FindPeople**.</span></span>
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
                             xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
                             xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013" />
   </soap:Header>
   <soap:Body >
      <m:AddEntityFeedback>
            <m:EntityFeedbackEntries>
                  <t:EntityFeedbackEntry>
                        <t:ClientEventTimeUTC> 2015-07-05T22:16:18+00:00</t:ClientEventTimeUTC>
                        <t:ClientEventTimeLocal> 2015-07-05T22:16:18+00:00</t:ClientEventTimeLocal>
                        <t:ClientSessionId>00000000-0000-0000-0000-000000000012</t:ClientSessionId>
                        <t:ClientVersion>15.01.0101.01</t:ClientVersion>
                        <t:ClientId>Web</t:ClientId>
                        <t:TransactionId>123456789</t:TransactionId>
                        <t:EventType>EntityAdded</t:EventType>
                        <t:TargetEntityList>["a","b","c"]</t:TargetEntityList>
                        <t:SourceOfEntityAdded></t:SourceOfEntityAdded>
                        <t:JSONPropertyBag></t:JSONPropertyBag>
                  </t:EntityFeedbackEntry>
                  <t:EntityFeedbackEntry>
                  …
                  </t:EntityFeedbackEntry>
            </m:EntityFeedbackEntries>
      </m:AddEntityFeedback>
   </soap:Body>
</soap:Envelope>

```

### <a name="the-request-soap-body-contents"></a><span data-ttu-id="beb83-112">Содержимое текста запроса SOAP</span><span class="sxs-lookup"><span data-stu-id="beb83-112">The request SOAP body contents</span></span>

<span data-ttu-id="beb83-113">Запрос soap содержит один элемент **EntityFeedbackEntries**.</span><span class="sxs-lookup"><span data-stu-id="beb83-113">The soap request contains a single element **EntityFeedbackEntries**.</span></span> <span data-ttu-id="beb83-114">В свою очередь содержит массив объектов **EntityFeedbackEntry** .</span><span class="sxs-lookup"><span data-stu-id="beb83-114">This in turn contains an array of **EntityFeedbackEntry** objects.</span></span> <span data-ttu-id="beb83-115">Каждая запись в массиве может содержать следующие элементы.</span><span class="sxs-lookup"><span data-stu-id="beb83-115">Each entry in the array can contain the following elements.</span></span> 
  
|<span data-ttu-id="beb83-116">**Параметры запроса**</span><span class="sxs-lookup"><span data-stu-id="beb83-116">**Request Parameters**</span></span>|<span data-ttu-id="beb83-117">**Обязательное**</span><span class="sxs-lookup"><span data-stu-id="beb83-117">**Required**</span></span>|<span data-ttu-id="beb83-118">**Описание**</span><span class="sxs-lookup"><span data-stu-id="beb83-118">**Description**</span></span>|<span data-ttu-id="beb83-119">**Тип**</span><span class="sxs-lookup"><span data-stu-id="beb83-119">**Type**</span></span>|
|:-----|:-----|:-----|:-----|
|<span data-ttu-id="beb83-120">**ClientEventTimeUtc**</span><span class="sxs-lookup"><span data-stu-id="beb83-120">**ClientEventTimeUtc**</span></span> <br/> |<span data-ttu-id="beb83-121">Да</span><span class="sxs-lookup"><span data-stu-id="beb83-121">Yes</span></span>  <br/> |<span data-ttu-id="beb83-122">Время в формате UTC произошло событие на стороне клиента.</span><span class="sxs-lookup"><span data-stu-id="beb83-122">The UTC time the event occurred on the client-side.</span></span>  <br/> |<span data-ttu-id="beb83-123">DateTime</span><span class="sxs-lookup"><span data-stu-id="beb83-123">DateTime</span></span>  <br/> |
|<span data-ttu-id="beb83-124">**ClientEventTimeLocal**</span><span class="sxs-lookup"><span data-stu-id="beb83-124">**ClientEventTimeLocal**</span></span> <br/> |<span data-ttu-id="beb83-125">Да</span><span class="sxs-lookup"><span data-stu-id="beb83-125">Yes</span></span>  <br/> |<span data-ttu-id="beb83-126">Местное время возникновения события на стороне клиента.</span><span class="sxs-lookup"><span data-stu-id="beb83-126">The local time the event occurred on the client side.</span></span>  <br/> |<span data-ttu-id="beb83-127">DateTime</span><span class="sxs-lookup"><span data-stu-id="beb83-127">DateTime</span></span>  <br/> |
|<span data-ttu-id="beb83-128">**ClientId**</span><span class="sxs-lookup"><span data-stu-id="beb83-128">**ClientId**</span></span> <br/> |<span data-ttu-id="beb83-129">Да</span><span class="sxs-lookup"><span data-stu-id="beb83-129">Yes</span></span>  <br/> |<span data-ttu-id="beb83-130">Тип клиента (например, Outlook, OWA, и т.д.).</span><span class="sxs-lookup"><span data-stu-id="beb83-130">Type of Client (E.g., Outlook, OWA, etc.).</span></span>  <br/> |<span data-ttu-id="beb83-131">Перечисление ClientIDType</span><span class="sxs-lookup"><span data-stu-id="beb83-131">ClientIDType Enumeration</span></span>  <br/> |
|<span data-ttu-id="beb83-132">**ClientSessionId**</span><span class="sxs-lookup"><span data-stu-id="beb83-132">**ClientSessionId**</span></span> <br/> |<span data-ttu-id="beb83-133">Да</span><span class="sxs-lookup"><span data-stu-id="beb83-133">Yes</span></span>  <br/> |<span data-ttu-id="beb83-134">Идентификатор GUID, идентифицирующий идентификатор сеанса.</span><span class="sxs-lookup"><span data-stu-id="beb83-134">GUID Identifying the session ID.</span></span> <span data-ttu-id="beb83-135">Созданный на стороне клиента.</span><span class="sxs-lookup"><span data-stu-id="beb83-135">Generated on the client.</span></span>  <br/> |<span data-ttu-id="beb83-136">GUID</span><span class="sxs-lookup"><span data-stu-id="beb83-136">GUID</span></span>  <br/> |
|<span data-ttu-id="beb83-137">**ClientVersion**</span><span class="sxs-lookup"><span data-stu-id="beb83-137">**ClientVersion**</span></span> <br/> |<span data-ttu-id="beb83-138">Да</span><span class="sxs-lookup"><span data-stu-id="beb83-138">Yes</span></span>  <br/> |<span data-ttu-id="beb83-139">Версия клиента (например, 15.01.0101.000).</span><span class="sxs-lookup"><span data-stu-id="beb83-139">Version of the client (E.g., 15.01.0101.000).</span></span>  <br/> |<span data-ttu-id="beb83-140">String</span><span class="sxs-lookup"><span data-stu-id="beb83-140">String</span></span>  <br/> |
|<span data-ttu-id="beb83-141">**EntityAddSource**</span><span class="sxs-lookup"><span data-stu-id="beb83-141">**EntityAddSource**</span></span> <br/> |<span data-ttu-id="beb83-142">Нет</span><span class="sxs-lookup"><span data-stu-id="beb83-142">No</span></span>  <br/> |<span data-ttu-id="beb83-143">Источник EntityAded (например, EntityRelevanceAPI, типы, вставляемую).</span><span class="sxs-lookup"><span data-stu-id="beb83-143">Source for EntityAded (E.g., EntityRelevanceAPI, types, pasted).</span></span>  <br/> |<span data-ttu-id="beb83-144">Перечисление EntityAddSource</span><span class="sxs-lookup"><span data-stu-id="beb83-144">EntityAddSource Enumeration</span></span>  <br/> |
|<span data-ttu-id="beb83-145">**EntrySequenceNumber**</span><span class="sxs-lookup"><span data-stu-id="beb83-145">**EntrySequenceNumber**</span></span> <br/> |<span data-ttu-id="beb83-146">Да</span><span class="sxs-lookup"><span data-stu-id="beb83-146">Yes</span></span>  <br/> |<span data-ttu-id="beb83-147">Целое число добавочного на сеанс клиента.</span><span class="sxs-lookup"><span data-stu-id="beb83-147">An incremental integer per client session.</span></span> <span data-ttu-id="beb83-148">Используется для выявления потери данных.</span><span class="sxs-lookup"><span data-stu-id="beb83-148">Used for detecting data loss.</span></span>  <br/> |<span data-ttu-id="beb83-149">Int</span><span class="sxs-lookup"><span data-stu-id="beb83-149">Int</span></span>  <br/> |
|<span data-ttu-id="beb83-150">**EventType**</span><span class="sxs-lookup"><span data-stu-id="beb83-150">**EventType**</span></span> <br/> |<span data-ttu-id="beb83-151">Да</span><span class="sxs-lookup"><span data-stu-id="beb83-151">Yes</span></span>  <br/> |<span data-ttu-id="beb83-152">Тип события (например добавлена сущности, сущность удалена).</span><span class="sxs-lookup"><span data-stu-id="beb83-152">Type of event (E.g., Entity Added, Entity Removed).</span></span>  <br/> |<span data-ttu-id="beb83-153">String</span><span class="sxs-lookup"><span data-stu-id="beb83-153">String</span></span>  <br/> |
|<span data-ttu-id="beb83-154">**JSONPropertyBag**</span><span class="sxs-lookup"><span data-stu-id="beb83-154">**JSONPropertyBag**</span></span> <br/> |<span data-ttu-id="beb83-155">Нет</span><span class="sxs-lookup"><span data-stu-id="beb83-155">No</span></span>  <br/> |<span data-ttu-id="beb83-156">Дополнительные свойства, связанные с событием (JSON больших двоичных объектов из пары "ключ значение").</span><span class="sxs-lookup"><span data-stu-id="beb83-156">Additional properties associated with the event (JSON blob of key/value pairs).</span></span>  <br/> |<span data-ttu-id="beb83-157">JSON больших двоичных объектов</span><span class="sxs-lookup"><span data-stu-id="beb83-157">JSON Blob</span></span>  <br/> |
|<span data-ttu-id="beb83-158">**TargetEntityList**</span><span class="sxs-lookup"><span data-stu-id="beb83-158">**TargetEntityList**</span></span> <br/> |<span data-ttu-id="beb83-159">Нет</span><span class="sxs-lookup"><span data-stu-id="beb83-159">No</span></span>  <br/> |<span data-ttu-id="beb83-160">Список сущностей, связанный с событием.</span><span class="sxs-lookup"><span data-stu-id="beb83-160">List of entities associated with the event.</span></span>  <br/> |<span data-ttu-id="beb83-161">Строка JSON</span><span class="sxs-lookup"><span data-stu-id="beb83-161">JSON String</span></span>  <br/> |
|<span data-ttu-id="beb83-162">**TransactionId**</span><span class="sxs-lookup"><span data-stu-id="beb83-162">**TransactionId**</span></span> <br/> |<span data-ttu-id="beb83-163">Нет</span><span class="sxs-lookup"><span data-stu-id="beb83-163">No</span></span>  <br/> |<span data-ttu-id="beb83-164">Идентификатор (GUID) сопоставления идентификатора журнала запросов.</span><span class="sxs-lookup"><span data-stu-id="beb83-164">ID (GUID) correlating the ID in query logs.</span></span>  <br/> |<span data-ttu-id="beb83-165">String</span><span class="sxs-lookup"><span data-stu-id="beb83-165">String</span></span>  <br/> |
   
### <a name="successful-addentityfeedback-operation-response"></a><span data-ttu-id="beb83-166">Успешные операции ответа AddEntityFeedback</span><span class="sxs-lookup"><span data-stu-id="beb83-166">Successful AddEntityFeedback operation response</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
    <s:Header>
        <h:ServerVersionInfo MajorVersion="15" 
                                MinorVersion="1" 
                                MajorBuildNumber="228" 
                                MinorBuildNumber="0" 
                                Version="V2_49" 
                                xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                                xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                                xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
    </s:Header>
    <s:Body>
        <AddEntityFeedbackResponse ResponseClass="Success" 
                                                              xmlns="http://schemas.microsoft.com/exchange/services/2006/messages" 
                                                              xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                                                              xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance">
            <ResponseCode>NoError</ResponseCode>
            <ErrorCount>0</ErrorCount>
            <ErrorDetails />
        </AddEntityFeedbackResponse>
    </s:Body>
</s:Envelope> 

```

### <a name="the-response-soap-body-contains-the-following-elements"></a><span data-ttu-id="beb83-167">Ответ SOAP body содержит следующие элементы</span><span class="sxs-lookup"><span data-stu-id="beb83-167">The response SOAP body contains the following elements</span></span>

#### <a name="errors"></a><span data-ttu-id="beb83-168">Ошибки</span><span class="sxs-lookup"><span data-stu-id="beb83-168">Errors</span></span> 
  
<span data-ttu-id="beb83-169">API-Интерфейс может войти в пакет записей свои отзывы и предложения, мы все, что мы можем журналов.</span><span class="sxs-lookup"><span data-stu-id="beb83-169">The API can log a batch of feedback entries, we log all that we can.</span></span> <span data-ttu-id="beb83-170">Это поле представляет номер записи об ошибках, которые не были зарегистрированы.</span><span class="sxs-lookup"><span data-stu-id="beb83-170">This field represents the number of error entries that were not logged.</span></span>
    
#### <a name="errordetails"></a><span data-ttu-id="beb83-171">ErrorDetails</span><span class="sxs-lookup"><span data-stu-id="beb83-171">ErrorDetails</span></span>
  
<span data-ttu-id="beb83-172">Сведения, относящиеся к ошибкам выше отделяет, `;`.</span><span class="sxs-lookup"><span data-stu-id="beb83-172">Details pertaining to the errors above separates by `;`.</span></span>
    
### <a name="currently-supported-values"></a><span data-ttu-id="beb83-173">В настоящее время поддерживаются значения</span><span class="sxs-lookup"><span data-stu-id="beb83-173">Currently supported values</span></span>

|<span data-ttu-id="beb83-174">**Перечисление ClientIdType**</span><span class="sxs-lookup"><span data-stu-id="beb83-174">**ClientIdType Enumeration**</span></span>|
|:-----|
|<span data-ttu-id="beb83-175">Настольный ПК</span><span class="sxs-lookup"><span data-stu-id="beb83-175">Desktop</span></span>  <br/> |
|<span data-ttu-id="beb83-176">Exchange</span><span class="sxs-lookup"><span data-stu-id="beb83-176">Exchange</span></span>  <br/> |
|<span data-ttu-id="beb83-177">IMAP4</span><span class="sxs-lookup"><span data-stu-id="beb83-177">IMAP4</span></span>  <br/> |
|<span data-ttu-id="beb83-178">Lync</span><span class="sxs-lookup"><span data-stu-id="beb83-178">Lync</span></span>  <br/> |
|<span data-ttu-id="beb83-179">MacMail</span><span class="sxs-lookup"><span data-stu-id="beb83-179">MacMail</span></span>  <br/> |
|<span data-ttu-id="beb83-180">MacOutlook</span><span class="sxs-lookup"><span data-stu-id="beb83-180">MacOutlook</span></span>  <br/> |
|<span data-ttu-id="beb83-181">Мобильная версия</span><span class="sxs-lookup"><span data-stu-id="beb83-181">Mobile</span></span>  <br/> |
|<span data-ttu-id="beb83-182">Other (другие)</span><span class="sxs-lookup"><span data-stu-id="beb83-182">Other</span></span>  <br/> |
|<span data-ttu-id="beb83-183">Outlook</span><span class="sxs-lookup"><span data-stu-id="beb83-183">Outlook</span></span>  <br/> |
|<span data-ttu-id="beb83-184">OutlookService</span><span class="sxs-lookup"><span data-stu-id="beb83-184">OutlookService</span></span>  <br/> |
|<span data-ttu-id="beb83-185">ПРОТОКОЛ POP3</span><span class="sxs-lookup"><span data-stu-id="beb83-185">POP3</span></span>  <br/> |
|<span data-ttu-id="beb83-186">Планшетный ПК</span><span class="sxs-lookup"><span data-stu-id="beb83-186">Tablet</span></span>  <br/> |
|<span data-ttu-id="beb83-187">"Web" (Интернет);</span><span class="sxs-lookup"><span data-stu-id="beb83-187">Web</span></span>  <br/> |
   
|<span data-ttu-id="beb83-188">**Перечисление EntityAddSource**</span><span class="sxs-lookup"><span data-stu-id="beb83-188">**EntityAddSource Enumeration**</span></span>|
|:-----|
|<span data-ttu-id="beb83-189">ActiveDirectory</span><span class="sxs-lookup"><span data-stu-id="beb83-189">ActiveDirectory</span></span>  <br/> |
|<span data-ttu-id="beb83-190">EntityRelevanceApi</span><span class="sxs-lookup"><span data-stu-id="beb83-190">EntityRelevanceApi</span></span>  <br/> |
|<span data-ttu-id="beb83-191">EntityRelevanceApiCache</span><span class="sxs-lookup"><span data-stu-id="beb83-191">EntityRelevanceApiCache</span></span>  <br/> |
|<span data-ttu-id="beb83-192">ExplicitTyping</span><span class="sxs-lookup"><span data-stu-id="beb83-192">ExplicitTyping</span></span>  <br/> |
|<span data-ttu-id="beb83-193">LocalCache</span><span class="sxs-lookup"><span data-stu-id="beb83-193">LocalCache</span></span>  <br/> |
|<span data-ttu-id="beb83-194">LocalCacheAndEntityRelevanceAPI</span><span class="sxs-lookup"><span data-stu-id="beb83-194">LocalCacheAndEntityRelevanceAPI</span></span>  <br/> |
|<span data-ttu-id="beb83-195">Нет</span><span class="sxs-lookup"><span data-stu-id="beb83-195">None</span></span>  <br/> |
|<span data-ttu-id="beb83-196">Other (другие)</span><span class="sxs-lookup"><span data-stu-id="beb83-196">Other</span></span>  <br/> |
|<span data-ttu-id="beb83-197">Вставить</span><span class="sxs-lookup"><span data-stu-id="beb83-197">Paste</span></span>  <br/> |
   
### <a name="addentityfeedback-operation-error-response"></a><span data-ttu-id="beb83-198">Ошибка операции AddEntityFeedback ответа</span><span class="sxs-lookup"><span data-stu-id="beb83-198">AddEntityFeedback operation error response</span></span>

<span data-ttu-id="beb83-199">Коды ошибок, которые являются общими для веб-служб Exchange в разделе [ResponseCode](responsecode.md).</span><span class="sxs-lookup"><span data-stu-id="beb83-199">For error codes that are generic to EWS, see [ResponseCode](responsecode.md).</span></span>
  
### <a name="example-of-addentityfeedback-in-conjunction-with-findpeople"></a><span data-ttu-id="beb83-200">Пример AddEntityFeedback в сочетании с FindPeople</span><span class="sxs-lookup"><span data-stu-id="beb83-200">Example of AddEntityFeedback in conjunction with FindPeople</span></span>

#### <a name="findpeople-request"></a><span data-ttu-id="beb83-201">Запрос на FindPeople</span><span class="sxs-lookup"><span data-stu-id="beb83-201">FindPeople request</span></span>
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2013" />
  </soap:Header>
<soap:Body >
    <m:FindPeople>
      <m:IndexedPageItemView BasePoint="Beginning" MaxEntriesReturned="100" Offset="0"/>
      <m:QueryString>user1</m:QueryString>
      <m:SearchPeopleSuggestionIndex>true</m:SearchPeopleSuggestionIndex>
    </m:FindPeople>
  </soap:Body>
</soap:Envelope>    
    
```

#### <a name="findpeople-response"></a><span data-ttu-id="beb83-202">FindPeople ответа</span><span class="sxs-lookup"><span data-stu-id="beb83-202">FindPeople response</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
    <s:Header>
        <h:ServerVersionInfo MajorVersion="15" MinorVersion="1" MajorBuildNumber="302" MinorBuildNumber="0" Version="V2_68" xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
    </s:Header>
    <s:Body>
        <FindPeopleResponse ResponseClass="Success" xmlns="http://schemas.microsoft.com/exchange/services/2006/messages" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance">
            <ResponseCode>NoError</ResponseCode>
            <People>
                <Persona xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
                    <PersonaId Id="AAUQAFjZ4UxX8SZCqSPFsmh0cSo=" />
                    <PersonaType>Person</PersonaType>
                    <CreationTime>2015-10-02T23:25:42</CreationTime>
                    <DisplayName>user2</DisplayName>
…
                  </Persona>
            </People>
            <TotalNumberOfPeopleInView>0</TotalNumberOfPeopleInView>
            <FirstMatchingRowIndex>0</FirstMatchingRowIndex>
            <FirstLoadedRowIndex>0</FirstLoadedRowIndex>
            <TransactionId>b56ad16e-5d5a-4574-90f8-b8dd57382be6</TransactionId>
        </FindPeopleResponse>
    </s:Body>
</s:Envelope>

```

#### <a name="addentityfeedback-request"></a><span data-ttu-id="beb83-203">Запрос на AddEntityFeedback</span><span class="sxs-lookup"><span data-stu-id="beb83-203">AddEntityFeedback request</span></span>

```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013" />
   </soap:Header>
   <soap:Body >
      <m:AddEntityFeedback>
<m:EntityFeedbackEntries>
<t:EntityFeedbackEntry>
         <t:ClientEventTimeUtc>2015-07-05T22:16:18+00:00</t:ClientEventTimeUtc>
         <t:ClientEventTimeLocal>2015-07-05T22:16:18+00:00</t:ClientEventTimeLocal>
         <t:ClientSessionId>00000000-0000-0000-0000-000000000012</t:ClientSessionId>
         <t:ClientVersion>15.01.0101.01</t:ClientVersion>
         <t:ClientId>Web</t:ClientId>
         <t:TransactionId>b56ad16e-5d5a-4574-90f8-b8dd57382be6</t:TransactionId>
         <t:EventType>EntityAdded</t:EventType>
         <t:TargetEntityList>["user1@ms7.com"]</t:TargetEntityList>
         <t:SourceOfEntityAdded>EntityRelevanceApi</t:SourceOfEntityAdded>
         <t:JSONPropertyBag></t:JSONPropertyBag>
</t:EntityFeedbackEntry>
</m:EntityFeedbackEntries>
      </m:AddEntityFeedback>
   </soap:Body>
</soap:Envelope>

```

> [!NOTE]
> <span data-ttu-id="beb83-204">С помощью FindPeople код ответа транзакций в качестве транзакций запрос AddEntityFeedback по идентификатору.</span><span class="sxs-lookup"><span data-stu-id="beb83-204">Using FindPeople response transaction ID as the AddEntityFeedback request transaction ID.</span></span> 
  
#### <a name="addentityfeedback-response"></a><span data-ttu-id="beb83-205">AddEntityFeedback ответа</span><span class="sxs-lookup"><span data-stu-id="beb83-205">AddEntityFeedback response</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
    <s:Header>
        <h:ServerVersionInfo MajorVersion="15" MinorVersion="1" MajorBuildNumber="302" MinorBuildNumber="0" Version="V2_68" xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
    </s:Header>
    <s:Body>
        <AddEntityFeedbackResponse ResponseClass="Success" xmlns="http://schemas.microsoft.com/exchange/services/2006/messages" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance">
            <ResponseCode>NoError</ResponseCode>
            <ErrorCount>0</ErrorCount>
            <ErrorDetails />
        </AddEntityFeedbackResponse>
    </s:Body>
</s:Envelope>

```


