---
title: Операция GetDiscoverySearchConfiguration
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 8a54a6dc-110c-4972-a8bc-5ddb43c4b857
description: Поиск сведений о GetDiscoverySearchConfigurationной операции EWS.
ms.openlocfilehash: 4db435988a9954b921e7851986b6f92ffedbad94
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44461025"
---
# <a name="getdiscoverysearchconfiguration-operation"></a><span data-ttu-id="266b4-103">Операция GetDiscoverySearchConfiguration</span><span class="sxs-lookup"><span data-stu-id="266b4-103">GetDiscoverySearchConfiguration operation</span></span>

<span data-ttu-id="266b4-104">Поиск сведений о **GetDiscoverySearchConfigurationной** операции EWS.</span><span class="sxs-lookup"><span data-stu-id="266b4-104">Find information about the **GetDiscoverySearchConfiguration** EWS operation.</span></span> 
  
<span data-ttu-id="266b4-105">Операция **GetDiscoverySearchConfiguration** возвращает сведения о конфигурации для удержаний на месте, сохраненных поисков и почтовых ящиков, которые включены для поиска обнаружения.</span><span class="sxs-lookup"><span data-stu-id="266b4-105">The **GetDiscoverySearchConfiguration** operation returns configuration information for in-place holds, saved discovery searches, and the mailboxes that are enabled for discovery search.</span></span> 
  
<span data-ttu-id="266b4-106">Эта операция появилась в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="266b4-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-getdiscoverysearchconfiguration-operation"></a><span data-ttu-id="266b4-107">Использование операции GetDiscoverySearchConfiguration</span><span class="sxs-lookup"><span data-stu-id="266b4-107">Using the GetDiscoverySearchConfiguration operation</span></span>

<span data-ttu-id="266b4-108">Операция **GetDiscoverySearchConfiguration** предоставляет сведения о конфигурации для поиска при обнаружении.</span><span class="sxs-lookup"><span data-stu-id="266b4-108">The **GetDiscoverySearchConfiguration** operation provides configuration information for discovery search.</span></span> <span data-ttu-id="266b4-109">Запросы могут содержать один или несколько из следующих аргументов:</span><span class="sxs-lookup"><span data-stu-id="266b4-109">Requests can contain one or more of the following arguments:</span></span> 
  
1. <span data-ttu-id="266b4-110">[Сеарчид](searchid.md) — определяет сохраненный поисковый запрос на обнаружение.</span><span class="sxs-lookup"><span data-stu-id="266b4-110">[SearchId](searchid.md) — Identifies a saved discovery search.</span></span> <span data-ttu-id="266b4-111">Если этот аргумент отправляется в запросе, значения других аргументов игнорируются.</span><span class="sxs-lookup"><span data-stu-id="266b4-111">If this argument is sent in the request, the values of the other arguments are ignored.</span></span> 
    
2. <span data-ttu-id="266b4-112">[Експандграупмембершип](expandgroupmembership.md) — указывает, развернут ли в ответе членство в группе.</span><span class="sxs-lookup"><span data-stu-id="266b4-112">[ExpandGroupMembership](expandgroupmembership.md) — Indicates whether group membership is expanded in the response.</span></span> <span data-ttu-id="266b4-113">Значение **true** указывает, что членство в группе развернуто, и в ответе возвращаются все доступные для поиска почтовые ящики.</span><span class="sxs-lookup"><span data-stu-id="266b4-113">A value of **true** indicates that group membership is expanded so that all searchable mailboxes are returned in the response.</span></span> <span data-ttu-id="266b4-114">Значение **false** указывает, что в ответе возвращается только группа.</span><span class="sxs-lookup"><span data-stu-id="266b4-114">A value of **false** indicates that only the group is returned in the response.</span></span> 
    
3. <span data-ttu-id="266b4-115">[Инплацехолдконфигуратиононли](inplaceholdconfigurationonly.md) — указывает, возвращаются ли все доступные для поиска почтовые ящики в дополнение к конфигурации хранения на месте.</span><span class="sxs-lookup"><span data-stu-id="266b4-115">[InPlaceHoldConfigurationOnly](inplaceholdconfigurationonly.md) — Indicates whether all searchable mailboxes are returned in addition to the in-place hold configuration.</span></span> <span data-ttu-id="266b4-116">Значение **true** указывает, что возвращаются только конфигурации хранения на месте.</span><span class="sxs-lookup"><span data-stu-id="266b4-116">A value of **true** indicates that only the in-place hold configurations are returned.</span></span> <span data-ttu-id="266b4-117">Значение **false** указывает, что все идентификаторы почтовых ящиков, доступные для поиска, возвращаются в дополнение к идентификаторам хранения на месте.</span><span class="sxs-lookup"><span data-stu-id="266b4-117">A value of **false** indicates that all searchable mailbox identifiers are returned in addition to the in-place hold identifiers.</span></span> <span data-ttu-id="266b4-118">Если этот элемент отсутствует, то поведением по умолчанию является эквивалент значения **false**.</span><span class="sxs-lookup"><span data-stu-id="266b4-118">If this element is not present, the default behavior is the equivalent of the value **false**.</span></span> 
    
### <a name="getdiscoverysearchconfiguration-operation-soap-headers"></a><span data-ttu-id="266b4-119">Заголовки SOAP операции GetDiscoverySearchConfiguration</span><span class="sxs-lookup"><span data-stu-id="266b4-119">GetDiscoverySearchConfiguration operation SOAP headers</span></span>

<span data-ttu-id="266b4-120">Операция **GetDiscoverySearchConfiguration** может использовать заголовки SOAP, указанные в приведенной ниже таблице.</span><span class="sxs-lookup"><span data-stu-id="266b4-120">The **GetDiscoverySearchConfiguration** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="266b4-121">**Имя заголовка**</span><span class="sxs-lookup"><span data-stu-id="266b4-121">**Header name**</span></span>|<span data-ttu-id="266b4-122">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="266b4-122">**Element**</span></span>|<span data-ttu-id="266b4-123">**Описание**</span><span class="sxs-lookup"><span data-stu-id="266b4-123">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="266b4-124">**ManagementRole**</span><span class="sxs-lookup"><span data-stu-id="266b4-124">**ManagementRole**</span></span> <br/> |[<span data-ttu-id="266b4-125">ManagementRole</span><span class="sxs-lookup"><span data-stu-id="266b4-125">ManagementRole</span></span>](managementrole.md) <br/> |<span data-ttu-id="266b4-126">Определяет роли сервера, необходимые для того, чтобы вызывающий абонент мог выполнить запрос.</span><span class="sxs-lookup"><span data-stu-id="266b4-126">Identifies the server roles that are necessary in order for the caller to make the request.</span></span> <span data-ttu-id="266b4-127">Этот заголовок является применимым для запроса.</span><span class="sxs-lookup"><span data-stu-id="266b4-127">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="266b4-128">**рекуестверсион**</span><span class="sxs-lookup"><span data-stu-id="266b4-128">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="266b4-129">рекуестсерверверсион</span><span class="sxs-lookup"><span data-stu-id="266b4-129">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="266b4-130">Определяет версию схемы для запроса операции.</span><span class="sxs-lookup"><span data-stu-id="266b4-130">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="266b4-131">Этот заголовок является применимым для запроса.</span><span class="sxs-lookup"><span data-stu-id="266b4-131">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="266b4-132">**серверверсион**</span><span class="sxs-lookup"><span data-stu-id="266b4-132">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="266b4-133">серверверсионинфо</span><span class="sxs-lookup"><span data-stu-id="266b4-133">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="266b4-134">Определяет версию сервера, который ответил на запрос.</span><span class="sxs-lookup"><span data-stu-id="266b4-134">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="266b4-135">Этот заголовок является применимым для отклика.</span><span class="sxs-lookup"><span data-stu-id="266b4-135">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="getdiscoverysearchconfiguration-operation-request-example-get-the-discovery-search-configuration-for-a-saved-search"></a><span data-ttu-id="266b4-136">Пример запроса операции GetDiscoverySearchConfiguration: получение конфигурации поиска при обнаружении для сохраненного поиска</span><span class="sxs-lookup"><span data-stu-id="266b4-136">GetDiscoverySearchConfiguration operation request example: Get the discovery search configuration for a saved search</span></span>

<span data-ttu-id="266b4-137">В следующем примере запроса операции **GetDiscoverySearchConfiguration** показано, как запросить конфигурацию сохраненного поиска с именем "мидисксеарчфор — сбровн".</span><span class="sxs-lookup"><span data-stu-id="266b4-137">The following example of a **GetDiscoverySearchConfiguration** operation request shows how to request the configuration of a saved search called "MyDiscSearchFor-sbrown".</span></span> <span data-ttu-id="266b4-138">Аргументы для элементов [експандграупмембершип](expandgroupmembership.md) и [инплацехолдконфигуратиононли](inplaceholdconfigurationonly.md) игнорируются.</span><span class="sxs-lookup"><span data-stu-id="266b4-138">The arguments for the [ExpandGroupMembership](expandgroupmembership.md) and [InPlaceHoldConfigurationOnly](inplaceholdconfigurationonly.md) elements are ignored.</span></span> 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
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

<span data-ttu-id="266b4-139">Текст SOAP Request содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="266b4-139">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="266b4-140">GetDiscoverySearchConfiguration</span><span class="sxs-lookup"><span data-stu-id="266b4-140">GetDiscoverySearchConfiguration</span></span>](getdiscoverysearchconfiguration.md)
    
- [<span data-ttu-id="266b4-141">сеарчид</span><span class="sxs-lookup"><span data-stu-id="266b4-141">SearchId</span></span>](searchid.md)
    
- [<span data-ttu-id="266b4-142">експандграупмембершип</span><span class="sxs-lookup"><span data-stu-id="266b4-142">ExpandGroupMembership</span></span>](expandgroupmembership.md)
    
- [<span data-ttu-id="266b4-143">инплацехолдконфигуратиононли</span><span class="sxs-lookup"><span data-stu-id="266b4-143">InPlaceHoldConfigurationOnly</span></span>](inplaceholdconfigurationonly.md)
    
## <a name="successful-getdiscoverysearchconfiguration-operation-response-request-for-a-single-saved-search"></a><span data-ttu-id="266b4-144">Успешный отклик операции GetDiscoverySearchConfiguration: запрос на один сохраненный поиск</span><span class="sxs-lookup"><span data-stu-id="266b4-144">Successful GetDiscoverySearchConfiguration operation response: Request for a single saved search</span></span>

<span data-ttu-id="266b4-145">В следующем примере показан успешный ответ на запрос операции **GetDiscoverySearchConfiguration** для получения конфигурации сохраненного поиска с именем "мидисксеарчфор — сбровн".</span><span class="sxs-lookup"><span data-stu-id="266b4-145">The following example shows a successful response to a **GetDiscoverySearchConfiguration** operation request to get the configuration of a saved search called "MyDiscSearchFor-sbrown".</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="526" MinorBuildNumber="0" Version="Exchange2013" xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" xmlns="https://schemas.microsoft.com/exchange/services/2006/types" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <GetDiscoverySearchConfigurationResponse ResponseClass="Success" xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseCode>NoError</ResponseCode>
      <DiscoverySearchConfigurations>
        <DiscoverySearchConfiguration xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
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

<span data-ttu-id="266b4-146">Тело SOAP отклика содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="266b4-146">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="266b4-147">жетдисковерисеарчконфигуратионреспонсе</span><span class="sxs-lookup"><span data-stu-id="266b4-147">GetDiscoverySearchConfigurationResponse</span></span>](getdiscoverysearchconfigurationresponse.md)
    
- [<span data-ttu-id="266b4-148">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="266b4-148">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="266b4-149">дисковерисеарчконфигуратионс</span><span class="sxs-lookup"><span data-stu-id="266b4-149">DiscoverySearchConfigurations</span></span>](discoverysearchconfigurations.md)
    
- [<span data-ttu-id="266b4-150">дисковерисеарчконфигуратион</span><span class="sxs-lookup"><span data-stu-id="266b4-150">DiscoverySearchConfiguration</span></span>](discoverysearchconfiguration.md)
    
- [<span data-ttu-id="266b4-151">сеарчид</span><span class="sxs-lookup"><span data-stu-id="266b4-151">SearchId</span></span>](searchid.md)
    
- [<span data-ttu-id="266b4-152">SearchQuery</span><span class="sxs-lookup"><span data-stu-id="266b4-152">SearchQuery</span></span>](searchquery.md)
    
- [<span data-ttu-id="266b4-153">сеарчаблемаилбоксес</span><span class="sxs-lookup"><span data-stu-id="266b4-153">SearchableMailboxes</span></span>](searchablemailboxes.md)
    
- [<span data-ttu-id="266b4-154">сеарчаблемаилбокс</span><span class="sxs-lookup"><span data-stu-id="266b4-154">SearchableMailbox</span></span>](searchablemailbox.md)
    
- [<span data-ttu-id="266b4-155">Guid</span><span class="sxs-lookup"><span data-stu-id="266b4-155">Guid</span></span>](guid-ex15websvcsotherref.md)
    
- [<span data-ttu-id="266b4-156">PrimarySmtpAddress (строка)</span><span class="sxs-lookup"><span data-stu-id="266b4-156">PrimarySmtpAddress (string)</span></span>](primarysmtpaddress-string.md)
    
- [<span data-ttu-id="266b4-157">исекстерналмаилбокс</span><span class="sxs-lookup"><span data-stu-id="266b4-157">IsExternalMailbox</span></span>](isexternalmailbox.md)
    
- [<span data-ttu-id="266b4-158">ExternalEmailAddress</span><span class="sxs-lookup"><span data-stu-id="266b4-158">ExternalEmailAddress</span></span>](externalemailaddress.md)
    
- [<span data-ttu-id="266b4-159">DisplayName (строка)</span><span class="sxs-lookup"><span data-stu-id="266b4-159">DisplayName (string)</span></span>](displayname-string.md)
    
- [<span data-ttu-id="266b4-160">исмембершипграуп</span><span class="sxs-lookup"><span data-stu-id="266b4-160">IsMembershipGroup</span></span>](ismembershipgroup.md)
    
- [<span data-ttu-id="266b4-161">ReferenceId</span><span class="sxs-lookup"><span data-stu-id="266b4-161">ReferenceId</span></span>](referenceid.md)
    
## <a name="successful-getdiscoverysearchconfiguration-operation-response-request-for-in-place-holds"></a><span data-ttu-id="266b4-162">Успешный отклик операции GetDiscoverySearchConfiguration: запрос удержания на месте</span><span class="sxs-lookup"><span data-stu-id="266b4-162">Successful GetDiscoverySearchConfiguration operation response: Request for in-place holds</span></span>

<span data-ttu-id="266b4-163">В следующем примере показан успешный ответ на запрос операции **GetDiscoverySearchConfiguration** для получения только удержаний на месте.</span><span class="sxs-lookup"><span data-stu-id="266b4-163">The following example shows a successful response to a **GetDiscoverySearchConfiguration** operation request to only get in-place holds.</span></span> 
  
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
      <GetDiscoverySearchConfigurationResponse ResponseClass="Success" 
                                               xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
         <DiscoverySearchConfigurations>
            <DiscoverySearchConfiguration xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
               <SearchId>MyDiscSearchFor-sbrown</SearchId>
               <SearchQuery>test item</SearchQuery>
               <InPlaceHoldIdentity>3f37d90f53144558a80814ef0272749a9</InPlaceHoldIdentity>
               <ManagedByOrganization/>
            </DiscoverySearchConfiguration>
            <DiscoverySearchConfiguration xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
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

<span data-ttu-id="266b4-164">Тело SOAP отклика содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="266b4-164">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="266b4-165">жетдисковерисеарчконфигуратионреспонсе</span><span class="sxs-lookup"><span data-stu-id="266b4-165">GetDiscoverySearchConfigurationResponse</span></span>](getdiscoverysearchconfigurationresponse.md)
    
- [<span data-ttu-id="266b4-166">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="266b4-166">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="266b4-167">дисковерисеарчконфигуратионс</span><span class="sxs-lookup"><span data-stu-id="266b4-167">DiscoverySearchConfigurations</span></span>](discoverysearchconfigurations.md)
    
- [<span data-ttu-id="266b4-168">дисковерисеарчконфигуратион</span><span class="sxs-lookup"><span data-stu-id="266b4-168">DiscoverySearchConfiguration</span></span>](discoverysearchconfiguration.md)
    
- [<span data-ttu-id="266b4-169">сеарчид</span><span class="sxs-lookup"><span data-stu-id="266b4-169">SearchId</span></span>](searchid.md)
    
- [<span data-ttu-id="266b4-170">SearchQuery</span><span class="sxs-lookup"><span data-stu-id="266b4-170">SearchQuery</span></span>](searchquery.md)
    
- [<span data-ttu-id="266b4-171">InPlaceHoldIdentity</span><span class="sxs-lookup"><span data-stu-id="266b4-171">InPlaceHoldIdentity</span></span>](inplaceholdidentity.md)
    
- [<span data-ttu-id="266b4-172">манажедбйорганизатион</span><span class="sxs-lookup"><span data-stu-id="266b4-172">ManagedByOrganization</span></span>](managedbyorganization.md)
    
## <a name="successful-getdiscoverysearchconfiguration-operation-response-request-for-all-saved-discovery-search-configurations"></a><span data-ttu-id="266b4-173">Успешный отклик операции GetDiscoverySearchConfiguration: запрос для всех сохраненных конфигураций поиска для обнаружения</span><span class="sxs-lookup"><span data-stu-id="266b4-173">Successful GetDiscoverySearchConfiguration operation response: Request for all saved discovery search configurations</span></span>

<span data-ttu-id="266b4-174">В следующем примере показан успешный ответ на запрос операции **GetDiscoverySearchConfiguration** для получения всех сохраненных поисков обнаружения.</span><span class="sxs-lookup"><span data-stu-id="266b4-174">The following example shows a successful response to a **GetDiscoverySearchConfiguration** operation request to get all saved discovery searches.</span></span> 
  
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
      <GetDiscoverySearchConfigurationResponse ResponseClass="Success" 
                                               xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
         <DiscoverySearchConfigurations>
            <DiscoverySearchConfiguration xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
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
            <DiscoverySearchConfiguration xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
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

<span data-ttu-id="266b4-175">Тело SOAP отклика содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="266b4-175">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="266b4-176">жетдисковерисеарчконфигуратионреспонсе</span><span class="sxs-lookup"><span data-stu-id="266b4-176">GetDiscoverySearchConfigurationResponse</span></span>](getdiscoverysearchconfigurationresponse.md)
    
- [<span data-ttu-id="266b4-177">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="266b4-177">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="266b4-178">дисковерисеарчконфигуратионс</span><span class="sxs-lookup"><span data-stu-id="266b4-178">DiscoverySearchConfigurations</span></span>](discoverysearchconfigurations.md)
    
- [<span data-ttu-id="266b4-179">дисковерисеарчконфигуратион</span><span class="sxs-lookup"><span data-stu-id="266b4-179">DiscoverySearchConfiguration</span></span>](discoverysearchconfiguration.md)
    
- [<span data-ttu-id="266b4-180">сеарчид</span><span class="sxs-lookup"><span data-stu-id="266b4-180">SearchId</span></span>](searchid.md)
    
- [<span data-ttu-id="266b4-181">SearchQuery</span><span class="sxs-lookup"><span data-stu-id="266b4-181">SearchQuery</span></span>](searchquery.md)
    
- [<span data-ttu-id="266b4-182">сеарчаблемаилбоксес</span><span class="sxs-lookup"><span data-stu-id="266b4-182">SearchableMailboxes</span></span>](searchablemailboxes.md)
    
- [<span data-ttu-id="266b4-183">сеарчаблемаилбокс</span><span class="sxs-lookup"><span data-stu-id="266b4-183">SearchableMailbox</span></span>](searchablemailbox.md)
    
- [<span data-ttu-id="266b4-184">Guid</span><span class="sxs-lookup"><span data-stu-id="266b4-184">Guid</span></span>](guid-ex15websvcsotherref.md)
    
- [<span data-ttu-id="266b4-185">PrimarySmtpAddress (строка)</span><span class="sxs-lookup"><span data-stu-id="266b4-185">PrimarySmtpAddress (string)</span></span>](primarysmtpaddress-string.md)
    
- [<span data-ttu-id="266b4-186">исекстерналмаилбокс</span><span class="sxs-lookup"><span data-stu-id="266b4-186">IsExternalMailbox</span></span>](isexternalmailbox.md)
    
- [<span data-ttu-id="266b4-187">ExternalEmailAddress</span><span class="sxs-lookup"><span data-stu-id="266b4-187">ExternalEmailAddress</span></span>](externalemailaddress.md)
    
- [<span data-ttu-id="266b4-188">DisplayName (строка)</span><span class="sxs-lookup"><span data-stu-id="266b4-188">DisplayName (string)</span></span>](displayname-string.md)
    
- [<span data-ttu-id="266b4-189">исмембершипграуп</span><span class="sxs-lookup"><span data-stu-id="266b4-189">IsMembershipGroup</span></span>](ismembershipgroup.md)
    
- [<span data-ttu-id="266b4-190">ReferenceId</span><span class="sxs-lookup"><span data-stu-id="266b4-190">ReferenceId</span></span>](referenceid.md)
    
## <a name="getdiscoverysearchconfiguration-operation-error-response"></a><span data-ttu-id="266b4-191">Ответ об ошибке операции GetDiscoverySearchConfiguration</span><span class="sxs-lookup"><span data-stu-id="266b4-191">GetDiscoverySearchConfiguration operation error response</span></span>

<span data-ttu-id="266b4-192">В следующем примере показан ответ об ошибке для запроса операции **GetDiscoverySearchConfiguration** .</span><span class="sxs-lookup"><span data-stu-id="266b4-192">The following example shows an error response to a **GetDiscoverySearchConfiguration** operation request.</span></span> <span data-ttu-id="266b4-193">Это ответ на запрос на получение сохраненного поиска, не найденного на сервере.</span><span class="sxs-lookup"><span data-stu-id="266b4-193">This is a response to a request to get a saved search that is not found on the server.</span></span> 
  
```XML
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
      <GetDiscoverySearchConfigurationResponse ResponseClass="Error" 
                                               xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>Search configuration corresponding to the search id was not found.</MessageText>
         <ResponseCode>ErrorInvalidArgument</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
         <DiscoverySearchConfigurations/>
      </GetDiscoverySearchConfigurationResponse>
   </s:Body>
</s:Envelope>

```

<span data-ttu-id="266b4-194">Основной текст сообщения об ошибке SOAP содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="266b4-194">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="266b4-195">жетдисковерисеарчконфигуратионреспонсе</span><span class="sxs-lookup"><span data-stu-id="266b4-195">GetDiscoverySearchConfigurationResponse</span></span>](getdiscoverysearchconfigurationresponse.md)
    
- [<span data-ttu-id="266b4-196">мессажетекст</span><span class="sxs-lookup"><span data-stu-id="266b4-196">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="266b4-197">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="266b4-197">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="266b4-198">дескриптивелинккэй</span><span class="sxs-lookup"><span data-stu-id="266b4-198">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
- [<span data-ttu-id="266b4-199">дисковерисеарчконфигуратионс</span><span class="sxs-lookup"><span data-stu-id="266b4-199">DiscoverySearchConfigurations</span></span>](discoverysearchconfigurations.md)
    
<span data-ttu-id="266b4-200">Дополнительные коды ошибок, которые являются общими для EWS и специфичными для этой операции, можно найти в разделе [респонсекоде](responsecode.md).</span><span class="sxs-lookup"><span data-stu-id="266b4-200">For additional error codes that are generic to EWS and specific to this operation, see [ResponseCode](responsecode.md).</span></span>
  
## <a name="see-also"></a><span data-ttu-id="266b4-201">См. также</span><span class="sxs-lookup"><span data-stu-id="266b4-201">See also</span></span>

- [<span data-ttu-id="266b4-202">Операции EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="266b4-202">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
    
- [<span data-ttu-id="266b4-203">GetSearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="266b4-203">GetSearchableMailboxes</span></span>](getsearchablemailboxes.md)
    
- [<span data-ttu-id="266b4-204">SearchMailboxes</span><span class="sxs-lookup"><span data-stu-id="266b4-204">SearchMailboxes</span></span>](searchmailboxes.md)
    
- [<span data-ttu-id="266b4-205">GetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="266b4-205">GetHoldOnMailboxes</span></span>](getholdonmailboxes.md)
    
- [<span data-ttu-id="266b4-206">SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="266b4-206">SetHoldOnMailboxes</span></span>](setholdonmailboxes.md)
    
- [<span data-ttu-id="266b4-207">GetNonIndexableItemDetails</span><span class="sxs-lookup"><span data-stu-id="266b4-207">GetNonIndexableItemDetails</span></span>](getnonindexableitemdetails.md)
    
- [<span data-ttu-id="266b4-208">GetNonIndexableItemStatistics</span><span class="sxs-lookup"><span data-stu-id="266b4-208">GetNonIndexableItemStatistics</span></span>](getnonindexableitemstatistics.md)
    

