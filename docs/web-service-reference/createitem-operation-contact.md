---
title: Операция CreateItem (Contact)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CreateItem
api_type:
- schema
ms.assetid: 417e994b-0a17-4c24-9527-04796b80b029
description: Операция CreateItem используется для создания контактов в хранилище Exchange.
ms.openlocfilehash: e1d78392b94d328cf687655cd93e6c9568f6274f
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457125"
---
# <a name="createitem-operation-contact"></a><span data-ttu-id="fea24-103">Операция CreateItem (Contact)</span><span class="sxs-lookup"><span data-stu-id="fea24-103">CreateItem operation (contact)</span></span>

<span data-ttu-id="fea24-104">Операция CreateItem используется для создания контактов в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="fea24-104">The CreateItem operation is used to create contacts in the Exchange store.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="fea24-105">Примечания</span><span class="sxs-lookup"><span data-stu-id="fea24-105">Remarks</span></span>

<span data-ttu-id="fea24-106">Создание частных списков рассылки не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fea24-106">The creation of private distribution lists is not supported.</span></span> <span data-ttu-id="fea24-107">Все свойства в контейнере [комплетенаме](completename.md) доступны только для чтения и не могут быть заданы для элемента контакта.</span><span class="sxs-lookup"><span data-stu-id="fea24-107">All properties within the [CompleteName](completename.md) container are read-only and cannot be set on a contact item.</span></span> 
  
## <a name="createitem-request-example"></a><span data-ttu-id="fea24-108">Пример запроса CreateItem</span><span class="sxs-lookup"><span data-stu-id="fea24-108">CreateItem request example</span></span>

### <a name="description"></a><span data-ttu-id="fea24-109">Описание</span><span class="sxs-lookup"><span data-stu-id="fea24-109">Description</span></span>

<span data-ttu-id="fea24-110">В приведенном ниже примере допустимого запроса в виде CreateItem SOAP показано, как создать контакт в папке "Контакты" по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="fea24-110">The following example of a valid CreateItem SOAP request shows how to create a contact in the default Contacts folder.</span></span>
  
### <a name="code"></a><span data-ttu-id="fea24-111">Код</span><span class="sxs-lookup"><span data-stu-id="fea24-111">Code</span></span>

```XML
<soap:Envelope
 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
 xmlns:xsd="http://www.w3.org/2001/XMLSchema"
 xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
 xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <CreateItem xmlns="https://schemas.microsoft.com/exchange/services/2006/messages" >
      <SavedItemFolderId>
        <t:DistinguishedFolderId Id="contacts"/>
      </SavedItemFolderId>
      <Items>
        <t:Contact>
          <t:FileAs>SampleContact</t:FileAs>
          <t:GivenName>Tanja</t:GivenName>
          <t:CompanyName>Blue Yonder Airlines</t:CompanyName>
          <t:EmailAddresses>
            <t:Entry Key="EmailAddress1">tplate@example.com</t:Entry>
          </t:EmailAddresses>
          <t:PhysicalAddresses>
            <t:Entry Key="Business">
              <t:Street>1234 56th Ave</t:Street>
              <t:City>La Habra</t:City>
              <t:State>CA</t:State>
              <t: CountryOrRegion>USA</t: CountryOrRegion>
            </t:Entry>
          </t:PhysicalAddresses>
          <t:PhoneNumbers>
            <t:Entry Key="BusinessPhone">4255550199</t:Entry>
          </t:PhoneNumbers>
          <t:JobTitle>Manager</t:JobTitle>
          <t:Surname>Plate</t:Surname>
        </t:Contact>
      </Items>
    </CreateItem>
  </soap:Body>
</soap:Envelope>
```

### <a name="request-elements"></a><span data-ttu-id="fea24-112">Элементы Request</span><span class="sxs-lookup"><span data-stu-id="fea24-112">Request elements</span></span>

<span data-ttu-id="fea24-113">В отклике используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="fea24-113">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="fea24-114">CreateItem</span><span class="sxs-lookup"><span data-stu-id="fea24-114">CreateItem</span></span>](createitem.md)
    
- [<span data-ttu-id="fea24-115">саведитемфолдерид</span><span class="sxs-lookup"><span data-stu-id="fea24-115">SavedItemFolderId</span></span>](saveditemfolderid.md)
    
- [<span data-ttu-id="fea24-116">дистингуишедфолдерид</span><span class="sxs-lookup"><span data-stu-id="fea24-116">DistinguishedFolderId</span></span>](distinguishedfolderid.md)
    
- [<span data-ttu-id="fea24-117">Элементы (Нонемптяррайофаллитемстипе)</span><span class="sxs-lookup"><span data-stu-id="fea24-117">Items (NonEmptyArrayOfAllItemsType)</span></span>](items-nonemptyarrayofallitemstype.md)
    
- <span data-ttu-id="fea24-118">[контакт](contact.md);</span><span class="sxs-lookup"><span data-stu-id="fea24-118">[Contact](contact.md)</span></span>
    
- [<span data-ttu-id="fea24-119">FileAs</span><span class="sxs-lookup"><span data-stu-id="fea24-119">FileAs</span></span>](fileas.md)
    
- [<span data-ttu-id="fea24-120">GivenName</span><span class="sxs-lookup"><span data-stu-id="fea24-120">GivenName</span></span>](givenname.md)
    
- [<span data-ttu-id="fea24-121">CompanyName</span><span class="sxs-lookup"><span data-stu-id="fea24-121">CompanyName</span></span>](companyname.md)
    
- [<span data-ttu-id="fea24-122">EmailAddresses</span><span class="sxs-lookup"><span data-stu-id="fea24-122">EmailAddresses</span></span>](emailaddresses.md)
    
- [<span data-ttu-id="fea24-123">Запись (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="fea24-123">Entry (EmailAddress)</span></span>](entry-emailaddress.md)
    
- [<span data-ttu-id="fea24-124">фисикаладдрессес</span><span class="sxs-lookup"><span data-stu-id="fea24-124">PhysicalAddresses</span></span>](physicaladdresses.md)
    
- [<span data-ttu-id="fea24-125">Запись (PhysicalAddress)</span><span class="sxs-lookup"><span data-stu-id="fea24-125">Entry (PhysicalAddress)</span></span>](entry-physicaladdress.md)
    
- [<span data-ttu-id="fea24-126">Назван</span><span class="sxs-lookup"><span data-stu-id="fea24-126">Street</span></span>](street.md)
    
- [<span data-ttu-id="fea24-127">City</span><span class="sxs-lookup"><span data-stu-id="fea24-127">City</span></span>](city.md)
    
- [<span data-ttu-id="fea24-128">State</span><span class="sxs-lookup"><span data-stu-id="fea24-128">State</span></span>](state-ex15websvcsotherref.md)
    
- [<span data-ttu-id="fea24-129">CountryOrRegion</span><span class="sxs-lookup"><span data-stu-id="fea24-129">CountryOrRegion</span></span>](countryorregion.md)
    
- [<span data-ttu-id="fea24-130">PhoneNumbers</span><span class="sxs-lookup"><span data-stu-id="fea24-130">PhoneNumbers</span></span>](phonenumbers.md)
    
- [<span data-ttu-id="fea24-131">Запись (PhoneNumber)</span><span class="sxs-lookup"><span data-stu-id="fea24-131">Entry (PhoneNumber)</span></span>](entry-phonenumber.md)
    
- [<span data-ttu-id="fea24-132">JobTitle</span><span class="sxs-lookup"><span data-stu-id="fea24-132">JobTitle</span></span>](jobtitle.md)
    
- [<span data-ttu-id="fea24-133">ФИО</span><span class="sxs-lookup"><span data-stu-id="fea24-133">Surname</span></span>](surname.md)
    
## <a name="successful-createitem-request"></a><span data-ttu-id="fea24-134">Успешный запрос CreateItem</span><span class="sxs-lookup"><span data-stu-id="fea24-134">Successful CreateItem Request</span></span>

### <a name="description"></a><span data-ttu-id="fea24-135">Описание</span><span class="sxs-lookup"><span data-stu-id="fea24-135">Description</span></span>

<span data-ttu-id="fea24-136">В следующем примере показан успешный ответ на запрос CreateItem, который создал контакт.</span><span class="sxs-lookup"><span data-stu-id="fea24-136">The following example shows a successful response to the CreateItem request that created a contact.</span></span> <span data-ttu-id="fea24-137">В этом примере ответ содержит идентификатор только что созданного элемента.</span><span class="sxs-lookup"><span data-stu-id="fea24-137">In this example, the response contains the identifier of the newly created item.</span></span>
  
### <a name="code"></a><span data-ttu-id="fea24-138">Код</span><span class="sxs-lookup"><span data-stu-id="fea24-138">Code</span></span>

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
    <CreateItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                        xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                        xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:CreateItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items>
            <t:Contact>
              <t:ItemId Id="AAAtA=" ChangeKey="EQAAAB" />
            </t:Contact>
          </m:Items>
        </m:CreateItemResponseMessage>
      </m:ResponseMessages>
    </CreateItemResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="fea24-139">Комментарии</span><span class="sxs-lookup"><span data-stu-id="fea24-139">Comments</span></span>

<span data-ttu-id="fea24-140">Идентификатор элемента был сокращен, чтобы сохранить удобочитаемость.</span><span class="sxs-lookup"><span data-stu-id="fea24-140">The item identifier has been shortened to preserve readability.</span></span>
  
### <a name="successful-response-elements"></a><span data-ttu-id="fea24-141">Элементы успешного ответа</span><span class="sxs-lookup"><span data-stu-id="fea24-141">Successful response elements</span></span>

<span data-ttu-id="fea24-142">В отклике используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="fea24-142">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="fea24-143">серверверсионинфо</span><span class="sxs-lookup"><span data-stu-id="fea24-143">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="fea24-144">креатеитемреспонсе</span><span class="sxs-lookup"><span data-stu-id="fea24-144">CreateItemResponse</span></span>](createitemresponse.md)
    
- [<span data-ttu-id="fea24-145">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="fea24-145">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="fea24-146">креатеитемреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="fea24-146">CreateItemResponseMessage</span></span>](createitemresponsemessage.md)
    
- [<span data-ttu-id="fea24-147">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="fea24-147">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="fea24-148">Элементы (Нонемптяррайофаллитемстипе)</span><span class="sxs-lookup"><span data-stu-id="fea24-148">Items (NonEmptyArrayOfAllItemsType)</span></span>](items-nonemptyarrayofallitemstype.md)
    
- <span data-ttu-id="fea24-149">[контакт](contact.md);</span><span class="sxs-lookup"><span data-stu-id="fea24-149">[Contact](contact.md)</span></span>
    
- [<span data-ttu-id="fea24-150">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="fea24-150">ItemId</span></span>](itemid.md)
    
## <a name="invalid-createitem-request-example"></a><span data-ttu-id="fea24-151">Недопустимый пример запроса CreateItem</span><span class="sxs-lookup"><span data-stu-id="fea24-151">Invalid CreateItem request example</span></span>

### <a name="description"></a><span data-ttu-id="fea24-152">Описание</span><span class="sxs-lookup"><span data-stu-id="fea24-152">Description</span></span>

<span data-ttu-id="fea24-153">В следующем примере показан запрос, который содержит допустимый XML, но несовместимые инструкции.</span><span class="sxs-lookup"><span data-stu-id="fea24-153">The following example shows a request that contains valid XML but incompatible instructions.</span></span> <span data-ttu-id="fea24-154">Невозможно создать контакт в папке поиска.</span><span class="sxs-lookup"><span data-stu-id="fea24-154">A contact cannot be created in a search folder.</span></span>
  
### <a name="code"></a><span data-ttu-id="fea24-155">Код</span><span class="sxs-lookup"><span data-stu-id="fea24-155">Code</span></span>

```XML
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <CreateItem xmlns='https://schemas.microsoft.com/exchange/services/2006/messages'>
      <SavedItemFolderId>
        <t:DistinguishedFolderId Id='searchfolders'/>
      </SavedItemFolderId>
      <Items>
        <t:Contact>
          <t:ItemClass>IPM.Contact</t:ItemClass>
        </t:Contact>
      </Items>
    </CreateItem>
  </soap:Body>
</soap:Envelope>
```

## <a name="createitem-contact-error-response"></a><span data-ttu-id="fea24-156">Запрос ошибки CreateItem (Contact)</span><span class="sxs-lookup"><span data-stu-id="fea24-156">CreateItem (Contact) error response</span></span>

### <a name="description"></a><span data-ttu-id="fea24-157">Описание</span><span class="sxs-lookup"><span data-stu-id="fea24-157">Description</span></span>

<span data-ttu-id="fea24-158">В приведенном ниже примере показан ответ об ошибке для запроса CreateItem (Contact).</span><span class="sxs-lookup"><span data-stu-id="fea24-158">The following example shows an error response to a CreateItem (Contact) request.</span></span>
  
### <a name="code"></a><span data-ttu-id="fea24-159">Код</span><span class="sxs-lookup"><span data-stu-id="fea24-159">Code</span></span>

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
    <CreateItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                        xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                        xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:CreateItemResponseMessage ResponseClass="Error">
          <m:MessageText>Cannot create a contact in a non-contact Folder.</m:MessageText>
          <m:ResponseCode>ErrorCannotCreateContactInNonContactFolder</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
          <m:Items />
        </m:CreateItemResponseMessage>
      </m:ResponseMessages>
    </CreateItemResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="error-response-elements"></a><span data-ttu-id="fea24-160">Элементы ошибочного ответа</span><span class="sxs-lookup"><span data-stu-id="fea24-160">Error response elements</span></span>

<span data-ttu-id="fea24-161">В ответе на сообщение об ошибке используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="fea24-161">The following elements are used in the error response:</span></span>
  
- [<span data-ttu-id="fea24-162">серверверсионинфо</span><span class="sxs-lookup"><span data-stu-id="fea24-162">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="fea24-163">креатеитемреспонсе</span><span class="sxs-lookup"><span data-stu-id="fea24-163">CreateItemResponse</span></span>](createitemresponse.md)
    
- [<span data-ttu-id="fea24-164">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="fea24-164">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="fea24-165">креатеитемреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="fea24-165">CreateItemResponseMessage</span></span>](createitemresponsemessage.md)
    
- [<span data-ttu-id="fea24-166">мессажетекст</span><span class="sxs-lookup"><span data-stu-id="fea24-166">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="fea24-167">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="fea24-167">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="fea24-168">дескриптивелинккэй</span><span class="sxs-lookup"><span data-stu-id="fea24-168">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
- [<span data-ttu-id="fea24-169">Элементы (Нонемптяррайофаллитемстипе)</span><span class="sxs-lookup"><span data-stu-id="fea24-169">Items (NonEmptyArrayOfAllItemsType)</span></span>](items-nonemptyarrayofallitemstype.md)
    
## <a name="see-also"></a><span data-ttu-id="fea24-170">См. также</span><span class="sxs-lookup"><span data-stu-id="fea24-170">See also</span></span>



[<span data-ttu-id="fea24-171">Операция CreateItem</span><span class="sxs-lookup"><span data-stu-id="fea24-171">CreateItem operation</span></span>](createitem-operation.md)

