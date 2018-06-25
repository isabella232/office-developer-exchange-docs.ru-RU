---
title: Операция AddNewTelUriContactToGroup
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: c9688ce8-2465-45bb-8bd2-94b32ed4885c
description: Найдите сведения о том, как использовать операцию AddNewTelUriContactToGroup веб-служб Exchange.
ms.openlocfilehash: 34450171776b4215d9c0a39700a309e2e2d755dd
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761352"
---
# <a name="addnewteluricontacttogroup-operation"></a><span data-ttu-id="cd762-103">Операция AddNewTelUriContactToGroup</span><span class="sxs-lookup"><span data-stu-id="cd762-103">AddNewTelUriContactToGroup operation</span></span>

<span data-ttu-id="cd762-104">Найдите сведения о том, как использовать операцию **AddNewTelUriContactToGroup** веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="cd762-104">Find information about how to use the **AddNewTelUriContactToGroup** EWS operation.</span></span> 
  
<span data-ttu-id="cd762-105">Операция **AddNewTelUriContactToGroup** добавляет новый контакт в группу на основании номер телефона контакта.</span><span class="sxs-lookup"><span data-stu-id="cd762-105">The **AddNewTelUriContactToGroup** operation adds a new contact to a group based on a contact's phone number.</span></span> 
  
<span data-ttu-id="cd762-106">Эта операция появилась в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="cd762-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-addnewteluricontacttogroup-operation"></a><span data-ttu-id="cd762-107">С помощью операции AddNewTelUriContactToGroup</span><span class="sxs-lookup"><span data-stu-id="cd762-107">Using the AddNewTelUriContactToGroup operation</span></span>

<span data-ttu-id="cd762-108">Операция запроса **AddNewTelUriContactToGroup** отправляет данные контакта TEL URI, SIP URI, номер телефона и группы для добавления контакта.</span><span class="sxs-lookup"><span data-stu-id="cd762-108">An **AddNewTelUriContactToGroup** operation request submits a contact's TEL URI, SIP URI, phone number, and the group to add the contact to.</span></span> <span data-ttu-id="cd762-109">Операция ответа на **AddNewTelUriContactToGroup** создает пользователь для нового контакта.</span><span class="sxs-lookup"><span data-stu-id="cd762-109">An **AddNewTelUriContactToGroup** operation response creates a persona for the new contact.</span></span> <span data-ttu-id="cd762-110">Эта операция позволяет клиентам для добавления нового контакта, даже в том случае, если контакт не имеет имя.</span><span class="sxs-lookup"><span data-stu-id="cd762-110">This operation allows clients to add a new contact even if the contact does not have a name.</span></span> 
  
### <a name="addnewteluricontacttogroup-operation-soap-headers"></a><span data-ttu-id="cd762-111">Заголовки SOAP AddNewTelUriContactToGroup операции</span><span class="sxs-lookup"><span data-stu-id="cd762-111">AddNewTelUriContactToGroup operation SOAP headers</span></span>

<span data-ttu-id="cd762-112">Операция **AddNewTelUriContactToGroup** можно использовать заголовки SOAP, которые перечислены в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="cd762-112">The **AddNewTelUriContactToGroup** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="cd762-113">**Имя заголовка**</span><span class="sxs-lookup"><span data-stu-id="cd762-113">**Header name**</span></span>|<span data-ttu-id="cd762-114">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="cd762-114">**Element**</span></span>|<span data-ttu-id="cd762-115">**Описание**</span><span class="sxs-lookup"><span data-stu-id="cd762-115">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="cd762-116">**Олицетворение**</span><span class="sxs-lookup"><span data-stu-id="cd762-116">**Impersonation**</span></span> <br/> |[<span data-ttu-id="cd762-117">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="cd762-117">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="cd762-118">Идентифицирует пользователя, которого олицетворения в клиентском приложении.</span><span class="sxs-lookup"><span data-stu-id="cd762-118">Identifies the user whom the client application is impersonating.</span></span> <span data-ttu-id="cd762-119">Этот заголовок можно применять к запросу.</span><span class="sxs-lookup"><span data-stu-id="cd762-119">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="cd762-120">**MailboxCulture**</span><span class="sxs-lookup"><span data-stu-id="cd762-120">**MailboxCulture**</span></span> <br/> |[<span data-ttu-id="cd762-121">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="cd762-121">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="cd762-122">Определяет язык и региональные параметры, как определено в RFC 3066, «Теги для идентификации языков», который будет использоваться для доступа к почтовому ящику.</span><span class="sxs-lookup"><span data-stu-id="cd762-122">Identifies the culture, as defined in RFC 3066, "Tags for the Identification of Languages", to be used to access the mailbox.</span></span> <span data-ttu-id="cd762-123">Этот заголовок можно применять к запросу.</span><span class="sxs-lookup"><span data-stu-id="cd762-123">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="cd762-124">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="cd762-124">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="cd762-125">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="cd762-125">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="cd762-126">Определяет версию схемы для операции запроса.</span><span class="sxs-lookup"><span data-stu-id="cd762-126">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="cd762-127">Этот заголовок можно применять к запросу.</span><span class="sxs-lookup"><span data-stu-id="cd762-127">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="cd762-128">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="cd762-128">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="cd762-129">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="cd762-129">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="cd762-130">Определяет версию сервера, ответившего на запрос.</span><span class="sxs-lookup"><span data-stu-id="cd762-130">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="cd762-131">Этот заголовок можно применять, чтобы получить ответ.</span><span class="sxs-lookup"><span data-stu-id="cd762-131">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="addnewteluricontacttogroup-operation-request-example-add-a-new-contact-to-a-group"></a><span data-ttu-id="cd762-132">Пример запроса AddNewTelUriContactToGroup операции: Добавление нового контакта в группу</span><span class="sxs-lookup"><span data-stu-id="cd762-132">AddNewTelUriContactToGroup operation request example: Add a new contact to a group</span></span>

<span data-ttu-id="cd762-133">В следующем примере запрос операции **AddNewTelUriContactToGroup** показано, как создание новых контактов и добавить новый контакт в группу мгновенного обмена сообщениями обмена Мгновенными сообщениями с помощью TEL и коды URI SIP контакта.</span><span class="sxs-lookup"><span data-stu-id="cd762-133">The following example of an **AddNewTelUriContactToGroup** operation request shows how to create a new contact and add the new contact to an instant messaging (IM) group by using the contact's TEL and SIP URIs.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="cd762-134">Все идентификаторы элементов и ключей изменения в этой статье URL были сокращены, чтобы сохранить удобочитаемость.</span><span class="sxs-lookup"><span data-stu-id="cd762-134">All item identifiers and change keys in this article have been shortened to preserve readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013" />
      <t:MailboxCulture>en-US</t:MailboxCulture>
   </soap:Header>
   <soap:Body >
      <m:AddNewTelUriContactToGroup>
         <m:TelUriAddress>tel:5625550100</m:TelUriAddress>
         <m:ImContactSipUriAddress>sip:john@contoso.com</m:ImContactSipUriAddress>
         <m:ImTelephoneNumber>5625550100</m:ImTelephoneNumber>
         <m:GroupId Id="AAMkADEzOTm4QrAABY7+0GAAA="/>
      </m:AddNewTelUriContactToGroup>
   </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="cd762-135">Запрос SOAP body содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="cd762-135">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="cd762-136">AddNewTelUriContactToGroup</span><span class="sxs-lookup"><span data-stu-id="cd762-136">AddNewTelUriContactToGroup</span></span>](addnewteluricontacttogroup.md)
    
- [<span data-ttu-id="cd762-137">TelUriAddress</span><span class="sxs-lookup"><span data-stu-id="cd762-137">TelUriAddress</span></span>](teluriaddress.md)
    
- [<span data-ttu-id="cd762-138">ImContactSipUriAddress</span><span class="sxs-lookup"><span data-stu-id="cd762-138">ImContactSipUriAddress</span></span>](imcontactsipuriaddress.md)
    
- [<span data-ttu-id="cd762-139">ImTelephoneNumber</span><span class="sxs-lookup"><span data-stu-id="cd762-139">ImTelephoneNumber</span></span>](imtelephonenumber.md)
    
- [<span data-ttu-id="cd762-140">GroupId</span><span class="sxs-lookup"><span data-stu-id="cd762-140">GroupId</span></span>](groupid.md)
    
## <a name="successful-addnewteluricontacttogroup-operation-response"></a><span data-ttu-id="cd762-141">Успешные операции ответа AddNewTelUriContactToGroup</span><span class="sxs-lookup"><span data-stu-id="cd762-141">Successful AddNewTelUriContactToGroup operation response</span></span>

<span data-ttu-id="cd762-142">В следующем примере показано успешного ответа на запрос операции **AddNewTelUriContactToGroup** для создания контакта.</span><span class="sxs-lookup"><span data-stu-id="cd762-142">The following example shows a successful response to an **AddNewTelUriContactToGroup** operation request to create a contact.</span></span> <span data-ttu-id="cd762-143">Ответ содержит идентификатор связанного пользователя для контакта, отображаемое имя пользователя, который в этом случае основан на номер телефона контакта, и идентификатор элемента контакта, которая отображается как часть атрибуты идентификатор источника.</span><span class="sxs-lookup"><span data-stu-id="cd762-143">The response contains the associated persona identifier for the contact, the display name of the persona, which in this case is based on the contact's phone number, and the contact's item identifier, which is displayed as part of the source identifier attribution.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/"                           
            xmlns:xsd="http://www.w3.org/2001/XMLSchema"
            xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
            xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="545" 
                           MinorBuildNumber="11" 
                           Version="Exchange2013" 
                           xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="http://schemas.microsoft.com/exchange/services/2006/types" />
   </s:Header>
   <s:Body>
      <AddNewTelUriContactToGroupResponse ResponseClass="Success" 
                                          xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
         <Persona>
            <t:PersonaId Id="AAQkADE686dX3s="/>
            <t:PersonaType>Person</t:PersonaType>
            <t:CreationTime>2012-10-29T23:10:13Z</t:CreationTime>
            <t:DisplayName/>
            <t:DisplayNameFirstLast>5625550100</t:DisplayNameFirstLast>
            <t:DisplayNameLastFirst>5625550100</t:DisplayNameLastFirst>
            <t:FileAs/>
            <t:FileAsId >None</t:FileAsId>
            <t:RelevanceScore >2147483647</t:RelevanceScore>
            <t:Attributions>
               <t:Attribution>
                  <t:Id>0</t:Id>
                  <t:SourceId Id="ABhHuhCAAA=" ChangeKey="EQAAABxFU"/>
                  <t:DisplayName>Lync Contacts</t:DisplayName>
                  <t:IsWritable>false</t:IsWritable>
                  <t:IsQuickContact>true</t:IsQuickContact>
                  <t:IsHidden>false</t:IsHidden>
               </t:Attribution>
            </t:Attributions>
            <t:FileAsIds>
               <t:StringAttributedValue>
                  <t:Value>None</t:Value>
                  <t:Attributions>
                     <t:Attribution>0</t:Attribution>
                  </t:Attributions>
               </t:StringAttributedValue>
            </t:FileAsIds>
            <t:OtherTelephones>
               <t:PhoneNumberAttributedValue>
                  <t:Value>
                     <t:Number>5625550100</t:Number>
                     <t:Type>Other</t:Type>
                  </t:Value>
                  <t:Attributions>
                     <t:Attribution>0</t:Attribution>
                  </t:Attributions>
               </t:PhoneNumberAttributedValue>
            </t:OtherTelephones>
         </Persona>
      </AddNewTelUriContactToGroupResponse>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="cd762-144">Ответ SOAP body содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="cd762-144">The response SOAP body contains following elements:</span></span>
  
- [<span data-ttu-id="cd762-145">AddNewTelUriContactToGroupResponse</span><span class="sxs-lookup"><span data-stu-id="cd762-145">AddNewTelUriContactToGroupResponse</span></span>](addnewteluricontacttogroupresponse.md)
    
- [<span data-ttu-id="cd762-146">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="cd762-146">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="cd762-147">Пользователь</span><span class="sxs-lookup"><span data-stu-id="cd762-147">Persona</span></span>](persona.md)
    
- [<span data-ttu-id="cd762-148">PersonaId</span><span class="sxs-lookup"><span data-stu-id="cd762-148">PersonaId</span></span>](personaid.md)
    
- [<span data-ttu-id="cd762-149">PersonaType</span><span class="sxs-lookup"><span data-stu-id="cd762-149">PersonaType</span></span>](personatype.md)
    
- [<span data-ttu-id="cd762-150">CreationTime</span><span class="sxs-lookup"><span data-stu-id="cd762-150">CreationTime</span></span>](creationtime.md)
    
- [<span data-ttu-id="cd762-151">Отображаемое имя (строка)</span><span class="sxs-lookup"><span data-stu-id="cd762-151">DisplayName (string)</span></span>](displayname-string.md)
    
- [<span data-ttu-id="cd762-152">DisplayNameFirstLast</span><span class="sxs-lookup"><span data-stu-id="cd762-152">DisplayNameFirstLast</span></span>](displaynamefirstlast.md)
    
- [<span data-ttu-id="cd762-153">DisplayNameLastFirst</span><span class="sxs-lookup"><span data-stu-id="cd762-153">DisplayNameLastFirst</span></span>](displaynamelastfirst.md)
    
- [<span data-ttu-id="cd762-154">FileAs</span><span class="sxs-lookup"><span data-stu-id="cd762-154">FileAs</span></span>](fileas.md)
    
- [<span data-ttu-id="cd762-155">FileAsId</span><span class="sxs-lookup"><span data-stu-id="cd762-155">FileAsId</span></span>](fileasid.md)
    
- [<span data-ttu-id="cd762-156">RelevanceScore</span><span class="sxs-lookup"><span data-stu-id="cd762-156">RelevanceScore</span></span>](relevancescore.md)
    
- [<span data-ttu-id="cd762-157">Атрибуты (ArrayOfPersonaAttributionsType)</span><span class="sxs-lookup"><span data-stu-id="cd762-157">Attributions (ArrayOfPersonaAttributionsType)</span></span>](attributions-arrayofpersonaattributionstype.md)
    
- [<span data-ttu-id="cd762-158">Атрибуты (PersonaAttributionType)</span><span class="sxs-lookup"><span data-stu-id="cd762-158">Attribution (PersonaAttributionType)</span></span>](attribution-personaattributiontype.md)
    
- [<span data-ttu-id="cd762-159">Идентификатор (строка)</span><span class="sxs-lookup"><span data-stu-id="cd762-159">ID (String)</span></span>](id-string.md)
    
- [<span data-ttu-id="cd762-160">SourceId</span><span class="sxs-lookup"><span data-stu-id="cd762-160">SourceId</span></span>](sourceid.md)
    
- [<span data-ttu-id="cd762-161">Отображаемое имя (строка)</span><span class="sxs-lookup"><span data-stu-id="cd762-161">DisplayName (string)</span></span>](displayname-string.md)
    
- [<span data-ttu-id="cd762-162">IsWritable</span><span class="sxs-lookup"><span data-stu-id="cd762-162">IsWritable</span></span>](iswritable.md)
    
- [<span data-ttu-id="cd762-163">IsQuickContact</span><span class="sxs-lookup"><span data-stu-id="cd762-163">IsQuickContact</span></span>](isquickcontact.md)
    
- [<span data-ttu-id="cd762-164">IsHidden</span><span class="sxs-lookup"><span data-stu-id="cd762-164">IsHidden</span></span>](ishidden.md)
    
- [<span data-ttu-id="cd762-165">FileAsIds</span><span class="sxs-lookup"><span data-stu-id="cd762-165">FileAsIds</span></span>](fileasids.md)
    
- [<span data-ttu-id="cd762-166">StringAttributedValue</span><span class="sxs-lookup"><span data-stu-id="cd762-166">StringAttributedValue</span></span>](stringattributedvalue.md)
    
- [<span data-ttu-id="cd762-167">Значение</span><span class="sxs-lookup"><span data-stu-id="cd762-167">Value</span></span>](value.md)
    
- [<span data-ttu-id="cd762-168">Атрибуты (ArrayOfValueAttributionsType)</span><span class="sxs-lookup"><span data-stu-id="cd762-168">Attributions (ArrayOfValueAttributionsType)</span></span>](attributions-arrayofvalueattributionstype.md)
    
- [<span data-ttu-id="cd762-169">Атрибуты (строка)</span><span class="sxs-lookup"><span data-stu-id="cd762-169">Attribution (string)</span></span>](attribution-string.md)
    
- [<span data-ttu-id="cd762-170">OtherTelephones</span><span class="sxs-lookup"><span data-stu-id="cd762-170">OtherTelephones</span></span>](othertelephones.md)
    
- [<span data-ttu-id="cd762-171">PhoneNumberAttributedValue</span><span class="sxs-lookup"><span data-stu-id="cd762-171">PhoneNumberAttributedValue</span></span>](phonenumberattributedvalue.md)
    
- [<span data-ttu-id="cd762-172">Значение</span><span class="sxs-lookup"><span data-stu-id="cd762-172">Value</span></span>](value.md)
    
- [<span data-ttu-id="cd762-173">Число</span><span class="sxs-lookup"><span data-stu-id="cd762-173">Number</span></span>](number.md)
    
- [<span data-ttu-id="cd762-174">Тип (строка)</span><span class="sxs-lookup"><span data-stu-id="cd762-174">Type (string)</span></span>](type-string.md)
    
- [<span data-ttu-id="cd762-175">Атрибуты (ArrayOfValueAttributionsType)</span><span class="sxs-lookup"><span data-stu-id="cd762-175">Attributions (ArrayOfValueAttributionsType)</span></span>](attributions-arrayofvalueattributionstype.md)
    
- [<span data-ttu-id="cd762-176">Атрибуты (строка)</span><span class="sxs-lookup"><span data-stu-id="cd762-176">Attribution (string)</span></span>](attribution-string.md)
    
## <a name="addnewteluricontacttogroup-operation-error-response-example"></a><span data-ttu-id="cd762-177">Пример ответа об ошибке AddNewTelUriContactToGroup операции</span><span class="sxs-lookup"><span data-stu-id="cd762-177">AddNewTelUriContactToGroup operation error response example</span></span>

<span data-ttu-id="cd762-178">В следующем примере показано ошибочный ответ на запрос операции **AddNewTelUriContactToGroup** , когда идентификатор группы содержит имеющийся значение, которое не определяет группу в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="cd762-178">The following example shows an error response to an **AddNewTelUriContactToGroup** operation request when the group identifier contains a well-formed value that does not identify a group in the mailbox.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="545" 
                           MinorBuildNumber="11" 
                           Version="Exchange2013" 
                           xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <AddNewTelUriContactToGroupResponse ResponseClass="Error" 
                                          xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>The specified object was not found in the store.</MessageText>
         <ResponseCode>ErrorItemNotFound</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
      </AddNewTelUriContactToGroupResponse>
   </s:Body>
</s:Envelope>

```

<span data-ttu-id="cd762-179">Ошибка ответ SOAP body содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="cd762-179">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="cd762-180">AddNewTelUriContactToGroupResponse</span><span class="sxs-lookup"><span data-stu-id="cd762-180">AddNewTelUriContactToGroupResponse</span></span>](addnewteluricontacttogroupresponse.md)
    
- [<span data-ttu-id="cd762-181">MessageText</span><span class="sxs-lookup"><span data-stu-id="cd762-181">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="cd762-182">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="cd762-182">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="cd762-183">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="cd762-183">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
## <a name="see-also"></a><span data-ttu-id="cd762-184">См. также</span><span class="sxs-lookup"><span data-stu-id="cd762-184">See also</span></span>

- [<span data-ttu-id="cd762-185">Операции EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="cd762-185">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
    
- [<span data-ttu-id="cd762-186">Пользователи и контакты в EWS для Exchange</span><span class="sxs-lookup"><span data-stu-id="cd762-186">People and contacts in EWS in Exchange</span></span>](http://msdn.microsoft.com/library/043c33be-a0d1-4bad-a840-85715eda4813%28Office.15%29.aspx)
    

