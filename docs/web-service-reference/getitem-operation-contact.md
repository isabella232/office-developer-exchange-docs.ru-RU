---
title: Операция GetItem (контакт)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetItem
api_type:
- schema
ms.assetid: 6b96dace-1260-4b83-869a-7c31c5583daa
description: Операция GetItem используется для получения элементов контактов из хранилища Exchange.
ms.openlocfilehash: 93e8dbe28e130ab64d4b8d12d2befde1f77ae8fa
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460024"
---
# <a name="getitem-operation-contact"></a><span data-ttu-id="fd608-103">Операция GetItem (контакт)</span><span class="sxs-lookup"><span data-stu-id="fd608-103">GetItem operation (contact)</span></span>

<span data-ttu-id="fd608-104">Операция GetItem используется для получения элементов контактов из хранилища Exchange.</span><span class="sxs-lookup"><span data-stu-id="fd608-104">The GetItem operation is used to get contact items from the Exchange store.</span></span>
  
## <a name="getitem-contact-request-example"></a><span data-ttu-id="fd608-105">Пример запроса GetItem (Contact)</span><span class="sxs-lookup"><span data-stu-id="fd608-105">GetItem (Contact) request example</span></span>

### <a name="description"></a><span data-ttu-id="fd608-106">Описание</span><span class="sxs-lookup"><span data-stu-id="fd608-106">Description</span></span>

<span data-ttu-id="fd608-107">В приведенном ниже примере показано, как получить элемент из хранилища Exchange.</span><span class="sxs-lookup"><span data-stu-id="fd608-107">The following example shows how to get an item from the Exchange store.</span></span>
  
### <a name="code"></a><span data-ttu-id="fd608-108">Код</span><span class="sxs-lookup"><span data-stu-id="fd608-108">Code</span></span>

```XML
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <GetItem xmlns='https://schemas.microsoft.com/exchange/services/2006/messages'>
      <ItemShape>
        <t:BaseShape>AllProperties</t:BaseShape>
      </ItemShape>
      <ItemIds>
        <t:ItemId Id="AAAtAE=" ChangeKey="EQAAABY" />
      </ItemIds>
    </GetItem>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="fd608-109">Комментарии</span><span class="sxs-lookup"><span data-stu-id="fd608-109">Comments</span></span>

<span data-ttu-id="fd608-110">Запрос на получение элемента из хранилища Exchange имеет одну и ту же форму для всех типов элементов.</span><span class="sxs-lookup"><span data-stu-id="fd608-110">The request to get an item from the Exchange store takes the same form for all item types.</span></span> <span data-ttu-id="fd608-111">Ответы на запросы для различных элементов будут отличаться, так как различные элементы возвращают разные сведения на основе фигур ответа.</span><span class="sxs-lookup"><span data-stu-id="fd608-111">The responses to requests for different items will be different because different items return different information based on the response shapes.</span></span>
  
> [!NOTE]
> <span data-ttu-id="fd608-112">Идентификатор элемента был сокращен, чтобы сохранить удобочитаемость.</span><span class="sxs-lookup"><span data-stu-id="fd608-112">The item identifier has been shortened to preserve readability.</span></span> 
  
### <a name="request-elements"></a><span data-ttu-id="fd608-113">Элементы Request</span><span class="sxs-lookup"><span data-stu-id="fd608-113">Request elements</span></span>

<span data-ttu-id="fd608-114">В запросе используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="fd608-114">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="fd608-115">GetItem</span><span class="sxs-lookup"><span data-stu-id="fd608-115">GetItem</span></span>](getitem.md)
    
- [<span data-ttu-id="fd608-116">итемшапе</span><span class="sxs-lookup"><span data-stu-id="fd608-116">ItemShape</span></span>](itemshape.md)
    
- [<span data-ttu-id="fd608-117">басешапе</span><span class="sxs-lookup"><span data-stu-id="fd608-117">BaseShape</span></span>](baseshape.md)
    
- [<span data-ttu-id="fd608-118">итемидс</span><span class="sxs-lookup"><span data-stu-id="fd608-118">ItemIds</span></span>](itemids.md)
    
- [<span data-ttu-id="fd608-119">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="fd608-119">ItemId</span></span>](itemid.md)
    
## <a name="successful-getitem-contact-response"></a><span data-ttu-id="fd608-120">Успешный отклик GetItem (контакт)</span><span class="sxs-lookup"><span data-stu-id="fd608-120">Successful GetItem (Contact) Response</span></span>

### <a name="description"></a><span data-ttu-id="fd608-121">Описание</span><span class="sxs-lookup"><span data-stu-id="fd608-121">Description</span></span>

<span data-ttu-id="fd608-122">В следующем примере кода показан успешный отклик GetItem для объекта **аллпропертиес**[басешапе](baseshape.md).</span><span class="sxs-lookup"><span data-stu-id="fd608-122">The following code example shows a successful GetItem response for the **AllProperties**[BaseShape](baseshape.md).</span></span>
  
### <a name="code"></a><span data-ttu-id="fd608-123">Код</span><span class="sxs-lookup"><span data-stu-id="fd608-123">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="602" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <GetItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                     xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                     xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:GetItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items>
            <t:Contact>
              <t:ItemId Id="AAAtAEA=" ChangeKey="EQAAABYq" />
              <t:ParentFolderId Id="AQAtAEFk==" ChangeKey="AQAAAA==" />
              <t:ItemClass>IPM.Contact</t:ItemClass>
              <t:Sensitivity>Normal</t:Sensitivity>
              <t:Body BodyType="Text" />
              <t:DateTimeReceived>2006-08-18T17:31:18Z</t:DateTimeReceived>
              <t:Size>382</t:Size>
              <t:Importance>Normal</t:Importance>
              <t:IsSubmitted>false</t:IsSubmitted>
              <t:IsDraft>true</t:IsDraft>
              <t:IsFromMe>false</t:IsFromMe>
              <t:IsResend>false</t:IsResend>
              <t:IsUnmodified>false</t:IsUnmodified>
              <t:DateTimeSent>2006-08-18T17:31:18Z</t:DateTimeSent>
              <t:DateTimeCreated>2006-08-18T17:31:18Z</t:DateTimeCreated>
              <t:HasAttachments>false</t:HasAttachments>
              <t:Culture>en</t:Culture>
              <t:FileAs>SampleContact</t:FileAs>
              <t:FileAsMapping>None</t:FileAsMapping>
              <t:DisplayName>Tanja Plate</t:DisplayName>
              <t:GivenName>Tanja</t:GivenName>
              <t:Initials>T.P.</t:Initials>
              <t:CompleteName>
                <t:FirstName>Tanja</t:FirstName>
                <t:LastName>Plate</t:LastName>
                <t:Initials>T.P.</t:Initials>
                <t:FullName>Tanja Plate</t:FullName>
              </t:CompleteName>
              <t:CompanyName>Northwind Traders</t:CompanyName>
              <t:EmailAddresses>
                <t:Entry Key="EmailAddress1">tplate@example.com</t:Entry>
                <t:Entry Key="EmailAddress2">tplate@example.com</t:Entry>
              </t:EmailAddresses>
              <t:PhysicalAddresses>
                <t:Entry Key="Business">
                  <t:Street>12345 67th Ave</t:Street>
                  <t:City>Whittier</t:City>
                  <t:State>CA</t:State>
                  <t:Country>USA</t:Country>
                </t:Entry>
              </t:PhysicalAddresses>
              <t:PhoneNumbers>
                <t:Entry Key="BusinessPhone">5625550199</t:Entry>
              </t:PhoneNumbers>
              <t:JobTitle>Project Manager</t:JobTitle>
              <t:Surname>Plate</t:Surname>
            </t:Contact>
          </m:Items>
        </m:GetItemResponseMessage>
      </m:ResponseMessages>
    </GetItemResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="fd608-124">Комментарии</span><span class="sxs-lookup"><span data-stu-id="fd608-124">Comments</span></span>

<span data-ttu-id="fd608-125">Идентификатор элемента был сокращен, чтобы сохранить удобочитаемость.</span><span class="sxs-lookup"><span data-stu-id="fd608-125">The item identifier has been shortened to preserve readability.</span></span>
  
### <a name="successful-response-elements"></a><span data-ttu-id="fd608-126">Элементы успешного ответа</span><span class="sxs-lookup"><span data-stu-id="fd608-126">Successful response elements</span></span>

<span data-ttu-id="fd608-127">Следующие элементы используются в ответе на запрос GetItem с формой ответа **аллпропертиес** для элемента Contact.</span><span class="sxs-lookup"><span data-stu-id="fd608-127">The following elements are used in the response for a GetItem request with a response shape of **AllProperties** for a contact item.</span></span> 
  
- [<span data-ttu-id="fd608-128">серверверсионинфо</span><span class="sxs-lookup"><span data-stu-id="fd608-128">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="fd608-129">жетитемреспонсе</span><span class="sxs-lookup"><span data-stu-id="fd608-129">GetItemResponse</span></span>](getitemresponse.md)
    
- [<span data-ttu-id="fd608-130">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="fd608-130">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="fd608-131">жетитемреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="fd608-131">GetItemResponseMessage</span></span>](getitemresponsemessage.md)
    
- [<span data-ttu-id="fd608-132">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="fd608-132">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="fd608-133">Items</span><span class="sxs-lookup"><span data-stu-id="fd608-133">Items</span></span>](items.md)
    
- <span data-ttu-id="fd608-134">[контакт](contact.md);</span><span class="sxs-lookup"><span data-stu-id="fd608-134">[Contact](contact.md)</span></span>
    
- [<span data-ttu-id="fd608-135">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="fd608-135">ItemId</span></span>](itemid.md)
    
- [<span data-ttu-id="fd608-136">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="fd608-136">ParentFolderId</span></span>](parentfolderid.md)
    
- [<span data-ttu-id="fd608-137">ItemClass</span><span class="sxs-lookup"><span data-stu-id="fd608-137">ItemClass</span></span>](itemclass.md)
    
- [<span data-ttu-id="fd608-138">Sensitivity</span><span class="sxs-lookup"><span data-stu-id="fd608-138">Sensitivity</span></span>](sensitivity.md)
    
- [<span data-ttu-id="fd608-139">Body</span><span class="sxs-lookup"><span data-stu-id="fd608-139">Body</span></span>](body.md)
    
- [<span data-ttu-id="fd608-140">DateTimeReceived</span><span class="sxs-lookup"><span data-stu-id="fd608-140">DateTimeReceived</span></span>](datetimereceived.md)
    
- [<span data-ttu-id="fd608-141">Размер</span><span class="sxs-lookup"><span data-stu-id="fd608-141">Size</span></span>](size.md)
    
- [<span data-ttu-id="fd608-142">Importance</span><span class="sxs-lookup"><span data-stu-id="fd608-142">Importance</span></span>](importance.md)
    
- [<span data-ttu-id="fd608-143">Отправлено</span><span class="sxs-lookup"><span data-stu-id="fd608-143">IsSubmitted</span></span>](issubmitted.md)
    
- [<span data-ttu-id="fd608-144">Черновик</span><span class="sxs-lookup"><span data-stu-id="fd608-144">IsDraft</span></span>](isdraft.md)
    
- [<span data-ttu-id="fd608-145">исфромме</span><span class="sxs-lookup"><span data-stu-id="fd608-145">IsFromMe</span></span>](isfromme.md)
    
- [<span data-ttu-id="fd608-146">исресенд</span><span class="sxs-lookup"><span data-stu-id="fd608-146">IsResend</span></span>](isresend.md)
    
- [<span data-ttu-id="fd608-147">исунмодифиед</span><span class="sxs-lookup"><span data-stu-id="fd608-147">IsUnmodified</span></span>](isunmodified.md)
    
- [<span data-ttu-id="fd608-148">датетимесент</span><span class="sxs-lookup"><span data-stu-id="fd608-148">DateTimeSent</span></span>](datetimesent.md)
    
- [<span data-ttu-id="fd608-149">DateTimeCreated</span><span class="sxs-lookup"><span data-stu-id="fd608-149">DateTimeCreated</span></span>](datetimecreated.md)
    
- [<span data-ttu-id="fd608-150">HasAttachments</span><span class="sxs-lookup"><span data-stu-id="fd608-150">HasAttachments</span></span>](hasattachments.md)
    
- [<span data-ttu-id="fd608-151">Culture</span><span class="sxs-lookup"><span data-stu-id="fd608-151">Culture</span></span>](culture.md)
    
- [<span data-ttu-id="fd608-152">FileAs</span><span class="sxs-lookup"><span data-stu-id="fd608-152">FileAs</span></span>](fileas.md)
    
- [<span data-ttu-id="fd608-153">филеасмаппинг</span><span class="sxs-lookup"><span data-stu-id="fd608-153">FileAsMapping</span></span>](fileasmapping.md)
    
- [<span data-ttu-id="fd608-154">DisplayName (строка)</span><span class="sxs-lookup"><span data-stu-id="fd608-154">DisplayName (string)</span></span>](displayname-string.md)
    
- [<span data-ttu-id="fd608-155">GivenName</span><span class="sxs-lookup"><span data-stu-id="fd608-155">GivenName</span></span>](givenname.md)
    
- [<span data-ttu-id="fd608-156">Initials</span><span class="sxs-lookup"><span data-stu-id="fd608-156">Initials</span></span>](initials.md)
    
- [<span data-ttu-id="fd608-157">комплетенаме</span><span class="sxs-lookup"><span data-stu-id="fd608-157">CompleteName</span></span>](completename.md)
    
- [<span data-ttu-id="fd608-158">FirstName</span><span class="sxs-lookup"><span data-stu-id="fd608-158">FirstName</span></span>](firstname.md)
    
- [<span data-ttu-id="fd608-159">LastName</span><span class="sxs-lookup"><span data-stu-id="fd608-159">LastName</span></span>](lastname.md)
    
- [<span data-ttu-id="fd608-160">FullName</span><span class="sxs-lookup"><span data-stu-id="fd608-160">FullName</span></span>](fullname.md)
    
- [<span data-ttu-id="fd608-161">CompanyName</span><span class="sxs-lookup"><span data-stu-id="fd608-161">CompanyName</span></span>](companyname.md)
    
- [<span data-ttu-id="fd608-162">EmailAddresses</span><span class="sxs-lookup"><span data-stu-id="fd608-162">EmailAddresses</span></span>](emailaddresses.md)
    
- [<span data-ttu-id="fd608-163">Запись (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="fd608-163">Entry (EmailAddress)</span></span>](entry-emailaddress.md)
    
- [<span data-ttu-id="fd608-164">фисикаладдрессес</span><span class="sxs-lookup"><span data-stu-id="fd608-164">PhysicalAddresses</span></span>](physicaladdresses.md)
    
- [<span data-ttu-id="fd608-165">Запись (PhysicalAddress)</span><span class="sxs-lookup"><span data-stu-id="fd608-165">Entry (PhysicalAddress)</span></span>](entry-physicaladdress.md)
    
- [<span data-ttu-id="fd608-166">Назван</span><span class="sxs-lookup"><span data-stu-id="fd608-166">Street</span></span>](street.md)
    
- [<span data-ttu-id="fd608-167">City</span><span class="sxs-lookup"><span data-stu-id="fd608-167">City</span></span>](city.md)
    
- [<span data-ttu-id="fd608-168">State</span><span class="sxs-lookup"><span data-stu-id="fd608-168">State</span></span>](state-ex15websvcsotherref.md)
    
- [<span data-ttu-id="fd608-169">CountryOrRegion</span><span class="sxs-lookup"><span data-stu-id="fd608-169">CountryOrRegion</span></span>](countryorregion.md)
    
- [<span data-ttu-id="fd608-170">PhoneNumbers</span><span class="sxs-lookup"><span data-stu-id="fd608-170">PhoneNumbers</span></span>](phonenumbers.md)
    
- [<span data-ttu-id="fd608-171">Запись (PhoneNumber)</span><span class="sxs-lookup"><span data-stu-id="fd608-171">Entry (PhoneNumber)</span></span>](entry-phonenumber.md)
    
- [<span data-ttu-id="fd608-172">JobTitle</span><span class="sxs-lookup"><span data-stu-id="fd608-172">JobTitle</span></span>](jobtitle.md)
    
- [<span data-ttu-id="fd608-173">ФИО</span><span class="sxs-lookup"><span data-stu-id="fd608-173">Surname</span></span>](surname.md)
    
## <a name="invalid-getitem-contact-request-example"></a><span data-ttu-id="fd608-174">Недопустимый пример запроса GetItem (Contact)</span><span class="sxs-lookup"><span data-stu-id="fd608-174">Invalid GetItem (Contact) request example</span></span>

### <a name="description"></a><span data-ttu-id="fd608-175">Описание</span><span class="sxs-lookup"><span data-stu-id="fd608-175">Description</span></span>

<span data-ttu-id="fd608-176">В следующем примере кода показан недопустимый запрос.</span><span class="sxs-lookup"><span data-stu-id="fd608-176">The following code example shows an invalid request.</span></span>
  
### <a name="code"></a><span data-ttu-id="fd608-177">Код</span><span class="sxs-lookup"><span data-stu-id="fd608-177">Code</span></span>

```XML
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <GetItem xmlns='https://schemas.microsoft.com/exchange/services/2006/messages'>
      <ItemShape>
        <t:BaseShape>AllProperties</t:BaseShape>
        <t:IncludeMimeContent>true</t:IncludeMimeContent>
      </ItemShape>
      <ItemIds>
        <t:ItemId Id="AAAtAEF=" ChangeKey="EQAAABq" />
      </ItemIds>
    </GetItem>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="fd608-178">Комментарии</span><span class="sxs-lookup"><span data-stu-id="fd608-178">Comments</span></span>

<span data-ttu-id="fd608-179">Идентификаторы элементов были сокращены для сохранения удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="fd608-179">Item identifiers have been shortened to preserve readability.</span></span>
  
## <a name="getitem-contact-error-response"></a><span data-ttu-id="fd608-180">Ответ об ошибке GetItem (Contact)</span><span class="sxs-lookup"><span data-stu-id="fd608-180">GetItem (Contact) error response</span></span>

### <a name="description"></a><span data-ttu-id="fd608-181">Описание</span><span class="sxs-lookup"><span data-stu-id="fd608-181">Description</span></span>

<span data-ttu-id="fd608-182">В следующем примере кода показан ответ с сообщением об ошибке для запроса GetItem (Contact).</span><span class="sxs-lookup"><span data-stu-id="fd608-182">The following code example shows an error response to a GetItem (Contact) request.</span></span>
  
### <a name="code"></a><span data-ttu-id="fd608-183">Код</span><span class="sxs-lookup"><span data-stu-id="fd608-183">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="602" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <GetItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                     xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                     xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:GetItemResponseMessage ResponseClass="Error">
          <m:MessageText>Mime conversion is not supported for this item type.</m:MessageText>
          <m:ResponseCode>ErrorUnsupportedMimeConversion</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
          <m:Items />
        </m:GetItemResponseMessage>
      </m:ResponseMessages>
    </GetItemResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="error-response-elements"></a><span data-ttu-id="fd608-184">Элементы ошибочного ответа</span><span class="sxs-lookup"><span data-stu-id="fd608-184">Error response elements</span></span>

<span data-ttu-id="fd608-185">В ответе на сообщение об ошибке используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="fd608-185">The following elements are used in the error response:</span></span>
  
- [<span data-ttu-id="fd608-186">серверверсионинфо</span><span class="sxs-lookup"><span data-stu-id="fd608-186">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="fd608-187">жетитемреспонсе</span><span class="sxs-lookup"><span data-stu-id="fd608-187">GetItemResponse</span></span>](getitemresponse.md)
    
- [<span data-ttu-id="fd608-188">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="fd608-188">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="fd608-189">жетитемреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="fd608-189">GetItemResponseMessage</span></span>](getitemresponsemessage.md)
    
- [<span data-ttu-id="fd608-190">мессажетекст</span><span class="sxs-lookup"><span data-stu-id="fd608-190">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="fd608-191">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="fd608-191">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="fd608-192">дескриптивелинккэй</span><span class="sxs-lookup"><span data-stu-id="fd608-192">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
- [<span data-ttu-id="fd608-193">Items</span><span class="sxs-lookup"><span data-stu-id="fd608-193">Items</span></span>](items.md)
    
## <a name="see-also"></a><span data-ttu-id="fd608-194">См. также</span><span class="sxs-lookup"><span data-stu-id="fd608-194">See also</span></span>



[<span data-ttu-id="fd608-195">Операция GetItem</span><span class="sxs-lookup"><span data-stu-id="fd608-195">GetItem operation</span></span>](getitem-operation.md)


- [<span data-ttu-id="fd608-196">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="fd608-196">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

