---
title: Операция FindItem
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
description: Найдите сведения о операции FindItem EWS.
ms.openlocfilehash: b033ac2930981819a20f1336d40058a5f7c03b89
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762579"
---
# <a name="finditem-operation"></a><span data-ttu-id="6b374-103">Операция FindItem</span><span class="sxs-lookup"><span data-stu-id="6b374-103">FindItem operation</span></span>

<span data-ttu-id="6b374-104">Найдите сведения о операции **FindItem** EWS.</span><span class="sxs-lookup"><span data-stu-id="6b374-104">Find information about the **FindItem** EWS operation.</span></span> 
  
<span data-ttu-id="6b374-105">Операция **FindItem** выполняет поиск элементов, расположенных в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="6b374-105">The **FindItem** operation searches for items that are located in a user's mailbox.</span></span> <span data-ttu-id="6b374-106">Эта операция предоставляет множество способов фильтрации и форматирования результатов поиска для вызывающего абонента.</span><span class="sxs-lookup"><span data-stu-id="6b374-106">This operation provides many ways to filter and format how search results are returned to the caller.</span></span> 
  
## <a name="using-the-finditem-operation"></a><span data-ttu-id="6b374-107">Использование операции FindItem</span><span class="sxs-lookup"><span data-stu-id="6b374-107">Using the FindItem operation</span></span>

<span data-ttu-id="6b374-108">Запрос операции **FindItem** предоставляет множество способов поиска в почтовом ящике и форматирования данных, возвращаемых в ответе.</span><span class="sxs-lookup"><span data-stu-id="6b374-108">The **FindItem** operation request provides many ways for you to search a mailbox and format how the data is returned in a response.</span></span> <span data-ttu-id="6b374-109">В запросе **FindItem** можно указать следующее:</span><span class="sxs-lookup"><span data-stu-id="6b374-109">You can specify the following in a **FindItem** request:</span></span> 
  
- <span data-ttu-id="6b374-110">Указывает, является ли поиск неповерхностным или обратимо удаленным.</span><span class="sxs-lookup"><span data-stu-id="6b374-110">Whether the search is a shallow or soft-deleted traversal.</span></span> <span data-ttu-id="6b374-111">Указание этого параметра является обязательным.</span><span class="sxs-lookup"><span data-stu-id="6b374-111">Specifying this is required.</span></span> <span data-ttu-id="6b374-112">Обратите внимание на то, что обратимо удаленный обход с ограничением поиска приведет к возвращению нулевых элементов, даже если имеются элементы, которые удовлетворяют условиям поиска.</span><span class="sxs-lookup"><span data-stu-id="6b374-112">Note that a soft-deleted traversal combined with a search restriction will result in zero items returned, even if there are items that match the search criteria.</span></span>
    
- <span data-ttu-id="6b374-113">Форма ответа элементов.</span><span class="sxs-lookup"><span data-stu-id="6b374-113">The response shape of items.</span></span> <span data-ttu-id="6b374-114">Определяет свойства, возвращаемые в ответе.</span><span class="sxs-lookup"><span data-stu-id="6b374-114">This identifies the properties that are returned in the response.</span></span> <span data-ttu-id="6b374-115">Указание этого параметра является обязательным.</span><span class="sxs-lookup"><span data-stu-id="6b374-115">Specifying this is required.</span></span>
    
- <span data-ttu-id="6b374-116">Папки, из которых выполняется поиск.</span><span class="sxs-lookup"><span data-stu-id="6b374-116">The folders from which to perform the search.</span></span> <span data-ttu-id="6b374-117">Указание этого параметра является обязательным.</span><span class="sxs-lookup"><span data-stu-id="6b374-117">Specifying this is required.</span></span>
    
- <span data-ttu-id="6b374-118">Механизм разбиения по страницам и типы представлений для возвращения данных представления на страницах.</span><span class="sxs-lookup"><span data-stu-id="6b374-118">The paging mechanism and view types for returning view data in pages.</span></span> <span data-ttu-id="6b374-119">Указание этого параметра необязательно.</span><span class="sxs-lookup"><span data-stu-id="6b374-119">Specifying this is optional.</span></span>
    
- <span data-ttu-id="6b374-120">Параметры для группировки и сортировки возвращаемых элементов.</span><span class="sxs-lookup"><span data-stu-id="6b374-120">Options for grouping and sorting the items that are returned.</span></span> <span data-ttu-id="6b374-121">Указание этого параметра необязательно.</span><span class="sxs-lookup"><span data-stu-id="6b374-121">Specifying this is optional.</span></span>
    
- <span data-ttu-id="6b374-122">Поисковые ограничения или строки расширенного синтаксиса запросов (AQS) для фильтрации возвращаемых элементов.</span><span class="sxs-lookup"><span data-stu-id="6b374-122">Search restrictions or Advanced Query Syntax (AQS) strings for filtering the items that are returned.</span></span> <span data-ttu-id="6b374-123">Дополнительные сведения об использовании AQS для поиска по индексу содержимого: [QueryString (String)](querystring-string.md).</span><span class="sxs-lookup"><span data-stu-id="6b374-123">For more information about using AQS for content index searches, see [QueryString (String)](querystring-string.md).</span></span> <span data-ttu-id="6b374-124">Указание этого параметра необязательно.</span><span class="sxs-lookup"><span data-stu-id="6b374-124">Specifying this is optional.</span></span>
    
- <span data-ttu-id="6b374-125">Порядок сортировки элементов, возвращаемых в ответе.</span><span class="sxs-lookup"><span data-stu-id="6b374-125">The sort order for items returned in the response.</span></span> <span data-ttu-id="6b374-126">Указание этого параметра необязательно.</span><span class="sxs-lookup"><span data-stu-id="6b374-126">Specifying this is optional.</span></span>
    
<span data-ttu-id="6b374-127">Операция **FindItem** возвращает только первые 512 байт любого потокового свойства.</span><span class="sxs-lookup"><span data-stu-id="6b374-127">The **FindItem** operation returns only the first 512 bytes of any streamable property.</span></span> <span data-ttu-id="6b374-128">Для Юникода он возвращает первые 255 символов, используя строку Юникода с завершающим нулем.</span><span class="sxs-lookup"><span data-stu-id="6b374-128">For Unicode, it returns the first 255 characters by using a null-terminated Unicode string.</span></span> <span data-ttu-id="6b374-129">Он не возвращает ни одного из форматов текста сообщения или списков получателей.</span><span class="sxs-lookup"><span data-stu-id="6b374-129">It does not return any of the message body formats or the recipient lists.</span></span> <span data-ttu-id="6b374-130">В **FindItem** будет возвращена сводка по получателю.</span><span class="sxs-lookup"><span data-stu-id="6b374-130">**FindItem** will return a recipient summary.</span></span> <span data-ttu-id="6b374-131">Вы можете использовать [операцию GetItem](getitem-operation.md) для получения сведений об элементе.</span><span class="sxs-lookup"><span data-stu-id="6b374-131">You can use the [GetItem operation](getitem-operation.md) to get the details of an item.</span></span> 
  
 <span data-ttu-id="6b374-132">**FindItem** возвращает только элемент [Name (EmailAddressType)](name-emailaddresstype.md) и не возвращает элемент [EmailAddress (нонемптистрингтипе)](emailaddress-nonemptystringtype.md) в элементе [Mailbox](mailbox.md) для следующих полей:</span><span class="sxs-lookup"><span data-stu-id="6b374-132">**FindItem** returns only the [Name (EmailAddressType)](name-emailaddresstype.md) element and does not return the [EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) element in the [Mailbox](mailbox.md) element for the following fields:</span></span> 
  
- <span data-ttu-id="6b374-133">Поле " [от](from.md) " для сообщений</span><span class="sxs-lookup"><span data-stu-id="6b374-133">The [From](from.md) field for messages</span></span> 
    
- <span data-ttu-id="6b374-134">Поле " [отправитель](sender.md) " для сообщений</span><span class="sxs-lookup"><span data-stu-id="6b374-134">The [Sender](sender.md) field for messages</span></span> 
    
- <span data-ttu-id="6b374-135">Поле " [Организатор](organizer.md) " для элементов календаря</span><span class="sxs-lookup"><span data-stu-id="6b374-135">The [Organizer](organizer.md) field for calendar items</span></span> 
    
> [!NOTE]
> <span data-ttu-id="6b374-136">Операция **FindItem** может возвращать результаты в элементе [CalendarView](calendarview.md) .</span><span class="sxs-lookup"><span data-stu-id="6b374-136">The **FindItem** operation can return results in a [CalendarView](calendarview.md) element.</span></span> <span data-ttu-id="6b374-137">Элемент **CalendarView** возвращает один и тот же элемент календаря и все экземпляры повторяющихся собраний.</span><span class="sxs-lookup"><span data-stu-id="6b374-137">The **CalendarView** element returns single calendar items and all occurrences of recurring meetings.</span></span> <span data-ttu-id="6b374-138">Если элемент **CalendarView** не используется, возвращаются элементы с одним календарем и повторяющиеся элементы основного календаря.</span><span class="sxs-lookup"><span data-stu-id="6b374-138">If a **CalendarView** element is not used, single calendar items and recurring master calendar items are returned.</span></span> <span data-ttu-id="6b374-139">Если элемент **CalendarView** не используется, эти экземпляры необходимо развернуть из повторяющейся основной реплики.</span><span class="sxs-lookup"><span data-stu-id="6b374-139">The occurrences must be expanded from the recurring master if a **CalendarView** element is not used.</span></span> 
  
<span data-ttu-id="6b374-140">Операция **FindItem** может использовать заголовки SOAP, указанные в приведенной ниже таблице.</span><span class="sxs-lookup"><span data-stu-id="6b374-140">The **FindItem** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
<span data-ttu-id="6b374-141">**Таблица 1. Заголовки SOAP для операций FindItem**</span><span class="sxs-lookup"><span data-stu-id="6b374-141">**Table 1. FindItem operation SOAP headers**</span></span>

|<span data-ttu-id="6b374-142">**Header**</span><span class="sxs-lookup"><span data-stu-id="6b374-142">**Header**</span></span>|<span data-ttu-id="6b374-143">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="6b374-143">**Element**</span></span>|<span data-ttu-id="6b374-144">**Описание**</span><span class="sxs-lookup"><span data-stu-id="6b374-144">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="6b374-145">**датетимепреЦисион**</span><span class="sxs-lookup"><span data-stu-id="6b374-145">**DateTimePrecision**</span></span> <br/> |[<span data-ttu-id="6b374-146">датетимепреЦисион</span><span class="sxs-lookup"><span data-stu-id="6b374-146">DateTimePrecision</span></span>](datetimeprecision.md) <br/> |<span data-ttu-id="6b374-147">Задает разрешение значений данных и времени в ответах от сервера: в секундах или в миллисекундах.</span><span class="sxs-lookup"><span data-stu-id="6b374-147">Specifies the resolution of data/time values in responses from the server, either in seconds or in milliseconds.</span></span> <span data-ttu-id="6b374-148">Это относится к запросу.</span><span class="sxs-lookup"><span data-stu-id="6b374-148">This is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="6b374-149">**Олицетворение**</span><span class="sxs-lookup"><span data-stu-id="6b374-149">**Impersonation**</span></span> <br/> |[<span data-ttu-id="6b374-150">ексчанжеимперсонатион</span><span class="sxs-lookup"><span data-stu-id="6b374-150">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="6b374-151">Идентифицирует пользователя, который олицетворяет клиентское приложение.</span><span class="sxs-lookup"><span data-stu-id="6b374-151">Identifies the user whom the client application is impersonating.</span></span> <span data-ttu-id="6b374-152">Это относится к запросу.</span><span class="sxs-lookup"><span data-stu-id="6b374-152">This is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="6b374-153">**маилбокскултуре**</span><span class="sxs-lookup"><span data-stu-id="6b374-153">**MailboxCulture**</span></span> <br/> |[<span data-ttu-id="6b374-154">маилбокскултуре</span><span class="sxs-lookup"><span data-stu-id="6b374-154">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="6b374-155">Определяет язык и региональные параметры RFC3066, которые будут использоваться для доступа к почтовому ящику.</span><span class="sxs-lookup"><span data-stu-id="6b374-155">Identifies the RFC3066 culture to be used to access the mailbox.</span></span> <span data-ttu-id="6b374-156">Это относится к запросу.</span><span class="sxs-lookup"><span data-stu-id="6b374-156">This is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="6b374-157">**рекуестверсион**</span><span class="sxs-lookup"><span data-stu-id="6b374-157">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="6b374-158">рекуестсерверверсион</span><span class="sxs-lookup"><span data-stu-id="6b374-158">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="6b374-159">Определяет версию схемы для запроса операции.</span><span class="sxs-lookup"><span data-stu-id="6b374-159">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="6b374-160">Это относится к запросу.</span><span class="sxs-lookup"><span data-stu-id="6b374-160">This is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="6b374-161">**серверверсион**</span><span class="sxs-lookup"><span data-stu-id="6b374-161">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="6b374-162">серверверсионинфо</span><span class="sxs-lookup"><span data-stu-id="6b374-162">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="6b374-163">Определяет версию сервера, который ответил на запрос.</span><span class="sxs-lookup"><span data-stu-id="6b374-163">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="6b374-164">Это относится к отклику.</span><span class="sxs-lookup"><span data-stu-id="6b374-164">This is applicable to a response.</span></span>  <br/> |
|<span data-ttu-id="6b374-165">**тимезонеконтекст**</span><span class="sxs-lookup"><span data-stu-id="6b374-165">**TimeZoneContext**</span></span> <br/> |[<span data-ttu-id="6b374-166">тимезонеконтекст</span><span class="sxs-lookup"><span data-stu-id="6b374-166">TimeZoneContext</span></span>](timezonecontext.md) <br/> |<span data-ttu-id="6b374-167">Определяет часовой пояс, который будет использоваться для всех ответов сервера.</span><span class="sxs-lookup"><span data-stu-id="6b374-167">Identifies the time zone to be used for all responses from the server.</span></span> <span data-ttu-id="6b374-168">Это относится к запросу.</span><span class="sxs-lookup"><span data-stu-id="6b374-168">This is applicable to a request.</span></span>  <br/> |
   
## <a name="finditem-operation-request-example"></a><span data-ttu-id="6b374-169">Пример запроса операции FindItem</span><span class="sxs-lookup"><span data-stu-id="6b374-169">FindItem operation request example</span></span>

<span data-ttu-id="6b374-170">В приведенном ниже примере запроса **FindItem** показано, как получить идентификатор элемента, определенный перечислением **идонли** элемента [басешапе](baseshape.md) для элементов, которые находятся в папке "Удаленные".</span><span class="sxs-lookup"><span data-stu-id="6b374-170">The following example of a **FindItem** request shows how to obtain the item identifier that is defined by the **IdOnly** enumeration of the [BaseShape](baseshape.md) element for items that are found in the Deleted Items folder.</span></span> 
  
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

<span data-ttu-id="6b374-171">В запросе используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="6b374-171">The following elements are used in the request:</span></span> 
  
- [<span data-ttu-id="6b374-172">FindItem</span><span class="sxs-lookup"><span data-stu-id="6b374-172">FindItem</span></span>](finditem.md)
    
- [<span data-ttu-id="6b374-173">итемшапе</span><span class="sxs-lookup"><span data-stu-id="6b374-173">ItemShape</span></span>](itemshape.md)
    
- [<span data-ttu-id="6b374-174">басешапе</span><span class="sxs-lookup"><span data-stu-id="6b374-174">BaseShape</span></span>](baseshape.md)
    
- [<span data-ttu-id="6b374-175">парентфолдеридс</span><span class="sxs-lookup"><span data-stu-id="6b374-175">ParentFolderIds</span></span>](parentfolderids.md)
    
- [<span data-ttu-id="6b374-176">дистингуишедфолдерид</span><span class="sxs-lookup"><span data-stu-id="6b374-176">DistinguishedFolderId</span></span>](distinguishedfolderid.md)
    
<span data-ttu-id="6b374-177">Чтобы получить дополнительные параметры для сообщения запроса **FindItem** , изучите иерархию схемы.</span><span class="sxs-lookup"><span data-stu-id="6b374-177">For more options for a **FindItem** request message, explore the schema hierarchy.</span></span> <span data-ttu-id="6b374-178">Начните с элемента [FindItem](finditem.md) .</span><span class="sxs-lookup"><span data-stu-id="6b374-178">Start at the [FindItem](finditem.md) element.</span></span> 
  
## <a name="successful-finditem-operation-response"></a><span data-ttu-id="6b374-179">Успешный отклик операции FindItem</span><span class="sxs-lookup"><span data-stu-id="6b374-179">Successful FindItem operation response</span></span>

<span data-ttu-id="6b374-180">В следующем примере показан успешный ответ на запрос **FindItem** .</span><span class="sxs-lookup"><span data-stu-id="6b374-180">The following example shows a successful response to the **FindItem** request.</span></span> 
  
<span data-ttu-id="6b374-181">Элементы [Message](message-ex15websvcsotherref.md) представляют сообщения электронной почты и все остальные элементы, которые не являются строго типизированными схемой EWS.</span><span class="sxs-lookup"><span data-stu-id="6b374-181">[Message](message-ex15websvcsotherref.md) elements represent email messages and all other items that are not strongly typed by the EWS schema.</span></span> <span data-ttu-id="6b374-182">Элементы, такие как IPM. Общий доступ и IPM. InfoPath возвращаются в виде элементов [Message](message-ex15websvcsotherref.md) .</span><span class="sxs-lookup"><span data-stu-id="6b374-182">Items such as IPM.Sharing and IPM.InfoPath are returned as [Message](message-ex15websvcsotherref.md) elements.</span></span> <span data-ttu-id="6b374-183">Exchange не возвращает элемент базового [элемента](item.md) в ответах.</span><span class="sxs-lookup"><span data-stu-id="6b374-183">Exchange does not return the base [Item](item.md) element in responses.</span></span> 
  
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

<span data-ttu-id="6b374-184">В отклике используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="6b374-184">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="6b374-185">серверверсионинфо</span><span class="sxs-lookup"><span data-stu-id="6b374-185">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="6b374-186">финдитемреспонсе</span><span class="sxs-lookup"><span data-stu-id="6b374-186">FindItemResponse</span></span>](finditemresponse.md)
    
- [<span data-ttu-id="6b374-187">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="6b374-187">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="6b374-188">финдитемреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="6b374-188">FindItemResponseMessage</span></span>](finditemresponsemessage.md)
    
- [<span data-ttu-id="6b374-189">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="6b374-189">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="6b374-190">Рутфолдер (Финдитемреспонсемессаже)</span><span class="sxs-lookup"><span data-stu-id="6b374-190">RootFolder (FindItemResponseMessage)</span></span>](rootfolder-finditemresponsemessage.md)
    
- [<span data-ttu-id="6b374-191">Items</span><span class="sxs-lookup"><span data-stu-id="6b374-191">Items</span></span>](items.md)
    
- [<span data-ttu-id="6b374-192">Сообщение</span><span class="sxs-lookup"><span data-stu-id="6b374-192">Message</span></span>](message-ex15websvcsotherref.md)
    
- [<span data-ttu-id="6b374-193">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="6b374-193">ItemId</span></span>](itemid.md)
    
<span data-ttu-id="6b374-194">Для получения дополнительных параметров для ответного сообщения **FindItem** изучите иерархию схемы.</span><span class="sxs-lookup"><span data-stu-id="6b374-194">For more options for a **FindItem** response message, explore the schema hierarchy.</span></span> <span data-ttu-id="6b374-195">Начните с элемента [финдитемреспонсе](finditemresponse.md) .</span><span class="sxs-lookup"><span data-stu-id="6b374-195">Start at the [FindItemResponse](finditemresponse.md) element.</span></span> 
  
## <a name="finditem-operation-error-response"></a><span data-ttu-id="6b374-196">Ответ об ошибке операции FindItem</span><span class="sxs-lookup"><span data-stu-id="6b374-196">FindItem operation error response</span></span>

<span data-ttu-id="6b374-197">В следующем примере показан ответ об ошибке для запроса **FindItem** .</span><span class="sxs-lookup"><span data-stu-id="6b374-197">The following example shows an error response to a **FindItem** request.</span></span> 
  
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

<span data-ttu-id="6b374-198">В ответе на сообщение об ошибке используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="6b374-198">The following elements are used in the error response:</span></span>
  
- [<span data-ttu-id="6b374-199">серверверсионинфо</span><span class="sxs-lookup"><span data-stu-id="6b374-199">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="6b374-200">финдитемреспонсе</span><span class="sxs-lookup"><span data-stu-id="6b374-200">FindItemResponse</span></span>](finditemresponse.md)
    
- [<span data-ttu-id="6b374-201">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="6b374-201">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="6b374-202">финдитемреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="6b374-202">FindItemResponseMessage</span></span>](finditemresponsemessage.md)
    
- [<span data-ttu-id="6b374-203">мессажетекст</span><span class="sxs-lookup"><span data-stu-id="6b374-203">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="6b374-204">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="6b374-204">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="6b374-205">дескриптивелинккэй</span><span class="sxs-lookup"><span data-stu-id="6b374-205">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
<span data-ttu-id="6b374-206">Чтобы получить дополнительные параметры для сообщения об ответе на ошибку **FindItem** , изучите иерархию схемы.</span><span class="sxs-lookup"><span data-stu-id="6b374-206">For more options for a **FindItem** error response message, explore the schema hierarchy.</span></span> <span data-ttu-id="6b374-207">Начните с элемента [финдитемреспонсе](finditemresponse.md) .</span><span class="sxs-lookup"><span data-stu-id="6b374-207">Start at the [FindItemResponse](finditemresponse.md) element.</span></span> 
  
## <a name="version-differences"></a><span data-ttu-id="6b374-208">Различия версий</span><span class="sxs-lookup"><span data-stu-id="6b374-208">Version differences</span></span>

<span data-ttu-id="6b374-209">Версии Exchange, начиная с основной версии 15 и заканчивая сборкой 15.0.898.11, возвращают значение Ерроринвалидоператион в элементе [респонсекоде](responsecode.md) , когда операция **FindItem** используется для поиска в нескольких папках в архивном почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="6b374-209">Versions of Exchange starting with major version 15 and ending with build 15.0.898.11 return an ErrorInvalidOperation value in the [ResponseCode](responsecode.md) element when the **FindItem** operation is used to search multiple folders in an archive mailbox.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="6b374-210">См. также</span><span class="sxs-lookup"><span data-stu-id="6b374-210">See also</span></span>

- [<span data-ttu-id="6b374-211">Поиск элементов</span><span class="sxs-lookup"><span data-stu-id="6b374-211">Finding Items</span></span>](http://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)
    
- [<span data-ttu-id="6b374-212">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="6b374-212">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
    
- <span data-ttu-id="6b374-213">**финдитемтипе**</span><span class="sxs-lookup"><span data-stu-id="6b374-213">**FindItemType**</span></span>
    

