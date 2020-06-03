---
title: Операция GetSearchableMailboxes
manager: sethgros
ms.date: 01/24/2020
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 47f8ff57-4835-4d2d-9136-44afb31a4cbe
description: Поиск сведений о GetSearchableMailboxesной операции EWS.
ms.openlocfilehash: e893a66eb1b638479eeccc6bd7548cb020f37243
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530841"
---
# <a name="getsearchablemailboxes-operation"></a><span data-ttu-id="a5d06-103">Операция GetSearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="a5d06-103">GetSearchableMailboxes operation</span></span>

> [!IMPORTANT]
> <span data-ttu-id="a5d06-104">Начиная с 1 апреля 2020, операция GetSearchableMailboxes больше не будет доступна в Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="a5d06-104">Starting on April 1, 2020, the GetSearchableMailboxes operation will no longer be available in Exchange Online.</span></span> <span data-ttu-id="a5d06-105">Эта операция не будет затронута в локальных версиях Exchange Server.</span><span class="sxs-lookup"><span data-stu-id="a5d06-105">This operation won't be affected in on-premises versions of Exchange Server.</span></span> <span data-ttu-id="a5d06-106">Дополнительные сведения см. [в статье выбытие средств прежних версий электронных данных в Exchange Online](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#getsearchablemailboxes-setholdonmailboxes-and-getholdonmailboxes-operations-in-the-ews-api).</span><span class="sxs-lookup"><span data-stu-id="a5d06-106">For more information, see [Retirement of legacy eDiscovery tools in Exchange Online](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#getsearchablemailboxes-setholdonmailboxes-and-getholdonmailboxes-operations-in-the-ews-api).</span></span>

<span data-ttu-id="a5d06-107">Поиск сведений о **GetSearchableMailboxesной** операции EWS.</span><span class="sxs-lookup"><span data-stu-id="a5d06-107">Find information about the **GetSearchableMailboxes** EWS operation.</span></span> 
  
<span data-ttu-id="a5d06-108">Операция **GetSearchableMailboxes** получает набор почтовых ящиков с возможностью поиска для поиска при обнаружении.</span><span class="sxs-lookup"><span data-stu-id="a5d06-108">The **GetSearchableMailboxes** operation gets a scoped set of searchable mailboxes for discovery searches.</span></span> <span data-ttu-id="a5d06-109">Область получаемых в ответе почтовых ящиков с возможностью поиска определяется фильтром поиска и развернутой группой рассылки.</span><span class="sxs-lookup"><span data-stu-id="a5d06-109">The scope of searchable mailboxes returned in the response is determined by the search filter and whether distribution group membership is expanded.</span></span> 

> [!NOTE] 
> <span data-ttu-id="a5d06-110">Эта операция предназначена для использования с фильтром поиска и извлечения только первых тысяч; Он не предназначен для получения исчерпывающей информации.</span><span class="sxs-lookup"><span data-stu-id="a5d06-110">This operation is intended to be used with the search filter and to retrieve only the first few thousands; it's not intended for exhaustive retrieval.</span></span>
  
<span data-ttu-id="a5d06-111">Эта операция появилась в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="a5d06-111">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-getsearchablemailboxes-operation"></a><span data-ttu-id="a5d06-112">Использование операции GetSearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="a5d06-112">Using the GetSearchableMailboxes operation</span></span>

<span data-ttu-id="a5d06-113">Операция **GetSearchableMailboxes** получает сведения о почтовых ящиках с возможностью поиска.</span><span class="sxs-lookup"><span data-stu-id="a5d06-113">The **GetSearchableMailboxes** operation gets information about searchable mailboxes.</span></span> <span data-ttu-id="a5d06-114">В запросе передаются следующие аргументы:</span><span class="sxs-lookup"><span data-stu-id="a5d06-114">The following arguments can be passed in the request:</span></span> 
  
- <span data-ttu-id="a5d06-115">[SearchFilter](searchfilter.md) — принимает один псевдоним электронной почты в качестве аргумента.</span><span class="sxs-lookup"><span data-stu-id="a5d06-115">[SearchFilter](searchfilter.md) - Accepts a single email alias as an argument.</span></span> 
    
- <span data-ttu-id="a5d06-116">[Експандграупмембершип](expandgroupmembership.md) — указывает, развернута ли членство в группе рассылки в результатах, возвращенных в ответе.</span><span class="sxs-lookup"><span data-stu-id="a5d06-116">[ExpandGroupMembership](expandgroupmembership.md) - Indicates whether the distribution group membership is expanded in the results returned in the response.</span></span> 
    
<span data-ttu-id="a5d06-117">Если набор псевдонимов электронной почты в фильтре поиска является группой рассылки, а членство в группе рассылки не развернуто, ответ будет содержать сведения о почтовом ящике для группы рассылки.</span><span class="sxs-lookup"><span data-stu-id="a5d06-117">If the email alias set in the search filter is a distribution group and the distribution group membership is not expanded, the response will contain the mailbox information for the distribution group.</span></span> <span data-ttu-id="a5d06-118">Если набор псевдонимов электронной почты в фильтре поиска является группой рассылки, а членство в группе рассылки развернуто, ответ будет содержать сведения о почтовом ящике для каждого почтового ящика, который является членом группы рассылки.</span><span class="sxs-lookup"><span data-stu-id="a5d06-118">If the email alias set in the search filter is a distribution group and the distribution group membership is expanded, the response will contain the mailbox information for each mailbox that is a member of the distribution group.</span></span> <span data-ttu-id="a5d06-119">Если фильтр поиска содержит псевдоним одного пользователя, ответ будет содержать сведения о почтовом ящике одного пользователя.</span><span class="sxs-lookup"><span data-stu-id="a5d06-119">If the search filter contains a single user's alias, the response will contain the mailbox information for the single user.</span></span> <span data-ttu-id="a5d06-120">Ответ будет содержать все почтовые ящики для поиска, если элемент [GetSearchableMailboxes](getsearchablemailboxes.md) пуст.</span><span class="sxs-lookup"><span data-stu-id="a5d06-120">The response will contain all searchable mailboxes if the [GetSearchableMailboxes](getsearchablemailboxes.md) element is empty.</span></span> <span data-ttu-id="a5d06-121">Это то же самое, что у пустого элемента [SearchFilter](searchfilter.md) , а для элемента [експандграупмембершип](expandgroupmembership.md) задано **значение false**.</span><span class="sxs-lookup"><span data-stu-id="a5d06-121">This is the same as having an empty [SearchFilter](searchfilter.md) element and the [ExpandGroupMembership](expandgroupmembership.md) element set to **false**.</span></span>
  
### <a name="getsearchablemailboxes-operation-soap-headers"></a><span data-ttu-id="a5d06-122">Заголовки SOAP операции GetSearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="a5d06-122">GetSearchableMailboxes operation SOAP headers</span></span>

<span data-ttu-id="a5d06-123">Операция **GetSearchableMailboxes** может использовать заголовки SOAP, указанные в приведенной ниже таблице.</span><span class="sxs-lookup"><span data-stu-id="a5d06-123">The **GetSearchableMailboxes** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="a5d06-124">Имя заголовка</span><span class="sxs-lookup"><span data-stu-id="a5d06-124">Header name</span></span>|<span data-ttu-id="a5d06-125">Элемент</span><span class="sxs-lookup"><span data-stu-id="a5d06-125">Element</span></span>|<span data-ttu-id="a5d06-126">Описание</span><span class="sxs-lookup"><span data-stu-id="a5d06-126">Description</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="a5d06-127">**ManagementRole**</span><span class="sxs-lookup"><span data-stu-id="a5d06-127">**ManagementRole**</span></span> <br/> |[<span data-ttu-id="a5d06-128">ManagementRole</span><span class="sxs-lookup"><span data-stu-id="a5d06-128">ManagementRole</span></span>](managementrole.md) <br/> |<span data-ttu-id="a5d06-129">Определяет роли сервера, необходимые для того, чтобы вызывающий абонент мог выполнить запрос.</span><span class="sxs-lookup"><span data-stu-id="a5d06-129">Identifies the server roles that are necessary in order for the caller to make the request.</span></span> <span data-ttu-id="a5d06-130">Этот заголовок является применимым для запроса.</span><span class="sxs-lookup"><span data-stu-id="a5d06-130">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="a5d06-131">**рекуестверсион**</span><span class="sxs-lookup"><span data-stu-id="a5d06-131">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="a5d06-132">рекуестсерверверсион</span><span class="sxs-lookup"><span data-stu-id="a5d06-132">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="a5d06-133">Определяет версию схемы для запроса операции.</span><span class="sxs-lookup"><span data-stu-id="a5d06-133">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="a5d06-134">Этот заголовок является применимым для запроса.</span><span class="sxs-lookup"><span data-stu-id="a5d06-134">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="a5d06-135">**серверверсион**</span><span class="sxs-lookup"><span data-stu-id="a5d06-135">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="a5d06-136">серверверсионинфо</span><span class="sxs-lookup"><span data-stu-id="a5d06-136">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="a5d06-137">Определяет версию сервера, который ответил на запрос.</span><span class="sxs-lookup"><span data-stu-id="a5d06-137">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="a5d06-138">Этот заголовок является применимым для отклика.</span><span class="sxs-lookup"><span data-stu-id="a5d06-138">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="getsearchablemailboxes-operation-request-example-request-information-about-a-distribution-group"></a><span data-ttu-id="a5d06-139">Пример запроса операции GetSearchableMailboxes: запрос сведений о группе рассылки</span><span class="sxs-lookup"><span data-stu-id="a5d06-139">GetSearchableMailboxes operation request example: Request information about a distribution group</span></span>

<span data-ttu-id="a5d06-140">В следующем примере запроса операции **GetSearchableMailboxes** показано, как получить сведения о почтовом ящике для группы рассылки лолграуп.</span><span class="sxs-lookup"><span data-stu-id="a5d06-140">The following example of a **GetSearchableMailboxes** operation request shows how to get the mailbox information for the lolgroup distribution group.</span></span> 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
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

<span data-ttu-id="a5d06-141">Текст SOAP Request содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="a5d06-141">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="a5d06-142">GetSearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="a5d06-142">GetSearchableMailboxes</span></span>](getsearchablemailboxes.md)   
- [<span data-ttu-id="a5d06-143">SearchFilter</span><span class="sxs-lookup"><span data-stu-id="a5d06-143">SearchFilter</span></span>](searchfilter.md)    
- [<span data-ttu-id="a5d06-144">експандграупмембершип</span><span class="sxs-lookup"><span data-stu-id="a5d06-144">ExpandGroupMembership</span></span>](expandgroupmembership.md)
    
## <a name="successful-getsearchablemailboxes-operation-response-get-information-about-a-distribution-group"></a><span data-ttu-id="a5d06-145">Успешный отклик операции GetSearchableMailboxes: получение сведений о группе рассылки</span><span class="sxs-lookup"><span data-stu-id="a5d06-145">Successful GetSearchableMailboxes operation response: Get information about a distribution group</span></span>

<span data-ttu-id="a5d06-146">В следующем примере показан успешный ответ на запрос операции **GetSearchableMailboxes** для получения сведений об обнаружении для группы рассылки лолграуп.</span><span class="sxs-lookup"><span data-stu-id="a5d06-146">The following example shows a successful response to a **GetSearchableMailboxes** operation request to get the discovery information for the lolgroup distribution group.</span></span> 
  
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
      <GetSearchableMailboxesResponse ResponseClass="Success" 
                                      xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
         <SearchableMailboxes>
            <SearchableMailbox xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
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

<span data-ttu-id="a5d06-147">Тело SOAP отклика содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="a5d06-147">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="a5d06-148">жетсеарчаблемаилбоксесреспонсе</span><span class="sxs-lookup"><span data-stu-id="a5d06-148">GetSearchableMailboxesResponse</span></span>](getsearchablemailboxesresponse.md)   
- [<span data-ttu-id="a5d06-149">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="a5d06-149">ResponseCode</span></span>](responsecode.md)   
- [<span data-ttu-id="a5d06-150">сеарчаблемаилбоксес</span><span class="sxs-lookup"><span data-stu-id="a5d06-150">SearchableMailboxes</span></span>](searchablemailboxes.md)    
- [<span data-ttu-id="a5d06-151">сеарчаблемаилбокс</span><span class="sxs-lookup"><span data-stu-id="a5d06-151">SearchableMailbox</span></span>](searchablemailbox.md)    
- [<span data-ttu-id="a5d06-152">Guid</span><span class="sxs-lookup"><span data-stu-id="a5d06-152">Guid</span></span>](guid-ex15websvcsotherref.md)    
- [<span data-ttu-id="a5d06-153">PrimarySmtpAddress</span><span class="sxs-lookup"><span data-stu-id="a5d06-153">PrimarySmtpAddress</span></span>](primarysmtpaddress.md)    
- [<span data-ttu-id="a5d06-154">исекстерналмаилбокс</span><span class="sxs-lookup"><span data-stu-id="a5d06-154">IsExternalMailbox</span></span>](isexternalmailbox.md)   
- [<span data-ttu-id="a5d06-155">ExternalEmailAddress</span><span class="sxs-lookup"><span data-stu-id="a5d06-155">ExternalEmailAddress</span></span>](externalemailaddress.md)    
- [<span data-ttu-id="a5d06-156">DisplayName (строка)</span><span class="sxs-lookup"><span data-stu-id="a5d06-156">DisplayName (string)</span></span>](displayname-string.md)    
- [<span data-ttu-id="a5d06-157">исмембершипграуп</span><span class="sxs-lookup"><span data-stu-id="a5d06-157">IsMembershipGroup</span></span>](ismembershipgroup.md)    
- [<span data-ttu-id="a5d06-158">ReferenceId</span><span class="sxs-lookup"><span data-stu-id="a5d06-158">ReferenceId</span></span>](referenceid.md)
    
## <a name="successful-getsearchablemailboxes-operation-response-get-information-about-an-expanded-distribution-group"></a><span data-ttu-id="a5d06-159">Успешный отклик операции GetSearchableMailboxes: получение сведений о расширенной группе рассылки</span><span class="sxs-lookup"><span data-stu-id="a5d06-159">Successful GetSearchableMailboxes operation response: Get information about an expanded distribution group</span></span>

<span data-ttu-id="a5d06-160">В следующем примере показан успешный ответ на запрос операции **GetSearchableMailboxes** для получения сведений об обнаружении членов развернутой группы рассылки лолграуп.</span><span class="sxs-lookup"><span data-stu-id="a5d06-160">The following example shows a successful response to a **GetSearchableMailboxes** operation request to get the discovery information about members of the expanded lolgroup distribution group.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="526" MinorBuildNumber="0" Version="Exchange2013" xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" xmlns="https://schemas.microsoft.com/exchange/services/2006/types" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <GetSearchableMailboxesResponse ResponseClass="Success" xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseCode>NoError</ResponseCode>
      <SearchableMailboxes>
        <SearchableMailbox xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
          <Guid>e2d42cdf-a227-1ec3-486b-6fa0ebaadb9f5</Guid>
          <PrimarySmtpAddress>JSmith@contoso.com</PrimarySmtpAddress>
          <IsExternalMailbox>false</IsExternalMailbox>
          <ExternalEmailAddress/>
          <DisplayName>Julia Smith</DisplayName>
          <IsMembershipGroup>false</IsMembershipGroup>
          <ReferenceId>/o=First Organization/ou=Exchange Administrative Group (FYDLT)/cn=Recipients/cn=0a1fc86f883846152405d60956dd02e7-Julia</ReferenceId>
        </SearchableMailbox>
        <SearchableMailbox xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
          <Guid>45d0fff1-6541-459a-a343-52453b30e12ca</Guid>
          <PrimarySmtpAddress>LMoore@contoso.com</PrimarySmtpAddress>
          <IsExternalMailbox>false</IsExternalMailbox>
          <ExternalEmailAddress/>
          <DisplayName>Laura Moore</DisplayName>
          <IsMembershipGroup>false</IsMembershipGroup>
          <ReferenceId>/o=First Organization/ou=Exchange Administrative Group (FYDLT)/cn=Recipients/cn=2910d8f8316f4378bbf9338d8f9d714b-Laura</ReferenceId>
        </SearchableMailbox>
        <SearchableMailbox xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
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

<span data-ttu-id="a5d06-161">Тело SOAP отклика содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="a5d06-161">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="a5d06-162">жетсеарчаблемаилбоксесреспонсе</span><span class="sxs-lookup"><span data-stu-id="a5d06-162">GetSearchableMailboxesResponse</span></span>](getsearchablemailboxesresponse.md)    
- [<span data-ttu-id="a5d06-163">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="a5d06-163">ResponseCode</span></span>](responsecode.md)   
- [<span data-ttu-id="a5d06-164">сеарчаблемаилбоксес</span><span class="sxs-lookup"><span data-stu-id="a5d06-164">SearchableMailboxes</span></span>](searchablemailboxes.md)    
- [<span data-ttu-id="a5d06-165">сеарчаблемаилбокс</span><span class="sxs-lookup"><span data-stu-id="a5d06-165">SearchableMailbox</span></span>](searchablemailbox.md)    
- [<span data-ttu-id="a5d06-166">Guid</span><span class="sxs-lookup"><span data-stu-id="a5d06-166">Guid</span></span>](guid-ex15websvcsotherref.md)    
- [<span data-ttu-id="a5d06-167">PrimarySmtpAddress</span><span class="sxs-lookup"><span data-stu-id="a5d06-167">PrimarySmtpAddress</span></span>](primarysmtpaddress.md)    
- [<span data-ttu-id="a5d06-168">исекстерналмаилбокс</span><span class="sxs-lookup"><span data-stu-id="a5d06-168">IsExternalMailbox</span></span>](isexternalmailbox.md)    
- [<span data-ttu-id="a5d06-169">ExternalEmailAddress</span><span class="sxs-lookup"><span data-stu-id="a5d06-169">ExternalEmailAddress</span></span>](externalemailaddress.md)    
- [<span data-ttu-id="a5d06-170">DisplayName (строка)</span><span class="sxs-lookup"><span data-stu-id="a5d06-170">DisplayName (string)</span></span>](displayname-string.md)    
- [<span data-ttu-id="a5d06-171">исмембершипграуп</span><span class="sxs-lookup"><span data-stu-id="a5d06-171">IsMembershipGroup</span></span>](ismembershipgroup.md)    
- [<span data-ttu-id="a5d06-172">ReferenceId</span><span class="sxs-lookup"><span data-stu-id="a5d06-172">ReferenceId</span></span>](referenceid.md)
    
## <a name="getsearchablemailboxes-operation-error-response"></a><span data-ttu-id="a5d06-173">Ответ об ошибке операции GetSearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="a5d06-173">GetSearchableMailboxes operation error response</span></span>

<span data-ttu-id="a5d06-174">В следующем примере показан ответ об ошибке для запроса операции **GetSearchableMailboxes** .</span><span class="sxs-lookup"><span data-stu-id="a5d06-174">The following example shows an error response to a **GetSearchableMailboxes** operation request.</span></span> <span data-ttu-id="a5d06-175">Это ответ на запрос на получение всех почтовых ящиков, для которых выполняется поиск, если для аргумента **експандграупмембершип** задано значение **true**.</span><span class="sxs-lookup"><span data-stu-id="a5d06-175">This is a response to a request to get all searchable mailboxes when the **ExpandGroupMembership** argument is set to **true**.</span></span> 
  
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
      <GetSearchableMailboxesResponse ResponseClass="Error" 
                                      xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>Cannot use wildcard or empty query when auto group expansion is enabled.</MessageText>
         <ResponseCode>ErrorInvalidArgument</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
         <SearchableMailboxes/>
      </GetSearchableMailboxesResponse>
   </s:Body>
</s:Envelope>

```

<span data-ttu-id="a5d06-176">Основной текст сообщения об ошибке SOAP содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="a5d06-176">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="a5d06-177">жетсеарчаблемаилбоксесреспонсе</span><span class="sxs-lookup"><span data-stu-id="a5d06-177">GetSearchableMailboxesResponse</span></span>](getsearchablemailboxesresponse.md)  
- [<span data-ttu-id="a5d06-178">мессажетекст</span><span class="sxs-lookup"><span data-stu-id="a5d06-178">MessageText</span></span>](messagetext.md)   
- [<span data-ttu-id="a5d06-179">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="a5d06-179">ResponseCode</span></span>](responsecode.md)   
- [<span data-ttu-id="a5d06-180">дескриптивелинккэй</span><span class="sxs-lookup"><span data-stu-id="a5d06-180">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) 
- [<span data-ttu-id="a5d06-181">сеарчаблемаилбоксес</span><span class="sxs-lookup"><span data-stu-id="a5d06-181">SearchableMailboxes</span></span>](searchablemailboxes.md)
    
<span data-ttu-id="a5d06-182">Дополнительные коды ошибок, которые являются общими для EWS и специфичными для этой операции, можно найти в разделе [респонсекоде](responsecode.md).</span><span class="sxs-lookup"><span data-stu-id="a5d06-182">For additional error codes that are generic to EWS and specific to this operation, see [ResponseCode](responsecode.md).</span></span>
  
## <a name="see-also"></a><span data-ttu-id="a5d06-183">См. также</span><span class="sxs-lookup"><span data-stu-id="a5d06-183">See also</span></span>

- [<span data-ttu-id="a5d06-184">Операции EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="a5d06-184">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)   
- [<span data-ttu-id="a5d06-185">Операция SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="a5d06-185">SetHoldOnMailboxes operation</span></span>](setholdonmailboxes-operation.md)   
- [<span data-ttu-id="a5d06-186">Операция SearchMailboxes</span><span class="sxs-lookup"><span data-stu-id="a5d06-186">SearchMailboxes operation</span></span>](searchmailboxes-operation.md)   
- [<span data-ttu-id="a5d06-187">Операция GetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="a5d06-187">GetHoldOnMailboxes operation</span></span>](getholdonmailboxes-operation.md)    
- [<span data-ttu-id="a5d06-188">Операция GetDiscoverySearchConfiguration</span><span class="sxs-lookup"><span data-stu-id="a5d06-188">GetDiscoverySearchConfiguration operation</span></span>](getdiscoverysearchconfiguration-operation.md)   
- [<span data-ttu-id="a5d06-189">Операция GetNonIndexableItemDetails</span><span class="sxs-lookup"><span data-stu-id="a5d06-189">GetNonIndexableItemDetails operation</span></span>](getnonindexableitemdetails-operation.md)   
- [<span data-ttu-id="a5d06-190">Операция GetNonIndexableItemStatistics</span><span class="sxs-lookup"><span data-stu-id="a5d06-190">GetNonIndexableItemStatistics operation</span></span>](getnonindexableitemstatistics-operation.md)
    

