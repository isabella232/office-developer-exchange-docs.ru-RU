---
title: Операция Аддентитифидбакк
manager: luken
ms.date: 4/18/2016
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 00e40197-5794-4268-b937-bd65aa044890
description: Операция Аддентитифидбакк возвращает сведения об ошибке, соответствующие проблемам на стороне сервера.
ms.openlocfilehash: a1027a0a1ee06cf3e83833b1d84c13d77b07c0b9
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458441"
---
# <a name="addentityfeedback-operation"></a><span data-ttu-id="881fd-103">Операция Аддентитифидбакк</span><span class="sxs-lookup"><span data-stu-id="881fd-103">AddEntityFeedback operation</span></span>

<span data-ttu-id="881fd-104">Операция **аддентитифидбакк** возвращает сведения об ошибке, соответствующие проблемам на стороне сервера.</span><span class="sxs-lookup"><span data-stu-id="881fd-104">The **AddEntityFeedback** operation returns error information corresponding to server-side issues.</span></span> 
  
<span data-ttu-id="881fd-105">Эта операция зависит от типа регистрируемого события.</span><span class="sxs-lookup"><span data-stu-id="881fd-105">This operation relies on the type of event being logged.</span></span> <span data-ttu-id="881fd-106">Одно из наиболее важных событий — **ентитяддед**, которое соответствует выбранному объекту.</span><span class="sxs-lookup"><span data-stu-id="881fd-106">One of the most important events is **EntityAdded**, which corresponds to an entity being selected.</span></span> <span data-ttu-id="881fd-107">Эта операция является пакетной, поэтому ее можно использовать для записи пакетов записей в один запрос.</span><span class="sxs-lookup"><span data-stu-id="881fd-107">This operation is batch, so it can be used to log batches of entries in a single request.</span></span> 
  
## <a name="findpeople-request-examples"></a><span data-ttu-id="881fd-108">Примеры запросов FindPeople</span><span class="sxs-lookup"><span data-stu-id="881fd-108">FindPeople request examples</span></span>

<span data-ttu-id="881fd-109">Операция **аддентитифидбакк** предоставляет клиентам возможность заносить в журнал сведения о взаимодействии с сущностями, возвращенными службой.</span><span class="sxs-lookup"><span data-stu-id="881fd-109">The **AddEntityFeedback** operation provides a way for clients to log details of interaction with entities returned by the service.</span></span> <span data-ttu-id="881fd-110">Его можно использовать в качестве сигнала, чтобы увеличить релевантность для каждого клиента.</span><span class="sxs-lookup"><span data-stu-id="881fd-110">This can be used as a signal to improve relevance behind the scenes for each client.</span></span> <span data-ttu-id="881fd-111">Например, клиенты могут использовать эту операцию для предоставления отзывов о сущностях людей, возвращенных из **FindPeople**.</span><span class="sxs-lookup"><span data-stu-id="881fd-111">E.g., Clients can use this operation to provide feedback on people entities returned from **FindPeople**.</span></span>
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
                             xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
                             xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="the-request-soap-body-contents"></a><span data-ttu-id="881fd-112">Содержимое SOAP в тексте запроса</span><span class="sxs-lookup"><span data-stu-id="881fd-112">The request SOAP body contents</span></span>

<span data-ttu-id="881fd-113">SOAP – запрос содержит один элемент **ентитифидбаккентриес**.</span><span class="sxs-lookup"><span data-stu-id="881fd-113">The soap request contains a single element **EntityFeedbackEntries**.</span></span> <span data-ttu-id="881fd-114">Это, в свою очередь, содержит массив объектов **ентитифидбаккентри** .</span><span class="sxs-lookup"><span data-stu-id="881fd-114">This in turn contains an array of **EntityFeedbackEntry** objects.</span></span> <span data-ttu-id="881fd-115">Каждая запись в массиве может содержать следующие элементы.</span><span class="sxs-lookup"><span data-stu-id="881fd-115">Each entry in the array can contain the following elements.</span></span> 
  
|<span data-ttu-id="881fd-116">**Параметры запроса**</span><span class="sxs-lookup"><span data-stu-id="881fd-116">**Request Parameters**</span></span>|<span data-ttu-id="881fd-117">**Обязательный**</span><span class="sxs-lookup"><span data-stu-id="881fd-117">**Required**</span></span>|<span data-ttu-id="881fd-118">**Описание**</span><span class="sxs-lookup"><span data-stu-id="881fd-118">**Description**</span></span>|<span data-ttu-id="881fd-119">**Тип**</span><span class="sxs-lookup"><span data-stu-id="881fd-119">**Type**</span></span>|
|:-----|:-----|:-----|:-----|
|<span data-ttu-id="881fd-120">**клиентевенттимеутк**</span><span class="sxs-lookup"><span data-stu-id="881fd-120">**ClientEventTimeUtc**</span></span> <br/> |<span data-ttu-id="881fd-121">Да</span><span class="sxs-lookup"><span data-stu-id="881fd-121">Yes</span></span>  <br/> |<span data-ttu-id="881fd-122">Время в формате UTC, в котором произошло событие на стороне клиента.</span><span class="sxs-lookup"><span data-stu-id="881fd-122">The UTC time the event occurred on the client-side.</span></span>  <br/> |<span data-ttu-id="881fd-123">DateTime</span><span class="sxs-lookup"><span data-stu-id="881fd-123">DateTime</span></span>  <br/> |
|<span data-ttu-id="881fd-124">**клиентевенттимелокал**</span><span class="sxs-lookup"><span data-stu-id="881fd-124">**ClientEventTimeLocal**</span></span> <br/> |<span data-ttu-id="881fd-125">Да</span><span class="sxs-lookup"><span data-stu-id="881fd-125">Yes</span></span>  <br/> |<span data-ttu-id="881fd-126">Местное время, в течение которого событие произошло на стороне клиента.</span><span class="sxs-lookup"><span data-stu-id="881fd-126">The local time the event occurred on the client side.</span></span>  <br/> |<span data-ttu-id="881fd-127">DateTime</span><span class="sxs-lookup"><span data-stu-id="881fd-127">DateTime</span></span>  <br/> |
|<span data-ttu-id="881fd-128">**ClientId**</span><span class="sxs-lookup"><span data-stu-id="881fd-128">**ClientId**</span></span> <br/> |<span data-ttu-id="881fd-129">Да</span><span class="sxs-lookup"><span data-stu-id="881fd-129">Yes</span></span>  <br/> |<span data-ttu-id="881fd-130">Тип клиента (например, Outlook, OWA и т. д.).</span><span class="sxs-lookup"><span data-stu-id="881fd-130">Type of Client (E.g., Outlook, OWA, etc.).</span></span>  <br/> |<span data-ttu-id="881fd-131">Перечисление Клиентидтипе</span><span class="sxs-lookup"><span data-stu-id="881fd-131">ClientIDType Enumeration</span></span>  <br/> |
|<span data-ttu-id="881fd-132">**клиентсессионид**</span><span class="sxs-lookup"><span data-stu-id="881fd-132">**ClientSessionId**</span></span> <br/> |<span data-ttu-id="881fd-133">Да</span><span class="sxs-lookup"><span data-stu-id="881fd-133">Yes</span></span>  <br/> |<span data-ttu-id="881fd-134">GUID, определяющий идентификатор сеанса.</span><span class="sxs-lookup"><span data-stu-id="881fd-134">GUID Identifying the session ID.</span></span> <span data-ttu-id="881fd-135">Создается на клиенте.</span><span class="sxs-lookup"><span data-stu-id="881fd-135">Generated on the client.</span></span>  <br/> |<span data-ttu-id="881fd-136">Идентификатор GUID</span><span class="sxs-lookup"><span data-stu-id="881fd-136">GUID</span></span>  <br/> |
|<span data-ttu-id="881fd-137">**ClientVersion**</span><span class="sxs-lookup"><span data-stu-id="881fd-137">**ClientVersion**</span></span> <br/> |<span data-ttu-id="881fd-138">Да</span><span class="sxs-lookup"><span data-stu-id="881fd-138">Yes</span></span>  <br/> |<span data-ttu-id="881fd-139">Версия клиента (например, 15.01.0101.000).</span><span class="sxs-lookup"><span data-stu-id="881fd-139">Version of the client (E.g., 15.01.0101.000).</span></span>  <br/> |<span data-ttu-id="881fd-140">String</span><span class="sxs-lookup"><span data-stu-id="881fd-140">String</span></span>  <br/> |
|<span data-ttu-id="881fd-141">**ентитяддсаурце**</span><span class="sxs-lookup"><span data-stu-id="881fd-141">**EntityAddSource**</span></span> <br/> |<span data-ttu-id="881fd-142">Нет</span><span class="sxs-lookup"><span data-stu-id="881fd-142">No</span></span>  <br/> |<span data-ttu-id="881fd-143">Источник для Ентитядед (например, Ентитирелеванцеапи, типы, вставленные).</span><span class="sxs-lookup"><span data-stu-id="881fd-143">Source for EntityAded (E.g., EntityRelevanceAPI, types, pasted).</span></span>  <br/> |<span data-ttu-id="881fd-144">Перечисление Ентитяддсаурце</span><span class="sxs-lookup"><span data-stu-id="881fd-144">EntityAddSource Enumeration</span></span>  <br/> |
|<span data-ttu-id="881fd-145">**ентрисекуенценумбер**</span><span class="sxs-lookup"><span data-stu-id="881fd-145">**EntrySequenceNumber**</span></span> <br/> |<span data-ttu-id="881fd-146">Да</span><span class="sxs-lookup"><span data-stu-id="881fd-146">Yes</span></span>  <br/> |<span data-ttu-id="881fd-147">Добавочное целое число на каждый сеанс клиента.</span><span class="sxs-lookup"><span data-stu-id="881fd-147">An incremental integer per client session.</span></span> <span data-ttu-id="881fd-148">Используется для обнаружения потери данных.</span><span class="sxs-lookup"><span data-stu-id="881fd-148">Used for detecting data loss.</span></span>  <br/> |<span data-ttu-id="881fd-149">Целое</span><span class="sxs-lookup"><span data-stu-id="881fd-149">Int</span></span>  <br/> |
|<span data-ttu-id="881fd-150">**EventType**</span><span class="sxs-lookup"><span data-stu-id="881fd-150">**EventType**</span></span> <br/> |<span data-ttu-id="881fd-151">Да</span><span class="sxs-lookup"><span data-stu-id="881fd-151">Yes</span></span>  <br/> |<span data-ttu-id="881fd-152">Тип события (например, добавленная сущность, Удаленная сущность).</span><span class="sxs-lookup"><span data-stu-id="881fd-152">Type of event (E.g., Entity Added, Entity Removed).</span></span>  <br/> |<span data-ttu-id="881fd-153">String</span><span class="sxs-lookup"><span data-stu-id="881fd-153">String</span></span>  <br/> |
|<span data-ttu-id="881fd-154">**жсонпропертибаг**</span><span class="sxs-lookup"><span data-stu-id="881fd-154">**JSONPropertyBag**</span></span> <br/> |<span data-ttu-id="881fd-155">Нет</span><span class="sxs-lookup"><span data-stu-id="881fd-155">No</span></span>  <br/> |<span data-ttu-id="881fd-156">Дополнительные свойства, связанные с событием (BLOB-объект JSON пар "ключ-значение").</span><span class="sxs-lookup"><span data-stu-id="881fd-156">Additional properties associated with the event (JSON blob of key/value pairs).</span></span>  <br/> |<span data-ttu-id="881fd-157">Большой двоичный объект JSON</span><span class="sxs-lookup"><span data-stu-id="881fd-157">JSON Blob</span></span>  <br/> |
|<span data-ttu-id="881fd-158">**таржетентитилист**</span><span class="sxs-lookup"><span data-stu-id="881fd-158">**TargetEntityList**</span></span> <br/> |<span data-ttu-id="881fd-159">Нет</span><span class="sxs-lookup"><span data-stu-id="881fd-159">No</span></span>  <br/> |<span data-ttu-id="881fd-160">Список сущностей, связанных с событием.</span><span class="sxs-lookup"><span data-stu-id="881fd-160">List of entities associated with the event.</span></span>  <br/> |<span data-ttu-id="881fd-161">Строка JSON</span><span class="sxs-lookup"><span data-stu-id="881fd-161">JSON String</span></span>  <br/> |
|<span data-ttu-id="881fd-162">**трансактионид**</span><span class="sxs-lookup"><span data-stu-id="881fd-162">**TransactionId**</span></span> <br/> |<span data-ttu-id="881fd-163">Нет</span><span class="sxs-lookup"><span data-stu-id="881fd-163">No</span></span>  <br/> |<span data-ttu-id="881fd-164">ID (GUID), который сопоставляет идентификатор в журналах запросов.</span><span class="sxs-lookup"><span data-stu-id="881fd-164">ID (GUID) correlating the ID in query logs.</span></span>  <br/> |<span data-ttu-id="881fd-165">String</span><span class="sxs-lookup"><span data-stu-id="881fd-165">String</span></span>  <br/> |
   
### <a name="successful-addentityfeedback-operation-response"></a><span data-ttu-id="881fd-166">Успешный отклик операции Аддентитифидбакк</span><span class="sxs-lookup"><span data-stu-id="881fd-166">Successful AddEntityFeedback operation response</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
    <s:Header>
        <h:ServerVersionInfo MajorVersion="15" 
                                MinorVersion="1" 
                                MajorBuildNumber="228" 
                                MinorBuildNumber="0" 
                                Version="V2_49" 
                                xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                                xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                                xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
    </s:Header>
    <s:Body>
        <AddEntityFeedbackResponse ResponseClass="Success" 
                                                              xmlns="https://schemas.microsoft.com/exchange/services/2006/messages" 
                                                              xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                                                              xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance">
            <ResponseCode>NoError</ResponseCode>
            <ErrorCount>0</ErrorCount>
            <ErrorDetails />
        </AddEntityFeedbackResponse>
    </s:Body>
</s:Envelope> 

```

### <a name="the-response-soap-body-contains-the-following-elements"></a><span data-ttu-id="881fd-167">Основной текст SOAP отклика содержит указанные ниже элементы.</span><span class="sxs-lookup"><span data-stu-id="881fd-167">The response SOAP body contains the following elements</span></span>

#### <a name="errors"></a><span data-ttu-id="881fd-168">Ошибки</span><span class="sxs-lookup"><span data-stu-id="881fd-168">Errors</span></span> 
  
<span data-ttu-id="881fd-169">API может заносить в журнал пакет записей отзывов, которые мы можем выполнить.</span><span class="sxs-lookup"><span data-stu-id="881fd-169">The API can log a batch of feedback entries, we log all that we can.</span></span> <span data-ttu-id="881fd-170">В этом поле представлено количество ошибочных операций, которые не были занесены в журнал.</span><span class="sxs-lookup"><span data-stu-id="881fd-170">This field represents the number of error entries that were not logged.</span></span>
    
#### <a name="errordetails"></a><span data-ttu-id="881fd-171">еррордетаилс</span><span class="sxs-lookup"><span data-stu-id="881fd-171">ErrorDetails</span></span>
  
<span data-ttu-id="881fd-172">Сведения, относящиеся к ошибкам, приведенным выше в разделе `;` .</span><span class="sxs-lookup"><span data-stu-id="881fd-172">Details pertaining to the errors above separates by `;`.</span></span>
    
### <a name="currently-supported-values"></a><span data-ttu-id="881fd-173">Текущие поддерживаемые значения</span><span class="sxs-lookup"><span data-stu-id="881fd-173">Currently supported values</span></span>

|<span data-ttu-id="881fd-174">**Перечисление Клиентидтипе**</span><span class="sxs-lookup"><span data-stu-id="881fd-174">**ClientIdType Enumeration**</span></span>|
|:-----|
|<span data-ttu-id="881fd-175">Desktop</span><span class="sxs-lookup"><span data-stu-id="881fd-175">Desktop</span></span>  <br/> |
|<span data-ttu-id="881fd-176">Exchange</span><span class="sxs-lookup"><span data-stu-id="881fd-176">Exchange</span></span>  <br/> |
|<span data-ttu-id="881fd-177">IMAP4</span><span class="sxs-lookup"><span data-stu-id="881fd-177">IMAP4</span></span>  <br/> |
|<span data-ttu-id="881fd-178">Lync</span><span class="sxs-lookup"><span data-stu-id="881fd-178">Lync</span></span>  <br/> |
|<span data-ttu-id="881fd-179">макмаил</span><span class="sxs-lookup"><span data-stu-id="881fd-179">MacMail</span></span>  <br/> |
|<span data-ttu-id="881fd-180">макаутлук</span><span class="sxs-lookup"><span data-stu-id="881fd-180">MacOutlook</span></span>  <br/> |
|<span data-ttu-id="881fd-181">Mobile</span><span class="sxs-lookup"><span data-stu-id="881fd-181">Mobile</span></span>  <br/> |
|<span data-ttu-id="881fd-182">Другое</span><span class="sxs-lookup"><span data-stu-id="881fd-182">Other</span></span>  <br/> |
|<span data-ttu-id="881fd-183">Outlook</span><span class="sxs-lookup"><span data-stu-id="881fd-183">Outlook</span></span>  <br/> |
|<span data-ttu-id="881fd-184">Откройте файл outlookservice</span><span class="sxs-lookup"><span data-stu-id="881fd-184">OutlookService</span></span>  <br/> |
|<span data-ttu-id="881fd-185">Служба</span><span class="sxs-lookup"><span data-stu-id="881fd-185">POP3</span></span>  <br/> |
|<span data-ttu-id="881fd-186">Tablet</span><span class="sxs-lookup"><span data-stu-id="881fd-186">Tablet</span></span>  <br/> |
|<span data-ttu-id="881fd-187">Web</span><span class="sxs-lookup"><span data-stu-id="881fd-187">Web</span></span>  <br/> |
   
|<span data-ttu-id="881fd-188">**Перечисление Ентитяддсаурце**</span><span class="sxs-lookup"><span data-stu-id="881fd-188">**EntityAddSource Enumeration**</span></span>|
|:-----|
|<span data-ttu-id="881fd-189">ActiveDirectory</span><span class="sxs-lookup"><span data-stu-id="881fd-189">ActiveDirectory</span></span>  <br/> |
|<span data-ttu-id="881fd-190">ентитирелеванцеапи</span><span class="sxs-lookup"><span data-stu-id="881fd-190">EntityRelevanceApi</span></span>  <br/> |
|<span data-ttu-id="881fd-191">ентитирелеванцеапикаче</span><span class="sxs-lookup"><span data-stu-id="881fd-191">EntityRelevanceApiCache</span></span>  <br/> |
|<span data-ttu-id="881fd-192">експлиЦиттипинг</span><span class="sxs-lookup"><span data-stu-id="881fd-192">ExplicitTyping</span></span>  <br/> |
|<span data-ttu-id="881fd-193">локалкаче</span><span class="sxs-lookup"><span data-stu-id="881fd-193">LocalCache</span></span>  <br/> |
|<span data-ttu-id="881fd-194">локалкачеандентитирелеванцеапи</span><span class="sxs-lookup"><span data-stu-id="881fd-194">LocalCacheAndEntityRelevanceAPI</span></span>  <br/> |
|<span data-ttu-id="881fd-195">Нет</span><span class="sxs-lookup"><span data-stu-id="881fd-195">None</span></span>  <br/> |
|<span data-ttu-id="881fd-196">Другое</span><span class="sxs-lookup"><span data-stu-id="881fd-196">Other</span></span>  <br/> |
|<span data-ttu-id="881fd-197">Вставить</span><span class="sxs-lookup"><span data-stu-id="881fd-197">Paste</span></span>  <br/> |
   
### <a name="addentityfeedback-operation-error-response"></a><span data-ttu-id="881fd-198">Ответ об ошибке операции Аддентитифидбакк</span><span class="sxs-lookup"><span data-stu-id="881fd-198">AddEntityFeedback operation error response</span></span>

<span data-ttu-id="881fd-199">Коды ошибок, являющиеся общими для EWS, представлены в разделе [респонсекоде](responsecode.md).</span><span class="sxs-lookup"><span data-stu-id="881fd-199">For error codes that are generic to EWS, see [ResponseCode](responsecode.md).</span></span>
  
### <a name="example-of-addentityfeedback-in-conjunction-with-findpeople"></a><span data-ttu-id="881fd-200">Пример Аддентитифидбакк в сочетании с FindPeople</span><span class="sxs-lookup"><span data-stu-id="881fd-200">Example of AddEntityFeedback in conjunction with FindPeople</span></span>

#### <a name="findpeople-request"></a><span data-ttu-id="881fd-201">Запрос FindPeople</span><span class="sxs-lookup"><span data-stu-id="881fd-201">FindPeople request</span></span>
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
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

#### <a name="findpeople-response"></a><span data-ttu-id="881fd-202">Ответ FindPeople</span><span class="sxs-lookup"><span data-stu-id="881fd-202">FindPeople response</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
    <s:Header>
        <h:ServerVersionInfo MajorVersion="15" MinorVersion="1" MajorBuildNumber="302" MinorBuildNumber="0" Version="V2_68" xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
    </s:Header>
    <s:Body>
        <FindPeopleResponse ResponseClass="Success" xmlns="https://schemas.microsoft.com/exchange/services/2006/messages" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance">
            <ResponseCode>NoError</ResponseCode>
            <People>
                <Persona xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
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

#### <a name="addentityfeedback-request"></a><span data-ttu-id="881fd-203">Запрос Аддентитифидбакк</span><span class="sxs-lookup"><span data-stu-id="881fd-203">AddEntityFeedback request</span></span>

```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
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
> <span data-ttu-id="881fd-204">Использование идентификатора транзакции ответа FindPeople в качестве идентификатора транзакции запроса Аддентитифидбакк.</span><span class="sxs-lookup"><span data-stu-id="881fd-204">Using FindPeople response transaction ID as the AddEntityFeedback request transaction ID.</span></span> 
  
#### <a name="addentityfeedback-response"></a><span data-ttu-id="881fd-205">Ответ Аддентитифидбакк</span><span class="sxs-lookup"><span data-stu-id="881fd-205">AddEntityFeedback response</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
    <s:Header>
        <h:ServerVersionInfo MajorVersion="15" MinorVersion="1" MajorBuildNumber="302" MinorBuildNumber="0" Version="V2_68" xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
    </s:Header>
    <s:Body>
        <AddEntityFeedbackResponse ResponseClass="Success" xmlns="https://schemas.microsoft.com/exchange/services/2006/messages" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance">
            <ResponseCode>NoError</ResponseCode>
            <ErrorCount>0</ErrorCount>
            <ErrorDetails />
        </AddEntityFeedbackResponse>
    </s:Body>
</s:Envelope>

```


