---
title: Операция AddNewTelUriContactToGroup
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: c9688ce8-2465-45bb-8bd2-94b32ed4885c
description: Найдите сведения об использовании операции AddNewTelUriContactToGroup EWS.
ms.openlocfilehash: 91228ec627ad928d2f1837c135af24846f811b1c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44464947"
---
# <a name="addnewteluricontacttogroup-operation"></a><span data-ttu-id="2819c-103">Операция AddNewTelUriContactToGroup</span><span class="sxs-lookup"><span data-stu-id="2819c-103">AddNewTelUriContactToGroup operation</span></span>

<span data-ttu-id="2819c-104">Найдите сведения об использовании операции **AddNewTelUriContactToGroup** EWS.</span><span class="sxs-lookup"><span data-stu-id="2819c-104">Find information about how to use the **AddNewTelUriContactToGroup** EWS operation.</span></span> 
  
<span data-ttu-id="2819c-105">Операция **AddNewTelUriContactToGroup** добавляет новый контакт в группу на основе номера телефона контакта.</span><span class="sxs-lookup"><span data-stu-id="2819c-105">The **AddNewTelUriContactToGroup** operation adds a new contact to a group based on a contact's phone number.</span></span> 
  
<span data-ttu-id="2819c-106">Эта операция появилась в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="2819c-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-addnewteluricontacttogroup-operation"></a><span data-ttu-id="2819c-107">Использование операции AddNewTelUriContactToGroup</span><span class="sxs-lookup"><span data-stu-id="2819c-107">Using the AddNewTelUriContactToGroup operation</span></span>

<span data-ttu-id="2819c-108">Запрос операции **AddNewTelUriContactToGroup** передает URI TEL контакта, универсальный код ресурса (URI) SIP, номер телефона и группу, в которую добавляется контакт.</span><span class="sxs-lookup"><span data-stu-id="2819c-108">An **AddNewTelUriContactToGroup** operation request submits a contact's TEL URI, SIP URI, phone number, and the group to add the contact to.</span></span> <span data-ttu-id="2819c-109">Ответ операции **AddNewTelUriContactToGroup** создает пользователя для нового контакта.</span><span class="sxs-lookup"><span data-stu-id="2819c-109">An **AddNewTelUriContactToGroup** operation response creates a persona for the new contact.</span></span> <span data-ttu-id="2819c-110">Эта операция позволяет клиентам добавлять новый контакт, даже если у него нет имени.</span><span class="sxs-lookup"><span data-stu-id="2819c-110">This operation allows clients to add a new contact even if the contact does not have a name.</span></span> 
  
### <a name="addnewteluricontacttogroup-operation-soap-headers"></a><span data-ttu-id="2819c-111">Заголовки SOAP операции AddNewTelUriContactToGroup</span><span class="sxs-lookup"><span data-stu-id="2819c-111">AddNewTelUriContactToGroup operation SOAP headers</span></span>

<span data-ttu-id="2819c-112">Операция **AddNewTelUriContactToGroup** может использовать заголовки SOAP, указанные в приведенной ниже таблице.</span><span class="sxs-lookup"><span data-stu-id="2819c-112">The **AddNewTelUriContactToGroup** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="2819c-113">**Имя заголовка**</span><span class="sxs-lookup"><span data-stu-id="2819c-113">**Header name**</span></span>|<span data-ttu-id="2819c-114">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="2819c-114">**Element**</span></span>|<span data-ttu-id="2819c-115">**Описание**</span><span class="sxs-lookup"><span data-stu-id="2819c-115">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="2819c-116">**Олицетворение**</span><span class="sxs-lookup"><span data-stu-id="2819c-116">**Impersonation**</span></span> <br/> |[<span data-ttu-id="2819c-117">ексчанжеимперсонатион</span><span class="sxs-lookup"><span data-stu-id="2819c-117">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="2819c-118">Идентифицирует пользователя, который олицетворяет клиентское приложение.</span><span class="sxs-lookup"><span data-stu-id="2819c-118">Identifies the user whom the client application is impersonating.</span></span> <span data-ttu-id="2819c-119">Этот заголовок является применимым для запроса.</span><span class="sxs-lookup"><span data-stu-id="2819c-119">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="2819c-120">**маилбокскултуре**</span><span class="sxs-lookup"><span data-stu-id="2819c-120">**MailboxCulture**</span></span> <br/> |[<span data-ttu-id="2819c-121">маилбокскултуре</span><span class="sxs-lookup"><span data-stu-id="2819c-121">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="2819c-122">Определяет язык и региональные параметры, определенные в документе RFC 3066 "Теги для идентификации языков", которые будут использоваться для доступа к почтовому ящику.</span><span class="sxs-lookup"><span data-stu-id="2819c-122">Identifies the culture, as defined in RFC 3066, "Tags for the Identification of Languages", to be used to access the mailbox.</span></span> <span data-ttu-id="2819c-123">Этот заголовок является применимым для запроса.</span><span class="sxs-lookup"><span data-stu-id="2819c-123">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="2819c-124">**рекуестверсион**</span><span class="sxs-lookup"><span data-stu-id="2819c-124">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="2819c-125">рекуестсерверверсион</span><span class="sxs-lookup"><span data-stu-id="2819c-125">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="2819c-126">Определяет версию схемы для запроса операции.</span><span class="sxs-lookup"><span data-stu-id="2819c-126">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="2819c-127">Этот заголовок является применимым для запроса.</span><span class="sxs-lookup"><span data-stu-id="2819c-127">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="2819c-128">**серверверсион**</span><span class="sxs-lookup"><span data-stu-id="2819c-128">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="2819c-129">серверверсионинфо</span><span class="sxs-lookup"><span data-stu-id="2819c-129">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="2819c-130">Определяет версию сервера, который ответил на запрос.</span><span class="sxs-lookup"><span data-stu-id="2819c-130">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="2819c-131">Этот заголовок является применимым для отклика.</span><span class="sxs-lookup"><span data-stu-id="2819c-131">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="addnewteluricontacttogroup-operation-request-example-add-a-new-contact-to-a-group"></a><span data-ttu-id="2819c-132">Пример запроса операции AddNewTelUriContactToGroup: Добавление нового контакта в группу</span><span class="sxs-lookup"><span data-stu-id="2819c-132">AddNewTelUriContactToGroup operation request example: Add a new contact to a group</span></span>

<span data-ttu-id="2819c-133">В следующем примере запроса операции **AddNewTelUriContactToGroup** показано, как создать новый контакт и добавить новый контакт в группу обмена мгновенными сообщениями с помощью URI TEL и SIP контакта.</span><span class="sxs-lookup"><span data-stu-id="2819c-133">The following example of an **AddNewTelUriContactToGroup** operation request shows how to create a new contact and add the new contact to an instant messaging (IM) group by using the contact's TEL and SIP URIs.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="2819c-134">Все идентификаторы элементов и изменения ключей в этой статье были сокращены, чтобы сохранить удобочитаемость.</span><span class="sxs-lookup"><span data-stu-id="2819c-134">All item identifiers and change keys in this article have been shortened to preserve readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
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

<span data-ttu-id="2819c-135">Текст SOAP Request содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="2819c-135">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="2819c-136">AddNewTelUriContactToGroup</span><span class="sxs-lookup"><span data-stu-id="2819c-136">AddNewTelUriContactToGroup</span></span>](addnewteluricontacttogroup.md)
    
- [<span data-ttu-id="2819c-137">телуриаддресс</span><span class="sxs-lookup"><span data-stu-id="2819c-137">TelUriAddress</span></span>](teluriaddress.md)
    
- [<span data-ttu-id="2819c-138">имконтактсипуриаддресс</span><span class="sxs-lookup"><span data-stu-id="2819c-138">ImContactSipUriAddress</span></span>](imcontactsipuriaddress.md)
    
- [<span data-ttu-id="2819c-139">имтелефоненумбер</span><span class="sxs-lookup"><span data-stu-id="2819c-139">ImTelephoneNumber</span></span>](imtelephonenumber.md)
    
- [<span data-ttu-id="2819c-140">GroupId</span><span class="sxs-lookup"><span data-stu-id="2819c-140">GroupId</span></span>](groupid.md)
    
## <a name="successful-addnewteluricontacttogroup-operation-response"></a><span data-ttu-id="2819c-141">Успешный отклик операции AddNewTelUriContactToGroup</span><span class="sxs-lookup"><span data-stu-id="2819c-141">Successful AddNewTelUriContactToGroup operation response</span></span>

<span data-ttu-id="2819c-142">В следующем примере показан успешный ответ на запрос операции **AddNewTelUriContactToGroup** для создания контакта.</span><span class="sxs-lookup"><span data-stu-id="2819c-142">The following example shows a successful response to an **AddNewTelUriContactToGroup** operation request to create a contact.</span></span> <span data-ttu-id="2819c-143">Ответ содержит связанный идентификатор персонажа для контакта, отображаемое имя пользователя, которое в данном случае основано на номере телефона контакта, и идентификатор элемента контакта, который отображается как часть атрибутов идентификатора источника.</span><span class="sxs-lookup"><span data-stu-id="2819c-143">The response contains the associated persona identifier for the contact, the display name of the persona, which in this case is based on the contact's phone number, and the contact's item identifier, which is displayed as part of the source identifier attribution.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/"                           
            xmlns:xsd="http://www.w3.org/2001/XMLSchema"
            xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
            xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="545" 
                           MinorBuildNumber="11" 
                           Version="Exchange2013" 
                           xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="https://schemas.microsoft.com/exchange/services/2006/types" />
   </s:Header>
   <s:Body>
      <AddNewTelUriContactToGroupResponse ResponseClass="Success" 
                                          xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
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

<span data-ttu-id="2819c-144">Тело SOAP отклика содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="2819c-144">The response SOAP body contains following elements:</span></span>
  
- [<span data-ttu-id="2819c-145">аддневтелуриконтакттограупреспонсе</span><span class="sxs-lookup"><span data-stu-id="2819c-145">AddNewTelUriContactToGroupResponse</span></span>](addnewteluricontacttogroupresponse.md)
    
- [<span data-ttu-id="2819c-146">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="2819c-146">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="2819c-147">Роль</span><span class="sxs-lookup"><span data-stu-id="2819c-147">Persona</span></span>](persona.md)
    
- [<span data-ttu-id="2819c-148">персонаид</span><span class="sxs-lookup"><span data-stu-id="2819c-148">PersonaId</span></span>](personaid.md)
    
- [<span data-ttu-id="2819c-149">персонатипе</span><span class="sxs-lookup"><span data-stu-id="2819c-149">PersonaType</span></span>](personatype.md)
    
- [<span data-ttu-id="2819c-150">CreationTime</span><span class="sxs-lookup"><span data-stu-id="2819c-150">CreationTime</span></span>](creationtime.md)
    
- [<span data-ttu-id="2819c-151">DisplayName (строка)</span><span class="sxs-lookup"><span data-stu-id="2819c-151">DisplayName (string)</span></span>](displayname-string.md)
    
- [<span data-ttu-id="2819c-152">дисплайнамефирстласт</span><span class="sxs-lookup"><span data-stu-id="2819c-152">DisplayNameFirstLast</span></span>](displaynamefirstlast.md)
    
- [<span data-ttu-id="2819c-153">дисплайнамеластфирст</span><span class="sxs-lookup"><span data-stu-id="2819c-153">DisplayNameLastFirst</span></span>](displaynamelastfirst.md)
    
- [<span data-ttu-id="2819c-154">FileAs</span><span class="sxs-lookup"><span data-stu-id="2819c-154">FileAs</span></span>](fileas.md)
    
- [<span data-ttu-id="2819c-155">филеасид</span><span class="sxs-lookup"><span data-stu-id="2819c-155">FileAsId</span></span>](fileasid.md)
    
- [<span data-ttu-id="2819c-156">релеванцескоре</span><span class="sxs-lookup"><span data-stu-id="2819c-156">RelevanceScore</span></span>](relevancescore.md)
    
- [<span data-ttu-id="2819c-157">Атрибуты (Аррайофперсонааттрибутионстипе)</span><span class="sxs-lookup"><span data-stu-id="2819c-157">Attributions (ArrayOfPersonaAttributionsType)</span></span>](attributions-arrayofpersonaattributionstype.md)
    
- [<span data-ttu-id="2819c-158">Атрибуты (Персонааттрибутионтипе)</span><span class="sxs-lookup"><span data-stu-id="2819c-158">Attribution (PersonaAttributionType)</span></span>](attribution-personaattributiontype.md)
    
- [<span data-ttu-id="2819c-159">ID (строка)</span><span class="sxs-lookup"><span data-stu-id="2819c-159">ID (String)</span></span>](id-string.md)
    
- [<span data-ttu-id="2819c-160">SourceId</span><span class="sxs-lookup"><span data-stu-id="2819c-160">SourceId</span></span>](sourceid.md)
    
- [<span data-ttu-id="2819c-161">DisplayName (строка)</span><span class="sxs-lookup"><span data-stu-id="2819c-161">DisplayName (string)</span></span>](displayname-string.md)
    
- [<span data-ttu-id="2819c-162">Доступный для записи</span><span class="sxs-lookup"><span data-stu-id="2819c-162">IsWritable</span></span>](iswritable.md)
    
- [<span data-ttu-id="2819c-163">искуиккконтакт</span><span class="sxs-lookup"><span data-stu-id="2819c-163">IsQuickContact</span></span>](isquickcontact.md)
    
- [<span data-ttu-id="2819c-164">IsHidden</span><span class="sxs-lookup"><span data-stu-id="2819c-164">IsHidden</span></span>](ishidden.md)
    
- [<span data-ttu-id="2819c-165">филеасидс</span><span class="sxs-lookup"><span data-stu-id="2819c-165">FileAsIds</span></span>](fileasids.md)
    
- [<span data-ttu-id="2819c-166">стрингаттрибутедвалуе</span><span class="sxs-lookup"><span data-stu-id="2819c-166">StringAttributedValue</span></span>](stringattributedvalue.md)
    
- [<span data-ttu-id="2819c-167">Значение</span><span class="sxs-lookup"><span data-stu-id="2819c-167">Value</span></span>](value.md)
    
- [<span data-ttu-id="2819c-168">Атрибуты (Аррайофвалуеаттрибутионстипе)</span><span class="sxs-lookup"><span data-stu-id="2819c-168">Attributions (ArrayOfValueAttributionsType)</span></span>](attributions-arrayofvalueattributionstype.md)
    
- [<span data-ttu-id="2819c-169">Атрибуты (строка)</span><span class="sxs-lookup"><span data-stu-id="2819c-169">Attribution (string)</span></span>](attribution-string.md)
    
- [<span data-ttu-id="2819c-170">осертелефонес</span><span class="sxs-lookup"><span data-stu-id="2819c-170">OtherTelephones</span></span>](othertelephones.md)
    
- [<span data-ttu-id="2819c-171">фоненумбераттрибутедвалуе</span><span class="sxs-lookup"><span data-stu-id="2819c-171">PhoneNumberAttributedValue</span></span>](phonenumberattributedvalue.md)
    
- [<span data-ttu-id="2819c-172">Значение</span><span class="sxs-lookup"><span data-stu-id="2819c-172">Value</span></span>](value.md)
    
- [<span data-ttu-id="2819c-173">Number</span><span class="sxs-lookup"><span data-stu-id="2819c-173">Number</span></span>](number.md)
    
- [<span data-ttu-id="2819c-174">Тип (строка)</span><span class="sxs-lookup"><span data-stu-id="2819c-174">Type (string)</span></span>](type-string.md)
    
- [<span data-ttu-id="2819c-175">Атрибуты (Аррайофвалуеаттрибутионстипе)</span><span class="sxs-lookup"><span data-stu-id="2819c-175">Attributions (ArrayOfValueAttributionsType)</span></span>](attributions-arrayofvalueattributionstype.md)
    
- [<span data-ttu-id="2819c-176">Атрибуты (строка)</span><span class="sxs-lookup"><span data-stu-id="2819c-176">Attribution (string)</span></span>](attribution-string.md)
    
## <a name="addnewteluricontacttogroup-operation-error-response-example"></a><span data-ttu-id="2819c-177">Пример ответа на сообщение об ошибке операции AddNewTelUriContactToGroup</span><span class="sxs-lookup"><span data-stu-id="2819c-177">AddNewTelUriContactToGroup operation error response example</span></span>

<span data-ttu-id="2819c-178">В следующем примере показан ответ об ошибке для запроса операции **AddNewTelUriContactToGroup** , когда идентификатор группы содержит правильное значение, не идентифицирующее группу в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="2819c-178">The following example shows an error response to an **AddNewTelUriContactToGroup** operation request when the group identifier contains a well-formed value that does not identify a group in the mailbox.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="545" 
                           MinorBuildNumber="11" 
                           Version="Exchange2013" 
                           xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <AddNewTelUriContactToGroupResponse ResponseClass="Error" 
                                          xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>The specified object was not found in the store.</MessageText>
         <ResponseCode>ErrorItemNotFound</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
      </AddNewTelUriContactToGroupResponse>
   </s:Body>
</s:Envelope>

```

<span data-ttu-id="2819c-179">Основной текст сообщения об ошибке SOAP содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="2819c-179">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="2819c-180">аддневтелуриконтакттограупреспонсе</span><span class="sxs-lookup"><span data-stu-id="2819c-180">AddNewTelUriContactToGroupResponse</span></span>](addnewteluricontacttogroupresponse.md)
    
- [<span data-ttu-id="2819c-181">мессажетекст</span><span class="sxs-lookup"><span data-stu-id="2819c-181">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="2819c-182">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="2819c-182">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="2819c-183">дескриптивелинккэй</span><span class="sxs-lookup"><span data-stu-id="2819c-183">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
## <a name="see-also"></a><span data-ttu-id="2819c-184">См. также</span><span class="sxs-lookup"><span data-stu-id="2819c-184">See also</span></span>

- [<span data-ttu-id="2819c-185">Операции EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="2819c-185">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
    
- [<span data-ttu-id="2819c-186">Пользователи и контакты в EWS для Exchange</span><span class="sxs-lookup"><span data-stu-id="2819c-186">People and contacts in EWS in Exchange</span></span>](https://msdn.microsoft.com/library/043c33be-a0d1-4bad-a840-85715eda4813%28Office.15%29.aspx)
    

