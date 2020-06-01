---
title: Операция GetPersona
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: e2146df0-53d0-4caf-9758-b600bbc14b6a
description: Поиск сведений о работе EWS.
ms.openlocfilehash: 2b335c694a85f87c96432ea6d7c1c674613d2f17
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460948"
---
# <a name="getpersona-operation"></a><span data-ttu-id="715df-103">Операция GetPersona</span><span class="sxs-lookup"><span data-stu-id="715df-103">GetPersona operation</span></span>

<span data-ttu-id="715df-104">Поиск сведений о работе **EWS.**</span><span class="sxs-lookup"><span data-stu-id="715df-104">Find information about the **GetPersona** EWS operation.</span></span> 
  
<span data-ttu-id="715df-105">Операция **Доличного пользователя** возвращает набор свойств, связанных с пользователем.</span><span class="sxs-lookup"><span data-stu-id="715df-105">The **GetPersona** operation returns a set of properties that are associated with a persona.</span></span> 
  
<span data-ttu-id="715df-106">Эта операция появилась в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="715df-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-getpersona-operation"></a><span data-ttu-id="715df-107">Использование операции "@ Person"</span><span class="sxs-lookup"><span data-stu-id="715df-107">Using the GetPersona operation</span></span>

<span data-ttu-id="715df-108">Операция **GetPersona** долево предоставляет доступ к сводным сведениям о контакте в форме пользователя.</span><span class="sxs-lookup"><span data-stu-id="715df-108">The **GetPersona** operation provides access to aggregated contact information in the form of a persona.</span></span> <span data-ttu-id="715df-109">Элемент [персонаид](personaid.md) в запросе определяет пользователя, возвращаемого в ответе.</span><span class="sxs-lookup"><span data-stu-id="715df-109">The [PersonaId](personaid.md) element in the request identifies the persona to return in the response.</span></span> <span data-ttu-id="715df-110">Отклик может содержать набор свойств пользователя по умолчанию или набор настраиваемых свойств.</span><span class="sxs-lookup"><span data-stu-id="715df-110">The response can contain a default set of persona properties or a custom property set.</span></span> <span data-ttu-id="715df-111">Рекомендуется указать набор настраиваемых свойств, чтобы неиспользуемые свойства не обрабатывались и не отправлялись с сервера клиенту.</span><span class="sxs-lookup"><span data-stu-id="715df-111">We recommend that you specify a custom property set so that unused properties are not processed and sent from the server to the client.</span></span> 
  
### <a name="getpersona-operation-soap-headers"></a><span data-ttu-id="715df-112">Заголовки SOAP для операции с сотрудниками</span><span class="sxs-lookup"><span data-stu-id="715df-112">GetPersona operation SOAP headers</span></span>

<span data-ttu-id="715df-113">Операция **Доличного пользователя** может использовать заголовки SOAP, перечисленные в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="715df-113">The **GetPersona** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="715df-114">**Имя заголовка**</span><span class="sxs-lookup"><span data-stu-id="715df-114">**Header name**</span></span>|<span data-ttu-id="715df-115">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="715df-115">**Element**</span></span>|<span data-ttu-id="715df-116">**Описание**</span><span class="sxs-lookup"><span data-stu-id="715df-116">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="715df-117">**Олицетворение**</span><span class="sxs-lookup"><span data-stu-id="715df-117">**Impersonation**</span></span> <br/> |[<span data-ttu-id="715df-118">ексчанжеимперсонатион</span><span class="sxs-lookup"><span data-stu-id="715df-118">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="715df-119">Идентифицирует пользователя, который олицетворяет клиентское приложение.</span><span class="sxs-lookup"><span data-stu-id="715df-119">Identifies the user whom the client application is impersonating.</span></span> <span data-ttu-id="715df-120">Этот заголовок является применимым для запроса.</span><span class="sxs-lookup"><span data-stu-id="715df-120">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="715df-121">**рекуестверсион**</span><span class="sxs-lookup"><span data-stu-id="715df-121">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="715df-122">рекуестсерверверсион</span><span class="sxs-lookup"><span data-stu-id="715df-122">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="715df-123">Определяет версию схемы для запроса операции.</span><span class="sxs-lookup"><span data-stu-id="715df-123">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="715df-124">Этот заголовок является применимым для запроса.</span><span class="sxs-lookup"><span data-stu-id="715df-124">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="715df-125">**серверверсион**</span><span class="sxs-lookup"><span data-stu-id="715df-125">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="715df-126">серверверсионинфо</span><span class="sxs-lookup"><span data-stu-id="715df-126">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="715df-127">Определяет версию сервера, который ответил на запрос.</span><span class="sxs-lookup"><span data-stu-id="715df-127">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="715df-128">Этот заголовок является применимым для отклика.</span><span class="sxs-lookup"><span data-stu-id="715df-128">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="getpersona-operation-request-example-return-a-default-set-of-properties-for-a-persona"></a><span data-ttu-id="715df-129">Пример запроса операции с помощью параметра "персоны пользователя": Возврат набора свойств пользователя по умолчанию</span><span class="sxs-lookup"><span data-stu-id="715df-129">GetPersona operation request example: Return a default set of properties for a persona</span></span>

<span data-ttu-id="715df-130">В примере ниже показано, как вернуть набор свойств, связанных с **пользователем** , по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="715df-130">The following example of a **GetPersona** operation request shows how to return a default set of properties that are associated with a persona.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013"/>
   </soap:Header>
   <soap:Body xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <GetPersona>
         <PersonaId Id="AAQkADEzAQAKtOtR/l4MlLqHWORfhSYKU="/>
      </GetPersona>
   </soap:Body>
</soap:Envelope>

```

<span data-ttu-id="715df-131">Тело SOAP отклика содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="715df-131">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="715df-132">GetPersona</span><span class="sxs-lookup"><span data-stu-id="715df-132">GetPersona</span></span>](getpersona.md)
    
- [<span data-ttu-id="715df-133">персонаид</span><span class="sxs-lookup"><span data-stu-id="715df-133">PersonaId</span></span>](personaid.md)
    
## <a name="successful-getpersona-operation-response"></a><span data-ttu-id="715df-134">Успешный отклик операции GetResponse.</span><span class="sxs-lookup"><span data-stu-id="715df-134">Successful GetPersona operation response</span></span>

<span data-ttu-id="715df-135">В следующем примере показан успешный **ответ на запрос операции GetResponse** .</span><span class="sxs-lookup"><span data-stu-id="715df-135">The following example shows a successful response to a **GetPersona** operation request.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="715df-136">Все идентификаторы элементов и изменения ключей в этой статье были сокращены, чтобы сохранить удобочитаемость.</span><span class="sxs-lookup"><span data-stu-id="715df-136">All item identifiers and change keys in this article have been shortened to preserve readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="432" 
                           MinorBuildNumber="5" 
                           Version="Exchange2013"
                           xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types"
                     xmlns="https://schemas.microsoft.com/exchange/services/2006/types"
      xmlns:xsd="http://www.w3.org/2001/XMLSchema"
         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <GetPersonaResponseMessage ResponseClass="Success"
                      xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
         <Persona>
            <PersonaId Id="AAQkADEzAQAKtOtR="
              xmlns="https://schemas.microsoft.com/exchange/services/2006/types"/>
            <PersonaType xmlns="https://schemas.microsoft.com/exchange/services/2006/types">Person</PersonaType>
            <CreationTime xmlns="https://schemas.microsoft.com/exchange/services/2006/types">2012-06-01T17:00:34Z</CreationTime>
            <DisplayName xmlns="https://schemas.microsoft.com/exchange/services/2006/types">Brian Johnson</DisplayName>
            <DisplayNameFirstLast xmlns="https://schemas.microsoft.com/exchange/services/2006/types">Brian Johnson</DisplayNameFirstLast>
            <DisplayNameLastFirst xmlns="https://schemas.microsoft.com/exchange/services/2006/types">Johnson Brian</DisplayNameLastFirst>
            <FileAs xmlns="https://schemas.microsoft.com/exchange/services/2006/types">Johnson, Brian</FileAs>
            <FileAsId xmlns="https://schemas.microsoft.com/exchange/services/2006/types">None</FileAsId>
            <GivenName xmlns="https://schemas.microsoft.com/exchange/services/2006/types">Brian</GivenName>
            <Surname xmlns="https://schemas.microsoft.com/exchange/services/2006/types">Johnsoon</Surname>
            <CompanyName xmlns="https://schemas.microsoft.com/exchange/services/2006/types">Contoso</CompanyName>
            <RelevanceScore xmlns="https://schemas.microsoft.com/exchange/services/2006/types">4255550110</RelevanceScore>
            <Attributions xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
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
            <DisplayNames xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
               <StringAttributedValue>
                  <Value>Brian Johnson</Value>
                  <Attributions>
                     <Attribution>0</Attribution>
                  </Attributions>
               </StringAttributedValue>
            </DisplayNames>
            <FileAses xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
               <StringAttributedValue>
                  <Value>Johnson, Brian</Value>
                  <Attributions>
                     <Attribution>0</Attribution>
                  </Attributions>
               </StringAttributedValue>
            </FileAses>
            <FileAsIds xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
               <StringAttributedValue>
                  <Value>None</Value>
                  <Attributions>
                     <Attribution>0</Attribution>
                  </Attributions>
               </StringAttributedValue>
            </FileAsIds>
            <GivenNames xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
               <StringAttributedValue>
                  <Value>Brian</Value>
                  <Attributions>
                     <Attribution>0</Attribution>
                  </Attributions>
               </StringAttributedValue>
            </GivenNames>
            <Surnames xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
               <StringAttributedValue>
                  <Value>Johnson</Value>
                  <Attributions>
                     <Attribution>0</Attribution>
                  </Attributions>
               </StringAttributedValue>
            </Surnames>
            <MobilePhones xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
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
            <CompanyNames xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
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

<span data-ttu-id="715df-137">Тело SOAP отклика содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="715df-137">The response SOAP body contains the following elements:</span></span>
  
- <span data-ttu-id="715df-138">жетперсонареспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="715df-138">GetPersonaResponseMessage</span></span>
    
- [<span data-ttu-id="715df-139">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="715df-139">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="715df-140">Роль</span><span class="sxs-lookup"><span data-stu-id="715df-140">Persona</span></span>](persona.md)
    
- [<span data-ttu-id="715df-141">персонаид</span><span class="sxs-lookup"><span data-stu-id="715df-141">PersonaId</span></span>](personaid.md)
    
- [<span data-ttu-id="715df-142">персонатипе</span><span class="sxs-lookup"><span data-stu-id="715df-142">PersonaType</span></span>](personatype.md)
    
- [<span data-ttu-id="715df-143">CreationTime</span><span class="sxs-lookup"><span data-stu-id="715df-143">CreationTime</span></span>](creationtime.md)
    
- [<span data-ttu-id="715df-144">дисплайнамефирстласт</span><span class="sxs-lookup"><span data-stu-id="715df-144">DisplayNameFirstLast</span></span>](displaynamefirstlast.md)
    
- [<span data-ttu-id="715df-145">дисплайнамеластфирст</span><span class="sxs-lookup"><span data-stu-id="715df-145">DisplayNameLastFirst</span></span>](displaynamelastfirst.md)
    
- [<span data-ttu-id="715df-146">FileAs</span><span class="sxs-lookup"><span data-stu-id="715df-146">FileAs</span></span>](fileas.md)
    
- [<span data-ttu-id="715df-147">филеасид</span><span class="sxs-lookup"><span data-stu-id="715df-147">FileAsId</span></span>](fileasid.md)
    
- [<span data-ttu-id="715df-148">GivenName</span><span class="sxs-lookup"><span data-stu-id="715df-148">GivenName</span></span>](givenname.md)
    
- [<span data-ttu-id="715df-149">ФИО</span><span class="sxs-lookup"><span data-stu-id="715df-149">Surname</span></span>](surname.md)
    
- [<span data-ttu-id="715df-150">CompanyName</span><span class="sxs-lookup"><span data-stu-id="715df-150">CompanyName</span></span>](companyname.md)
    
- [<span data-ttu-id="715df-151">релеванцескоре</span><span class="sxs-lookup"><span data-stu-id="715df-151">RelevanceScore</span></span>](relevancescore.md)
    
- [<span data-ttu-id="715df-152">Атрибуты (Аррайофвалуеаттрибутионстипе)</span><span class="sxs-lookup"><span data-stu-id="715df-152">Attributions (ArrayOfValueAttributionsType)</span></span>](attributions-arrayofvalueattributionstype.md)
    
- [<span data-ttu-id="715df-153">Атрибуты (строка)</span><span class="sxs-lookup"><span data-stu-id="715df-153">Attribution (string)</span></span>](attribution-string.md)
    
- [<span data-ttu-id="715df-154">ID (строка)</span><span class="sxs-lookup"><span data-stu-id="715df-154">ID (String)</span></span>](id-string.md)
    
- <span data-ttu-id="715df-155">[SourceID](sourceid.md) Идентификатор</span><span class="sxs-lookup"><span data-stu-id="715df-155">[SourceId](sourceid.md) SourceId</span></span> 
    
- [<span data-ttu-id="715df-156">DisplayName (строка)</span><span class="sxs-lookup"><span data-stu-id="715df-156">DisplayName (string)</span></span>](displayname-string.md)
    
- [<span data-ttu-id="715df-157">Доступный для записи</span><span class="sxs-lookup"><span data-stu-id="715df-157">IsWritable</span></span>](iswritable.md)
    
- [<span data-ttu-id="715df-158">искуиккконтакт</span><span class="sxs-lookup"><span data-stu-id="715df-158">IsQuickContact</span></span>](isquickcontact.md)
    
- [<span data-ttu-id="715df-159">IsHidden</span><span class="sxs-lookup"><span data-stu-id="715df-159">IsHidden</span></span>](ishidden.md)
    
- [<span data-ttu-id="715df-160">FolderId</span><span class="sxs-lookup"><span data-stu-id="715df-160">FolderId</span></span>](folderid.md)
    
- [<span data-ttu-id="715df-161">DisplayName</span><span class="sxs-lookup"><span data-stu-id="715df-161">DisplayNames</span></span>](displaynames.md)
    
- [<span data-ttu-id="715df-162">стрингаттрибутедвалуе</span><span class="sxs-lookup"><span data-stu-id="715df-162">StringAttributedValue</span></span>](stringattributedvalue.md)
    
- [<span data-ttu-id="715df-163">Значение (Аррайофстрингвалуетипе)</span><span class="sxs-lookup"><span data-stu-id="715df-163">Value (ArrayOfStringValueType)</span></span>](value-arrayofstringvaluetype.md)
    
- [<span data-ttu-id="715df-164">Атрибуты (Аррайофперсонааттрибутионстипе)</span><span class="sxs-lookup"><span data-stu-id="715df-164">Attributions (ArrayOfPersonaAttributionsType)</span></span>](attributions-arrayofpersonaattributionstype.md)
    
- [<span data-ttu-id="715df-165">Атрибуты (Персонааттрибутионтипе)</span><span class="sxs-lookup"><span data-stu-id="715df-165">Attribution (PersonaAttributionType)</span></span>](attribution-personaattributiontype.md)
    
- [<span data-ttu-id="715df-166">филеасес</span><span class="sxs-lookup"><span data-stu-id="715df-166">FileAses</span></span>](fileases.md)
    
- [<span data-ttu-id="715df-167">филеасидс</span><span class="sxs-lookup"><span data-stu-id="715df-167">FileAsIds</span></span>](fileasids.md)
    
- [<span data-ttu-id="715df-168">гивеннамес</span><span class="sxs-lookup"><span data-stu-id="715df-168">GivenNames</span></span>](givennames.md)
    
- [<span data-ttu-id="715df-169">Фамилии</span><span class="sxs-lookup"><span data-stu-id="715df-169">Surnames</span></span>](surnames.md)
    
- [<span data-ttu-id="715df-170">мобилефонес</span><span class="sxs-lookup"><span data-stu-id="715df-170">MobilePhones</span></span>](mobilephones.md)
    
- [<span data-ttu-id="715df-171">фоненумбераттрибутедвалуе</span><span class="sxs-lookup"><span data-stu-id="715df-171">PhoneNumberAttributedValue</span></span>](phonenumberattributedvalue.md)
    
- [<span data-ttu-id="715df-172">Значение (Персонафоненумбертипе)</span><span class="sxs-lookup"><span data-stu-id="715df-172">Value (PersonaPhoneNumberType)</span></span>](value-personaphonenumbertype.md)
    
- [<span data-ttu-id="715df-173">Number</span><span class="sxs-lookup"><span data-stu-id="715df-173">Number</span></span>](number.md)
    
- [<span data-ttu-id="715df-174">Тип (строка)</span><span class="sxs-lookup"><span data-stu-id="715df-174">Type (string)</span></span>](type-string.md)
    
- [<span data-ttu-id="715df-175">компанинамес</span><span class="sxs-lookup"><span data-stu-id="715df-175">CompanyNames</span></span>](companynames.md)
    
## <a name="getpersona-operation-error-response"></a><span data-ttu-id="715df-176">Ответ на ошибку операции GetResponse.</span><span class="sxs-lookup"><span data-stu-id="715df-176">GetPersona operation error response</span></span>

<span data-ttu-id="715df-177">В следующем примере показан ответ об ошибке для **запроса операции GetResponse** .</span><span class="sxs-lookup"><span data-stu-id="715df-177">The following example shows an error response to a **GetPersona** operation request.</span></span> <span data-ttu-id="715df-178">Это ответ на запрос, который содержит неправильно указанный идентификатор пользователя.</span><span class="sxs-lookup"><span data-stu-id="715df-178">This is a response to a request that contains an incorrectly specified persona identifier.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="578" 
                           MinorBuildNumber="11" 
                           Version="Exchange2013" 
                           xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <GetPersonaResponseMessage ResponseClass="Error" 
                                 xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>Id is malformed.</MessageText>
         <ResponseCode>ErrorInvalidIdMalformed</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
      </GetPersonaResponseMessage>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="715df-179">Основной текст сообщения об ошибке SOAP содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="715df-179">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="715df-180">жетперсонареспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="715df-180">GetPersonaResponseMessage</span></span>](getpersonaresponsemessage.md)
    
- [<span data-ttu-id="715df-181">мессажетекст</span><span class="sxs-lookup"><span data-stu-id="715df-181">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="715df-182">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="715df-182">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="715df-183">дескриптивелинккэй</span><span class="sxs-lookup"><span data-stu-id="715df-183">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
<span data-ttu-id="715df-184">Дополнительные коды ошибок, которые являются общими для EWS и специфичными для этой операции, можно найти в разделе [респонсекоде](responsecode.md).</span><span class="sxs-lookup"><span data-stu-id="715df-184">For additional error codes that are generic to EWS and specific to this operation, see [ResponseCode](responsecode.md).</span></span>
  
## <a name="see-also"></a><span data-ttu-id="715df-185">См. также</span><span class="sxs-lookup"><span data-stu-id="715df-185">See also</span></span>

- [<span data-ttu-id="715df-186">Операции EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="715df-186">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
    
- [<span data-ttu-id="715df-187">Пользователи и контакты в EWS для Exchange</span><span class="sxs-lookup"><span data-stu-id="715df-187">People and contacts in EWS in Exchange</span></span>](https://msdn.microsoft.com/library/043c33be-a0d1-4bad-a840-85715eda4813%28Office.15%29.aspx)
    
- [<span data-ttu-id="715df-188">Операция FindPeople</span><span class="sxs-lookup"><span data-stu-id="715df-188">FindPeople operation</span></span>](findpeople-operation.md)
    

