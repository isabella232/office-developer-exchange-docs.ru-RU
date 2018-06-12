---
title: Операция FindPeople
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 446106b7-ff2d-4107-90c1-29f4d38ba128
description: Найдите сведения о веб-служб Exchange FindPeople операции.
ms.openlocfilehash: 97c34d7df590d20513e8f1ad476d62f16815a42b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762590"
---
# <a name="findpeople-operation"></a><span data-ttu-id="8b9cb-103">Операция FindPeople</span><span class="sxs-lookup"><span data-stu-id="8b9cb-103">FindPeople operation</span></span>

<span data-ttu-id="8b9cb-104">Найдите сведения о **FindPeople** операции веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="8b9cb-104">Find information about the **FindPeople** EWS operation.</span></span> 
  
<span data-ttu-id="8b9cb-105">Операция **FindPeople** возвращает все объекты пользователя из указанной папки контактов или получает контакты, соответствующие указанному запросу строки.</span><span class="sxs-lookup"><span data-stu-id="8b9cb-105">The **FindPeople** operation returns all persona objects from a specified Contacts folder or retrieves contacts that match a specified query string.</span></span> 
  
<span data-ttu-id="8b9cb-106">Эта операция появилась в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="8b9cb-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-findpeople-operation"></a><span data-ttu-id="8b9cb-107">С помощью операции FindPeople</span><span class="sxs-lookup"><span data-stu-id="8b9cb-107">Using the FindPeople operation</span></span>

<span data-ttu-id="8b9cb-108">Операция **FindPeople** возвращает объединенные контактные сведения.</span><span class="sxs-lookup"><span data-stu-id="8b9cb-108">The **FindPeople** operation returns aggregated contact information.</span></span> 
  
<span data-ttu-id="8b9cb-109">Операция **FindPeople** построена на существующую функциональность [ограничение](restriction.md) и [BaseShape](baseshape.md) сложные типы, добавив ограничение объединение и возможность получить дополнительные свойства.</span><span class="sxs-lookup"><span data-stu-id="8b9cb-109">The **FindPeople** operation builds on the existing functionality of the [Restriction](restriction.md) and [BaseShape](baseshape.md) complex types by adding an aggregation restriction and the ability to return additional properties.</span></span> <span data-ttu-id="8b9cb-110">С помощью ограничения клиента можно указать фильтры, такие как «возвращать только результаты с адресом обмена мгновенными Сообщениями».</span><span class="sxs-lookup"><span data-stu-id="8b9cb-110">By using a restriction, a client can specify filters such as "only return results that have an IM address".</span></span> <span data-ttu-id="8b9cb-111">Параметры поиска по умолчанию предназначен для указанного пользователя личных почтовых ящиков и глобальный список адресов (GAL).</span><span class="sxs-lookup"><span data-stu-id="8b9cb-111">The default search behavior targets both the specified user's personal mailbox and the global address list (GAL).</span></span> <span data-ttu-id="8b9cb-112">При поиске в глобальном списке адресов как папки поиска, необходимо указать строку запроса вместо ограничение, поскольку эта операция не позволяет для просмотра глобального списка адресов.</span><span class="sxs-lookup"><span data-stu-id="8b9cb-112">When searching the GAL as the primary search folder, you must specify a query string instead of a restriction, because this operation does not allow for browsing of the GAL.</span></span> 
  
### <a name="findpeople-operation-soap-headers"></a><span data-ttu-id="8b9cb-113">Заголовки SOAP FindPeople операции</span><span class="sxs-lookup"><span data-stu-id="8b9cb-113">FindPeople operation SOAP headers</span></span>

<span data-ttu-id="8b9cb-114">Операция **FindPeople** можно использовать заголовки SOAP, которые перечислены в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="8b9cb-114">The **FindPeople** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="8b9cb-115">**Имя заголовка**</span><span class="sxs-lookup"><span data-stu-id="8b9cb-115">**Header name**</span></span>|<span data-ttu-id="8b9cb-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="8b9cb-116">**Element**</span></span>|<span data-ttu-id="8b9cb-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="8b9cb-117">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="8b9cb-118">**Олицетворение**</span><span class="sxs-lookup"><span data-stu-id="8b9cb-118">**Impersonation**</span></span> <br/> |[<span data-ttu-id="8b9cb-119">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="8b9cb-119">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="8b9cb-120">Идентифицирует пользователя, которого олицетворения в клиентском приложении.</span><span class="sxs-lookup"><span data-stu-id="8b9cb-120">Identifies the user whom the client application is impersonating.</span></span> <span data-ttu-id="8b9cb-121">Этот заголовок можно применять к запросу.</span><span class="sxs-lookup"><span data-stu-id="8b9cb-121">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="8b9cb-122">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="8b9cb-122">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="8b9cb-123">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="8b9cb-123">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="8b9cb-124">Определяет версию схемы для операции запроса.</span><span class="sxs-lookup"><span data-stu-id="8b9cb-124">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="8b9cb-125">Этот заголовок можно применять к запросу.</span><span class="sxs-lookup"><span data-stu-id="8b9cb-125">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="8b9cb-126">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="8b9cb-126">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="8b9cb-127">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="8b9cb-127">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="8b9cb-128">Определяет версию сервера, ответившего на запрос.</span><span class="sxs-lookup"><span data-stu-id="8b9cb-128">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="8b9cb-129">Этот заголовок можно применять, чтобы получить ответ.</span><span class="sxs-lookup"><span data-stu-id="8b9cb-129">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="findpeople-operation-request-example"></a><span data-ttu-id="8b9cb-130">Пример запроса FindPeople операции</span><span class="sxs-lookup"><span data-stu-id="8b9cb-130">FindPeople operation request example</span></span>

<span data-ttu-id="8b9cb-131">В следующем примере запрос операции **FindPeople** показано, как возвратить первые 100 контакты из папки «Контакты».</span><span class="sxs-lookup"><span data-stu-id="8b9cb-131">The following example of a **FindPeople** operation request shows how to return the first 100 contacts from the Contacts folder.</span></span> 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013" />
   </soap:Header>
   <soap:Body >
      <m:FindPeople>
         <m:IndexedPageItemView BasePoint="Beginning" MaxEntriesReturned="100" Offset="0"/>
         <m:ParentFolderId>
            <t:DistinguishedFolderId Id="contacts"/>
         </m:ParentFolderId>
      </m:FindPeople>
   </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="8b9cb-132">Запрос SOAP body содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="8b9cb-132">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="8b9cb-133">FindPeople</span><span class="sxs-lookup"><span data-stu-id="8b9cb-133">FindPeople</span></span>](findpeople.md)
    
- [<span data-ttu-id="8b9cb-134">IndexedPageItemView</span><span class="sxs-lookup"><span data-stu-id="8b9cb-134">IndexedPageItemView</span></span>](indexedpageitemview.md)
    
- [<span data-ttu-id="8b9cb-135">ParentFolderId (TargetFolderIdType)</span><span class="sxs-lookup"><span data-stu-id="8b9cb-135">ParentFolderId (TargetFolderIdType)</span></span>](parentfolderid-targetfolderidtype.md)
    
- [<span data-ttu-id="8b9cb-136">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="8b9cb-136">DistinguishedFolderId</span></span>](distinguishedfolderid.md)
    
<span data-ttu-id="8b9cb-137">В следующем примере запрос операции **FindPeople** показано, как возвратить первые 100 контактов из глобального списка адресов с помощью строки запроса.</span><span class="sxs-lookup"><span data-stu-id="8b9cb-137">The following example of a **FindPeople** operation request shows how to return the first 100 contacts from the GAL by using a query string.</span></span> <span data-ttu-id="8b9cb-138">Установка **DistinguishedFolderId** «каталог» выполняет поиск глобального списка адресов как основной источник пользователей.</span><span class="sxs-lookup"><span data-stu-id="8b9cb-138">Setting the **DistinguishedFolderId** to "directory" will search the GAL as the primary source of personas.</span></span> 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
   <soap:Header>
    <t:RequestServerVersion Version="Exchange2013" />
   </soap:Header>
   <soap:Body >
    <m:FindPeople>
      <m:PersonaShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="persona:DisplayName"/>
          <t:FieldURI FieldURI="persona:Title"/>
        </t:AdditionalProperties>
      </m:PersonaShape>
      <m:IndexedPageItemView BasePoint="Beginning" MaxEntriesReturned="100" Offset="0"/>
      <m:ParentFolderId>
        <t:DistinguishedFolderId Id="directory"/>
      </m:ParentFolderId>
      <m:QueryString>adams</m:QueryString>
    </m:FindPeople>
  </soap:Body>
</soap:Envelope>
```

## <a name="successful-findpeople-operation-response"></a><span data-ttu-id="8b9cb-139">Успешные операции ответа FindPeople</span><span class="sxs-lookup"><span data-stu-id="8b9cb-139">Successful FindPeople operation response</span></span>

<span data-ttu-id="8b9cb-140">В следующем примере показано успешного ответа на запрос операции **FindPeople** .</span><span class="sxs-lookup"><span data-stu-id="8b9cb-140">The following example shows a successful response to a **FindPeople** operation request.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?><s:Envelope 
   xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" 
                         MinorVersion="0" 
                         MajorBuildNumber="349" 
                         MinorBuildNumber="0" 
                         Version="Exchange2013" 
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
                         xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <FindPeopleResponse ResponseClass="Success" 
                        xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseCode>NoError</ResponseCode>
      <People>
        <Persona xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
          <PersonaId Id="AAQkAGQ1MjJjMTBkLTc4Y2UtNDA5Ny04ZjU5LWI3MTYzNGNkZmRkYQAQAOjFqObcLmtOlzlRnHdXQjo=" />
          <CreationTime>2012-01-11T22:25:37Z</CreationTime>
          <DisplayName>Terry Adams</DisplayName>
          <DisplayNameFirstLast>Terry Adams</DisplayNameFirstLast>
          <DisplayNameLastFirst>Adams Terry</DisplayNameLastFirst>
          <FileAs>Adams, Terry</FileAs>
          <GivenName>Terry</GivenName>
          <Surname>Adams</Surname>
          <EmailAddress>
            <Name>terry@litwareinc.com</Name>
            <EmailAddress>terry@litwareinc.com</EmailAddress>
            <RoutingType>SMTP</RoutingType>
          </EmailAddress>
          <EmailAddresses>
            <EmailAddress>
              <Name>terry@litwareinc.com</Name>
              <EmailAddress>terry@litwareinc.com</EmailAddress>
              <RoutingType>SMTP</RoutingType>
            </EmailAddress>
            <EmailAddress>
              <Name>tadams@contoso.com</Name>
              <EmailAddress>tadams@contoso.com</EmailAddress>
              <RoutingType>SMTP</RoutingType>
            </EmailAddress>
          </EmailAddresses>
          <RelevanceScore>2147483647</RelevanceScore>
        </Persona>
      </People>
      <TotalNumberOfPeopleInView>1</TotalNumberOfPeopleInView>
    </FindPeopleResponse>
  </s:Body>
</s:Envelope>
```

<span data-ttu-id="8b9cb-141">Ответ SOAP body содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="8b9cb-141">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="8b9cb-142">FindPeopleResponse</span><span class="sxs-lookup"><span data-stu-id="8b9cb-142">FindPeopleResponse</span></span>](findpeopleresponse.md)
    
- [<span data-ttu-id="8b9cb-143">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="8b9cb-143">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="8b9cb-144">Людей</span><span class="sxs-lookup"><span data-stu-id="8b9cb-144">People</span></span>](people.md)
    
- [<span data-ttu-id="8b9cb-145">Пользователь</span><span class="sxs-lookup"><span data-stu-id="8b9cb-145">Persona</span></span>](persona.md)
    
- [<span data-ttu-id="8b9cb-146">PersonaId</span><span class="sxs-lookup"><span data-stu-id="8b9cb-146">PersonaId</span></span>](personaid.md)
    
- [<span data-ttu-id="8b9cb-147">CreationTime</span><span class="sxs-lookup"><span data-stu-id="8b9cb-147">CreationTime</span></span>](creationtime.md)
    
- [<span data-ttu-id="8b9cb-148">Отображаемое имя (строка)</span><span class="sxs-lookup"><span data-stu-id="8b9cb-148">DisplayName (string)</span></span>](displayname-string.md)
    
- [<span data-ttu-id="8b9cb-149">DisplayNameFirstLast</span><span class="sxs-lookup"><span data-stu-id="8b9cb-149">DisplayNameFirstLast</span></span>](displaynamefirstlast.md)
    
- [<span data-ttu-id="8b9cb-150">DisplayNameLastFirst</span><span class="sxs-lookup"><span data-stu-id="8b9cb-150">DisplayNameLastFirst</span></span>](displaynamelastfirst.md)
    
- [<span data-ttu-id="8b9cb-151">FileAs</span><span class="sxs-lookup"><span data-stu-id="8b9cb-151">FileAs</span></span>](fileas.md)
    
- [<span data-ttu-id="8b9cb-152">GivenName</span><span class="sxs-lookup"><span data-stu-id="8b9cb-152">GivenName</span></span>](givenname.md)
    
- [<span data-ttu-id="8b9cb-153">Фамилия</span><span class="sxs-lookup"><span data-stu-id="8b9cb-153">Surname</span></span>](surname.md)
    
- [<span data-ttu-id="8b9cb-154">EmailAddresses (ArrayOfEmailAddressesType)</span><span class="sxs-lookup"><span data-stu-id="8b9cb-154">EmailAddresses (ArrayOfEmailAddressesType)</span></span>](emailaddresses-arrayofemailaddressestype.md)
    
- [<span data-ttu-id="8b9cb-155">EmailAddress (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="8b9cb-155">EmailAddress (EmailAddressType)</span></span>](emailaddress-emailaddresstype.md)
    
- [<span data-ttu-id="8b9cb-156">Имя (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="8b9cb-156">Name (EmailAddressType)</span></span>](name-emailaddresstype.md)
    
- [<span data-ttu-id="8b9cb-157">EmailAddress (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="8b9cb-157">EmailAddress (EmailAddressType)</span></span>](emailaddress-emailaddresstype.md)
    
- [<span data-ttu-id="8b9cb-158">RoutingType (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="8b9cb-158">RoutingType (EmailAddressType)</span></span>](routingtype-emailaddresstype.md)
    
- [<span data-ttu-id="8b9cb-159">RelevanceScore</span><span class="sxs-lookup"><span data-stu-id="8b9cb-159">RelevanceScore</span></span>](relevancescore.md)
    
- [<span data-ttu-id="8b9cb-160">TotalNumberOfPeopleInView</span><span class="sxs-lookup"><span data-stu-id="8b9cb-160">TotalNumberOfPeopleInView</span></span>](totalnumberofpeopleinview.md)
    
## <a name="findpeople-operation-error-response"></a><span data-ttu-id="8b9cb-161">Ошибка операции FindPeople ответа</span><span class="sxs-lookup"><span data-stu-id="8b9cb-161">FindPeople operation error response</span></span>

<span data-ttu-id="8b9cb-162">Коды ошибок, которые являются общими для веб-служб Exchange в разделе [ResponseCode](responsecode.md).</span><span class="sxs-lookup"><span data-stu-id="8b9cb-162">For error codes that are generic to EWS, see [ResponseCode](responsecode.md).</span></span>
  
## <a name="see-also"></a><span data-ttu-id="8b9cb-163">См. также</span><span class="sxs-lookup"><span data-stu-id="8b9cb-163">See also</span></span>

- [<span data-ttu-id="8b9cb-164">Пользователи и контакты в EWS для Exchange</span><span class="sxs-lookup"><span data-stu-id="8b9cb-164">People and contacts in EWS in Exchange</span></span>](http://msdn.microsoft.com/library/043c33be-a0d1-4bad-a840-85715eda4813%28Office.15%29.aspx)
    
- [<span data-ttu-id="8b9cb-165">Операция GetPersona</span><span class="sxs-lookup"><span data-stu-id="8b9cb-165">GetPersona operation</span></span>](getpersona-operation.md)
    

