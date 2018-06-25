---
title: Операция GetPersona
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: e2146df0-53d0-4caf-9758-b600bbc14b6a
description: Найдите сведения о веб-служб Exchange GetPersona операции.
ms.openlocfilehash: c6ac357eaa34e9bae2fe0a79a4a2d02449100e78
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762886"
---
# <a name="getpersona-operation"></a><span data-ttu-id="49da7-103">Операция GetPersona</span><span class="sxs-lookup"><span data-stu-id="49da7-103">GetPersona operation</span></span>

<span data-ttu-id="49da7-104">Найдите сведения о **GetPersona** операции веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="49da7-104">Find information about the **GetPersona** EWS operation.</span></span> 
  
<span data-ttu-id="49da7-105">Операция **GetPersona** возвращает набор свойств, связанных с пользователя.</span><span class="sxs-lookup"><span data-stu-id="49da7-105">The **GetPersona** operation returns a set of properties that are associated with a persona.</span></span> 
  
<span data-ttu-id="49da7-106">Эта операция появилась в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="49da7-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-getpersona-operation"></a><span data-ttu-id="49da7-107">С помощью операции GetPersona</span><span class="sxs-lookup"><span data-stu-id="49da7-107">Using the GetPersona operation</span></span>

<span data-ttu-id="49da7-108">Операция **GetPersona** предоставляет доступ к статистическим контактные данные в форме пользователя.</span><span class="sxs-lookup"><span data-stu-id="49da7-108">The **GetPersona** operation provides access to aggregated contact information in the form of a persona.</span></span> <span data-ttu-id="49da7-109">Элемент [PersonaId](personaid.md) в запросе идентифицирует пользователя, чтобы вернуться в ответе.</span><span class="sxs-lookup"><span data-stu-id="49da7-109">The [PersonaId](personaid.md) element in the request identifies the persona to return in the response.</span></span> <span data-ttu-id="49da7-110">Ответ может содержать набор свойств пользователя по умолчанию или набор пользовательских свойств.</span><span class="sxs-lookup"><span data-stu-id="49da7-110">The response can contain a default set of persona properties or a custom property set.</span></span> <span data-ttu-id="49da7-111">Рекомендуется указать настраиваемое свойство задать, чтобы неиспользуемые свойства не обрабатываются и отправляются клиенту с сервера.</span><span class="sxs-lookup"><span data-stu-id="49da7-111">We recommend that you specify a custom property set so that unused properties are not processed and sent from the server to the client.</span></span> 
  
### <a name="getpersona-operation-soap-headers"></a><span data-ttu-id="49da7-112">Заголовки SOAP GetPersona операции</span><span class="sxs-lookup"><span data-stu-id="49da7-112">GetPersona operation SOAP headers</span></span>

<span data-ttu-id="49da7-113">Операция **GetPersona** можно использовать заголовки SOAP, которые перечислены в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="49da7-113">The **GetPersona** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="49da7-114">**Имя заголовка**</span><span class="sxs-lookup"><span data-stu-id="49da7-114">**Header name**</span></span>|<span data-ttu-id="49da7-115">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="49da7-115">**Element**</span></span>|<span data-ttu-id="49da7-116">**Описание**</span><span class="sxs-lookup"><span data-stu-id="49da7-116">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="49da7-117">**Олицетворение**</span><span class="sxs-lookup"><span data-stu-id="49da7-117">**Impersonation**</span></span> <br/> |[<span data-ttu-id="49da7-118">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="49da7-118">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="49da7-119">Идентифицирует пользователя, которого олицетворения в клиентском приложении.</span><span class="sxs-lookup"><span data-stu-id="49da7-119">Identifies the user whom the client application is impersonating.</span></span> <span data-ttu-id="49da7-120">Этот заголовок можно применять к запросу.</span><span class="sxs-lookup"><span data-stu-id="49da7-120">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="49da7-121">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="49da7-121">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="49da7-122">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="49da7-122">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="49da7-123">Определяет версию схемы для операции запроса.</span><span class="sxs-lookup"><span data-stu-id="49da7-123">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="49da7-124">Этот заголовок можно применять к запросу.</span><span class="sxs-lookup"><span data-stu-id="49da7-124">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="49da7-125">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="49da7-125">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="49da7-126">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="49da7-126">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="49da7-127">Определяет версию сервера, ответившего на запрос.</span><span class="sxs-lookup"><span data-stu-id="49da7-127">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="49da7-128">Этот заголовок можно применять, чтобы получить ответ.</span><span class="sxs-lookup"><span data-stu-id="49da7-128">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="getpersona-operation-request-example-return-a-default-set-of-properties-for-a-persona"></a><span data-ttu-id="49da7-129">Пример запроса GetPersona операции: возврата по умолчанию набор свойств для пользователя</span><span class="sxs-lookup"><span data-stu-id="49da7-129">GetPersona operation request example: Return a default set of properties for a persona</span></span>

<span data-ttu-id="49da7-130">В следующем примере запрос операции **GetPersona** показано, как для возврата по умолчанию набор свойств, связанных с пользователя.</span><span class="sxs-lookup"><span data-stu-id="49da7-130">The following example of a **GetPersona** operation request shows how to return a default set of properties that are associated with a persona.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013"/>
   </soap:Header>
   <soap:Body xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <GetPersona>
         <PersonaId Id="AAQkADEzAQAKtOtR/l4MlLqHWORfhSYKU="/>
      </GetPersona>
   </soap:Body>
</soap:Envelope>

```

<span data-ttu-id="49da7-131">Ответ SOAP body содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="49da7-131">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="49da7-132">GetPersona</span><span class="sxs-lookup"><span data-stu-id="49da7-132">GetPersona</span></span>](getpersona.md)
    
- [<span data-ttu-id="49da7-133">PersonaId</span><span class="sxs-lookup"><span data-stu-id="49da7-133">PersonaId</span></span>](personaid.md)
    
## <a name="successful-getpersona-operation-response"></a><span data-ttu-id="49da7-134">Успешные операции ответа GetPersona</span><span class="sxs-lookup"><span data-stu-id="49da7-134">Successful GetPersona operation response</span></span>

<span data-ttu-id="49da7-135">В следующем примере показано успешного ответа на запрос операции **GetPersona** .</span><span class="sxs-lookup"><span data-stu-id="49da7-135">The following example shows a successful response to a **GetPersona** operation request.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="49da7-136">Все идентификаторы элементов и ключей изменения в этой статье URL были сокращены, чтобы сохранить удобочитаемость.</span><span class="sxs-lookup"><span data-stu-id="49da7-136">All item identifiers and change keys in this article have been shortened to preserve readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="432" 
                           MinorBuildNumber="5" 
                           Version="Exchange2013"
                           xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types"
                     xmlns="http://schemas.microsoft.com/exchange/services/2006/types"
      xmlns:xsd="http://www.w3.org/2001/XMLSchema"
         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <GetPersonaResponseMessage ResponseClass="Success"
                      xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
         <Persona>
            <PersonaId Id="AAQkADEzAQAKtOtR="
              xmlns="http://schemas.microsoft.com/exchange/services/2006/types"/>
            <PersonaType xmlns="http://schemas.microsoft.com/exchange/services/2006/types">Person</PersonaType>
            <CreationTime xmlns="http://schemas.microsoft.com/exchange/services/2006/types">2012-06-01T17:00:34Z</CreationTime>
            <DisplayName xmlns="http://schemas.microsoft.com/exchange/services/2006/types">Brian Johnson</DisplayName>
            <DisplayNameFirstLast xmlns="http://schemas.microsoft.com/exchange/services/2006/types">Brian Johnson</DisplayNameFirstLast>
            <DisplayNameLastFirst xmlns="http://schemas.microsoft.com/exchange/services/2006/types">Johnson Brian</DisplayNameLastFirst>
            <FileAs xmlns="http://schemas.microsoft.com/exchange/services/2006/types">Johnson, Brian</FileAs>
            <FileAsId xmlns="http://schemas.microsoft.com/exchange/services/2006/types">None</FileAsId>
            <GivenName xmlns="http://schemas.microsoft.com/exchange/services/2006/types">Brian</GivenName>
            <Surname xmlns="http://schemas.microsoft.com/exchange/services/2006/types">Johnsoon</Surname>
            <CompanyName xmlns="http://schemas.microsoft.com/exchange/services/2006/types">Contoso</CompanyName>
            <RelevanceScore xmlns="http://schemas.microsoft.com/exchange/services/2006/types">4255550110</RelevanceScore>
            <Attributions xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
               <Attribution>
                  <Id>0</Id>
                  <SourceId Id="AAMkA =" ChangeKey="EQAAABY+"/>
                  <DisplayName>Outlook</DisplayName>
                  <IsWritable>true</IsWritable>
                  <IsQuickContact>false</IsQuickContact>
                  <IsHidden>false</IsHidden>
                  <FolderId Id="AAMkA=" ChangeKey="AQAAAA=="/>
               </Attribution>
            </Attributions>
            <DisplayNames xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
               <StringAttributedValue>
                  <Value>Brian Johnson</Value>
                  <Attributions>
                     <Attribution>0</Attribution>
                  </Attributions>
               </StringAttributedValue>
            </DisplayNames>
            <FileAses xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
               <StringAttributedValue>
                  <Value>Johnson, Brian</Value>
                  <Attributions>
                     <Attribution>0</Attribution>
                  </Attributions>
               </StringAttributedValue>
            </FileAses>
            <FileAsIds xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
               <StringAttributedValue>
                  <Value>None</Value>
                  <Attributions>
                     <Attribution>0</Attribution>
                  </Attributions>
               </StringAttributedValue>
            </FileAsIds>
            <GivenNames xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
               <StringAttributedValue>
                  <Value>Brian</Value>
                  <Attributions>
                     <Attribution>0</Attribution>
                  </Attributions>
               </StringAttributedValue>
            </GivenNames>
            <Surnames xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
               <StringAttributedValue>
                  <Value>Johnson</Value>
                  <Attributions>
                     <Attribution>0</Attribution>
                  </Attributions>
               </StringAttributedValue>
            </Surnames>
            <MobilePhones xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
               <PhoneNumberAttributedValue>
                  <Value>
                     <Number>(425)555-0110</Number>
                     <Type>Mobile</Type>
                  </Value>
                  <Attributions>
                     <Attribution>0</Attribution>
                  </Attributions>
               </PhoneNumberAttributedValue>
            </MobilePhones>
            <CompanyNames xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
               <StringAttributedValue>
                  <Value>Contoso</Value>
                  <Attributions>
                     <Attribution>0</Attribution>
                  </Attributions>
               </StringAttributedValue>
            </CompanyNames>
         </Persona>
      </GetPersonaResponseMessage>
   </s:Body>
</s:Envelope>

```

<span data-ttu-id="49da7-137">Ответ SOAP body содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="49da7-137">The response SOAP body contains the following elements:</span></span>
  
- <span data-ttu-id="49da7-138">GetPersonaResponseMessage</span><span class="sxs-lookup"><span data-stu-id="49da7-138">GetPersonaResponseMessage</span></span>
    
- [<span data-ttu-id="49da7-139">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="49da7-139">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="49da7-140">Пользователь</span><span class="sxs-lookup"><span data-stu-id="49da7-140">Persona</span></span>](persona.md)
    
- [<span data-ttu-id="49da7-141">PersonaId</span><span class="sxs-lookup"><span data-stu-id="49da7-141">PersonaId</span></span>](personaid.md)
    
- [<span data-ttu-id="49da7-142">PersonaType</span><span class="sxs-lookup"><span data-stu-id="49da7-142">PersonaType</span></span>](personatype.md)
    
- [<span data-ttu-id="49da7-143">CreationTime</span><span class="sxs-lookup"><span data-stu-id="49da7-143">CreationTime</span></span>](creationtime.md)
    
- [<span data-ttu-id="49da7-144">DisplayNameFirstLast</span><span class="sxs-lookup"><span data-stu-id="49da7-144">DisplayNameFirstLast</span></span>](displaynamefirstlast.md)
    
- [<span data-ttu-id="49da7-145">DisplayNameLastFirst</span><span class="sxs-lookup"><span data-stu-id="49da7-145">DisplayNameLastFirst</span></span>](displaynamelastfirst.md)
    
- [<span data-ttu-id="49da7-146">FileAs</span><span class="sxs-lookup"><span data-stu-id="49da7-146">FileAs</span></span>](fileas.md)
    
- [<span data-ttu-id="49da7-147">FileAsId</span><span class="sxs-lookup"><span data-stu-id="49da7-147">FileAsId</span></span>](fileasid.md)
    
- [<span data-ttu-id="49da7-148">GivenName</span><span class="sxs-lookup"><span data-stu-id="49da7-148">GivenName</span></span>](givenname.md)
    
- [<span data-ttu-id="49da7-149">Фамилия</span><span class="sxs-lookup"><span data-stu-id="49da7-149">Surname</span></span>](surname.md)
    
- [<span data-ttu-id="49da7-150">Название организации</span><span class="sxs-lookup"><span data-stu-id="49da7-150">CompanyName</span></span>](companyname.md)
    
- [<span data-ttu-id="49da7-151">RelevanceScore</span><span class="sxs-lookup"><span data-stu-id="49da7-151">RelevanceScore</span></span>](relevancescore.md)
    
- [<span data-ttu-id="49da7-152">Атрибуты (ArrayOfValueAttributionsType)</span><span class="sxs-lookup"><span data-stu-id="49da7-152">Attributions (ArrayOfValueAttributionsType)</span></span>](attributions-arrayofvalueattributionstype.md)
    
- [<span data-ttu-id="49da7-153">Атрибуты (строка)</span><span class="sxs-lookup"><span data-stu-id="49da7-153">Attribution (string)</span></span>](attribution-string.md)
    
- [<span data-ttu-id="49da7-154">Идентификатор (строка)</span><span class="sxs-lookup"><span data-stu-id="49da7-154">ID (String)</span></span>](id-string.md)
    
- <span data-ttu-id="49da7-155">[SourceId](sourceid.md) SourceId</span><span class="sxs-lookup"><span data-stu-id="49da7-155">[SourceId](sourceid.md) SourceId</span></span> 
    
- [<span data-ttu-id="49da7-156">Отображаемое имя (строка)</span><span class="sxs-lookup"><span data-stu-id="49da7-156">DisplayName (string)</span></span>](displayname-string.md)
    
- [<span data-ttu-id="49da7-157">IsWritable</span><span class="sxs-lookup"><span data-stu-id="49da7-157">IsWritable</span></span>](iswritable.md)
    
- [<span data-ttu-id="49da7-158">IsQuickContact</span><span class="sxs-lookup"><span data-stu-id="49da7-158">IsQuickContact</span></span>](isquickcontact.md)
    
- [<span data-ttu-id="49da7-159">IsHidden</span><span class="sxs-lookup"><span data-stu-id="49da7-159">IsHidden</span></span>](ishidden.md)
    
- [<span data-ttu-id="49da7-160">FolderId</span><span class="sxs-lookup"><span data-stu-id="49da7-160">FolderId</span></span>](folderid.md)
    
- [<span data-ttu-id="49da7-161">DisplayNames</span><span class="sxs-lookup"><span data-stu-id="49da7-161">DisplayNames</span></span>](displaynames.md)
    
- [<span data-ttu-id="49da7-162">StringAttributedValue</span><span class="sxs-lookup"><span data-stu-id="49da7-162">StringAttributedValue</span></span>](stringattributedvalue.md)
    
- [<span data-ttu-id="49da7-163">Значение (ArrayOfStringValueType)</span><span class="sxs-lookup"><span data-stu-id="49da7-163">Value (ArrayOfStringValueType)</span></span>](value-arrayofstringvaluetype.md)
    
- [<span data-ttu-id="49da7-164">Атрибуты (ArrayOfPersonaAttributionsType)</span><span class="sxs-lookup"><span data-stu-id="49da7-164">Attributions (ArrayOfPersonaAttributionsType)</span></span>](attributions-arrayofpersonaattributionstype.md)
    
- [<span data-ttu-id="49da7-165">Атрибуты (PersonaAttributionType)</span><span class="sxs-lookup"><span data-stu-id="49da7-165">Attribution (PersonaAttributionType)</span></span>](attribution-personaattributiontype.md)
    
- [<span data-ttu-id="49da7-166">FileAses</span><span class="sxs-lookup"><span data-stu-id="49da7-166">FileAses</span></span>](fileases.md)
    
- [<span data-ttu-id="49da7-167">FileAsIds</span><span class="sxs-lookup"><span data-stu-id="49da7-167">FileAsIds</span></span>](fileasids.md)
    
- [<span data-ttu-id="49da7-168">GivenNames</span><span class="sxs-lookup"><span data-stu-id="49da7-168">GivenNames</span></span>](givennames.md)
    
- [<span data-ttu-id="49da7-169">Фамилии</span><span class="sxs-lookup"><span data-stu-id="49da7-169">Surnames</span></span>](surnames.md)
    
- [<span data-ttu-id="49da7-170">MobilePhones</span><span class="sxs-lookup"><span data-stu-id="49da7-170">MobilePhones</span></span>](mobilephones.md)
    
- [<span data-ttu-id="49da7-171">PhoneNumberAttributedValue</span><span class="sxs-lookup"><span data-stu-id="49da7-171">PhoneNumberAttributedValue</span></span>](phonenumberattributedvalue.md)
    
- [<span data-ttu-id="49da7-172">Значение (PersonaPhoneNumberType)</span><span class="sxs-lookup"><span data-stu-id="49da7-172">Value (PersonaPhoneNumberType)</span></span>](value-personaphonenumbertype.md)
    
- [<span data-ttu-id="49da7-173">Число</span><span class="sxs-lookup"><span data-stu-id="49da7-173">Number</span></span>](number.md)
    
- [<span data-ttu-id="49da7-174">Тип (строка)</span><span class="sxs-lookup"><span data-stu-id="49da7-174">Type (string)</span></span>](type-string.md)
    
- [<span data-ttu-id="49da7-175">CompanyNames</span><span class="sxs-lookup"><span data-stu-id="49da7-175">CompanyNames</span></span>](companynames.md)
    
## <a name="getpersona-operation-error-response"></a><span data-ttu-id="49da7-176">Ошибка операции GetPersona ответа</span><span class="sxs-lookup"><span data-stu-id="49da7-176">GetPersona operation error response</span></span>

<span data-ttu-id="49da7-177">В следующем примере показано ошибочный ответ на запрос операции **GetPersona** .</span><span class="sxs-lookup"><span data-stu-id="49da7-177">The following example shows an error response to a **GetPersona** operation request.</span></span> <span data-ttu-id="49da7-178">Это ответ на запрос, содержащая идентификатор неправильно указанного пользователя.</span><span class="sxs-lookup"><span data-stu-id="49da7-178">This is a response to a request that contains an incorrectly specified persona identifier.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="578" 
                           MinorBuildNumber="11" 
                           Version="Exchange2013" 
                           xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <GetPersonaResponseMessage ResponseClass="Error" 
                                 xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>Id is malformed.</MessageText>
         <ResponseCode>ErrorInvalidIdMalformed</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
      </GetPersonaResponseMessage>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="49da7-179">Ошибка ответ SOAP body содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="49da7-179">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="49da7-180">GetPersonaResponseMessage</span><span class="sxs-lookup"><span data-stu-id="49da7-180">GetPersonaResponseMessage</span></span>](getpersonaresponsemessage.md)
    
- [<span data-ttu-id="49da7-181">MessageText</span><span class="sxs-lookup"><span data-stu-id="49da7-181">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="49da7-182">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="49da7-182">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="49da7-183">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="49da7-183">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
<span data-ttu-id="49da7-184">Дополнительные коды ошибок, которые являются общими для веб-служб Exchange и специально для этой операции в разделе [ResponseCode](responsecode.md).</span><span class="sxs-lookup"><span data-stu-id="49da7-184">For additional error codes that are generic to EWS and specific to this operation, see [ResponseCode](responsecode.md).</span></span>
  
## <a name="see-also"></a><span data-ttu-id="49da7-185">См. также</span><span class="sxs-lookup"><span data-stu-id="49da7-185">See also</span></span>

- [<span data-ttu-id="49da7-186">Операции EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="49da7-186">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
    
- [<span data-ttu-id="49da7-187">Пользователи и контакты в EWS для Exchange</span><span class="sxs-lookup"><span data-stu-id="49da7-187">People and contacts in EWS in Exchange</span></span>](http://msdn.microsoft.com/library/043c33be-a0d1-4bad-a840-85715eda4813%28Office.15%29.aspx)
    
- [<span data-ttu-id="49da7-188">Операция FindPeople</span><span class="sxs-lookup"><span data-stu-id="49da7-188">FindPeople operation</span></span>](findpeople-operation.md)
    

