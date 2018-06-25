---
title: Операция GetImItems
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 51186691-46d2-4d5c-b8bc-4ee2bb20fbe7
description: Найдите сведения о веб-служб Exchange GetImItems операции.
ms.openlocfilehash: 4335cc22b22dc5f102f2221f7fdb22a506ba026f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762817"
---
# <a name="getimitems-operation"></a><span data-ttu-id="fd404-103">Операция GetImItems</span><span class="sxs-lookup"><span data-stu-id="fd404-103">GetImItems operation</span></span>

<span data-ttu-id="fd404-104">Найдите сведения о **GetImItems** операции веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="fd404-104">Find information about the **GetImItems** EWS operation.</span></span> 
  
<span data-ttu-id="fd404-105">Операция **GetImItems** извлекаются сведения о группах мгновенного обмена мгновенными сообщениями и обмена мгновенными Сообщениями контактов пользователей.</span><span class="sxs-lookup"><span data-stu-id="fd404-105">The **GetImItems** operation retrieves information about instant messaging (IM) groups and IM contact personas.</span></span> 
  
<span data-ttu-id="fd404-106">Эта операция появилась в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="fd404-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-getimitems-operation"></a><span data-ttu-id="fd404-107">С помощью операции GetImItems</span><span class="sxs-lookup"><span data-stu-id="fd404-107">Using the GetImItems operation</span></span>

<span data-ttu-id="fd404-108">Операция **GetImItems** принимает группы и контакт item идентификаторы и возвращает набор сведений о групп и контактов.</span><span class="sxs-lookup"><span data-stu-id="fd404-108">The **GetImItems** operation accepts group and contact item identifiers and returns a set of information about the groups and contacts.</span></span> <span data-ttu-id="fd404-109">Наборы свойств, возвращаемого в ответе идентификатор расширенные свойства, несколько контактов идентификаторов идентификаторы групп и расширенные определения свойств в качестве аргументов.</span><span class="sxs-lookup"><span data-stu-id="fd404-109">The property sets returned in the response are identified by extended properties, multiple contact identifiers, group identifiers, and extended property definitions as arguments.</span></span> 
  
### <a name="getimitems-operation-soap-headers"></a><span data-ttu-id="fd404-110">Заголовки SOAP GetImItems операции</span><span class="sxs-lookup"><span data-stu-id="fd404-110">GetImItems operation SOAP headers</span></span>

<span data-ttu-id="fd404-111">Операция **GetImItems** можно использовать заголовки SOAP, которые перечислены в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="fd404-111">The **GetImItems** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="fd404-112">**Имя заголовка**</span><span class="sxs-lookup"><span data-stu-id="fd404-112">**Header name**</span></span>|<span data-ttu-id="fd404-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="fd404-113">**Element**</span></span>|<span data-ttu-id="fd404-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="fd404-114">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="fd404-115">**Олицетворение**</span><span class="sxs-lookup"><span data-stu-id="fd404-115">**Impersonation**</span></span> <br/> |[<span data-ttu-id="fd404-116">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="fd404-116">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="fd404-117">Идентифицирует пользователя, которого олицетворения в клиентском приложении.</span><span class="sxs-lookup"><span data-stu-id="fd404-117">Identifies the user whom the client application is impersonating.</span></span> <span data-ttu-id="fd404-118">Этот заголовок можно применять к запросу.</span><span class="sxs-lookup"><span data-stu-id="fd404-118">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="fd404-119">**MailboxCulture**</span><span class="sxs-lookup"><span data-stu-id="fd404-119">**MailboxCulture**</span></span> <br/> |[<span data-ttu-id="fd404-120">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="fd404-120">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="fd404-121">Определяет язык и региональные параметры, как определено в RFC 3066, «Теги для идентификации языков», который будет использоваться для доступа к почтовому ящику.</span><span class="sxs-lookup"><span data-stu-id="fd404-121">Identifies the culture, as defined in RFC 3066, "Tags for the Identification of Languages", to be used to access the mailbox.</span></span> <span data-ttu-id="fd404-122">Этот заголовок можно применять к запросу.</span><span class="sxs-lookup"><span data-stu-id="fd404-122">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="fd404-123">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="fd404-123">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="fd404-124">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="fd404-124">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="fd404-125">Определяет версию схемы для операции запроса.</span><span class="sxs-lookup"><span data-stu-id="fd404-125">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="fd404-126">Этот заголовок можно применять к запросу.</span><span class="sxs-lookup"><span data-stu-id="fd404-126">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="fd404-127">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="fd404-127">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="fd404-128">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="fd404-128">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="fd404-129">Определяет версию сервера, ответившего на запрос.</span><span class="sxs-lookup"><span data-stu-id="fd404-129">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="fd404-130">Этот заголовок можно применять, чтобы получить ответ.</span><span class="sxs-lookup"><span data-stu-id="fd404-130">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="getimitems-operation-request-example-get-detailed-information-about-im-contacts-and-groups"></a><span data-ttu-id="fd404-131">Пример запроса GetImItems операции: получить подробные сведения о служб обмена мгновенными сообщениями и группы</span><span class="sxs-lookup"><span data-stu-id="fd404-131">GetImItems operation request example: Get detailed information about IM contacts and groups</span></span>

<span data-ttu-id="fd404-132">В следующем примере запрос операции **GetImItems** показано, как запросить подробные сведения о служб обмена мгновенными сообщениями и группы.</span><span class="sxs-lookup"><span data-stu-id="fd404-132">The following example of a **GetImItems** operation request shows how to request detailed information about IM contacts and groups.</span></span> <span data-ttu-id="fd404-133">Операция **GetImItems** можно запросить один или несколько контактов или группу подробные сведения.</span><span class="sxs-lookup"><span data-stu-id="fd404-133">A **GetImItems** operation can request one or more contact or group details.</span></span> <span data-ttu-id="fd404-134">Расширенные свойства можно также использовать для получения настраиваемых свойств на групп и контактов.</span><span class="sxs-lookup"><span data-stu-id="fd404-134">You can also use extended properties to get custom properties on groups and contacts.</span></span> <span data-ttu-id="fd404-135">Если запрошенный расширенные свойства не существует на элемент, ответ игнорировать нужное свойство и возвратить ответ для набора свойств по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="fd404-135">If a requested extended property does not exist on an item, the response will ignore the requested property and return the response for the default property set.</span></span> <span data-ttu-id="fd404-136">В этом примере показано, как для получения отображаемых имен с помощью расширенных свойств.</span><span class="sxs-lookup"><span data-stu-id="fd404-136">This example shows you how to get the display name by using extended properties.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="fd404-137">Все идентификаторы элементов и ключей изменения в этой статье URL были сокращены, чтобы сохранить удобочитаемость.</span><span class="sxs-lookup"><span data-stu-id="fd404-137">All item identifiers and change keys in this article have been shortened to preserve readability.</span></span> <span data-ttu-id="fd404-138">Обратите внимание, что изменения ключей игнорируются службой для этой операции.</span><span class="sxs-lookup"><span data-stu-id="fd404-138">Note that change keys are ignored by the service for this operation.</span></span> 
  
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
      <m:GetImItems>
         <m:ContactIds>
            <t:ItemId Id="AAMkADEzOTExYACABmEhpSAAA=" ChangeKey="EQAAABBmNDjF"/>
         </m:ContactIds>
         <m:GroupIds>
            <t:ItemId Id="AAMkADEzOTExYjJkBY7+0EAAA=" ChangeKey="EgAAAA=="/>
         </m:GroupIds>         
         <m:ExtendedProperties>
            <t:ExtendedProperty PropertyTag="0x3001" PropertyType="String"/>
         </m:ExtendedProperties>
      </m:GetImItems>
   </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="fd404-139">Запрос SOAP body содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="fd404-139">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="fd404-140">GetImItems</span><span class="sxs-lookup"><span data-stu-id="fd404-140">GetImItems</span></span>](getimitems.md)
    
- [<span data-ttu-id="fd404-141">ContactIds</span><span class="sxs-lookup"><span data-stu-id="fd404-141">ContactIds</span></span>](contactids.md)
    
- [<span data-ttu-id="fd404-142">Идентификатор элемента</span><span class="sxs-lookup"><span data-stu-id="fd404-142">ItemId</span></span>](itemid.md)
    
- [<span data-ttu-id="fd404-143">GroupIds</span><span class="sxs-lookup"><span data-stu-id="fd404-143">GroupIds</span></span>](groupids.md)
    
- [<span data-ttu-id="fd404-144">Свойство ExtendedProperties (NonEmptyArrayOfExtendedFieldURIs)</span><span class="sxs-lookup"><span data-stu-id="fd404-144">ExtendedProperties (NonEmptyArrayOfExtendedFieldURIs)</span></span>](extendedproperties-nonemptyarrayofextendedfielduris.md)
    
- [<span data-ttu-id="fd404-145">ExtendedProperty (PathToExtendedFieldType)</span><span class="sxs-lookup"><span data-stu-id="fd404-145">ExtendedProperty (PathToExtendedFieldType)</span></span>](extendedproperty-pathtoextendedfieldtype.md)
    
## <a name="successful-getimitems-operation-response"></a><span data-ttu-id="fd404-146">Успешные операции ответа GetImItems</span><span class="sxs-lookup"><span data-stu-id="fd404-146">Successful GetImItems operation response</span></span>

<span data-ttu-id="fd404-147">В следующем примере показано успешного ответа на запрос **GetImItems** для получения системы мгновенных сообщений и группы.</span><span class="sxs-lookup"><span data-stu-id="fd404-147">The following example shows a successful response to a **GetImItems** request to get an IM contact and group.</span></span> <span data-ttu-id="fd404-148">Отображаемое имя запрашивается в расширенном свойстве.</span><span class="sxs-lookup"><span data-stu-id="fd404-148">The display name is requested in an extended property.</span></span> <span data-ttu-id="fd404-149">Мгновенные сообщения контактам возвращаются в виде пользователя.</span><span class="sxs-lookup"><span data-stu-id="fd404-149">IM contacts are returned in the form of a persona.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="556" 
                           MinorBuildNumber="8" 
                           Version="Exchange2013" 
                           xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <GetImItemsResponse ResponseClass="Success" 
                          xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
         <ImItemList>
            <Groups xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
               <ImGroup>
                  <DisplayName>Exchange SDK Team</DisplayName>
                  <GroupType>IPM.DistList.MOC.UserGroup</GroupType>
                  <ExchangeStoreId Id="AAMkADEzQrAABY7+0EAAA=" ChangeKey="EgAAAA=="/>
                  <MemberCorrelationKey>
                     <ItemId Id="AAMkADEzOTExYjeGgGqm4QrAABmEhpSAAA=" ChangeKey="EQAAAA=="/>
                  </MemberCorrelationKey>
                  <ExtendedProperties>
                     <ExtendedProperty>
                        <ExtendedFieldURI PropertyTag="0x3001" PropertyType="String"/>
                        <Value>Exchange SDK Team</Value>
                     </ExtendedProperty>
                  </ExtendedProperties>
               </ImGroup>
            </Groups>
            <Personas xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
               <Persona>
                  <PersonaId Id="AAQkADEzOTBZImBzN5J/uHXc="/>
                  <PersonaType>Person</PersonaType>
                  <CreationTime>2012-11-07T00:10:35Z</CreationTime>
                  <DisplayName>Tony Smith</DisplayName>
                  <DisplayNameFirstLast>Tony Smith</DisplayNameFirstLast>
                  <DisplayNameLastFirst>Tony Smith</DisplayNameLastFirst>
                  <FileAs/>
                  <FileAsId>None</FileAsId>
                  <ImAddress>tsmith@contoso.com</ImAddress>
                  <RelevanceScore>2147483647</RelevanceScore>
                  <Attributions>
                     <Attribution>
                        <Id>0</Id>
                        <SourceId Id="AAMkADEzhQaoeGgGqm4QrAABmEhpSAAA=" ChangeKey="EQArAABmNDjF"/>
                        <DisplayName>Lync Contacts</DisplayName>
                        <IsWritable>false</IsWritable>
                        <IsQuickContact>true</IsQuickContact>
                        <IsHidden>false</IsHidden>
                     </Attribution>
                  </Attributions>
                  <DisplayNames>
                     <StringAttributedValue>
                        <Value>Tony Smith</Value>
                        <Attributions>
                           <Attribution>0</Attribution>
                        </Attributions>
                     </StringAttributedValue>
                  </DisplayNames>
                  <FileAsIds>
                     <StringAttributedValue>
                        <Value>None</Value>
                        <Attributions>
                           <Attribution>0</Attribution>
                        </Attributions>
                     </StringAttributedValue>
                  </FileAsIds>
                  <ImAddresses>
                     <StringAttributedValue>
                        <Value>tsmith@contoso.com</Value>
                        <Attributions>
                           <Attribution>0</Attribution>
                        </Attributions>
                     </StringAttributedValue>
                  </ImAddresses>
                  <ExtendedProperties>
                     <ExtendedPropertyAttributedValue>
                        <Value>
                           <ExtendedFieldURI PropertyTag="0x3001" PropertyType="String"/>
                           <Value>Tony Smith</Value>
                        </Value>
                        <Attributions>
                           <Attribution>0</Attribution>
                        </Attributions>
                     </ExtendedPropertyAttributedValue>
                  </ExtendedProperties>
               </Persona>
            </Personas>
         </ImItemList>
      </GetImItemsResponse>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="fd404-150">Ответ SOAP body содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="fd404-150">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="fd404-151">GetImItemsResponse</span><span class="sxs-lookup"><span data-stu-id="fd404-151">GetImItemsResponse</span></span>](getimitemsresponse.md)
    
- [<span data-ttu-id="fd404-152">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="fd404-152">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="fd404-153">ImItemList</span><span class="sxs-lookup"><span data-stu-id="fd404-153">ImItemList</span></span>](imitemlist.md)
    
- [<span data-ttu-id="fd404-154">Группы (ArrayOfImGroupType)</span><span class="sxs-lookup"><span data-stu-id="fd404-154">Groups (ArrayOfImGroupType)</span></span>](groups-arrayofimgrouptype.md)
    
- [<span data-ttu-id="fd404-155">ImGroup</span><span class="sxs-lookup"><span data-stu-id="fd404-155">ImGroup</span></span>](imgroup.md)
    
- [<span data-ttu-id="fd404-156">Отображаемое имя (строка)</span><span class="sxs-lookup"><span data-stu-id="fd404-156">DisplayName (string)</span></span>](displayname-string.md)
    
- [<span data-ttu-id="fd404-157">GroupType</span><span class="sxs-lookup"><span data-stu-id="fd404-157">GroupType</span></span>](grouptype.md)
    
- [<span data-ttu-id="fd404-158">ExchangeStoreId</span><span class="sxs-lookup"><span data-stu-id="fd404-158">ExchangeStoreId</span></span>](exchangestoreid.md)
    
- [<span data-ttu-id="fd404-159">MemberCorrelationKey</span><span class="sxs-lookup"><span data-stu-id="fd404-159">MemberCorrelationKey</span></span>](membercorrelationkey.md)
    
- [<span data-ttu-id="fd404-160">Идентификатор элемента</span><span class="sxs-lookup"><span data-stu-id="fd404-160">ItemId</span></span>](itemid.md)
    
- [<span data-ttu-id="fd404-161">Свойство ExtendedProperties (NonEmptyArrayOfExtendedFieldURIs)</span><span class="sxs-lookup"><span data-stu-id="fd404-161">ExtendedProperties (NonEmptyArrayOfExtendedFieldURIs)</span></span>](extendedproperties-nonemptyarrayofextendedfielduris.md)
    
- [<span data-ttu-id="fd404-162">ExtendedProperty (PathToExtendedFieldType)</span><span class="sxs-lookup"><span data-stu-id="fd404-162">ExtendedProperty (PathToExtendedFieldType)</span></span>](extendedproperty-pathtoextendedfieldtype.md)
    
- [<span data-ttu-id="fd404-163">Действующие лица</span><span class="sxs-lookup"><span data-stu-id="fd404-163">Personas</span></span>](personas-ex15websvcsotherref.md)
    
- [<span data-ttu-id="fd404-164">PersonaId</span><span class="sxs-lookup"><span data-stu-id="fd404-164">PersonaId</span></span>](personaid.md)
    
- [<span data-ttu-id="fd404-165">PersonaType</span><span class="sxs-lookup"><span data-stu-id="fd404-165">PersonaType</span></span>](personatype.md)
    
- [<span data-ttu-id="fd404-166">CreationTime</span><span class="sxs-lookup"><span data-stu-id="fd404-166">CreationTime</span></span>](creationtime.md)
    
- [<span data-ttu-id="fd404-167">DisplayNameFirstLast</span><span class="sxs-lookup"><span data-stu-id="fd404-167">DisplayNameFirstLast</span></span>](displaynamefirstlast.md)
    
- [<span data-ttu-id="fd404-168">DisplayNameLastFirst</span><span class="sxs-lookup"><span data-stu-id="fd404-168">DisplayNameLastFirst</span></span>](displaynamelastfirst.md)
    
- [<span data-ttu-id="fd404-169">FileAs</span><span class="sxs-lookup"><span data-stu-id="fd404-169">FileAs</span></span>](fileas.md)
    
- <span data-ttu-id="fd404-170">[FileAsId](fileasid.md) FileAsId</span><span class="sxs-lookup"><span data-stu-id="fd404-170">[FileAsId](fileasid.md) FileAsId</span></span> 
    
- [<span data-ttu-id="fd404-171">ImAddress (строка)</span><span class="sxs-lookup"><span data-stu-id="fd404-171">ImAddress (String)</span></span>](imaddress-string.md)
    
- [<span data-ttu-id="fd404-172">RelevanceScore</span><span class="sxs-lookup"><span data-stu-id="fd404-172">RelevanceScore</span></span>](relevancescore.md)
    
- [<span data-ttu-id="fd404-173">Атрибуты (ArrayOfPersonaAttributionsType)</span><span class="sxs-lookup"><span data-stu-id="fd404-173">Attributions (ArrayOfPersonaAttributionsType)</span></span>](attributions-arrayofpersonaattributionstype.md)
    
- [<span data-ttu-id="fd404-174">Атрибуты (PersonaAttributionType)</span><span class="sxs-lookup"><span data-stu-id="fd404-174">Attribution (PersonaAttributionType)</span></span>](attribution-personaattributiontype.md)
    
- [<span data-ttu-id="fd404-175">Идентификатор (строка)</span><span class="sxs-lookup"><span data-stu-id="fd404-175">ID (String)</span></span>](id-string.md)
    
- [<span data-ttu-id="fd404-176">SourceId</span><span class="sxs-lookup"><span data-stu-id="fd404-176">SourceId</span></span>](sourceid.md)
    
- [<span data-ttu-id="fd404-177">IsWritable</span><span class="sxs-lookup"><span data-stu-id="fd404-177">IsWritable</span></span>](iswritable.md)
    
- [<span data-ttu-id="fd404-178">IsQuickContact</span><span class="sxs-lookup"><span data-stu-id="fd404-178">IsQuickContact</span></span>](isquickcontact.md)
    
- [<span data-ttu-id="fd404-179">IsHidden</span><span class="sxs-lookup"><span data-stu-id="fd404-179">IsHidden</span></span>](ishidden.md)
    
- [<span data-ttu-id="fd404-180">StringAttributedValue</span><span class="sxs-lookup"><span data-stu-id="fd404-180">StringAttributedValue</span></span>](stringattributedvalue.md)
    
- [<span data-ttu-id="fd404-181">FileAsIds</span><span class="sxs-lookup"><span data-stu-id="fd404-181">FileAsIds</span></span>](fileasids.md)
    
- [<span data-ttu-id="fd404-182">ImAddresses</span><span class="sxs-lookup"><span data-stu-id="fd404-182">ImAddresses</span></span>](imaddresses.md)
    
- [<span data-ttu-id="fd404-183">Значение (ExtendedPropertyType)</span><span class="sxs-lookup"><span data-stu-id="fd404-183">Value (ExtendedPropertyType)</span></span>](value-extendedpropertytype.md)
    
## <a name="getimitems-operation-error-response"></a><span data-ttu-id="fd404-184">Ошибка операции GetImItems ответа</span><span class="sxs-lookup"><span data-stu-id="fd404-184">GetImItems operation error response</span></span>

<span data-ttu-id="fd404-185">Операция **GetImItems** не выполняет проверку идентификаторы и не возвращает ожидаемых **ErrorInvalidImContactId** или **ErrorInvalidImGroupId** ответ на ошибку, если недопустимый контакт или идентификатор группы предоставляется в службу.</span><span class="sxs-lookup"><span data-stu-id="fd404-185">The **GetImItems** operation does not validate identifiers and will not return the expected **ErrorInvalidImContactId** or **ErrorInvalidImGroupId** error response if an invalid contact or group identifier is provided to the service.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="fd404-186">См. также</span><span class="sxs-lookup"><span data-stu-id="fd404-186">See also</span></span>

- [<span data-ttu-id="fd404-187">Операции EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="fd404-187">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
    
- [<span data-ttu-id="fd404-188">Операция GetImItemList</span><span class="sxs-lookup"><span data-stu-id="fd404-188">GetImItemList operation</span></span>](getimitemlist-operation.md)
    

