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
description: Адреса ResolveNames операция переносов неоднозначные электронной почты и отображаемые имена.
ms.openlocfilehash: 8443cf834dfdf104daeaaa92fdee3742c3fa3719
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19835162"
---
# <a name="resolvenames-operation"></a><span data-ttu-id="ba224-103">Операция ResolveNames</span><span class="sxs-lookup"><span data-stu-id="ba224-103">ResolveNames operation</span></span>

<span data-ttu-id="ba224-104">Адреса **ResolveNames** операция переносов неоднозначные электронной почты и отображаемые имена.</span><span class="sxs-lookup"><span data-stu-id="ba224-104">The **ResolveNames** operation resolves ambiguous email addresses and display names.</span></span> 
  
## <a name="using-the-resolvenames-operation"></a><span data-ttu-id="ba224-105">С помощью операции ResolveNames</span><span class="sxs-lookup"><span data-stu-id="ba224-105">Using the ResolveNames operation</span></span>

<span data-ttu-id="ba224-106">Эту операцию можно использовать для проверки псевдонимы и разрешения отображаемые имена в соответствующий почтовый ящик пользователя.</span><span class="sxs-lookup"><span data-stu-id="ba224-106">This operation can be used to verify aliases and resolve display names to the appropriate mailbox user.</span></span> <span data-ttu-id="ba224-107">Если существует неоднозначные имена ответа операции **ResolveNames** сведения о каждого почтового ящика пользователя, чтобы клиентское приложение может разрешения имен.</span><span class="sxs-lookup"><span data-stu-id="ba224-107">If ambiguous names exist, the **ResolveNames** operation response provides information about each mailbox user so that the client application can resolve the names.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="ba224-108">Замечания</span><span class="sxs-lookup"><span data-stu-id="ba224-108">Remarks</span></span>

<span data-ttu-id="ba224-109">Ответ ResolveNames возвращает не более 100 кандидатов.</span><span class="sxs-lookup"><span data-stu-id="ba224-109">The ResolveNames response returns a maximum of 100 candidates.</span></span> <span data-ttu-id="ba224-110">100 кандидатов, возвращенных — это первый 100 обнаружения в операции поиска.</span><span class="sxs-lookup"><span data-stu-id="ba224-110">The 100 candidates that are returned are the first 100 that are encountered in the lookup operation.</span></span>
  
<span data-ttu-id="ba224-111">Адреса электронной почты с с префиксами типов маршрутизации, например smtp или sip, сохраняются в нескольких значений массива.</span><span class="sxs-lookup"><span data-stu-id="ba224-111">Email addresses with prefixed routing types, such as smtp or sip, are saved in a multivalue array.</span></span> <span data-ttu-id="ba224-112">Операция **ResolveNames** выполняет частичное соответствие каждого значения этого массива, при добавлении типа маршрутизации в начале неизвестное имя, например «sip:User1@Contoso.com».</span><span class="sxs-lookup"><span data-stu-id="ba224-112">The **ResolveNames** operation performs a partial match against each value of that array when you add the routing type at the beginning of the unresolved name, such as "sip:User1@Contoso.com".</span></span> <span data-ttu-id="ba224-113">Если не указать тип маршрутизации, **ResolveNames** по умолчанию для типа маршрутизации smtp, соответствует свойству основной адрес smtp и поиск нескольких значений массива.</span><span class="sxs-lookup"><span data-stu-id="ba224-113">If you don't specify a routing type, **ResolveNames** will default to the routing type of smtp, match it to a primary smtp address property, and not search the multivalue array.</span></span> 
  
<span data-ttu-id="ba224-114">В одном запросе можно указать только один неоднозначное имя.</span><span class="sxs-lookup"><span data-stu-id="ba224-114">Only one ambiguous name can be specified in a single request.</span></span> <span data-ttu-id="ba224-115">Сначала выполняется поиск Active Directory, а затем осуществляется в папке контактов пользователя.</span><span class="sxs-lookup"><span data-stu-id="ba224-115">Active Directory is searched first, and then the user's contact folder is searched.</span></span> <span data-ttu-id="ba224-116">Записей в папке контактов пользователя имеют свойство **ItemId** ненулевое, которую можно использовать в запросе GetItem.</span><span class="sxs-lookup"><span data-stu-id="ba224-116">Resolved entries from a user's contact folder have a non-null **ItemId** property, which can then be used in a GetItem request.</span></span> <span data-ttu-id="ba224-117">Если идентификатор списка рассылки частный, его можно использовать в рамках одной [операции ExpandDL](expanddl-operation.md).</span><span class="sxs-lookup"><span data-stu-id="ba224-117">If it is the ID of a private distribution list, then it can be used in an [ExpandDL operation](expanddl-operation.md).</span></span> <span data-ttu-id="ba224-118">Если атрибут **ReturnFullContactData** имеет значение **true**, найдено Active Directory с помощью операции **ResolveNames** возвращает дополнительные свойства, описывающие [контакт](contact.md).</span><span class="sxs-lookup"><span data-stu-id="ba224-118">If the **ReturnFullContactData** attribute is set to **true**, then Active Directory entries found with the **ResolveNames** operation will return additional properties that describe a [Contact](contact.md).</span></span> <span data-ttu-id="ba224-119">Атрибут **ReturnFullContactData** не влияет на данные, возвращаемые для контактов и частных списки рассылки из папки контактов пользователя.</span><span class="sxs-lookup"><span data-stu-id="ba224-119">The **ReturnFullContactData** attribute does not affect the data that is returned for contacts and private distribution lists from the user's contact folder.</span></span> 
  
## <a name="resolvenames-request-example"></a><span data-ttu-id="ba224-120">Пример запроса ResolveNames</span><span class="sxs-lookup"><span data-stu-id="ba224-120">ResolveNames request example</span></span>

### <a name="description"></a><span data-ttu-id="ba224-121">Описание</span><span class="sxs-lookup"><span data-stu-id="ba224-121">Description</span></span>

<span data-ttu-id="ba224-122">В следующем примере запрос **ResolveNames** показано, как разрешить запись пользователя.</span><span class="sxs-lookup"><span data-stu-id="ba224-122">The following example of a **ResolveNames** request shows how to resolve the entry of User.</span></span>
  
### <a name="code"></a><span data-ttu-id="ba224-123">Программа</span><span class="sxs-lookup"><span data-stu-id="ba224-123">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <ResolveNames xmlns="http://schemas.microsoft.com/exchange/services/2006/messages"
                  xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
                  ReturnFullContactData="true">
      <UnresolvedEntry>User2</UnresolvedEntry>
    </ResolveNames>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="ba224-124">Комментарии</span><span class="sxs-lookup"><span data-stu-id="ba224-124">Comments</span></span>

<span data-ttu-id="ba224-125">Ответ на этот запрос будет возвращать все записи, начинающиеся с «Петр» или «Mi».</span><span class="sxs-lookup"><span data-stu-id="ba224-125">The response to this request will return all entries that start with "Jo" or "Mi."</span></span> <span data-ttu-id="ba224-126">Возвращенные элементы, общих почтовых ящиков, списки рассылки общедоступных и частных и контакты.</span><span class="sxs-lookup"><span data-stu-id="ba224-126">The returned items are public mailboxes, public and private distribution lists, and contacts.</span></span>
  
> [!NOTE]
> <span data-ttu-id="ba224-127">Поиск осуществляется только контактов в папке личных контактов по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="ba224-127">Only contacts in the default personal Contacts folder are searched.</span></span> 
  
<span data-ttu-id="ba224-128">Ниже приведены возможные результаты запроса **ResolveNames** .</span><span class="sxs-lookup"><span data-stu-id="ba224-128">The following are the possible results for a **ResolveNames** request:</span></span> 
  
- <span data-ttu-id="ba224-129">Ответы, которые не содержат разрешения сущности возвращает значение атрибута **ResponseClass** равно **ошибки**.</span><span class="sxs-lookup"><span data-stu-id="ba224-129">Responses that do not contain a resolved entity will return a **ResponseClass** attribute value equal to **Error**.</span></span> <span data-ttu-id="ba224-130">Элемент **MessageText** будет содержать « **Нет результатов**».</span><span class="sxs-lookup"><span data-stu-id="ba224-130">The **MessageText** element will contain " **No results are found**."</span></span>
    
- <span data-ttu-id="ba224-131">Ответы, которые содержат одного объекта разрешения возвращает значение атрибута **ResponseClass** равно **успеха**.</span><span class="sxs-lookup"><span data-stu-id="ba224-131">Responses that contain a single resolved entity will return a **ResponseClass** attribute value equal to **Success**.</span></span>
    
- <span data-ttu-id="ba224-132">Ответы, которые содержат несколько возможных сущностей возвращает значение атрибута **ResponseClass** равно **предупреждения**.</span><span class="sxs-lookup"><span data-stu-id="ba224-132">Responses that contain multiple possible entities will return a **ResponseClass** attribute value equal to **Warning**.</span></span> <span data-ttu-id="ba224-133">В этом случае сущность не удалось разрешить уникальное удостоверение.</span><span class="sxs-lookup"><span data-stu-id="ba224-133">In this case, the entity could not be resolved to a unique identity.</span></span> <span data-ttu-id="ba224-134">Элемент **MessageText** будет содержать «находятся несколько результатов».</span><span class="sxs-lookup"><span data-stu-id="ba224-134">The **MessageText** element will contain "Multiple results are found."</span></span> 
    
### <a name="request-elements"></a><span data-ttu-id="ba224-135">Элементы запроса</span><span class="sxs-lookup"><span data-stu-id="ba224-135">Request elements</span></span>

<span data-ttu-id="ba224-136">В запросе используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="ba224-136">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="ba224-137">ResolveNames</span><span class="sxs-lookup"><span data-stu-id="ba224-137">ResolveNames</span></span>](resolvenames.md)
    
- [<span data-ttu-id="ba224-138">UnresolvedEntry</span><span class="sxs-lookup"><span data-stu-id="ba224-138">UnresolvedEntry</span></span>](unresolvedentry.md)
    
## <a name="successful-resolvenames-operation-response-example"></a><span data-ttu-id="ba224-139">Пример ответа операция успешно ResolveNames</span><span class="sxs-lookup"><span data-stu-id="ba224-139">Successful ResolveNames operation response example</span></span>

### <a name="description"></a><span data-ttu-id="ba224-140">Описание</span><span class="sxs-lookup"><span data-stu-id="ba224-140">Description</span></span>

<span data-ttu-id="ba224-141">В следующем примере показано успешного ответа на запрос **ResolveNames** .</span><span class="sxs-lookup"><span data-stu-id="ba224-141">The following example shows a successful response to a **ResolveNames** request.</span></span> 
  
### <a name="code"></a><span data-ttu-id="ba224-142">Программа</span><span class="sxs-lookup"><span data-stu-id="ba224-142">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="685" MinorBuildNumber="8" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <ResolveNamesResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                          xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                          xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="successful-resolvenames-response-elements"></a><span data-ttu-id="ba224-143">Элементы ответов успешно ResolveNames</span><span class="sxs-lookup"><span data-stu-id="ba224-143">Successful ResolveNames response elements</span></span>

<span data-ttu-id="ba224-144">В ответе используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="ba224-144">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="ba224-145">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="ba224-145">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="ba224-146">ResolveNamesResponse</span><span class="sxs-lookup"><span data-stu-id="ba224-146">ResolveNamesResponse</span></span>](resolvenamesresponse.md)
    
- [<span data-ttu-id="ba224-147">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="ba224-147">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="ba224-148">ResolveNamesResponseMessage</span><span class="sxs-lookup"><span data-stu-id="ba224-148">ResolveNamesResponseMessage</span></span>](resolvenamesresponsemessage.md)
    
- [<span data-ttu-id="ba224-149">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="ba224-149">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="ba224-150">ResolutionSet</span><span class="sxs-lookup"><span data-stu-id="ba224-150">ResolutionSet</span></span>](resolutionset.md)
    
- [<span data-ttu-id="ba224-151">Решение</span><span class="sxs-lookup"><span data-stu-id="ba224-151">Resolution</span></span>](resolution.md)
    
- [<span data-ttu-id="ba224-152">Mailbox</span><span class="sxs-lookup"><span data-stu-id="ba224-152">Mailbox</span></span>](mailbox.md)
    
- [<span data-ttu-id="ba224-153">Имя (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="ba224-153">Name (EmailAddressType)</span></span>](name-emailaddresstype.md)
    
- [<span data-ttu-id="ba224-154">EmailAddress (NonEmptyStringType)</span><span class="sxs-lookup"><span data-stu-id="ba224-154">EmailAddress (NonEmptyStringType)</span></span>](emailaddress-nonemptystringtype.md)
    
- [<span data-ttu-id="ba224-155">RoutingType (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="ba224-155">RoutingType (EmailAddressType)</span></span>](routingtype-emailaddresstype.md)
    
- [<span data-ttu-id="ba224-156">MailboxType</span><span class="sxs-lookup"><span data-stu-id="ba224-156">MailboxType</span></span>](mailboxtype.md)
    
- [<span data-ttu-id="ba224-157">Контакт</span><span class="sxs-lookup"><span data-stu-id="ba224-157">Contact</span></span>](contact.md)
    
- [<span data-ttu-id="ba224-158">Отображаемое имя (строка)</span><span class="sxs-lookup"><span data-stu-id="ba224-158">DisplayName (string)</span></span>](displayname-string.md)
    
- [<span data-ttu-id="ba224-159">EmailAddresses</span><span class="sxs-lookup"><span data-stu-id="ba224-159">EmailAddresses</span></span>](emailaddresses.md)
    
- [<span data-ttu-id="ba224-160">Запись (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="ba224-160">Entry (EmailAddress)</span></span>](entry-emailaddress.md)
    
- [<span data-ttu-id="ba224-161">ContactSource</span><span class="sxs-lookup"><span data-stu-id="ba224-161">ContactSource</span></span>](contactsource.md)
    
## <a name="resolvenames-operation-error-response"></a><span data-ttu-id="ba224-162">Ошибка операции ResolveNames ответа</span><span class="sxs-lookup"><span data-stu-id="ba224-162">ResolveNames operation error response</span></span>

### <a name="description"></a><span data-ttu-id="ba224-163">Описание</span><span class="sxs-lookup"><span data-stu-id="ba224-163">Description</span></span>

<span data-ttu-id="ba224-164">В следующем примере показано ошибочный ответ на запрос **ResolveNames** .</span><span class="sxs-lookup"><span data-stu-id="ba224-164">The following example shows an error response to a **ResolveNames** request.</span></span> <span data-ttu-id="ba224-165">Ошибки, возникающие при попытке определить имя, которое не может быть разрешен.</span><span class="sxs-lookup"><span data-stu-id="ba224-165">The error is caused by trying to resolve a name that cannot be resolved.</span></span> 
  
### <a name="code"></a><span data-ttu-id="ba224-166">Программа</span><span class="sxs-lookup"><span data-stu-id="ba224-166">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="685" MinorBuildNumber="8" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <ResolveNamesResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                          xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                          xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="error-response-elements"></a><span data-ttu-id="ba224-167">Элементы ответа об ошибках</span><span class="sxs-lookup"><span data-stu-id="ba224-167">Error response elements</span></span>

<span data-ttu-id="ba224-168">В ответ на ошибку используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="ba224-168">The following elements are used in the error response:</span></span>
  
- [<span data-ttu-id="ba224-169">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="ba224-169">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="ba224-170">ResolveNamesResponse</span><span class="sxs-lookup"><span data-stu-id="ba224-170">ResolveNamesResponse</span></span>](resolvenamesresponse.md)
    
- [<span data-ttu-id="ba224-171">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="ba224-171">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="ba224-172">ResolveNamesResponseMessage</span><span class="sxs-lookup"><span data-stu-id="ba224-172">ResolveNamesResponseMessage</span></span>](resolvenamesresponsemessage.md)
    
- [<span data-ttu-id="ba224-173">MessageText</span><span class="sxs-lookup"><span data-stu-id="ba224-173">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="ba224-174">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="ba224-174">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="ba224-175">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="ba224-175">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
## <a name="see-also"></a><span data-ttu-id="ba224-176">См. также</span><span class="sxs-lookup"><span data-stu-id="ba224-176">See also</span></span>



[<span data-ttu-id="ba224-177">Операция ExpandDL</span><span class="sxs-lookup"><span data-stu-id="ba224-177">ExpandDL operation</span></span>](expanddl-operation.md)


[<span data-ttu-id="ba224-178">С помощью разрешения имен</span><span class="sxs-lookup"><span data-stu-id="ba224-178">Using Name Resolution</span></span>](http://msdn.microsoft.com/library/9257fb07-89d2-46eb-b885-e2173fe6fbc1%28Office.15%29.aspx)

