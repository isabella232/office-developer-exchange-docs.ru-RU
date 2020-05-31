---
title: Операция FindPeople
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 446106b7-ff2d-4107-90c1-29f4d38ba128
description: Поиск сведений о FindPeopleной операции EWS.
ms.openlocfilehash: 97c34d7df590d20513e8f1ad476d62f16815a42b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762590"
---
# <a name="findpeople-operation"></a><span data-ttu-id="d4dd5-103">Операция FindPeople</span><span class="sxs-lookup"><span data-stu-id="d4dd5-103">FindPeople operation</span></span>

<span data-ttu-id="d4dd5-104">Поиск сведений о **FindPeopleной** операции EWS.</span><span class="sxs-lookup"><span data-stu-id="d4dd5-104">Find information about the **FindPeople** EWS operation.</span></span> 
  
<span data-ttu-id="d4dd5-105">Операция **FindPeople** возвращает все объекты персоны из указанной папки контактов или получает контакты, которые совпадают с указанной строкой запроса.</span><span class="sxs-lookup"><span data-stu-id="d4dd5-105">The **FindPeople** operation returns all persona objects from a specified Contacts folder or retrieves contacts that match a specified query string.</span></span> 
  
<span data-ttu-id="d4dd5-106">Эта операция появилась в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="d4dd5-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-findpeople-operation"></a><span data-ttu-id="d4dd5-107">Использование операции FindPeople</span><span class="sxs-lookup"><span data-stu-id="d4dd5-107">Using the FindPeople operation</span></span>

<span data-ttu-id="d4dd5-108">Операция **FindPeople** возвращает объединенные сведения о контакте.</span><span class="sxs-lookup"><span data-stu-id="d4dd5-108">The **FindPeople** operation returns aggregated contact information.</span></span> 
  
<span data-ttu-id="d4dd5-109">Операция **FindPeople** строится на существующих функциональных возможностях сложных типов [restriction](restriction.md) и [басешапе](baseshape.md) , добавляя ограничение статистической обработки и возвращая возможность возврата дополнительных свойств.</span><span class="sxs-lookup"><span data-stu-id="d4dd5-109">The **FindPeople** operation builds on the existing functionality of the [Restriction](restriction.md) and [BaseShape](baseshape.md) complex types by adding an aggregation restriction and the ability to return additional properties.</span></span> <span data-ttu-id="d4dd5-110">С помощью ограничения клиент может указать такие фильтры, как "только возвращаемые результаты с адресом для обмена мгновенными сообщениями".</span><span class="sxs-lookup"><span data-stu-id="d4dd5-110">By using a restriction, a client can specify filters such as "only return results that have an IM address".</span></span> <span data-ttu-id="d4dd5-111">Поведение поиска по умолчанию предназначено для личного почтового ящика указанного пользователя и глобального списка адресов (GAL).</span><span class="sxs-lookup"><span data-stu-id="d4dd5-111">The default search behavior targets both the specified user's personal mailbox and the global address list (GAL).</span></span> <span data-ttu-id="d4dd5-112">При поиске в глобальном списке адресов в качестве основной папки поиска необходимо указать строку запроса вместо ограничения, так как эта операция не позволяет просматривать глобальный список адресов.</span><span class="sxs-lookup"><span data-stu-id="d4dd5-112">When searching the GAL as the primary search folder, you must specify a query string instead of a restriction, because this operation does not allow for browsing of the GAL.</span></span> 
  
### <a name="findpeople-operation-soap-headers"></a><span data-ttu-id="d4dd5-113">Заголовки SOAP операции FindPeople</span><span class="sxs-lookup"><span data-stu-id="d4dd5-113">FindPeople operation SOAP headers</span></span>

<span data-ttu-id="d4dd5-114">Операция **FindPeople** может использовать заголовки SOAP, указанные в приведенной ниже таблице.</span><span class="sxs-lookup"><span data-stu-id="d4dd5-114">The **FindPeople** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="d4dd5-115">**Имя заголовка**</span><span class="sxs-lookup"><span data-stu-id="d4dd5-115">**Header name**</span></span>|<span data-ttu-id="d4dd5-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="d4dd5-116">**Element**</span></span>|<span data-ttu-id="d4dd5-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d4dd5-117">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="d4dd5-118">**Олицетворение**</span><span class="sxs-lookup"><span data-stu-id="d4dd5-118">**Impersonation**</span></span> <br/> |[<span data-ttu-id="d4dd5-119">ексчанжеимперсонатион</span><span class="sxs-lookup"><span data-stu-id="d4dd5-119">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="d4dd5-120">Идентифицирует пользователя, который олицетворяет клиентское приложение.</span><span class="sxs-lookup"><span data-stu-id="d4dd5-120">Identifies the user whom the client application is impersonating.</span></span> <span data-ttu-id="d4dd5-121">Этот заголовок является применимым для запроса.</span><span class="sxs-lookup"><span data-stu-id="d4dd5-121">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="d4dd5-122">**рекуестверсион**</span><span class="sxs-lookup"><span data-stu-id="d4dd5-122">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="d4dd5-123">рекуестсерверверсион</span><span class="sxs-lookup"><span data-stu-id="d4dd5-123">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="d4dd5-124">Определяет версию схемы для запроса операции.</span><span class="sxs-lookup"><span data-stu-id="d4dd5-124">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="d4dd5-125">Этот заголовок является применимым для запроса.</span><span class="sxs-lookup"><span data-stu-id="d4dd5-125">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="d4dd5-126">**серверверсион**</span><span class="sxs-lookup"><span data-stu-id="d4dd5-126">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="d4dd5-127">серверверсионинфо</span><span class="sxs-lookup"><span data-stu-id="d4dd5-127">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="d4dd5-128">Определяет версию сервера, который ответил на запрос.</span><span class="sxs-lookup"><span data-stu-id="d4dd5-128">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="d4dd5-129">Этот заголовок является применимым для отклика.</span><span class="sxs-lookup"><span data-stu-id="d4dd5-129">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="findpeople-operation-request-example"></a><span data-ttu-id="d4dd5-130">Пример запроса операции FindPeople</span><span class="sxs-lookup"><span data-stu-id="d4dd5-130">FindPeople operation request example</span></span>

<span data-ttu-id="d4dd5-131">В следующем примере запроса операции **FindPeople** показано, как вернуть первые 100 контактов из папки "Контакты".</span><span class="sxs-lookup"><span data-stu-id="d4dd5-131">The following example of a **FindPeople** operation request shows how to return the first 100 contacts from the Contacts folder.</span></span> 
  
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

<span data-ttu-id="d4dd5-132">Текст SOAP Request содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="d4dd5-132">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="d4dd5-133">FindPeople</span><span class="sxs-lookup"><span data-stu-id="d4dd5-133">FindPeople</span></span>](findpeople.md)
    
- [<span data-ttu-id="d4dd5-134">индекседпажеитемвиев</span><span class="sxs-lookup"><span data-stu-id="d4dd5-134">IndexedPageItemView</span></span>](indexedpageitemview.md)
    
- [<span data-ttu-id="d4dd5-135">ParentFolderId (Таржетфолдеридтипе)</span><span class="sxs-lookup"><span data-stu-id="d4dd5-135">ParentFolderId (TargetFolderIdType)</span></span>](parentfolderid-targetfolderidtype.md)
    
- [<span data-ttu-id="d4dd5-136">дистингуишедфолдерид</span><span class="sxs-lookup"><span data-stu-id="d4dd5-136">DistinguishedFolderId</span></span>](distinguishedfolderid.md)
    
<span data-ttu-id="d4dd5-137">В приведенном ниже примере запроса операции **FindPeople** показано, как возвратить первые 100 контактов из глобального списка адресов с помощью строки запроса.</span><span class="sxs-lookup"><span data-stu-id="d4dd5-137">The following example of a **FindPeople** operation request shows how to return the first 100 contacts from the GAL by using a query string.</span></span> <span data-ttu-id="d4dd5-138">Если задать для **дистингуишедфолдерид** значение "каталог", будет осуществляться поиск глобального источника адресов в глобальном списке адресов.</span><span class="sxs-lookup"><span data-stu-id="d4dd5-138">Setting the **DistinguishedFolderId** to "directory" will search the GAL as the primary source of personas.</span></span> 
  
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

## <a name="successful-findpeople-operation-response"></a><span data-ttu-id="d4dd5-139">Успешный отклик операции FindPeople</span><span class="sxs-lookup"><span data-stu-id="d4dd5-139">Successful FindPeople operation response</span></span>

<span data-ttu-id="d4dd5-140">В следующем примере показан успешный ответ на запрос операции **FindPeople** .</span><span class="sxs-lookup"><span data-stu-id="d4dd5-140">The following example shows a successful response to a **FindPeople** operation request.</span></span> 
  
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

<span data-ttu-id="d4dd5-141">Тело SOAP отклика содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="d4dd5-141">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="d4dd5-142">финдпеоплереспонсе</span><span class="sxs-lookup"><span data-stu-id="d4dd5-142">FindPeopleResponse</span></span>](findpeopleresponse.md)
    
- [<span data-ttu-id="d4dd5-143">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="d4dd5-143">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="d4dd5-144">Люди</span><span class="sxs-lookup"><span data-stu-id="d4dd5-144">People</span></span>](people.md)
    
- [<span data-ttu-id="d4dd5-145">Роль</span><span class="sxs-lookup"><span data-stu-id="d4dd5-145">Persona</span></span>](persona.md)
    
- [<span data-ttu-id="d4dd5-146">персонаид</span><span class="sxs-lookup"><span data-stu-id="d4dd5-146">PersonaId</span></span>](personaid.md)
    
- [<span data-ttu-id="d4dd5-147">CreationTime</span><span class="sxs-lookup"><span data-stu-id="d4dd5-147">CreationTime</span></span>](creationtime.md)
    
- [<span data-ttu-id="d4dd5-148">DisplayName (строка)</span><span class="sxs-lookup"><span data-stu-id="d4dd5-148">DisplayName (string)</span></span>](displayname-string.md)
    
- [<span data-ttu-id="d4dd5-149">дисплайнамефирстласт</span><span class="sxs-lookup"><span data-stu-id="d4dd5-149">DisplayNameFirstLast</span></span>](displaynamefirstlast.md)
    
- [<span data-ttu-id="d4dd5-150">дисплайнамеластфирст</span><span class="sxs-lookup"><span data-stu-id="d4dd5-150">DisplayNameLastFirst</span></span>](displaynamelastfirst.md)
    
- [<span data-ttu-id="d4dd5-151">FileAs</span><span class="sxs-lookup"><span data-stu-id="d4dd5-151">FileAs</span></span>](fileas.md)
    
- [<span data-ttu-id="d4dd5-152">GivenName</span><span class="sxs-lookup"><span data-stu-id="d4dd5-152">GivenName</span></span>](givenname.md)
    
- [<span data-ttu-id="d4dd5-153">ФИО</span><span class="sxs-lookup"><span data-stu-id="d4dd5-153">Surname</span></span>](surname.md)
    
- [<span data-ttu-id="d4dd5-154">EmailAddresses (Аррайофемаиладдрессестипе)</span><span class="sxs-lookup"><span data-stu-id="d4dd5-154">EmailAddresses (ArrayOfEmailAddressesType)</span></span>](emailaddresses-arrayofemailaddressestype.md)
    
- [<span data-ttu-id="d4dd5-155">EmailAddress (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="d4dd5-155">EmailAddress (EmailAddressType)</span></span>](emailaddress-emailaddresstype.md)
    
- [<span data-ttu-id="d4dd5-156">Имя (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="d4dd5-156">Name (EmailAddressType)</span></span>](name-emailaddresstype.md)
    
- [<span data-ttu-id="d4dd5-157">EmailAddress (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="d4dd5-157">EmailAddress (EmailAddressType)</span></span>](emailaddress-emailaddresstype.md)
    
- [<span data-ttu-id="d4dd5-158">Раутингтипе (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="d4dd5-158">RoutingType (EmailAddressType)</span></span>](routingtype-emailaddresstype.md)
    
- [<span data-ttu-id="d4dd5-159">релеванцескоре</span><span class="sxs-lookup"><span data-stu-id="d4dd5-159">RelevanceScore</span></span>](relevancescore.md)
    
- [<span data-ttu-id="d4dd5-160">тоталнумберофпеоплеинвиев</span><span class="sxs-lookup"><span data-stu-id="d4dd5-160">TotalNumberOfPeopleInView</span></span>](totalnumberofpeopleinview.md)
    
## <a name="findpeople-operation-error-response"></a><span data-ttu-id="d4dd5-161">Ответ об ошибке операции FindPeople</span><span class="sxs-lookup"><span data-stu-id="d4dd5-161">FindPeople operation error response</span></span>

<span data-ttu-id="d4dd5-162">Коды ошибок, являющиеся общими для EWS, представлены в разделе [респонсекоде](responsecode.md).</span><span class="sxs-lookup"><span data-stu-id="d4dd5-162">For error codes that are generic to EWS, see [ResponseCode](responsecode.md).</span></span>
  
## <a name="see-also"></a><span data-ttu-id="d4dd5-163">См. также</span><span class="sxs-lookup"><span data-stu-id="d4dd5-163">See also</span></span>

- [<span data-ttu-id="d4dd5-164">Пользователи и контакты в EWS для Exchange</span><span class="sxs-lookup"><span data-stu-id="d4dd5-164">People and contacts in EWS in Exchange</span></span>](http://msdn.microsoft.com/library/043c33be-a0d1-4bad-a840-85715eda4813%28Office.15%29.aspx)
    
- [<span data-ttu-id="d4dd5-165">Операция GetPersona</span><span class="sxs-lookup"><span data-stu-id="d4dd5-165">GetPersona operation</span></span>](getpersona-operation.md)
    

