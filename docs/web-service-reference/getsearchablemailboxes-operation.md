---
title: Операция GetSearchableMailboxes
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 47f8ff57-4835-4d2d-9136-44afb31a4cbe
description: Поиск сведений о GetSearchableMailboxesной операции EWS.
ms.openlocfilehash: 5e14288280b23e2555eea4fce0f77743d7d210ce
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762910"
---
# <a name="getsearchablemailboxes-operation"></a><span data-ttu-id="129fd-103">Операция GetSearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="129fd-103">GetSearchableMailboxes operation</span></span>

<span data-ttu-id="129fd-104">Поиск сведений о **GetSearchableMailboxesной** операции EWS.</span><span class="sxs-lookup"><span data-stu-id="129fd-104">Find information about the **GetSearchableMailboxes** EWS operation.</span></span> 
  
<span data-ttu-id="129fd-105">Операция **GetSearchableMailboxes** получает набор почтовых ящиков с возможностью поиска для поиска при обнаружении.</span><span class="sxs-lookup"><span data-stu-id="129fd-105">The **GetSearchableMailboxes** operation gets a scoped set of searchable mailboxes for discovery searches.</span></span> <span data-ttu-id="129fd-106">Область получаемых в ответе почтовых ящиков с возможностью поиска определяется фильтром поиска и развернутой группой рассылки.</span><span class="sxs-lookup"><span data-stu-id="129fd-106">The scope of searchable mailboxes returned in the response is determined by the search filter and whether distribution group membership is expanded.</span></span> 
  
<span data-ttu-id="129fd-107">Эта операция появилась в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="129fd-107">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-getsearchablemailboxes-operation"></a><span data-ttu-id="129fd-108">Использование операции GetSearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="129fd-108">Using the GetSearchableMailboxes operation</span></span>

<span data-ttu-id="129fd-109">Операция **GetSearchableMailboxes** получает сведения о почтовых ящиках с возможностью поиска.</span><span class="sxs-lookup"><span data-stu-id="129fd-109">The **GetSearchableMailboxes** operation gets information about searchable mailboxes.</span></span> <span data-ttu-id="129fd-110">В запросе передаются следующие аргументы:</span><span class="sxs-lookup"><span data-stu-id="129fd-110">The following arguments can be passed in the request:</span></span> 
  
- <span data-ttu-id="129fd-111">[SearchFilter](searchfilter.md) — принимает один псевдоним электронной почты в качестве аргумента.</span><span class="sxs-lookup"><span data-stu-id="129fd-111">[SearchFilter](searchfilter.md) —Accepts a single email alias as an argument.</span></span> 
    
- <span data-ttu-id="129fd-112">[Експандграупмембершип](expandgroupmembership.md) — указывает, развернута ли членство в группе рассылки в результатах, возвращенных в ответе.</span><span class="sxs-lookup"><span data-stu-id="129fd-112">[ExpandGroupMembership](expandgroupmembership.md) — Indicates whether the distribution group membership is expanded in the results returned in the response.</span></span> 
    
<span data-ttu-id="129fd-113">Если набор псевдонимов электронной почты в фильтре поиска является группой рассылки, а членство в группе рассылки не развернуто, ответ будет содержать сведения о почтовом ящике для группы рассылки.</span><span class="sxs-lookup"><span data-stu-id="129fd-113">If the email alias set in the search filter is a distribution group and the distribution group membership is not expanded, the response will contain the mailbox information for the distribution group.</span></span> <span data-ttu-id="129fd-114">Если набор псевдонимов электронной почты в фильтре поиска является группой рассылки, а членство в группе рассылки развернуто, ответ будет содержать сведения о почтовом ящике для каждого почтового ящика, который является членом группы рассылки.</span><span class="sxs-lookup"><span data-stu-id="129fd-114">If the email alias set in the search filter is a distribution group and the distribution group membership is expanded, the response will contain the mailbox information for each mailbox that is a member of the distribution group.</span></span> <span data-ttu-id="129fd-115">Если фильтр поиска содержит псевдоним одного пользователя, ответ будет содержать сведения о почтовом ящике одного пользователя.</span><span class="sxs-lookup"><span data-stu-id="129fd-115">If the search filter contains a single user's alias, the response will contain the mailbox information for the single user.</span></span> <span data-ttu-id="129fd-116">Ответ будет содержать все почтовые ящики для поиска, если элемент [GetSearchableMailboxes](getsearchablemailboxes.md) пуст.</span><span class="sxs-lookup"><span data-stu-id="129fd-116">The response will contain all searchable mailboxes if the [GetSearchableMailboxes](getsearchablemailboxes.md) element is empty.</span></span> <span data-ttu-id="129fd-117">Это то же самое, что у пустого элемента [SearchFilter](searchfilter.md) , а для элемента [експандграупмембершип](expandgroupmembership.md) задано **значение false**.</span><span class="sxs-lookup"><span data-stu-id="129fd-117">This is the same as having an empty [SearchFilter](searchfilter.md) element and the [ExpandGroupMembership](expandgroupmembership.md) element set to **false**.</span></span>
  
### <a name="getsearchablemailboxes-operation-soap-headers"></a><span data-ttu-id="129fd-118">Заголовки SOAP операции GetSearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="129fd-118">GetSearchableMailboxes operation SOAP headers</span></span>

<span data-ttu-id="129fd-119">Операция **GetSearchableMailboxes** может использовать заголовки SOAP, указанные в приведенной ниже таблице.</span><span class="sxs-lookup"><span data-stu-id="129fd-119">The **GetSearchableMailboxes** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="129fd-120">**Имя заголовка**</span><span class="sxs-lookup"><span data-stu-id="129fd-120">**Header name**</span></span>|<span data-ttu-id="129fd-121">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="129fd-121">**Element**</span></span>|<span data-ttu-id="129fd-122">**Описание**</span><span class="sxs-lookup"><span data-stu-id="129fd-122">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="129fd-123">**ManagementRole**</span><span class="sxs-lookup"><span data-stu-id="129fd-123">**ManagementRole**</span></span> <br/> |[<span data-ttu-id="129fd-124">ManagementRole</span><span class="sxs-lookup"><span data-stu-id="129fd-124">ManagementRole</span></span>](managementrole.md) <br/> |<span data-ttu-id="129fd-125">Определяет роли сервера, необходимые для того, чтобы вызывающий абонент мог выполнить запрос.</span><span class="sxs-lookup"><span data-stu-id="129fd-125">Identifies the server roles that are necessary in order for the caller to make the request.</span></span> <span data-ttu-id="129fd-126">Этот заголовок является применимым для запроса.</span><span class="sxs-lookup"><span data-stu-id="129fd-126">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="129fd-127">**рекуестверсион**</span><span class="sxs-lookup"><span data-stu-id="129fd-127">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="129fd-128">рекуестсерверверсион</span><span class="sxs-lookup"><span data-stu-id="129fd-128">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="129fd-129">Определяет версию схемы для запроса операции.</span><span class="sxs-lookup"><span data-stu-id="129fd-129">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="129fd-130">Этот заголовок является применимым для запроса.</span><span class="sxs-lookup"><span data-stu-id="129fd-130">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="129fd-131">**серверверсион**</span><span class="sxs-lookup"><span data-stu-id="129fd-131">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="129fd-132">серверверсионинфо</span><span class="sxs-lookup"><span data-stu-id="129fd-132">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="129fd-133">Определяет версию сервера, который ответил на запрос.</span><span class="sxs-lookup"><span data-stu-id="129fd-133">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="129fd-134">Этот заголовок является применимым для отклика.</span><span class="sxs-lookup"><span data-stu-id="129fd-134">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="getsearchablemailboxes-operation-request-example-request-information-about-a-distribution-group"></a><span data-ttu-id="129fd-135">Пример запроса операции GetSearchableMailboxes: запрос сведений о группе рассылки</span><span class="sxs-lookup"><span data-stu-id="129fd-135">GetSearchableMailboxes operation request example: Request information about a distribution group</span></span>

<span data-ttu-id="129fd-136">В следующем примере запроса операции **GetSearchableMailboxes** показано, как получить сведения о почтовом ящике для группы рассылки лолграуп.</span><span class="sxs-lookup"><span data-stu-id="129fd-136">The following example of a **GetSearchableMailboxes** operation request shows how to get the mailbox information for the lolgroup distribution group.</span></span> 
  
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

<span data-ttu-id="129fd-137">Текст SOAP Request содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="129fd-137">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="129fd-138">GetSearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="129fd-138">GetSearchableMailboxes</span></span>](getsearchablemailboxes.md)
    
- [<span data-ttu-id="129fd-139">SearchFilter</span><span class="sxs-lookup"><span data-stu-id="129fd-139">SearchFilter</span></span>](searchfilter.md)
    
- [<span data-ttu-id="129fd-140">експандграупмембершип</span><span class="sxs-lookup"><span data-stu-id="129fd-140">ExpandGroupMembership</span></span>](expandgroupmembership.md)
    
## <a name="successful-getsearchablemailboxes-operation-response-get-information-about-a-distribution-group"></a><span data-ttu-id="129fd-141">Успешный отклик операции GetSearchableMailboxes: получение сведений о группе рассылки</span><span class="sxs-lookup"><span data-stu-id="129fd-141">Successful GetSearchableMailboxes operation response: Get information about a distribution group</span></span>

<span data-ttu-id="129fd-142">В следующем примере показан успешный ответ на запрос операции **GetSearchableMailboxes** для получения сведений об обнаружении для группы рассылки лолграуп.</span><span class="sxs-lookup"><span data-stu-id="129fd-142">The following example shows a successful response to a **GetSearchableMailboxes** operation request to get the discovery information for the lolgroup distribution group.</span></span> 
  
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

<span data-ttu-id="129fd-143">Тело SOAP отклика содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="129fd-143">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="129fd-144">жетсеарчаблемаилбоксесреспонсе</span><span class="sxs-lookup"><span data-stu-id="129fd-144">GetSearchableMailboxesResponse</span></span>](getsearchablemailboxesresponse.md)
    
- [<span data-ttu-id="129fd-145">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="129fd-145">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="129fd-146">сеарчаблемаилбоксес</span><span class="sxs-lookup"><span data-stu-id="129fd-146">SearchableMailboxes</span></span>](searchablemailboxes.md)
    
- [<span data-ttu-id="129fd-147">сеарчаблемаилбокс</span><span class="sxs-lookup"><span data-stu-id="129fd-147">SearchableMailbox</span></span>](searchablemailbox.md)
    
- [<span data-ttu-id="129fd-148">Guid</span><span class="sxs-lookup"><span data-stu-id="129fd-148">Guid</span></span>](guid-ex15websvcsotherref.md)
    
- [<span data-ttu-id="129fd-149">PrimarySmtpAddress</span><span class="sxs-lookup"><span data-stu-id="129fd-149">PrimarySmtpAddress</span></span>](primarysmtpaddress.md)
    
- [<span data-ttu-id="129fd-150">исекстерналмаилбокс</span><span class="sxs-lookup"><span data-stu-id="129fd-150">IsExternalMailbox</span></span>](isexternalmailbox.md)
    
- [<span data-ttu-id="129fd-151">ExternalEmailAddress</span><span class="sxs-lookup"><span data-stu-id="129fd-151">ExternalEmailAddress</span></span>](externalemailaddress.md)
    
- [<span data-ttu-id="129fd-152">DisplayName (строка)</span><span class="sxs-lookup"><span data-stu-id="129fd-152">DisplayName (string)</span></span>](displayname-string.md)
    
- [<span data-ttu-id="129fd-153">исмембершипграуп</span><span class="sxs-lookup"><span data-stu-id="129fd-153">IsMembershipGroup</span></span>](ismembershipgroup.md)
    
- [<span data-ttu-id="129fd-154">ReferenceId</span><span class="sxs-lookup"><span data-stu-id="129fd-154">ReferenceId</span></span>](referenceid.md)
    
## <a name="successful-getsearchablemailboxes-operation-response-get-information-about-an-expanded-distribution-group"></a><span data-ttu-id="129fd-155">Успешный отклик операции GetSearchableMailboxes: получение сведений о расширенной группе рассылки</span><span class="sxs-lookup"><span data-stu-id="129fd-155">Successful GetSearchableMailboxes operation response: Get information about an expanded distribution group</span></span>

<span data-ttu-id="129fd-156">В следующем примере показан успешный ответ на запрос операции **GetSearchableMailboxes** для получения сведений об обнаружении членов развернутой группы рассылки лолграуп.</span><span class="sxs-lookup"><span data-stu-id="129fd-156">The following example shows a successful response to a **GetSearchableMailboxes** operation request to get the discovery information about members of the expanded lolgroup distribution group.</span></span> 
  
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

<span data-ttu-id="129fd-157">Тело SOAP отклика содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="129fd-157">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="129fd-158">жетсеарчаблемаилбоксесреспонсе</span><span class="sxs-lookup"><span data-stu-id="129fd-158">GetSearchableMailboxesResponse</span></span>](getsearchablemailboxesresponse.md)
    
- [<span data-ttu-id="129fd-159">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="129fd-159">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="129fd-160">сеарчаблемаилбоксес</span><span class="sxs-lookup"><span data-stu-id="129fd-160">SearchableMailboxes</span></span>](searchablemailboxes.md)
    
- [<span data-ttu-id="129fd-161">сеарчаблемаилбокс</span><span class="sxs-lookup"><span data-stu-id="129fd-161">SearchableMailbox</span></span>](searchablemailbox.md)
    
- [<span data-ttu-id="129fd-162">Guid</span><span class="sxs-lookup"><span data-stu-id="129fd-162">Guid</span></span>](guid-ex15websvcsotherref.md)
    
- [<span data-ttu-id="129fd-163">PrimarySmtpAddress</span><span class="sxs-lookup"><span data-stu-id="129fd-163">PrimarySmtpAddress</span></span>](primarysmtpaddress.md)
    
- [<span data-ttu-id="129fd-164">исекстерналмаилбокс</span><span class="sxs-lookup"><span data-stu-id="129fd-164">IsExternalMailbox</span></span>](isexternalmailbox.md)
    
- [<span data-ttu-id="129fd-165">ExternalEmailAddress</span><span class="sxs-lookup"><span data-stu-id="129fd-165">ExternalEmailAddress</span></span>](externalemailaddress.md)
    
- [<span data-ttu-id="129fd-166">DisplayName (строка)</span><span class="sxs-lookup"><span data-stu-id="129fd-166">DisplayName (string)</span></span>](displayname-string.md)
    
- [<span data-ttu-id="129fd-167">исмембершипграуп</span><span class="sxs-lookup"><span data-stu-id="129fd-167">IsMembershipGroup</span></span>](ismembershipgroup.md)
    
- [<span data-ttu-id="129fd-168">ReferenceId</span><span class="sxs-lookup"><span data-stu-id="129fd-168">ReferenceId</span></span>](referenceid.md)
    
## <a name="getsearchablemailboxes-operation-error-response"></a><span data-ttu-id="129fd-169">Ответ об ошибке операции GetSearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="129fd-169">GetSearchableMailboxes operation error response</span></span>

<span data-ttu-id="129fd-170">В следующем примере показан ответ об ошибке для запроса операции **GetSearchableMailboxes** .</span><span class="sxs-lookup"><span data-stu-id="129fd-170">The following example shows an error response to a **GetSearchableMailboxes** operation request.</span></span> <span data-ttu-id="129fd-171">Это ответ на запрос на получение всех почтовых ящиков, для которых выполняется поиск, если для аргумента **експандграупмембершип** задано значение **true**.</span><span class="sxs-lookup"><span data-stu-id="129fd-171">This is a response to a request to get all searchable mailboxes when the **ExpandGroupMembership** argument is set to **true**.</span></span> 
  
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

<span data-ttu-id="129fd-172">Основной текст сообщения об ошибке SOAP содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="129fd-172">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="129fd-173">жетсеарчаблемаилбоксесреспонсе</span><span class="sxs-lookup"><span data-stu-id="129fd-173">GetSearchableMailboxesResponse</span></span>](getsearchablemailboxesresponse.md)
    
- [<span data-ttu-id="129fd-174">мессажетекст</span><span class="sxs-lookup"><span data-stu-id="129fd-174">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="129fd-175">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="129fd-175">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="129fd-176">дескриптивелинккэй</span><span class="sxs-lookup"><span data-stu-id="129fd-176">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
- [<span data-ttu-id="129fd-177">сеарчаблемаилбоксес</span><span class="sxs-lookup"><span data-stu-id="129fd-177">SearchableMailboxes</span></span>](searchablemailboxes.md)
    
<span data-ttu-id="129fd-178">Дополнительные коды ошибок, которые являются общими для EWS и специфичными для этой операции, можно найти в разделе [респонсекоде](responsecode.md).</span><span class="sxs-lookup"><span data-stu-id="129fd-178">For additional error codes that are generic to EWS and specific to this operation, see [ResponseCode](responsecode.md).</span></span>
  
## <a name="see-also"></a><span data-ttu-id="129fd-179">См. также</span><span class="sxs-lookup"><span data-stu-id="129fd-179">See also</span></span>

- [<span data-ttu-id="129fd-180">Операции EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="129fd-180">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
    
- [<span data-ttu-id="129fd-181">Операция SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="129fd-181">SetHoldOnMailboxes operation</span></span>](setholdonmailboxes-operation.md)
    
- [<span data-ttu-id="129fd-182">Операция SearchMailboxes</span><span class="sxs-lookup"><span data-stu-id="129fd-182">SearchMailboxes operation</span></span>](searchmailboxes-operation.md)
    
- [<span data-ttu-id="129fd-183">Операция GetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="129fd-183">GetHoldOnMailboxes operation</span></span>](getholdonmailboxes-operation.md)
    
- [<span data-ttu-id="129fd-184">Операция GetDiscoverySearchConfiguration</span><span class="sxs-lookup"><span data-stu-id="129fd-184">GetDiscoverySearchConfiguration operation</span></span>](getdiscoverysearchconfiguration-operation.md)
    
- [<span data-ttu-id="129fd-185">Операция GetNonIndexableItemDetails</span><span class="sxs-lookup"><span data-stu-id="129fd-185">GetNonIndexableItemDetails operation</span></span>](getnonindexableitemdetails-operation.md)
    
- [<span data-ttu-id="129fd-186">Операция GetNonIndexableItemStatistics</span><span class="sxs-lookup"><span data-stu-id="129fd-186">GetNonIndexableItemStatistics operation</span></span>](getnonindexableitemstatistics-operation.md)
    

