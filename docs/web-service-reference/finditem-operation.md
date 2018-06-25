---
title: FindItem Operation
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FindItem
api_type:
- schema
ms.assetid: ebad6aae-16e7-44de-ae63-a95b24539729
description: Найдите сведения о веб-служб Exchange FindItem операции.
ms.openlocfilehash: b033ac2930981819a20f1336d40058a5f7c03b89
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762579"
---
# <a name="finditem-operation"></a><span data-ttu-id="30e0c-103">FindItem Operation</span><span class="sxs-lookup"><span data-stu-id="30e0c-103">FindItem operation</span></span>

<span data-ttu-id="30e0c-104">Найдите сведения о операции **FindItem** веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="30e0c-104">Find information about the **FindItem** EWS operation.</span></span> 
  
<span data-ttu-id="30e0c-105">Операция **FindItem** выполняет поиск элементов, которые расположены в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="30e0c-105">The **FindItem** operation searches for items that are located in a user's mailbox.</span></span> <span data-ttu-id="30e0c-106">Эта операция предоставляет множество способов для фильтрации и формат возвращения результатов поиска с абонентом.</span><span class="sxs-lookup"><span data-stu-id="30e0c-106">This operation provides many ways to filter and format how search results are returned to the caller.</span></span> 
  
## <a name="using-the-finditem-operation"></a><span data-ttu-id="30e0c-107">С помощью операции FindItem</span><span class="sxs-lookup"><span data-stu-id="30e0c-107">Using the FindItem operation</span></span>

<span data-ttu-id="30e0c-108">Операция запроса **FindItem** предоставляет функциональные возможности для поиска почтовых ящиков и формат, как данные возвращаются в ответе.</span><span class="sxs-lookup"><span data-stu-id="30e0c-108">The **FindItem** operation request provides many ways for you to search a mailbox and format how the data is returned in a response.</span></span> <span data-ttu-id="30e0c-109">В запросе **FindItem** можно указать следующее:</span><span class="sxs-lookup"><span data-stu-id="30e0c-109">You can specify the following in a **FindItem** request:</span></span> 
  
- <span data-ttu-id="30e0c-110">Является ли поиск частичного или удаленные обхода.</span><span class="sxs-lookup"><span data-stu-id="30e0c-110">Whether the search is a shallow or soft-deleted traversal.</span></span> <span data-ttu-id="30e0c-111">Это задание не требуется.</span><span class="sxs-lookup"><span data-stu-id="30e0c-111">Specifying this is required.</span></span> <span data-ttu-id="30e0c-112">Обратите внимание, что удаленные обхода, в сочетании с ограничения поиска приведет к нулю, найденном даже в том случае, если существуют элементы, соответствующие условиям поиска.</span><span class="sxs-lookup"><span data-stu-id="30e0c-112">Note that a soft-deleted traversal combined with a search restriction will result in zero items returned, even if there are items that match the search criteria.</span></span>
    
- <span data-ttu-id="30e0c-113">Форма ответа элементов.</span><span class="sxs-lookup"><span data-stu-id="30e0c-113">The response shape of items.</span></span> <span data-ttu-id="30e0c-114">Определяет свойства, возвращаемого в ответе.</span><span class="sxs-lookup"><span data-stu-id="30e0c-114">This identifies the properties that are returned in the response.</span></span> <span data-ttu-id="30e0c-115">Это задание не требуется.</span><span class="sxs-lookup"><span data-stu-id="30e0c-115">Specifying this is required.</span></span>
    
- <span data-ttu-id="30e0c-116">Папки, из которого требуется выполнить поиск.</span><span class="sxs-lookup"><span data-stu-id="30e0c-116">The folders from which to perform the search.</span></span> <span data-ttu-id="30e0c-117">Это задание не требуется.</span><span class="sxs-lookup"><span data-stu-id="30e0c-117">Specifying this is required.</span></span>
    
- <span data-ttu-id="30e0c-118">Подкачки механизм и Просмотр типов для возврата просматривать данные на страницах.</span><span class="sxs-lookup"><span data-stu-id="30e0c-118">The paging mechanism and view types for returning view data in pages.</span></span> <span data-ttu-id="30e0c-119">Это задание не является обязательным.</span><span class="sxs-lookup"><span data-stu-id="30e0c-119">Specifying this is optional.</span></span>
    
- <span data-ttu-id="30e0c-120">Параметры для группировки и сортировки элементов, которые будут возвращены.</span><span class="sxs-lookup"><span data-stu-id="30e0c-120">Options for grouping and sorting the items that are returned.</span></span> <span data-ttu-id="30e0c-121">Это задание не является обязательным.</span><span class="sxs-lookup"><span data-stu-id="30e0c-121">Specifying this is optional.</span></span>
    
- <span data-ttu-id="30e0c-122">Ограничения поиска или расширенный синтаксис запроса (AQS) строки для фильтрации элементов, которые будут возвращены.</span><span class="sxs-lookup"><span data-stu-id="30e0c-122">Search restrictions or Advanced Query Syntax (AQS) strings for filtering the items that are returned.</span></span> <span data-ttu-id="30e0c-123">Дополнительные сведения об использовании AQS для поиска контента индекса [строки запроса (String)](querystring-string.md)см.</span><span class="sxs-lookup"><span data-stu-id="30e0c-123">For more information about using AQS for content index searches, see [QueryString (String)](querystring-string.md).</span></span> <span data-ttu-id="30e0c-124">Это задание не является обязательным.</span><span class="sxs-lookup"><span data-stu-id="30e0c-124">Specifying this is optional.</span></span>
    
- <span data-ttu-id="30e0c-125">Порядок сортировки для элементов, возвращаемого в ответе.</span><span class="sxs-lookup"><span data-stu-id="30e0c-125">The sort order for items returned in the response.</span></span> <span data-ttu-id="30e0c-126">Это задание не является обязательным.</span><span class="sxs-lookup"><span data-stu-id="30e0c-126">Specifying this is optional.</span></span>
    
<span data-ttu-id="30e0c-127">Операция **FindItem** возвращает только первые 512 байт поддерживающего потоковую передачу свойства.</span><span class="sxs-lookup"><span data-stu-id="30e0c-127">The **FindItem** operation returns only the first 512 bytes of any streamable property.</span></span> <span data-ttu-id="30e0c-128">Для Юникод возвращает первые 255 символов, используя строку Юникода символом null.</span><span class="sxs-lookup"><span data-stu-id="30e0c-128">For Unicode, it returns the first 255 characters by using a null-terminated Unicode string.</span></span> <span data-ttu-id="30e0c-129">Он не возвращает какие-либо форматы текста сообщения или получателей списков.</span><span class="sxs-lookup"><span data-stu-id="30e0c-129">It does not return any of the message body formats or the recipient lists.</span></span> <span data-ttu-id="30e0c-130">**FindItem** возвращает получателя сводки.</span><span class="sxs-lookup"><span data-stu-id="30e0c-130">**FindItem** will return a recipient summary.</span></span> <span data-ttu-id="30e0c-131">Можно использовать [операции GetItem](getitem-operation.md) , чтобы получить дополнительные сведения об элементе.</span><span class="sxs-lookup"><span data-stu-id="30e0c-131">You can use the [GetItem operation](getitem-operation.md) to get the details of an item.</span></span> 
  
 <span data-ttu-id="30e0c-132">**FindItem** возвращает только элемент [Name (EmailAddressType)](name-emailaddresstype.md) и не возвращает элемент [EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) в элементе [почтовых ящиков](mailbox.md) для следующих полей:</span><span class="sxs-lookup"><span data-stu-id="30e0c-132">**FindItem** returns only the [Name (EmailAddressType)](name-emailaddresstype.md) element and does not return the [EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) element in the [Mailbox](mailbox.md) element for the following fields:</span></span> 
  
- <span data-ttu-id="30e0c-133">Поля [из](from.md) сообщений</span><span class="sxs-lookup"><span data-stu-id="30e0c-133">The [From](from.md) field for messages</span></span> 
    
- <span data-ttu-id="30e0c-134">Поле [отправителя](sender.md) для сообщений</span><span class="sxs-lookup"><span data-stu-id="30e0c-134">The [Sender](sender.md) field for messages</span></span> 
    
- <span data-ttu-id="30e0c-135">Поле [Организатор](organizer.md) для элементов календаря</span><span class="sxs-lookup"><span data-stu-id="30e0c-135">The [Organizer](organizer.md) field for calendar items</span></span> 
    
> [!NOTE]
> <span data-ttu-id="30e0c-136">Операция **FindItem** может возвращать результаты в элементе [представления календаря](calendarview.md) .</span><span class="sxs-lookup"><span data-stu-id="30e0c-136">The **FindItem** operation can return results in a [CalendarView](calendarview.md) element.</span></span> <span data-ttu-id="30e0c-137">Элемент **представления календаря** возвращает элементы одного календаря и все вхождения повторяющиеся собрания.</span><span class="sxs-lookup"><span data-stu-id="30e0c-137">The **CalendarView** element returns single calendar items and all occurrences of recurring meetings.</span></span> <span data-ttu-id="30e0c-138">Если элемент **представления календаря** не используется, возвращаются элементы одного календаря и повторяющихся элементов главного календаря.</span><span class="sxs-lookup"><span data-stu-id="30e0c-138">If a **CalendarView** element is not used, single calendar items and recurring master calendar items are returned.</span></span> <span data-ttu-id="30e0c-139">Необходимо развернуть вхождения из образца повторения, если не используется элемент **представления календаря** .</span><span class="sxs-lookup"><span data-stu-id="30e0c-139">The occurrences must be expanded from the recurring master if a **CalendarView** element is not used.</span></span> 
  
<span data-ttu-id="30e0c-140">Операция **FindItem** можно использовать заголовки SOAP, которые перечислены в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="30e0c-140">The **FindItem** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
<span data-ttu-id="30e0c-141">**В таблице 1. Заголовки SOAP FindItem операции**</span><span class="sxs-lookup"><span data-stu-id="30e0c-141">**Table 1. FindItem operation SOAP headers**</span></span>

|<span data-ttu-id="30e0c-142">**Header**</span><span class="sxs-lookup"><span data-stu-id="30e0c-142">**Header**</span></span>|<span data-ttu-id="30e0c-143">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="30e0c-143">**Element**</span></span>|<span data-ttu-id="30e0c-144">**Описание**</span><span class="sxs-lookup"><span data-stu-id="30e0c-144">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="30e0c-145">**DateTimePrecision**</span><span class="sxs-lookup"><span data-stu-id="30e0c-145">**DateTimePrecision**</span></span> <br/> |[<span data-ttu-id="30e0c-146">DateTimePrecision</span><span class="sxs-lookup"><span data-stu-id="30e0c-146">DateTimePrecision</span></span>](datetimeprecision.md) <br/> |<span data-ttu-id="30e0c-147">Указывает разрешение значения времени и данных в ответов с сервера, в секундах или в миллисекундах.</span><span class="sxs-lookup"><span data-stu-id="30e0c-147">Specifies the resolution of data/time values in responses from the server, either in seconds or in milliseconds.</span></span> <span data-ttu-id="30e0c-148">Это применимо к запросу.</span><span class="sxs-lookup"><span data-stu-id="30e0c-148">This is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="30e0c-149">**Олицетворение**</span><span class="sxs-lookup"><span data-stu-id="30e0c-149">**Impersonation**</span></span> <br/> |[<span data-ttu-id="30e0c-150">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="30e0c-150">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="30e0c-151">Идентифицирует пользователя, которого олицетворения в клиентском приложении.</span><span class="sxs-lookup"><span data-stu-id="30e0c-151">Identifies the user whom the client application is impersonating.</span></span> <span data-ttu-id="30e0c-152">Это применимо к запросу.</span><span class="sxs-lookup"><span data-stu-id="30e0c-152">This is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="30e0c-153">**MailboxCulture**</span><span class="sxs-lookup"><span data-stu-id="30e0c-153">**MailboxCulture**</span></span> <br/> |[<span data-ttu-id="30e0c-154">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="30e0c-154">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="30e0c-155">Идентифицирует культуры RFC3066, которые будут использоваться для доступа к почтовому ящику.</span><span class="sxs-lookup"><span data-stu-id="30e0c-155">Identifies the RFC3066 culture to be used to access the mailbox.</span></span> <span data-ttu-id="30e0c-156">Это применимо к запросу.</span><span class="sxs-lookup"><span data-stu-id="30e0c-156">This is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="30e0c-157">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="30e0c-157">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="30e0c-158">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="30e0c-158">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="30e0c-159">Определяет версию схемы для операции запроса.</span><span class="sxs-lookup"><span data-stu-id="30e0c-159">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="30e0c-160">Это применимо к запросу.</span><span class="sxs-lookup"><span data-stu-id="30e0c-160">This is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="30e0c-161">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="30e0c-161">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="30e0c-162">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="30e0c-162">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="30e0c-163">Определяет версию сервера, ответившего на запрос.</span><span class="sxs-lookup"><span data-stu-id="30e0c-163">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="30e0c-164">Это применимо для ответа.</span><span class="sxs-lookup"><span data-stu-id="30e0c-164">This is applicable to a response.</span></span>  <br/> |
|<span data-ttu-id="30e0c-165">**TimeZoneContext**</span><span class="sxs-lookup"><span data-stu-id="30e0c-165">**TimeZoneContext**</span></span> <br/> |[<span data-ttu-id="30e0c-166">TimeZoneContext</span><span class="sxs-lookup"><span data-stu-id="30e0c-166">TimeZoneContext</span></span>](timezonecontext.md) <br/> |<span data-ttu-id="30e0c-167">Определяет часовой пояс, который будет использоваться для всех ответов с сервера.</span><span class="sxs-lookup"><span data-stu-id="30e0c-167">Identifies the time zone to be used for all responses from the server.</span></span> <span data-ttu-id="30e0c-168">Это применимо к запросу.</span><span class="sxs-lookup"><span data-stu-id="30e0c-168">This is applicable to a request.</span></span>  <br/> |
   
## <a name="finditem-operation-request-example"></a><span data-ttu-id="30e0c-169">Пример запроса FindItem операции</span><span class="sxs-lookup"><span data-stu-id="30e0c-169">FindItem operation request example</span></span>

<span data-ttu-id="30e0c-170">В следующем примере запроса **FindItem** показано, как получить идентификатор элемента, определенного в перечислении **IdOnly** [BaseShape](baseshape.md) элемента для элементов, которые находятся в папке «Удаленные».</span><span class="sxs-lookup"><span data-stu-id="30e0c-170">The following example of a **FindItem** request shows how to obtain the item identifier that is defined by the **IdOnly** enumeration of the [BaseShape](baseshape.md) element for items that are found in the Deleted Items folder.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <FindItem xmlns="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
              Traversal="Shallow">
      <ItemShape>
        <t:BaseShape>IdOnly</t:BaseShape>
      </ItemShape>
      <ParentFolderIds>
        <t:DistinguishedFolderId Id="deleteditems"/>
      </ParentFolderIds>
    </FindItem>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="30e0c-171">В запросе используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="30e0c-171">The following elements are used in the request:</span></span> 
  
- [<span data-ttu-id="30e0c-172">FindItem</span><span class="sxs-lookup"><span data-stu-id="30e0c-172">FindItem</span></span>](finditem.md)
    
- [<span data-ttu-id="30e0c-173">ItemShape</span><span class="sxs-lookup"><span data-stu-id="30e0c-173">ItemShape</span></span>](itemshape.md)
    
- [<span data-ttu-id="30e0c-174">BaseShape</span><span class="sxs-lookup"><span data-stu-id="30e0c-174">BaseShape</span></span>](baseshape.md)
    
- [<span data-ttu-id="30e0c-175">ParentFolderIds</span><span class="sxs-lookup"><span data-stu-id="30e0c-175">ParentFolderIds</span></span>](parentfolderids.md)
    
- [<span data-ttu-id="30e0c-176">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="30e0c-176">DistinguishedFolderId</span></span>](distinguishedfolderid.md)
    
<span data-ttu-id="30e0c-177">Дополнительные параметры для сообщения запроса **FindItem** изучите иерархия схемы.</span><span class="sxs-lookup"><span data-stu-id="30e0c-177">For more options for a **FindItem** request message, explore the schema hierarchy.</span></span> <span data-ttu-id="30e0c-178">Начать с [FindItem](finditem.md) элемента.</span><span class="sxs-lookup"><span data-stu-id="30e0c-178">Start at the [FindItem](finditem.md) element.</span></span> 
  
## <a name="successful-finditem-operation-response"></a><span data-ttu-id="30e0c-179">Успешные операции ответа FindItem</span><span class="sxs-lookup"><span data-stu-id="30e0c-179">Successful FindItem operation response</span></span>

<span data-ttu-id="30e0c-180">В следующем примере показано успешного ответа на запрос **FindItem** .</span><span class="sxs-lookup"><span data-stu-id="30e0c-180">The following example shows a successful response to the **FindItem** request.</span></span> 
  
<span data-ttu-id="30e0c-181">Элементы [сообщения](message-ex15websvcsotherref.md) представляют сообщения электронной почты и другие элементы, которые не строго типизированные схемой веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="30e0c-181">[Message](message-ex15websvcsotherref.md) elements represent email messages and all other items that are not strongly typed by the EWS schema.</span></span> <span data-ttu-id="30e0c-182">Элементы, такие как IPM. Общий доступ и IPM.InfoPath возвращаются в виде элементы [сообщения](message-ex15websvcsotherref.md) .</span><span class="sxs-lookup"><span data-stu-id="30e0c-182">Items such as IPM.Sharing and IPM.InfoPath are returned as [Message](message-ex15websvcsotherref.md) elements.</span></span> <span data-ttu-id="30e0c-183">Exchange не возвращает [базовый элемент](item.md) в ответы.</span><span class="sxs-lookup"><span data-stu-id="30e0c-183">Exchange does not return the base [Item](item.md) element in responses.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="595" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <FindItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                      xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                      xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:FindItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:RootFolder TotalItemsInView="10" IncludesLastItemInRange="true">
            <t:Items>
              <t:Message>
                <t:ItemId Id="AS4AUn=" ChangeKey="fsVU4==" />
              </t:Message>
              <t:Message>
                <t:ItemId Id="AS4AUM=" ChangeKey="fsVUA==" />
              </t:Message>
            </t:Items>
          </m:RootFolder>
        </m:FindItemResponseMessage>
      </m:ResponseMessages>
    </FindItemResponse>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="30e0c-184">В ответе используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="30e0c-184">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="30e0c-185">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="30e0c-185">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="30e0c-186">FindItemResponse</span><span class="sxs-lookup"><span data-stu-id="30e0c-186">FindItemResponse</span></span>](finditemresponse.md)
    
- [<span data-ttu-id="30e0c-187">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="30e0c-187">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="30e0c-188">FindItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="30e0c-188">FindItemResponseMessage</span></span>](finditemresponsemessage.md)
    
- [<span data-ttu-id="30e0c-189">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="30e0c-189">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="30e0c-190">RootFolder (FindItemResponseMessage)</span><span class="sxs-lookup"><span data-stu-id="30e0c-190">RootFolder (FindItemResponseMessage)</span></span>](rootfolder-finditemresponsemessage.md)
    
- [<span data-ttu-id="30e0c-191">Элементы</span><span class="sxs-lookup"><span data-stu-id="30e0c-191">Items</span></span>](items.md)
    
- [<span data-ttu-id="30e0c-192">Message</span><span class="sxs-lookup"><span data-stu-id="30e0c-192">Message</span></span>](message-ex15websvcsotherref.md)
    
- [<span data-ttu-id="30e0c-193">Идентификатор элемента</span><span class="sxs-lookup"><span data-stu-id="30e0c-193">ItemId</span></span>](itemid.md)
    
<span data-ttu-id="30e0c-194">Дополнительные параметры для сообщения ответа **FindItem** изучите иерархия схемы.</span><span class="sxs-lookup"><span data-stu-id="30e0c-194">For more options for a **FindItem** response message, explore the schema hierarchy.</span></span> <span data-ttu-id="30e0c-195">Запустите в элементе [FindItemResponse](finditemresponse.md) .</span><span class="sxs-lookup"><span data-stu-id="30e0c-195">Start at the [FindItemResponse](finditemresponse.md) element.</span></span> 
  
## <a name="finditem-operation-error-response"></a><span data-ttu-id="30e0c-196">Ошибка операции FindItem ответа</span><span class="sxs-lookup"><span data-stu-id="30e0c-196">FindItem operation error response</span></span>

<span data-ttu-id="30e0c-197">В следующем примере показано возврату ошибки **FindItem** запрос.</span><span class="sxs-lookup"><span data-stu-id="30e0c-197">The following example shows an error response to a **FindItem** request.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="595" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <FindItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                      xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                      xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:FindItemResponseMessage ResponseClass="Error">
          <m:MessageText>Id is malformed.</m:MessageText>
          <m:ResponseCode>ErrorInvalidIdMalformed</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
        </m:FindItemResponseMessage>
      </m:ResponseMessages>
    </FindItemResponse>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="30e0c-198">В ответ на ошибку используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="30e0c-198">The following elements are used in the error response:</span></span>
  
- [<span data-ttu-id="30e0c-199">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="30e0c-199">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="30e0c-200">FindItemResponse</span><span class="sxs-lookup"><span data-stu-id="30e0c-200">FindItemResponse</span></span>](finditemresponse.md)
    
- [<span data-ttu-id="30e0c-201">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="30e0c-201">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="30e0c-202">FindItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="30e0c-202">FindItemResponseMessage</span></span>](finditemresponsemessage.md)
    
- [<span data-ttu-id="30e0c-203">MessageText</span><span class="sxs-lookup"><span data-stu-id="30e0c-203">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="30e0c-204">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="30e0c-204">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="30e0c-205">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="30e0c-205">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
<span data-ttu-id="30e0c-206">Дополнительные параметры для ответное сообщение об ошибке **FindItem** изучите иерархия схемы.</span><span class="sxs-lookup"><span data-stu-id="30e0c-206">For more options for a **FindItem** error response message, explore the schema hierarchy.</span></span> <span data-ttu-id="30e0c-207">Запустите в элементе [FindItemResponse](finditemresponse.md) .</span><span class="sxs-lookup"><span data-stu-id="30e0c-207">Start at the [FindItemResponse](finditemresponse.md) element.</span></span> 
  
## <a name="version-differences"></a><span data-ttu-id="30e0c-208">Различия версий</span><span class="sxs-lookup"><span data-stu-id="30e0c-208">Version differences</span></span>

<span data-ttu-id="30e0c-209">Версии Exchange, начиная с версии 15 и выполните построение 15.0.898.11 возвращаемое значение ErrorInvalidOperation в элементе [ResponseCode](responsecode.md) при использовании операции **FindItem** для нескольких папки поиска в архивный почтовый ящик.</span><span class="sxs-lookup"><span data-stu-id="30e0c-209">Versions of Exchange starting with major version 15 and ending with build 15.0.898.11 return an ErrorInvalidOperation value in the [ResponseCode](responsecode.md) element when the **FindItem** operation is used to search multiple folders in an archive mailbox.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="30e0c-210">См. также</span><span class="sxs-lookup"><span data-stu-id="30e0c-210">See also</span></span>

- [<span data-ttu-id="30e0c-211">Поиск элементов</span><span class="sxs-lookup"><span data-stu-id="30e0c-211">Finding Items</span></span>](http://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)
    
- [<span data-ttu-id="30e0c-212">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="30e0c-212">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
    
- <span data-ttu-id="30e0c-213">**FindItemType**</span><span class="sxs-lookup"><span data-stu-id="30e0c-213">**FindItemType**</span></span>
    

