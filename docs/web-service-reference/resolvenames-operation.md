---
title: Операция ResolveNames
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ResolveNames
api_type:
- schema
ms.assetid: 6b4eb4b3-9ad6-4804-a09f-7e20cfea4dbb
description: Операция ResolveNames разрешает неоднозначные адреса электронной почты и отображаемые имена.
ms.openlocfilehash: 51728addddd2bfb9d35b874ae8c11e83a4c8629b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44468280"
---
# <a name="resolvenames-operation"></a><span data-ttu-id="38109-103">Операция ResolveNames</span><span class="sxs-lookup"><span data-stu-id="38109-103">ResolveNames operation</span></span>

<span data-ttu-id="38109-104">Операция **ResolveNames** разрешает неоднозначные адреса электронной почты и отображаемые имена.</span><span class="sxs-lookup"><span data-stu-id="38109-104">The **ResolveNames** operation resolves ambiguous email addresses and display names.</span></span> 
  
## <a name="using-the-resolvenames-operation"></a><span data-ttu-id="38109-105">Использование операции ResolveNames</span><span class="sxs-lookup"><span data-stu-id="38109-105">Using the ResolveNames operation</span></span>

<span data-ttu-id="38109-106">Эту операцию можно использовать для проверки псевдонимов и разрешения отображаемых имен соответствующему пользователю почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="38109-106">This operation can be used to verify aliases and resolve display names to the appropriate mailbox user.</span></span> <span data-ttu-id="38109-107">Если существуют неоднозначные имена, ответ операции **ResolveNames** предоставляет сведения о каждом пользователе почтового ящика, чтобы клиентское приложение могло разрешить имена.</span><span class="sxs-lookup"><span data-stu-id="38109-107">If ambiguous names exist, the **ResolveNames** operation response provides information about each mailbox user so that the client application can resolve the names.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="38109-108">Примечания</span><span class="sxs-lookup"><span data-stu-id="38109-108">Remarks</span></span>

<span data-ttu-id="38109-109">Ответ ResolveNames возвращает не более 100 кандидатов.</span><span class="sxs-lookup"><span data-stu-id="38109-109">The ResolveNames response returns a maximum of 100 candidates.</span></span> <span data-ttu-id="38109-110">Возвращаемые кандидаты 100 являются первыми 100, которые встречаются в операции поиска.</span><span class="sxs-lookup"><span data-stu-id="38109-110">The 100 candidates that are returned are the first 100 that are encountered in the lookup operation.</span></span>
  
<span data-ttu-id="38109-111">Адреса электронной почты с предфиксированными типами маршрутизации, такими как SMTP или SIP, сохраняются в массиве с несколькими значениями.</span><span class="sxs-lookup"><span data-stu-id="38109-111">Email addresses with prefixed routing types, such as smtp or sip, are saved in a multivalue array.</span></span> <span data-ttu-id="38109-112">Операция **ResolveNames** выполняет частичное соответствие с каждым значением этого массива при добавлении типа маршрутизации в начале неизвестного имени, например "SIP:user1@Contoso.com".</span><span class="sxs-lookup"><span data-stu-id="38109-112">The **ResolveNames** operation performs a partial match against each value of that array when you add the routing type at the beginning of the unresolved name, such as "sip:User1@Contoso.com".</span></span> <span data-ttu-id="38109-113">Если не указать тип маршрутизации, **ResolveNames** по умолчанию будет иметь тип маршрутизации SMTP, сопоставлять его с основным свойством SMTP-адреса, а не выполнять поиск по многозначному массиву.</span><span class="sxs-lookup"><span data-stu-id="38109-113">If you don't specify a routing type, **ResolveNames** will default to the routing type of smtp, match it to a primary smtp address property, and not search the multivalue array.</span></span> 
  
<span data-ttu-id="38109-114">В одном запросе можно указать только одно неоднозначное имя.</span><span class="sxs-lookup"><span data-stu-id="38109-114">Only one ambiguous name can be specified in a single request.</span></span> <span data-ttu-id="38109-115">Сначала выполняется поиск в Active Directory, а затем выполняется поиск в папке контактов пользователя.</span><span class="sxs-lookup"><span data-stu-id="38109-115">Active Directory is searched first, and then the user's contact folder is searched.</span></span> <span data-ttu-id="38109-116">Разрешенные записи из папки контактов пользователя имеют свойство **ItemId** , отличное от NULL, которое затем можно использовать в запросе GetItem.</span><span class="sxs-lookup"><span data-stu-id="38109-116">Resolved entries from a user's contact folder have a non-null **ItemId** property, which can then be used in a GetItem request.</span></span> <span data-ttu-id="38109-117">Если это идентификатор частного списка рассылки, его можно использовать в [операции ExpandDL](expanddl-operation.md).</span><span class="sxs-lookup"><span data-stu-id="38109-117">If it is the ID of a private distribution list, then it can be used in an [ExpandDL operation](expanddl-operation.md).</span></span> <span data-ttu-id="38109-118">Если для атрибута **ретурнфуллконтактдата** задано **значение true**, то записи Active Directory, найденные с помощью операции **ResolveNames** , будут возвращать дополнительные свойства, описывающие [контакт](contact.md).</span><span class="sxs-lookup"><span data-stu-id="38109-118">If the **ReturnFullContactData** attribute is set to **true**, then Active Directory entries found with the **ResolveNames** operation will return additional properties that describe a [Contact](contact.md).</span></span> <span data-ttu-id="38109-119">Атрибут **ретурнфуллконтактдата** не влияет на данные, возвращаемые для контактов и частных списков рассылки из папки контактов пользователя.</span><span class="sxs-lookup"><span data-stu-id="38109-119">The **ReturnFullContactData** attribute does not affect the data that is returned for contacts and private distribution lists from the user's contact folder.</span></span> 
  
## <a name="resolvenames-request-example"></a><span data-ttu-id="38109-120">Пример запроса ResolveNames</span><span class="sxs-lookup"><span data-stu-id="38109-120">ResolveNames request example</span></span>

### <a name="description"></a><span data-ttu-id="38109-121">Description</span><span class="sxs-lookup"><span data-stu-id="38109-121">Description</span></span>

<span data-ttu-id="38109-122">В приведенном ниже примере запроса **ResolveNames** показано, как разрешить запись пользователя.</span><span class="sxs-lookup"><span data-stu-id="38109-122">The following example of a **ResolveNames** request shows how to resolve the entry of User.</span></span>
  
### <a name="code"></a><span data-ttu-id="38109-123">Код</span><span class="sxs-lookup"><span data-stu-id="38109-123">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <ResolveNames xmlns="https://schemas.microsoft.com/exchange/services/2006/messages"
                  xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
                  ReturnFullContactData="true">
      <UnresolvedEntry>User2</UnresolvedEntry>
    </ResolveNames>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="38109-124">Комментарии</span><span class="sxs-lookup"><span data-stu-id="38109-124">Comments</span></span>

<span data-ttu-id="38109-125">Ответ на этот запрос возвратит все записи, начинающиеся с "Петр" или "MI".</span><span class="sxs-lookup"><span data-stu-id="38109-125">The response to this request will return all entries that start with "Jo" or "Mi."</span></span> <span data-ttu-id="38109-126">Возвращенные элементы представляют собой общедоступные почтовые ящики, общедоступные и частные списки рассылки, а также контакты.</span><span class="sxs-lookup"><span data-stu-id="38109-126">The returned items are public mailboxes, public and private distribution lists, and contacts.</span></span>
  
> [!NOTE]
> <span data-ttu-id="38109-127">Поиск осуществляется только по контактам из папки личных контактов по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="38109-127">Only contacts in the default personal Contacts folder are searched.</span></span> 
  
<span data-ttu-id="38109-128">Ниже приведены возможные результаты запроса **ResolveNames** .</span><span class="sxs-lookup"><span data-stu-id="38109-128">The following are the possible results for a **ResolveNames** request:</span></span> 
  
- <span data-ttu-id="38109-129">Ответы, которые не содержат разрешенных сущностей, возвращают значение атрибута **респонсекласс** , равное **Error**.</span><span class="sxs-lookup"><span data-stu-id="38109-129">Responses that do not contain a resolved entity will return a **ResponseClass** attribute value equal to **Error**.</span></span> <span data-ttu-id="38109-130">Элемент **мессажетекст** будет содержать " **результаты не найдены**".</span><span class="sxs-lookup"><span data-stu-id="38109-130">The **MessageText** element will contain " **No results are found**."</span></span>
    
- <span data-ttu-id="38109-131">Ответы, содержащие одну разрешенную сущность, возвращают значение атрибута **респонсекласс** , равное **Success**.</span><span class="sxs-lookup"><span data-stu-id="38109-131">Responses that contain a single resolved entity will return a **ResponseClass** attribute value equal to **Success**.</span></span>
    
- <span data-ttu-id="38109-132">Ответы, которые содержат несколько возможных сущностей, будут возвращать значение атрибута **респонсекласс** , равное **warning**.</span><span class="sxs-lookup"><span data-stu-id="38109-132">Responses that contain multiple possible entities will return a **ResponseClass** attribute value equal to **Warning**.</span></span> <span data-ttu-id="38109-133">В этом случае сущность не может быть сопоставлена с уникальным идентификатором.</span><span class="sxs-lookup"><span data-stu-id="38109-133">In this case, the entity could not be resolved to a unique identity.</span></span> <span data-ttu-id="38109-134">Элемент **мессажетекст** будет содержать "несколько результатов поиска".</span><span class="sxs-lookup"><span data-stu-id="38109-134">The **MessageText** element will contain "Multiple results are found."</span></span> 
    
### <a name="request-elements"></a><span data-ttu-id="38109-135">Элементы Request</span><span class="sxs-lookup"><span data-stu-id="38109-135">Request elements</span></span>

<span data-ttu-id="38109-136">В запросе используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="38109-136">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="38109-137">ResolveNames</span><span class="sxs-lookup"><span data-stu-id="38109-137">ResolveNames</span></span>](resolvenames.md)
    
- [<span data-ttu-id="38109-138">унресолведентри</span><span class="sxs-lookup"><span data-stu-id="38109-138">UnresolvedEntry</span></span>](unresolvedentry.md)
    
## <a name="successful-resolvenames-operation-response-example"></a><span data-ttu-id="38109-139">Пример успешного ответа операции ResolveNames</span><span class="sxs-lookup"><span data-stu-id="38109-139">Successful ResolveNames operation response example</span></span>

### <a name="description"></a><span data-ttu-id="38109-140">Description</span><span class="sxs-lookup"><span data-stu-id="38109-140">Description</span></span>

<span data-ttu-id="38109-141">В следующем примере показан успешный ответ на запрос **ResolveNames** .</span><span class="sxs-lookup"><span data-stu-id="38109-141">The following example shows a successful response to a **ResolveNames** request.</span></span> 
  
### <a name="code"></a><span data-ttu-id="38109-142">Код</span><span class="sxs-lookup"><span data-stu-id="38109-142">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="685" MinorBuildNumber="8" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <ResolveNamesResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                          xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                          xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:ResolveNamesResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:ResolutionSet TotalItemsInView="1" IncludesLastItemInRange="true">
            <t:Resolution>
              <t:Mailbox>
                <t:Name>User2</t:Name>
                <t:EmailAddress>User2@example.com</t:EmailAddress>
                <t:RoutingType>SMTP</t:RoutingType>
                <t:MailboxType>Mailbox</t:MailboxType>
              </t:Mailbox>
              <t:Contact>
                <t:DisplayName>User2</t:DisplayName>
                <t:EmailAddresses>
                  <t:Entry Key="EmailAddress1">SMTP:User2@example.com</t:Entry>
                </t:EmailAddresses>
                <t:ContactSource>ActiveDirectory</t:ContactSource>
              </t:Contact>
            </t:Resolution>
          </m:ResolutionSet>
        </m:ResolveNamesResponseMessage>
      </m:ResponseMessages>
    </ResolveNamesResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="successful-resolvenames-response-elements"></a><span data-ttu-id="38109-143">Успешные элементы ответа ResolveNames</span><span class="sxs-lookup"><span data-stu-id="38109-143">Successful ResolveNames response elements</span></span>

<span data-ttu-id="38109-144">В отклике используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="38109-144">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="38109-145">серверверсионинфо</span><span class="sxs-lookup"><span data-stu-id="38109-145">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="38109-146">ресолвенамесреспонсе</span><span class="sxs-lookup"><span data-stu-id="38109-146">ResolveNamesResponse</span></span>](resolvenamesresponse.md)
    
- [<span data-ttu-id="38109-147">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="38109-147">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="38109-148">ресолвенамесреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="38109-148">ResolveNamesResponseMessage</span></span>](resolvenamesresponsemessage.md)
    
- [<span data-ttu-id="38109-149">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="38109-149">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="38109-150">Авторешение</span><span class="sxs-lookup"><span data-stu-id="38109-150">ResolutionSet</span></span>](resolutionset.md)
    
- [<span data-ttu-id="38109-151">Resolution</span><span class="sxs-lookup"><span data-stu-id="38109-151">Resolution</span></span>](resolution.md)
    
- [<span data-ttu-id="38109-152">Mailbox</span><span class="sxs-lookup"><span data-stu-id="38109-152">Mailbox</span></span>](mailbox.md)
    
- [<span data-ttu-id="38109-153">Имя (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="38109-153">Name (EmailAddressType)</span></span>](name-emailaddresstype.md)
    
- [<span data-ttu-id="38109-154">EmailAddress (Нонемптистрингтипе)</span><span class="sxs-lookup"><span data-stu-id="38109-154">EmailAddress (NonEmptyStringType)</span></span>](emailaddress-nonemptystringtype.md)
    
- [<span data-ttu-id="38109-155">Раутингтипе (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="38109-155">RoutingType (EmailAddressType)</span></span>](routingtype-emailaddresstype.md)
    
- [<span data-ttu-id="38109-156">MailboxType</span><span class="sxs-lookup"><span data-stu-id="38109-156">MailboxType</span></span>](mailboxtype.md)
    
- <span data-ttu-id="38109-157">[контакт](contact.md);</span><span class="sxs-lookup"><span data-stu-id="38109-157">[Contact](contact.md)</span></span>
    
- [<span data-ttu-id="38109-158">DisplayName (строка)</span><span class="sxs-lookup"><span data-stu-id="38109-158">DisplayName (string)</span></span>](displayname-string.md)
    
- [<span data-ttu-id="38109-159">EmailAddresses</span><span class="sxs-lookup"><span data-stu-id="38109-159">EmailAddresses</span></span>](emailaddresses.md)
    
- [<span data-ttu-id="38109-160">Запись (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="38109-160">Entry (EmailAddress)</span></span>](entry-emailaddress.md)
    
- [<span data-ttu-id="38109-161">контактсаурце</span><span class="sxs-lookup"><span data-stu-id="38109-161">ContactSource</span></span>](contactsource.md)
    
## <a name="resolvenames-operation-error-response"></a><span data-ttu-id="38109-162">Ответ об ошибке операции ResolveNames</span><span class="sxs-lookup"><span data-stu-id="38109-162">ResolveNames operation error response</span></span>

### <a name="description"></a><span data-ttu-id="38109-163">Description</span><span class="sxs-lookup"><span data-stu-id="38109-163">Description</span></span>

<span data-ttu-id="38109-164">В следующем примере показан ответ об ошибке для запроса **ResolveNames** .</span><span class="sxs-lookup"><span data-stu-id="38109-164">The following example shows an error response to a **ResolveNames** request.</span></span> <span data-ttu-id="38109-165">Ошибка возникает при попытке разрешить имя, которое не удается разрешить.</span><span class="sxs-lookup"><span data-stu-id="38109-165">The error is caused by trying to resolve a name that cannot be resolved.</span></span> 
  
### <a name="code"></a><span data-ttu-id="38109-166">Код</span><span class="sxs-lookup"><span data-stu-id="38109-166">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="685" MinorBuildNumber="8" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <ResolveNamesResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                          xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                          xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:ResolveNamesResponseMessage ResponseClass="Error">
          <m:MessageText>No results were found.</m:MessageText>
          <m:ResponseCode>ErrorNameResolutionNoResults</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
        </m:ResolveNamesResponseMessage>
      </m:ResponseMessages>
    </ResolveNamesResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="error-response-elements"></a><span data-ttu-id="38109-167">Элементы ошибочного ответа</span><span class="sxs-lookup"><span data-stu-id="38109-167">Error response elements</span></span>

<span data-ttu-id="38109-168">В ответе на сообщение об ошибке используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="38109-168">The following elements are used in the error response:</span></span>
  
- [<span data-ttu-id="38109-169">серверверсионинфо</span><span class="sxs-lookup"><span data-stu-id="38109-169">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="38109-170">ресолвенамесреспонсе</span><span class="sxs-lookup"><span data-stu-id="38109-170">ResolveNamesResponse</span></span>](resolvenamesresponse.md)
    
- [<span data-ttu-id="38109-171">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="38109-171">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="38109-172">ресолвенамесреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="38109-172">ResolveNamesResponseMessage</span></span>](resolvenamesresponsemessage.md)
    
- [<span data-ttu-id="38109-173">мессажетекст</span><span class="sxs-lookup"><span data-stu-id="38109-173">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="38109-174">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="38109-174">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="38109-175">дескриптивелинккэй</span><span class="sxs-lookup"><span data-stu-id="38109-175">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
## <a name="see-also"></a><span data-ttu-id="38109-176">См. также</span><span class="sxs-lookup"><span data-stu-id="38109-176">See also</span></span>



[<span data-ttu-id="38109-177">Операция ExpandDL</span><span class="sxs-lookup"><span data-stu-id="38109-177">ExpandDL operation</span></span>](expanddl-operation.md)


[<span data-ttu-id="38109-178">Использование разрешения имен</span><span class="sxs-lookup"><span data-stu-id="38109-178">Using Name Resolution</span></span>](https://msdn.microsoft.com/library/9257fb07-89d2-46eb-b885-e2173fe6fbc1%28Office.15%29.aspx)

