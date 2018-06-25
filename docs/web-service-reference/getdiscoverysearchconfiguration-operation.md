---
title: Операция GetDiscoverySearchConfiguration
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 8a54a6dc-110c-4972-a8bc-5ddb43c4b857
description: Найдите сведения о веб-служб Exchange GetDiscoverySearchConfiguration операции.
ms.openlocfilehash: a50463e575bf5a4ffdafc357d91563b0ca0486f4
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762747"
---
# <a name="getdiscoverysearchconfiguration-operation"></a><span data-ttu-id="e1478-103">Операция GetDiscoverySearchConfiguration</span><span class="sxs-lookup"><span data-stu-id="e1478-103">GetDiscoverySearchConfiguration operation</span></span>

<span data-ttu-id="e1478-104">Найдите сведения о **GetDiscoverySearchConfiguration** операции веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="e1478-104">Find information about the **GetDiscoverySearchConfiguration** EWS operation.</span></span> 
  
<span data-ttu-id="e1478-105">Операция **GetDiscoverySearchConfiguration** возвращает содержит сведения о конфигурации на месте, сохраненные операций поиска обнаружения и почтовые ящики, которые разрешены для поиска обнаружения.</span><span class="sxs-lookup"><span data-stu-id="e1478-105">The **GetDiscoverySearchConfiguration** operation returns configuration information for in-place holds, saved discovery searches, and the mailboxes that are enabled for discovery search.</span></span> 
  
<span data-ttu-id="e1478-106">Эта операция появилась в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="e1478-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-getdiscoverysearchconfiguration-operation"></a><span data-ttu-id="e1478-107">С помощью операции GetDiscoverySearchConfiguration</span><span class="sxs-lookup"><span data-stu-id="e1478-107">Using the GetDiscoverySearchConfiguration operation</span></span>

<span data-ttu-id="e1478-108">Операция **GetDiscoverySearchConfiguration** предоставляет сведения о конфигурации для поиска обнаружения.</span><span class="sxs-lookup"><span data-stu-id="e1478-108">The **GetDiscoverySearchConfiguration** operation provides configuration information for discovery search.</span></span> <span data-ttu-id="e1478-109">Запросы могут содержать один или несколько следующих аргументов:</span><span class="sxs-lookup"><span data-stu-id="e1478-109">Requests can contain one or more of the following arguments:</span></span> 
  
1. <span data-ttu-id="e1478-110">[SearchId](searchid.md) — определяет поиска сохраненных обнаружения.</span><span class="sxs-lookup"><span data-stu-id="e1478-110">[SearchId](searchid.md) — Identifies a saved discovery search.</span></span> <span data-ttu-id="e1478-111">Если этот аргумент отправляется в запросе, значения других аргументов игнорируются.</span><span class="sxs-lookup"><span data-stu-id="e1478-111">If this argument is sent in the request, the values of the other arguments are ignored.</span></span> 
    
2. <span data-ttu-id="e1478-112">[ExpandGroupMembership](expandgroupmembership.md) — указывает, развернут ли членство в группах в ответе.</span><span class="sxs-lookup"><span data-stu-id="e1478-112">[ExpandGroupMembership](expandgroupmembership.md) — Indicates whether group membership is expanded in the response.</span></span> <span data-ttu-id="e1478-113">Значение **true** указывает, что членство в группах будет развернут, чтобы все почтовые ящики с возможностью поиска возвращаемого в ответе.</span><span class="sxs-lookup"><span data-stu-id="e1478-113">A value of **true** indicates that group membership is expanded so that all searchable mailboxes are returned in the response.</span></span> <span data-ttu-id="e1478-114">Значение **false** указывает, что возвращаются только группы в ответе.</span><span class="sxs-lookup"><span data-stu-id="e1478-114">A value of **false** indicates that only the group is returned in the response.</span></span> 
    
3. <span data-ttu-id="e1478-115">[InPlaceHoldConfigurationOnly](inplaceholdconfigurationonly.md) — указывает, возвращаются ли все почтовые ящики для поиска в дополнение к конфигурации хранения на месте.</span><span class="sxs-lookup"><span data-stu-id="e1478-115">[InPlaceHoldConfigurationOnly](inplaceholdconfigurationonly.md) — Indicates whether all searchable mailboxes are returned in addition to the in-place hold configuration.</span></span> <span data-ttu-id="e1478-116">Значение **true** указывает, что возвращаются только конфигурации хранения на месте.</span><span class="sxs-lookup"><span data-stu-id="e1478-116">A value of **true** indicates that only the in-place hold configurations are returned.</span></span> <span data-ttu-id="e1478-117">Значение **false** указывает, что возвращаются все идентификаторы для поиска почтовых ящиков в дополнение к идентификаторы хранения на месте.</span><span class="sxs-lookup"><span data-stu-id="e1478-117">A value of **false** indicates that all searchable mailbox identifiers are returned in addition to the in-place hold identifiers.</span></span> <span data-ttu-id="e1478-118">Если этот элемент не указан, поведение по умолчанию является эквивалентом значение **false**.</span><span class="sxs-lookup"><span data-stu-id="e1478-118">If this element is not present, the default behavior is the equivalent of the value **false**.</span></span> 
    
### <a name="getdiscoverysearchconfiguration-operation-soap-headers"></a><span data-ttu-id="e1478-119">Заголовки SOAP GetDiscoverySearchConfiguration операции</span><span class="sxs-lookup"><span data-stu-id="e1478-119">GetDiscoverySearchConfiguration operation SOAP headers</span></span>

<span data-ttu-id="e1478-120">Операция **GetDiscoverySearchConfiguration** можно использовать заголовки SOAP, которые перечислены в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="e1478-120">The **GetDiscoverySearchConfiguration** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="e1478-121">**Имя заголовка**</span><span class="sxs-lookup"><span data-stu-id="e1478-121">**Header name**</span></span>|<span data-ttu-id="e1478-122">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="e1478-122">**Element**</span></span>|<span data-ttu-id="e1478-123">**Описание**</span><span class="sxs-lookup"><span data-stu-id="e1478-123">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="e1478-124">**ManagementRole**</span><span class="sxs-lookup"><span data-stu-id="e1478-124">**ManagementRole**</span></span> <br/> |[<span data-ttu-id="e1478-125">ManagementRole</span><span class="sxs-lookup"><span data-stu-id="e1478-125">ManagementRole</span></span>](managementrole.md) <br/> |<span data-ttu-id="e1478-126">Идентифицирует ролей сервера, необходимых в порядке для абонентов для запроса.</span><span class="sxs-lookup"><span data-stu-id="e1478-126">Identifies the server roles that are necessary in order for the caller to make the request.</span></span> <span data-ttu-id="e1478-127">Этот заголовок можно применять к запросу.</span><span class="sxs-lookup"><span data-stu-id="e1478-127">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="e1478-128">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="e1478-128">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="e1478-129">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="e1478-129">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="e1478-130">Определяет версию схемы для операции запроса.</span><span class="sxs-lookup"><span data-stu-id="e1478-130">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="e1478-131">Этот заголовок можно применять к запросу.</span><span class="sxs-lookup"><span data-stu-id="e1478-131">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="e1478-132">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="e1478-132">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="e1478-133">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="e1478-133">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="e1478-134">Определяет версию сервера, ответившего на запрос.</span><span class="sxs-lookup"><span data-stu-id="e1478-134">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="e1478-135">Этот заголовок можно применять, чтобы получить ответ.</span><span class="sxs-lookup"><span data-stu-id="e1478-135">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="getdiscoverysearchconfiguration-operation-request-example-get-the-discovery-search-configuration-for-a-saved-search"></a><span data-ttu-id="e1478-136">Пример запроса GetDiscoverySearchConfiguration операции: получение конфигурации поиска обнаружения для сохраненного поиска</span><span class="sxs-lookup"><span data-stu-id="e1478-136">GetDiscoverySearchConfiguration operation request example: Get the discovery search configuration for a saved search</span></span>

<span data-ttu-id="e1478-137">В следующем примере запрос операции **GetDiscoverySearchConfiguration** показано, как запросить конфигурации сохраненный поисковый называется «MyDiscSearchFor sbrown».</span><span class="sxs-lookup"><span data-stu-id="e1478-137">The following example of a **GetDiscoverySearchConfiguration** operation request shows how to request the configuration of a saved search called "MyDiscSearchFor-sbrown".</span></span> <span data-ttu-id="e1478-138">Аргументы для [ExpandGroupMembership](expandgroupmembership.md) и [InPlaceHoldConfigurationOnly](inplaceholdconfigurationonly.md) элементы игнорируются.</span><span class="sxs-lookup"><span data-stu-id="e1478-138">The arguments for the [ExpandGroupMembership](expandgroupmembership.md) and [InPlaceHoldConfigurationOnly](inplaceholdconfigurationonly.md) elements are ignored.</span></span> 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013" />
   </soap:Header>
   <soap:Body >
      <m:GetDiscoverySearchConfiguration>
         <m:SearchId>MyDiscSearchFor-sbrown</m:SearchId>
         <m:ExpandGroupMembership>true</m:ExpandGroupMembership>
         <m:InPlaceHoldConfigurationOnly>false</m:InPlaceHoldConfigurationOnly>
      </m:GetDiscoverySearchConfiguration>
   </soap:Body>
</soap:Envelope>

```

<span data-ttu-id="e1478-139">Запрос SOAP body содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="e1478-139">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="e1478-140">GetDiscoverySearchConfiguration</span><span class="sxs-lookup"><span data-stu-id="e1478-140">GetDiscoverySearchConfiguration</span></span>](getdiscoverysearchconfiguration.md)
    
- [<span data-ttu-id="e1478-141">SearchId</span><span class="sxs-lookup"><span data-stu-id="e1478-141">SearchId</span></span>](searchid.md)
    
- [<span data-ttu-id="e1478-142">ExpandGroupMembership</span><span class="sxs-lookup"><span data-stu-id="e1478-142">ExpandGroupMembership</span></span>](expandgroupmembership.md)
    
- [<span data-ttu-id="e1478-143">InPlaceHoldConfigurationOnly</span><span class="sxs-lookup"><span data-stu-id="e1478-143">InPlaceHoldConfigurationOnly</span></span>](inplaceholdconfigurationonly.md)
    
## <a name="successful-getdiscoverysearchconfiguration-operation-response-request-for-a-single-saved-search"></a><span data-ttu-id="e1478-144">Успешные операции ответа GetDiscoverySearchConfiguration: для одного сохраненный поисковый запрос</span><span class="sxs-lookup"><span data-stu-id="e1478-144">Successful GetDiscoverySearchConfiguration operation response: Request for a single saved search</span></span>

<span data-ttu-id="e1478-145">В следующем примере показано успешного ответа на запрос операции **GetDiscoverySearchConfiguration** для получения конфигурации сохраненный поисковый называется «MyDiscSearchFor sbrown».</span><span class="sxs-lookup"><span data-stu-id="e1478-145">The following example shows a successful response to a **GetDiscoverySearchConfiguration** operation request to get the configuration of a saved search called "MyDiscSearchFor-sbrown".</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="526" MinorBuildNumber="0" Version="Exchange2013" xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" xmlns="http://schemas.microsoft.com/exchange/services/2006/types" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <GetDiscoverySearchConfigurationResponse ResponseClass="Success" xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseCode>NoError</ResponseCode>
      <DiscoverySearchConfigurations>
        <DiscoverySearchConfiguration xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
          <SearchId>MyDiscSearchFor-sbrown</SearchId>
          <SearchQuery>test item</SearchQuery>
          <SearchableMailboxes>
            <SearchableMailbox>
              <Guid>3c620d04-8b22-432e-92be-5b9321599576</Guid>
              <PrimarySmtpAddress>SBrown@contoso.com</PrimarySmtpAddress>
              <IsExternalMailbox>false</IsExternalMailbox>
              <ExternalEmailAddress/>
              <DisplayName>Steven Brown</DisplayName>
              <IsMembershipGroup>false</IsMembershipGroup>
              <ReferenceId>/o=First/ou=Exchange(FYDILT)/cn=Recipients/cn=313ecf-Steve</ReferenceId>
            </SearchableMailbox>
          </SearchableMailboxes>
        </DiscoverySearchConfiguration>
      </DiscoverySearchConfigurations>
    </GetDiscoverySearchConfigurationResponse>
  </s:Body>
</s:Envelope>
```

<span data-ttu-id="e1478-146">Ответ SOAP body содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="e1478-146">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="e1478-147">GetDiscoverySearchConfigurationResponse</span><span class="sxs-lookup"><span data-stu-id="e1478-147">GetDiscoverySearchConfigurationResponse</span></span>](getdiscoverysearchconfigurationresponse.md)
    
- [<span data-ttu-id="e1478-148">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="e1478-148">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="e1478-149">DiscoverySearchConfigurations</span><span class="sxs-lookup"><span data-stu-id="e1478-149">DiscoverySearchConfigurations</span></span>](discoverysearchconfigurations.md)
    
- [<span data-ttu-id="e1478-150">DiscoverySearchConfiguration</span><span class="sxs-lookup"><span data-stu-id="e1478-150">DiscoverySearchConfiguration</span></span>](discoverysearchconfiguration.md)
    
- [<span data-ttu-id="e1478-151">SearchId</span><span class="sxs-lookup"><span data-stu-id="e1478-151">SearchId</span></span>](searchid.md)
    
- [<span data-ttu-id="e1478-152">SearchQuery</span><span class="sxs-lookup"><span data-stu-id="e1478-152">SearchQuery</span></span>](searchquery.md)
    
- [<span data-ttu-id="e1478-153">SearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="e1478-153">SearchableMailboxes</span></span>](searchablemailboxes.md)
    
- [<span data-ttu-id="e1478-154">SearchableMailbox</span><span class="sxs-lookup"><span data-stu-id="e1478-154">SearchableMailbox</span></span>](searchablemailbox.md)
    
- [<span data-ttu-id="e1478-155">Guid</span><span class="sxs-lookup"><span data-stu-id="e1478-155">Guid</span></span>](guid-ex15websvcsotherref.md)
    
- [<span data-ttu-id="e1478-156">Параметр PrimarySmtpAddress (строка)</span><span class="sxs-lookup"><span data-stu-id="e1478-156">PrimarySmtpAddress (string)</span></span>](primarysmtpaddress-string.md)
    
- [<span data-ttu-id="e1478-157">IsExternalMailbox</span><span class="sxs-lookup"><span data-stu-id="e1478-157">IsExternalMailbox</span></span>](isexternalmailbox.md)
    
- [<span data-ttu-id="e1478-158">ExternalEmailAddress</span><span class="sxs-lookup"><span data-stu-id="e1478-158">ExternalEmailAddress</span></span>](externalemailaddress.md)
    
- [<span data-ttu-id="e1478-159">Отображаемое имя (строка)</span><span class="sxs-lookup"><span data-stu-id="e1478-159">DisplayName (string)</span></span>](displayname-string.md)
    
- [<span data-ttu-id="e1478-160">IsMembershipGroup</span><span class="sxs-lookup"><span data-stu-id="e1478-160">IsMembershipGroup</span></span>](ismembershipgroup.md)
    
- [<span data-ttu-id="e1478-161">ReferenceId</span><span class="sxs-lookup"><span data-stu-id="e1478-161">ReferenceId</span></span>](referenceid.md)
    
## <a name="successful-getdiscoverysearchconfiguration-operation-response-request-for-in-place-holds"></a><span data-ttu-id="e1478-162">Успешные операции ответа GetDiscoverySearchConfiguration: запрос на удержание на месте</span><span class="sxs-lookup"><span data-stu-id="e1478-162">Successful GetDiscoverySearchConfiguration operation response: Request for in-place holds</span></span>

<span data-ttu-id="e1478-163">В следующем примере показано, что содержит успешного ответа на запрос операции **GetDiscoverySearchConfiguration** , чтобы получить только на месте.</span><span class="sxs-lookup"><span data-stu-id="e1478-163">The following example shows a successful response to a **GetDiscoverySearchConfiguration** operation request to only get in-place holds.</span></span> 
  
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
      <GetDiscoverySearchConfigurationResponse ResponseClass="Success" 
                                               xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
         <DiscoverySearchConfigurations>
            <DiscoverySearchConfiguration xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
               <SearchId>MyDiscSearchFor-sbrown</SearchId>
               <SearchQuery>test item</SearchQuery>
               <InPlaceHoldIdentity>3f37d90f53144558a80814ef0272749a9</InPlaceHoldIdentity>
               <ManagedByOrganization/>
            </DiscoverySearchConfiguration>
            <DiscoverySearchConfiguration xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
               <SearchId>MyDiscSearch</SearchId>
               <SearchQuery>test</SearchQuery>
               <InPlaceHoldIdentity>6ea486f0f3f140efb044682a2e782abdf</InPlaceHoldIdentity>
               <ManagedByOrganization/>
            </DiscoverySearchConfiguration>
         </DiscoverySearchConfigurations>
      </GetDiscoverySearchConfigurationResponse>
   </s:Body>
</s:Envelope>

```

<span data-ttu-id="e1478-164">Ответ SOAP body содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="e1478-164">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="e1478-165">GetDiscoverySearchConfigurationResponse</span><span class="sxs-lookup"><span data-stu-id="e1478-165">GetDiscoverySearchConfigurationResponse</span></span>](getdiscoverysearchconfigurationresponse.md)
    
- [<span data-ttu-id="e1478-166">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="e1478-166">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="e1478-167">DiscoverySearchConfigurations</span><span class="sxs-lookup"><span data-stu-id="e1478-167">DiscoverySearchConfigurations</span></span>](discoverysearchconfigurations.md)
    
- [<span data-ttu-id="e1478-168">DiscoverySearchConfiguration</span><span class="sxs-lookup"><span data-stu-id="e1478-168">DiscoverySearchConfiguration</span></span>](discoverysearchconfiguration.md)
    
- [<span data-ttu-id="e1478-169">SearchId</span><span class="sxs-lookup"><span data-stu-id="e1478-169">SearchId</span></span>](searchid.md)
    
- [<span data-ttu-id="e1478-170">SearchQuery</span><span class="sxs-lookup"><span data-stu-id="e1478-170">SearchQuery</span></span>](searchquery.md)
    
- [<span data-ttu-id="e1478-171">InPlaceHoldIdentity</span><span class="sxs-lookup"><span data-stu-id="e1478-171">InPlaceHoldIdentity</span></span>](inplaceholdidentity.md)
    
- [<span data-ttu-id="e1478-172">ManagedByOrganization</span><span class="sxs-lookup"><span data-stu-id="e1478-172">ManagedByOrganization</span></span>](managedbyorganization.md)
    
## <a name="successful-getdiscoverysearchconfiguration-operation-response-request-for-all-saved-discovery-search-configurations"></a><span data-ttu-id="e1478-173">Успешные операции ответа GetDiscoverySearchConfiguration: запрос на все сохраненные обнаружения конфигурации поиска</span><span class="sxs-lookup"><span data-stu-id="e1478-173">Successful GetDiscoverySearchConfiguration operation response: Request for all saved discovery search configurations</span></span>

<span data-ttu-id="e1478-174">В следующем примере показано успешного ответа на запрос операции **GetDiscoverySearchConfiguration** для получения всех поисков сохраненного обнаружения.</span><span class="sxs-lookup"><span data-stu-id="e1478-174">The following example shows a successful response to a **GetDiscoverySearchConfiguration** operation request to get all saved discovery searches.</span></span> 
  
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
      <GetDiscoverySearchConfigurationResponse ResponseClass="Success" 
                                               xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
         <DiscoverySearchConfigurations>
            <DiscoverySearchConfiguration xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
               <SearchId>MyDiscSearchFor-sbrown</SearchId>
               <SearchQuery>test item</SearchQuery>
               <SearchableMailboxes>
                  <SearchableMailbox>
                     <Guid>3c620d04-8b33-435e-95be-5b9351599576</Guid>
                     <PrimarySmtpAddress>SBrown@contoso.com</PrimarySmtpAddress>
                     <IsExternalMailbox>false</IsExternalMailbox>
                     <ExternalEmailAddress/>
                     <DisplayName>Steven Brown</DisplayName>
                     <IsMembershipGroup>false</IsMembershipGroup>
                     <ReferenceId>/o=First/ou=Exchange (FYLT)/cn=Recipients/cn=35381a742f0e47e395c8601a60d13ecz-Steve</ReferenceId>
                  </SearchableMailbox>
               </SearchableMailboxes>
            </DiscoverySearchConfiguration>
            <DiscoverySearchConfiguration xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
               <SearchId>MyDiscSearch</SearchId>
               <SearchQuery>test</SearchQuery>
               <SearchableMailboxes>
                  <SearchableMailbox>
                     <Guid>e788c4b0-54a2-458c-83b2-22d5bb02b23f</Guid>
                     <PrimarySmtpAddress>Administrator@contoso.com</PrimarySmtpAddress>
                     <IsExternalMailbox>false</IsExternalMailbox>
                     <ExternalEmailAddress/>
                     <DisplayName>Administrator</DisplayName>
                     <IsMembershipGroup>false</IsMembershipGroup>
                     <ReferenceId>/o=First/ou=Exchange (FYLT)/cn=Recipients/cn=ebez7871332d4595abe1c62962911a58-Admin</ReferenceId>
                  </SearchableMailbox>
                  <SearchableMailbox>
                     <Guid>6f6cff39-8967-4a60-b43f-328413c25199</Guid>
                     <PrimarySmtpAddress>ADavis@contoso.com</PrimarySmtpAddress>
                     <IsExternalMailbox>false</IsExternalMailbox>
                     <ExternalEmailAddress/>
                     <DisplayName>Anthony Davis</DisplayName>
                     <IsMembershipGroup>false</IsMembershipGroup>
                     <ReferenceId>/o=First/ou=Exchange (FYLT)/cn=Recipients/cn=f10c9f70519844beb04101d8f40c572z-Antho</ReferenceId>
                  </SearchableMailbox>
               </SearchableMailboxes>
            </DiscoverySearchConfiguration>
         </DiscoverySearchConfigurations>
      </GetDiscoverySearchConfigurationResponse>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="e1478-175">Ответ SOAP body содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="e1478-175">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="e1478-176">GetDiscoverySearchConfigurationResponse</span><span class="sxs-lookup"><span data-stu-id="e1478-176">GetDiscoverySearchConfigurationResponse</span></span>](getdiscoverysearchconfigurationresponse.md)
    
- [<span data-ttu-id="e1478-177">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="e1478-177">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="e1478-178">DiscoverySearchConfigurations</span><span class="sxs-lookup"><span data-stu-id="e1478-178">DiscoverySearchConfigurations</span></span>](discoverysearchconfigurations.md)
    
- [<span data-ttu-id="e1478-179">DiscoverySearchConfiguration</span><span class="sxs-lookup"><span data-stu-id="e1478-179">DiscoverySearchConfiguration</span></span>](discoverysearchconfiguration.md)
    
- [<span data-ttu-id="e1478-180">SearchId</span><span class="sxs-lookup"><span data-stu-id="e1478-180">SearchId</span></span>](searchid.md)
    
- [<span data-ttu-id="e1478-181">SearchQuery</span><span class="sxs-lookup"><span data-stu-id="e1478-181">SearchQuery</span></span>](searchquery.md)
    
- [<span data-ttu-id="e1478-182">SearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="e1478-182">SearchableMailboxes</span></span>](searchablemailboxes.md)
    
- [<span data-ttu-id="e1478-183">SearchableMailbox</span><span class="sxs-lookup"><span data-stu-id="e1478-183">SearchableMailbox</span></span>](searchablemailbox.md)
    
- [<span data-ttu-id="e1478-184">Guid</span><span class="sxs-lookup"><span data-stu-id="e1478-184">Guid</span></span>](guid-ex15websvcsotherref.md)
    
- [<span data-ttu-id="e1478-185">Параметр PrimarySmtpAddress (строка)</span><span class="sxs-lookup"><span data-stu-id="e1478-185">PrimarySmtpAddress (string)</span></span>](primarysmtpaddress-string.md)
    
- [<span data-ttu-id="e1478-186">IsExternalMailbox</span><span class="sxs-lookup"><span data-stu-id="e1478-186">IsExternalMailbox</span></span>](isexternalmailbox.md)
    
- [<span data-ttu-id="e1478-187">ExternalEmailAddress</span><span class="sxs-lookup"><span data-stu-id="e1478-187">ExternalEmailAddress</span></span>](externalemailaddress.md)
    
- [<span data-ttu-id="e1478-188">Отображаемое имя (строка)</span><span class="sxs-lookup"><span data-stu-id="e1478-188">DisplayName (string)</span></span>](displayname-string.md)
    
- [<span data-ttu-id="e1478-189">IsMembershipGroup</span><span class="sxs-lookup"><span data-stu-id="e1478-189">IsMembershipGroup</span></span>](ismembershipgroup.md)
    
- [<span data-ttu-id="e1478-190">ReferenceId</span><span class="sxs-lookup"><span data-stu-id="e1478-190">ReferenceId</span></span>](referenceid.md)
    
## <a name="getdiscoverysearchconfiguration-operation-error-response"></a><span data-ttu-id="e1478-191">Ошибка операции GetDiscoverySearchConfiguration ответа</span><span class="sxs-lookup"><span data-stu-id="e1478-191">GetDiscoverySearchConfiguration operation error response</span></span>

<span data-ttu-id="e1478-192">В следующем примере показано ошибочный ответ на запрос операции **GetDiscoverySearchConfiguration** .</span><span class="sxs-lookup"><span data-stu-id="e1478-192">The following example shows an error response to a **GetDiscoverySearchConfiguration** operation request.</span></span> <span data-ttu-id="e1478-193">Это ответ на запрос для получения поиска не найден на сервере.</span><span class="sxs-lookup"><span data-stu-id="e1478-193">This is a response to a request to get a saved search that is not found on the server.</span></span> 
  
```XML
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
      <GetDiscoverySearchConfigurationResponse ResponseClass="Error" 
                                               xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>Search configuration corresponding to the search id was not found.</MessageText>
         <ResponseCode>ErrorInvalidArgument</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
         <DiscoverySearchConfigurations/>
      </GetDiscoverySearchConfigurationResponse>
   </s:Body>
</s:Envelope>

```

<span data-ttu-id="e1478-194">Ошибка ответ SOAP body содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="e1478-194">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="e1478-195">GetDiscoverySearchConfigurationResponse</span><span class="sxs-lookup"><span data-stu-id="e1478-195">GetDiscoverySearchConfigurationResponse</span></span>](getdiscoverysearchconfigurationresponse.md)
    
- [<span data-ttu-id="e1478-196">MessageText</span><span class="sxs-lookup"><span data-stu-id="e1478-196">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="e1478-197">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="e1478-197">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="e1478-198">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="e1478-198">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
- [<span data-ttu-id="e1478-199">DiscoverySearchConfigurations</span><span class="sxs-lookup"><span data-stu-id="e1478-199">DiscoverySearchConfigurations</span></span>](discoverysearchconfigurations.md)
    
<span data-ttu-id="e1478-200">Дополнительные коды ошибок, которые являются общими для веб-служб Exchange и специально для этой операции в разделе [ResponseCode](responsecode.md).</span><span class="sxs-lookup"><span data-stu-id="e1478-200">For additional error codes that are generic to EWS and specific to this operation, see [ResponseCode](responsecode.md).</span></span>
  
## <a name="see-also"></a><span data-ttu-id="e1478-201">См. также</span><span class="sxs-lookup"><span data-stu-id="e1478-201">See also</span></span>

- [<span data-ttu-id="e1478-202">Операции EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="e1478-202">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
    
- [<span data-ttu-id="e1478-203">GetSearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="e1478-203">GetSearchableMailboxes</span></span>](getsearchablemailboxes.md)
    
- [<span data-ttu-id="e1478-204">SearchMailboxes</span><span class="sxs-lookup"><span data-stu-id="e1478-204">SearchMailboxes</span></span>](searchmailboxes.md)
    
- [<span data-ttu-id="e1478-205">GetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="e1478-205">GetHoldOnMailboxes</span></span>](getholdonmailboxes.md)
    
- [<span data-ttu-id="e1478-206">SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="e1478-206">SetHoldOnMailboxes</span></span>](setholdonmailboxes.md)
    
- [<span data-ttu-id="e1478-207">GetNonIndexableItemDetails</span><span class="sxs-lookup"><span data-stu-id="e1478-207">GetNonIndexableItemDetails</span></span>](getnonindexableitemdetails.md)
    
- [<span data-ttu-id="e1478-208">GetNonIndexableItemStatistics</span><span class="sxs-lookup"><span data-stu-id="e1478-208">GetNonIndexableItemStatistics</span></span>](getnonindexableitemstatistics.md)
    

