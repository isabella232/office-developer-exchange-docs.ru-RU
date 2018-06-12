---
title: Операция GetSearchableMailboxes
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 47f8ff57-4835-4d2d-9136-44afb31a4cbe
description: Найдите сведения о веб-служб Exchange GetSearchableMailboxes операции.
ms.openlocfilehash: 5e14288280b23e2555eea4fce0f77743d7d210ce
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762910"
---
# <a name="getsearchablemailboxes-operation"></a><span data-ttu-id="398fe-103">Операция GetSearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="398fe-103">GetSearchableMailboxes operation</span></span>

<span data-ttu-id="398fe-104">Найдите сведения о **GetSearchableMailboxes** операции веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="398fe-104">Find information about the **GetSearchableMailboxes** EWS operation.</span></span> 
  
<span data-ttu-id="398fe-105">Операция **GetSearchableMailboxes** получает областью видимости набора для поиска почтовых ящиков для операций поиска обнаружения.</span><span class="sxs-lookup"><span data-stu-id="398fe-105">The **GetSearchableMailboxes** operation gets a scoped set of searchable mailboxes for discovery searches.</span></span> <span data-ttu-id="398fe-106">Область поиска почтовых ящиков, возвращаемого в ответе определяется поисковый фильтр и ли расширенное членство в группах рассылки.</span><span class="sxs-lookup"><span data-stu-id="398fe-106">The scope of searchable mailboxes returned in the response is determined by the search filter and whether distribution group membership is expanded.</span></span> 
  
<span data-ttu-id="398fe-107">Эта операция появилась в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="398fe-107">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-getsearchablemailboxes-operation"></a><span data-ttu-id="398fe-108">С помощью операции GetSearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="398fe-108">Using the GetSearchableMailboxes operation</span></span>

<span data-ttu-id="398fe-109">Операция **GetSearchableMailboxes** получает сведения о почтовых ящиках с возможностью поиска.</span><span class="sxs-lookup"><span data-stu-id="398fe-109">The **GetSearchableMailboxes** operation gets information about searchable mailboxes.</span></span> <span data-ttu-id="398fe-110">Следующие аргументы могут передаваться в запросе:</span><span class="sxs-lookup"><span data-stu-id="398fe-110">The following arguments can be passed in the request:</span></span> 
  
- <span data-ttu-id="398fe-111">[SearchFilter](searchfilter.md) — принимает псевдоним одного адреса электронной почты в качестве аргумента.</span><span class="sxs-lookup"><span data-stu-id="398fe-111">[SearchFilter](searchfilter.md) —Accepts a single email alias as an argument.</span></span> 
    
- <span data-ttu-id="398fe-112">[ExpandGroupMembership](expandgroupmembership.md) — указывает, развернут ли группы рассылки в списке результатов, возвращаемого в ответе.</span><span class="sxs-lookup"><span data-stu-id="398fe-112">[ExpandGroupMembership](expandgroupmembership.md) — Indicates whether the distribution group membership is expanded in the results returned in the response.</span></span> 
    
<span data-ttu-id="398fe-113">Если группа рассылки — это псевдоним электронной почты, задайте в фильтре поиска и членство в группах рассылки не развернут, ответ будет содержать сведения о почтовых ящиках для группы рассылки.</span><span class="sxs-lookup"><span data-stu-id="398fe-113">If the email alias set in the search filter is a distribution group and the distribution group membership is not expanded, the response will contain the mailbox information for the distribution group.</span></span> <span data-ttu-id="398fe-114">Если группа рассылки — это псевдоним электронной почты, задайте в поисковый фильтр и расширенное членство в группах рассылки, ответ будет содержать сведения о почтовых ящиках для каждого почтового ящика, который является членом группы рассылки.</span><span class="sxs-lookup"><span data-stu-id="398fe-114">If the email alias set in the search filter is a distribution group and the distribution group membership is expanded, the response will contain the mailbox information for each mailbox that is a member of the distribution group.</span></span> <span data-ttu-id="398fe-115">Если фильтр поиска содержит псевдоним одного пользователя, ответ будет содержать сведения о почтовых ящиках для одного пользователя.</span><span class="sxs-lookup"><span data-stu-id="398fe-115">If the search filter contains a single user's alias, the response will contain the mailbox information for the single user.</span></span> <span data-ttu-id="398fe-116">Ответ будет содержать все почтовые ящики с возможностью поиска, если элемент [GetSearchableMailboxes](getsearchablemailboxes.md) пуст.</span><span class="sxs-lookup"><span data-stu-id="398fe-116">The response will contain all searchable mailboxes if the [GetSearchableMailboxes](getsearchablemailboxes.md) element is empty.</span></span> <span data-ttu-id="398fe-117">Это то же, как имеющий пустой элемент [SearchFilter](searchfilter.md) и [ExpandGroupMembership](expandgroupmembership.md) элемент, значение **false**.</span><span class="sxs-lookup"><span data-stu-id="398fe-117">This is the same as having an empty [SearchFilter](searchfilter.md) element and the [ExpandGroupMembership](expandgroupmembership.md) element set to **false**.</span></span>
  
### <a name="getsearchablemailboxes-operation-soap-headers"></a><span data-ttu-id="398fe-118">Заголовки SOAP GetSearchableMailboxes операции</span><span class="sxs-lookup"><span data-stu-id="398fe-118">GetSearchableMailboxes operation SOAP headers</span></span>

<span data-ttu-id="398fe-119">Операция **GetSearchableMailboxes** можно использовать заголовки SOAP, которые перечислены в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="398fe-119">The **GetSearchableMailboxes** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="398fe-120">**Имя заголовка**</span><span class="sxs-lookup"><span data-stu-id="398fe-120">**Header name**</span></span>|<span data-ttu-id="398fe-121">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="398fe-121">**Element**</span></span>|<span data-ttu-id="398fe-122">**Описание**</span><span class="sxs-lookup"><span data-stu-id="398fe-122">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="398fe-123">**ManagementRole**</span><span class="sxs-lookup"><span data-stu-id="398fe-123">**ManagementRole**</span></span> <br/> |[<span data-ttu-id="398fe-124">ManagementRole</span><span class="sxs-lookup"><span data-stu-id="398fe-124">ManagementRole</span></span>](managementrole.md) <br/> |<span data-ttu-id="398fe-125">Идентифицирует ролей сервера, необходимых в порядке для абонентов для запроса.</span><span class="sxs-lookup"><span data-stu-id="398fe-125">Identifies the server roles that are necessary in order for the caller to make the request.</span></span> <span data-ttu-id="398fe-126">Этот заголовок можно применять к запросу.</span><span class="sxs-lookup"><span data-stu-id="398fe-126">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="398fe-127">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="398fe-127">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="398fe-128">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="398fe-128">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="398fe-129">Определяет версию схемы для операции запроса.</span><span class="sxs-lookup"><span data-stu-id="398fe-129">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="398fe-130">Этот заголовок можно применять к запросу.</span><span class="sxs-lookup"><span data-stu-id="398fe-130">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="398fe-131">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="398fe-131">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="398fe-132">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="398fe-132">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="398fe-133">Определяет версию сервера, ответившего на запрос.</span><span class="sxs-lookup"><span data-stu-id="398fe-133">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="398fe-134">Этот заголовок можно применять, чтобы получить ответ.</span><span class="sxs-lookup"><span data-stu-id="398fe-134">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="getsearchablemailboxes-operation-request-example-request-information-about-a-distribution-group"></a><span data-ttu-id="398fe-135">Пример запроса операции GetSearchableMailboxes: запрос сведений о группе рассылки</span><span class="sxs-lookup"><span data-stu-id="398fe-135">GetSearchableMailboxes operation request example: Request information about a distribution group</span></span>

<span data-ttu-id="398fe-136">В следующем примере запрос операции **GetSearchableMailboxes** показано, как получить сведения о почтовых ящиках для группы рассылки lolgroup.</span><span class="sxs-lookup"><span data-stu-id="398fe-136">The following example of a **GetSearchableMailboxes** operation request shows how to get the mailbox information for the lolgroup distribution group.</span></span> 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013" />
   </soap:Header>
   <soap:Body >
      <m:GetSearchableMailboxes>
         <m:SearchFilter>lolgroup</m:SearchFilter>
         <m:ExpandGroupMembership>false</m:ExpandGroupMembership>
      </m:GetSearchableMailboxes>
   </soap:Body>
</soap:Envelope>

```

<span data-ttu-id="398fe-137">Запрос SOAP body содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="398fe-137">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="398fe-138">GetSearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="398fe-138">GetSearchableMailboxes</span></span>](getsearchablemailboxes.md)
    
- [<span data-ttu-id="398fe-139">SearchFilter</span><span class="sxs-lookup"><span data-stu-id="398fe-139">SearchFilter</span></span>](searchfilter.md)
    
- [<span data-ttu-id="398fe-140">ExpandGroupMembership</span><span class="sxs-lookup"><span data-stu-id="398fe-140">ExpandGroupMembership</span></span>](expandgroupmembership.md)
    
## <a name="successful-getsearchablemailboxes-operation-response-get-information-about-a-distribution-group"></a><span data-ttu-id="398fe-141">Успешные операции ответа GetSearchableMailboxes: получение сведений о группе рассылки</span><span class="sxs-lookup"><span data-stu-id="398fe-141">Successful GetSearchableMailboxes operation response: Get information about a distribution group</span></span>

<span data-ttu-id="398fe-142">В следующем примере показано успешного ответа на запрос операции **GetSearchableMailboxes** для получения сведений обнаружения lolgroup группу рассылки.</span><span class="sxs-lookup"><span data-stu-id="398fe-142">The following example shows a successful response to a **GetSearchableMailboxes** operation request to get the discovery information for the lolgroup distribution group.</span></span> 
  
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
      <GetSearchableMailboxesResponse ResponseClass="Success" 
                                      xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
         <SearchableMailboxes>
            <SearchableMailbox xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
               <Guid>33a408fe-2574-4e3b-49f5-5e1e000a3035</Guid>
               <PrimarySmtpAddress>LOLgroup@contoso.com</PrimarySmtpAddress>
               <IsExternalMailbox>false</IsExternalMailbox>
               <ExternalEmailAddress/>
               <DisplayName>LOLgroup</DisplayName>
               <IsMembershipGroup>true</IsMembershipGroup>
               <ReferenceId>/o=First/ou=Exchange(FYLT)/cn=Recipients/cn=81213b958a0b5295b13b3f02b812bf1bc-LOLgroup</ReferenceId>
            </SearchableMailbox>
         </SearchableMailboxes>
      </GetSearchableMailboxesResponse>
   </s:Body>
</s:Envelope>

```

<span data-ttu-id="398fe-143">Ответ SOAP body содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="398fe-143">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="398fe-144">GetSearchableMailboxesResponse</span><span class="sxs-lookup"><span data-stu-id="398fe-144">GetSearchableMailboxesResponse</span></span>](getsearchablemailboxesresponse.md)
    
- [<span data-ttu-id="398fe-145">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="398fe-145">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="398fe-146">SearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="398fe-146">SearchableMailboxes</span></span>](searchablemailboxes.md)
    
- [<span data-ttu-id="398fe-147">SearchableMailbox</span><span class="sxs-lookup"><span data-stu-id="398fe-147">SearchableMailbox</span></span>](searchablemailbox.md)
    
- [<span data-ttu-id="398fe-148">Guid</span><span class="sxs-lookup"><span data-stu-id="398fe-148">Guid</span></span>](guid-ex15websvcsotherref.md)
    
- [<span data-ttu-id="398fe-149">Параметр PrimarySmtpAddress</span><span class="sxs-lookup"><span data-stu-id="398fe-149">PrimarySmtpAddress</span></span>](primarysmtpaddress.md)
    
- [<span data-ttu-id="398fe-150">IsExternalMailbox</span><span class="sxs-lookup"><span data-stu-id="398fe-150">IsExternalMailbox</span></span>](isexternalmailbox.md)
    
- [<span data-ttu-id="398fe-151">ExternalEmailAddress</span><span class="sxs-lookup"><span data-stu-id="398fe-151">ExternalEmailAddress</span></span>](externalemailaddress.md)
    
- [<span data-ttu-id="398fe-152">Отображаемое имя (строка)</span><span class="sxs-lookup"><span data-stu-id="398fe-152">DisplayName (string)</span></span>](displayname-string.md)
    
- [<span data-ttu-id="398fe-153">IsMembershipGroup</span><span class="sxs-lookup"><span data-stu-id="398fe-153">IsMembershipGroup</span></span>](ismembershipgroup.md)
    
- [<span data-ttu-id="398fe-154">ReferenceId</span><span class="sxs-lookup"><span data-stu-id="398fe-154">ReferenceId</span></span>](referenceid.md)
    
## <a name="successful-getsearchablemailboxes-operation-response-get-information-about-an-expanded-distribution-group"></a><span data-ttu-id="398fe-155">Успешные операции ответа GetSearchableMailboxes: получение сведений о расширенной группы рассылки</span><span class="sxs-lookup"><span data-stu-id="398fe-155">Successful GetSearchableMailboxes operation response: Get information about an expanded distribution group</span></span>

<span data-ttu-id="398fe-156">В следующем примере показано успешного ответа на запрос операции **GetSearchableMailboxes** для получения обнаружения сведений о членов группы рассылки расширенное lolgroup.</span><span class="sxs-lookup"><span data-stu-id="398fe-156">The following example shows a successful response to a **GetSearchableMailboxes** operation request to get the discovery information about members of the expanded lolgroup distribution group.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="526" MinorBuildNumber="0" Version="Exchange2013" xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" xmlns="http://schemas.microsoft.com/exchange/services/2006/types" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <GetSearchableMailboxesResponse ResponseClass="Success" xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseCode>NoError</ResponseCode>
      <SearchableMailboxes>
        <SearchableMailbox xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
          <Guid>e2d42cdf-a227-1ec3-486b-6fa0ebaadb9f5</Guid>
          <PrimarySmtpAddress>JSmith@contoso.com</PrimarySmtpAddress>
          <IsExternalMailbox>false</IsExternalMailbox>
          <ExternalEmailAddress/>
          <DisplayName>Julia Smith</DisplayName>
          <IsMembershipGroup>false</IsMembershipGroup>
          <ReferenceId>/o=First Organization/ou=Exchange Administrative Group (FYDLT)/cn=Recipients/cn=0a1fc86f883846152405d60956dd02e7-Julia</ReferenceId>
        </SearchableMailbox>
        <SearchableMailbox xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
          <Guid>45d0fff1-6541-459a-a343-52453b30e12ca</Guid>
          <PrimarySmtpAddress>LMoore@contoso.com</PrimarySmtpAddress>
          <IsExternalMailbox>false</IsExternalMailbox>
          <ExternalEmailAddress/>
          <DisplayName>Laura Moore</DisplayName>
          <IsMembershipGroup>false</IsMembershipGroup>
          <ReferenceId>/o=First Organization/ou=Exchange Administrative Group (FYDLT)/cn=Recipients/cn=2910d8f8316f4378bbf9338d8f9d714b-Laura</ReferenceId>
        </SearchableMailbox>
        <SearchableMailbox xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
          <Guid>3c620d04-8b33-435a-95be-5b939375576</Guid>
          <PrimarySmtpAddress>SBrown@contoso.com</PrimarySmtpAddress>
          <IsExternalMailbox>false</IsExternalMailbox>
          <ExternalEmailAddress/>
          <DisplayName>Steven Brown</DisplayName>
          <IsMembershipGroup>false</IsMembershipGroup>
          <ReferenceId>/o=First Organization/ou=Exchange Administrative Group (FYDLT)/cn=Recipients/cn=90312341a742f0e47e392c80a60d13ecf-Steve</ReferenceId>
        </SearchableMailbox>
      </SearchableMailboxes>
    </GetSearchableMailboxesResponse>
  </s:Body>
</s:Envelope>
```

<span data-ttu-id="398fe-157">Ответ SOAP body содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="398fe-157">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="398fe-158">GetSearchableMailboxesResponse</span><span class="sxs-lookup"><span data-stu-id="398fe-158">GetSearchableMailboxesResponse</span></span>](getsearchablemailboxesresponse.md)
    
- [<span data-ttu-id="398fe-159">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="398fe-159">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="398fe-160">SearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="398fe-160">SearchableMailboxes</span></span>](searchablemailboxes.md)
    
- [<span data-ttu-id="398fe-161">SearchableMailbox</span><span class="sxs-lookup"><span data-stu-id="398fe-161">SearchableMailbox</span></span>](searchablemailbox.md)
    
- [<span data-ttu-id="398fe-162">Guid</span><span class="sxs-lookup"><span data-stu-id="398fe-162">Guid</span></span>](guid-ex15websvcsotherref.md)
    
- [<span data-ttu-id="398fe-163">Параметр PrimarySmtpAddress</span><span class="sxs-lookup"><span data-stu-id="398fe-163">PrimarySmtpAddress</span></span>](primarysmtpaddress.md)
    
- [<span data-ttu-id="398fe-164">IsExternalMailbox</span><span class="sxs-lookup"><span data-stu-id="398fe-164">IsExternalMailbox</span></span>](isexternalmailbox.md)
    
- [<span data-ttu-id="398fe-165">ExternalEmailAddress</span><span class="sxs-lookup"><span data-stu-id="398fe-165">ExternalEmailAddress</span></span>](externalemailaddress.md)
    
- [<span data-ttu-id="398fe-166">Отображаемое имя (строка)</span><span class="sxs-lookup"><span data-stu-id="398fe-166">DisplayName (string)</span></span>](displayname-string.md)
    
- [<span data-ttu-id="398fe-167">IsMembershipGroup</span><span class="sxs-lookup"><span data-stu-id="398fe-167">IsMembershipGroup</span></span>](ismembershipgroup.md)
    
- [<span data-ttu-id="398fe-168">ReferenceId</span><span class="sxs-lookup"><span data-stu-id="398fe-168">ReferenceId</span></span>](referenceid.md)
    
## <a name="getsearchablemailboxes-operation-error-response"></a><span data-ttu-id="398fe-169">Ошибка операции GetSearchableMailboxes ответа</span><span class="sxs-lookup"><span data-stu-id="398fe-169">GetSearchableMailboxes operation error response</span></span>

<span data-ttu-id="398fe-170">В следующем примере показано ошибочный ответ на запрос операции **GetSearchableMailboxes** .</span><span class="sxs-lookup"><span data-stu-id="398fe-170">The following example shows an error response to a **GetSearchableMailboxes** operation request.</span></span> <span data-ttu-id="398fe-171">Это ответ на запрос для получения всех почтовых ящиков с возможностью поиска, если аргумент **ExpandGroupMembership** имеет значение **true**.</span><span class="sxs-lookup"><span data-stu-id="398fe-171">This is a response to a request to get all searchable mailboxes when the **ExpandGroupMembership** argument is set to **true**.</span></span> 
  
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
      <GetSearchableMailboxesResponse ResponseClass="Error" 
                                      xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>Cannot use wildcard or empty query when auto group expansion is enabled.</MessageText>
         <ResponseCode>ErrorInvalidArgument</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
         <SearchableMailboxes/>
      </GetSearchableMailboxesResponse>
   </s:Body>
</s:Envelope>

```

<span data-ttu-id="398fe-172">Ошибка ответ SOAP body содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="398fe-172">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="398fe-173">GetSearchableMailboxesResponse</span><span class="sxs-lookup"><span data-stu-id="398fe-173">GetSearchableMailboxesResponse</span></span>](getsearchablemailboxesresponse.md)
    
- [<span data-ttu-id="398fe-174">MessageText</span><span class="sxs-lookup"><span data-stu-id="398fe-174">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="398fe-175">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="398fe-175">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="398fe-176">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="398fe-176">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
- [<span data-ttu-id="398fe-177">SearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="398fe-177">SearchableMailboxes</span></span>](searchablemailboxes.md)
    
<span data-ttu-id="398fe-178">Дополнительные коды ошибок, которые являются общими для веб-служб Exchange и специально для этой операции в разделе [ResponseCode](responsecode.md).</span><span class="sxs-lookup"><span data-stu-id="398fe-178">For additional error codes that are generic to EWS and specific to this operation, see [ResponseCode](responsecode.md).</span></span>
  
## <a name="see-also"></a><span data-ttu-id="398fe-179">См. также</span><span class="sxs-lookup"><span data-stu-id="398fe-179">See also</span></span>

- [<span data-ttu-id="398fe-180">Операции EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="398fe-180">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
    
- [<span data-ttu-id="398fe-181">Операция SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="398fe-181">SetHoldOnMailboxes operation</span></span>](setholdonmailboxes-operation.md)
    
- [<span data-ttu-id="398fe-182">Операция SearchMailboxes</span><span class="sxs-lookup"><span data-stu-id="398fe-182">SearchMailboxes operation</span></span>](searchmailboxes-operation.md)
    
- [<span data-ttu-id="398fe-183">Операция GetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="398fe-183">GetHoldOnMailboxes operation</span></span>](getholdonmailboxes-operation.md)
    
- [<span data-ttu-id="398fe-184">Операция GetDiscoverySearchConfiguration</span><span class="sxs-lookup"><span data-stu-id="398fe-184">GetDiscoverySearchConfiguration operation</span></span>](getdiscoverysearchconfiguration-operation.md)
    
- [<span data-ttu-id="398fe-185">Операция GetNonIndexableItemDetails</span><span class="sxs-lookup"><span data-stu-id="398fe-185">GetNonIndexableItemDetails operation</span></span>](getnonindexableitemdetails-operation.md)
    
- [<span data-ttu-id="398fe-186">Операция GetNonIndexableItemStatistics</span><span class="sxs-lookup"><span data-stu-id="398fe-186">GetNonIndexableItemStatistics operation</span></span>](getnonindexableitemstatistics-operation.md)
    

