---
title: Операции CreateItem (контактов)
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
ms.openlocfilehash: 05e4715f3c6675401ae7afac852395f7459c02c9
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761892"
---
# <a name="createitem-operation-contact"></a><span data-ttu-id="0d654-103">Операции CreateItem (контактов)</span><span class="sxs-lookup"><span data-stu-id="0d654-103">CreateItem operation (contact)</span></span>

<span data-ttu-id="0d654-104">Операция CreateItem используется для создания контактов в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="0d654-104">The CreateItem operation is used to create contacts in the Exchange store.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="0d654-105">Замечания</span><span class="sxs-lookup"><span data-stu-id="0d654-105">Remarks</span></span>

<span data-ttu-id="0d654-106">Создание частные списки рассылки не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0d654-106">The creation of private distribution lists is not supported.</span></span> <span data-ttu-id="0d654-107">Все свойства в контейнере [CompleteName](completename.md) доступны только для чтения и не могут задаваться на элемента контакта.</span><span class="sxs-lookup"><span data-stu-id="0d654-107">All properties within the [CompleteName](completename.md) container are read-only and cannot be set on a contact item.</span></span> 
  
## <a name="createitem-request-example"></a><span data-ttu-id="0d654-108">Пример запроса CreateItem</span><span class="sxs-lookup"><span data-stu-id="0d654-108">CreateItem request example</span></span>

### <a name="description"></a><span data-ttu-id="0d654-109">Описание</span><span class="sxs-lookup"><span data-stu-id="0d654-109">Description</span></span>

<span data-ttu-id="0d654-110">Допустимый запрос CreateItem SOAP в следующем примере показано, как создание контактов в папке контактов по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="0d654-110">The following example of a valid CreateItem SOAP request shows how to create a contact in the default Contacts folder.</span></span>
  
### <a name="code"></a><span data-ttu-id="0d654-111">Программа</span><span class="sxs-lookup"><span data-stu-id="0d654-111">Code</span></span>

```XML
<soap:Envelope
 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
 xmlns:xsd="http://www.w3.org/2001/XMLSchema"
 xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
 xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <CreateItem xmlns="http://schemas.microsoft.com/exchange/services/2006/messages" >
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

### <a name="request-elements"></a><span data-ttu-id="0d654-112">Элементы запроса</span><span class="sxs-lookup"><span data-stu-id="0d654-112">Request elements</span></span>

<span data-ttu-id="0d654-113">В ответе используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="0d654-113">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="0d654-114">CreateItem</span><span class="sxs-lookup"><span data-stu-id="0d654-114">CreateItem</span></span>](createitem.md)
    
- [<span data-ttu-id="0d654-115">SavedItemFolderId</span><span class="sxs-lookup"><span data-stu-id="0d654-115">SavedItemFolderId</span></span>](saveditemfolderid.md)
    
- [<span data-ttu-id="0d654-116">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="0d654-116">DistinguishedFolderId</span></span>](distinguishedfolderid.md)
    
- [<span data-ttu-id="0d654-117">Элементы (NonEmptyArrayOfAllItemsType)</span><span class="sxs-lookup"><span data-stu-id="0d654-117">Items (NonEmptyArrayOfAllItemsType)</span></span>](items-nonemptyarrayofallitemstype.md)
    
- [<span data-ttu-id="0d654-118">Контакт</span><span class="sxs-lookup"><span data-stu-id="0d654-118">Contact</span></span>](contact.md)
    
- [<span data-ttu-id="0d654-119">FileAs</span><span class="sxs-lookup"><span data-stu-id="0d654-119">FileAs</span></span>](fileas.md)
    
- [<span data-ttu-id="0d654-120">GivenName</span><span class="sxs-lookup"><span data-stu-id="0d654-120">GivenName</span></span>](givenname.md)
    
- [<span data-ttu-id="0d654-121">Название организации</span><span class="sxs-lookup"><span data-stu-id="0d654-121">CompanyName</span></span>](companyname.md)
    
- [<span data-ttu-id="0d654-122">EmailAddresses</span><span class="sxs-lookup"><span data-stu-id="0d654-122">EmailAddresses</span></span>](emailaddresses.md)
    
- [<span data-ttu-id="0d654-123">Запись (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="0d654-123">Entry (EmailAddress)</span></span>](entry-emailaddress.md)
    
- [<span data-ttu-id="0d654-124">PhysicalAddresses</span><span class="sxs-lookup"><span data-stu-id="0d654-124">PhysicalAddresses</span></span>](physicaladdresses.md)
    
- [<span data-ttu-id="0d654-125">Запись (PhysicalAddress)</span><span class="sxs-lookup"><span data-stu-id="0d654-125">Entry (PhysicalAddress)</span></span>](entry-physicaladdress.md)
    
- [<span data-ttu-id="0d654-126">Улица</span><span class="sxs-lookup"><span data-stu-id="0d654-126">Street</span></span>](street.md)
    
- [<span data-ttu-id="0d654-127">Город</span><span class="sxs-lookup"><span data-stu-id="0d654-127">City</span></span>](city.md)
    
- [<span data-ttu-id="0d654-128">Состояние</span><span class="sxs-lookup"><span data-stu-id="0d654-128">State</span></span>](state-ex15websvcsotherref.md)
    
- [<span data-ttu-id="0d654-129">CountryOrRegion</span><span class="sxs-lookup"><span data-stu-id="0d654-129">CountryOrRegion</span></span>](countryorregion.md)
    
- [<span data-ttu-id="0d654-130">PhoneNumbers</span><span class="sxs-lookup"><span data-stu-id="0d654-130">PhoneNumbers</span></span>](phonenumbers.md)
    
- [<span data-ttu-id="0d654-131">Запись (PhoneNumber)</span><span class="sxs-lookup"><span data-stu-id="0d654-131">Entry (PhoneNumber)</span></span>](entry-phonenumber.md)
    
- [<span data-ttu-id="0d654-132">Название должности</span><span class="sxs-lookup"><span data-stu-id="0d654-132">JobTitle</span></span>](jobtitle.md)
    
- [<span data-ttu-id="0d654-133">Фамилия</span><span class="sxs-lookup"><span data-stu-id="0d654-133">Surname</span></span>](surname.md)
    
## <a name="successful-createitem-request"></a><span data-ttu-id="0d654-134">Успешный запрос CreateItem</span><span class="sxs-lookup"><span data-stu-id="0d654-134">Successful CreateItem Request</span></span>

### <a name="description"></a><span data-ttu-id="0d654-135">Описание</span><span class="sxs-lookup"><span data-stu-id="0d654-135">Description</span></span>

<span data-ttu-id="0d654-136">В следующем примере показано успешного ответа на запрос CreateItem, создавшего контакт.</span><span class="sxs-lookup"><span data-stu-id="0d654-136">The following example shows a successful response to the CreateItem request that created a contact.</span></span> <span data-ttu-id="0d654-137">В этом примере ответ содержит идентификатор только что созданный элемента.</span><span class="sxs-lookup"><span data-stu-id="0d654-137">In this example, the response contains the identifier of the newly created item.</span></span>
  
### <a name="code"></a><span data-ttu-id="0d654-138">Программа</span><span class="sxs-lookup"><span data-stu-id="0d654-138">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="602" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <CreateItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                        xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                        xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="comments"></a><span data-ttu-id="0d654-139">Комментарии</span><span class="sxs-lookup"><span data-stu-id="0d654-139">Comments</span></span>

<span data-ttu-id="0d654-140">Идентификатор элемента был усечен, чтобы сохранить удобочитаемость.</span><span class="sxs-lookup"><span data-stu-id="0d654-140">The item identifier has been shortened to preserve readability.</span></span>
  
### <a name="successful-response-elements"></a><span data-ttu-id="0d654-141">Элементы успешного ответа</span><span class="sxs-lookup"><span data-stu-id="0d654-141">Successful response elements</span></span>

<span data-ttu-id="0d654-142">В ответе используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="0d654-142">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="0d654-143">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="0d654-143">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="0d654-144">CreateItemResponse</span><span class="sxs-lookup"><span data-stu-id="0d654-144">CreateItemResponse</span></span>](createitemresponse.md)
    
- [<span data-ttu-id="0d654-145">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="0d654-145">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="0d654-146">CreateItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="0d654-146">CreateItemResponseMessage</span></span>](createitemresponsemessage.md)
    
- [<span data-ttu-id="0d654-147">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="0d654-147">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="0d654-148">Элементы (NonEmptyArrayOfAllItemsType)</span><span class="sxs-lookup"><span data-stu-id="0d654-148">Items (NonEmptyArrayOfAllItemsType)</span></span>](items-nonemptyarrayofallitemstype.md)
    
- [<span data-ttu-id="0d654-149">Контакт</span><span class="sxs-lookup"><span data-stu-id="0d654-149">Contact</span></span>](contact.md)
    
- [<span data-ttu-id="0d654-150">Идентификатор элемента</span><span class="sxs-lookup"><span data-stu-id="0d654-150">ItemId</span></span>](itemid.md)
    
## <a name="invalid-createitem-request-example"></a><span data-ttu-id="0d654-151">Пример запроса недопустимый CreateItem</span><span class="sxs-lookup"><span data-stu-id="0d654-151">Invalid CreateItem request example</span></span>

### <a name="description"></a><span data-ttu-id="0d654-152">Описание</span><span class="sxs-lookup"><span data-stu-id="0d654-152">Description</span></span>

<span data-ttu-id="0d654-153">В следующем примере показано запрос, содержащий допустимый XML, но несовместимым инструкции.</span><span class="sxs-lookup"><span data-stu-id="0d654-153">The following example shows a request that contains valid XML but incompatible instructions.</span></span> <span data-ttu-id="0d654-154">Контакт не может быть создано в папки поиска.</span><span class="sxs-lookup"><span data-stu-id="0d654-154">A contact cannot be created in a search folder.</span></span>
  
### <a name="code"></a><span data-ttu-id="0d654-155">Программа</span><span class="sxs-lookup"><span data-stu-id="0d654-155">Code</span></span>

```XML
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <CreateItem xmlns='http://schemas.microsoft.com/exchange/services/2006/messages'>
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

## <a name="createitem-contact-error-response"></a><span data-ttu-id="0d654-156">Отклик CreateItem (контактов)</span><span class="sxs-lookup"><span data-stu-id="0d654-156">CreateItem (Contact) error response</span></span>

### <a name="description"></a><span data-ttu-id="0d654-157">Описание</span><span class="sxs-lookup"><span data-stu-id="0d654-157">Description</span></span>

<span data-ttu-id="0d654-158">В следующем примере показано ошибочный ответ на запрос CreateItem (контактов).</span><span class="sxs-lookup"><span data-stu-id="0d654-158">The following example shows an error response to a CreateItem (Contact) request.</span></span>
  
### <a name="code"></a><span data-ttu-id="0d654-159">Программа</span><span class="sxs-lookup"><span data-stu-id="0d654-159">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="602" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <CreateItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                        xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                        xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="error-response-elements"></a><span data-ttu-id="0d654-160">Элементы ответа об ошибках</span><span class="sxs-lookup"><span data-stu-id="0d654-160">Error response elements</span></span>

<span data-ttu-id="0d654-161">В ответ на ошибку используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="0d654-161">The following elements are used in the error response:</span></span>
  
- [<span data-ttu-id="0d654-162">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="0d654-162">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="0d654-163">CreateItemResponse</span><span class="sxs-lookup"><span data-stu-id="0d654-163">CreateItemResponse</span></span>](createitemresponse.md)
    
- [<span data-ttu-id="0d654-164">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="0d654-164">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="0d654-165">CreateItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="0d654-165">CreateItemResponseMessage</span></span>](createitemresponsemessage.md)
    
- [<span data-ttu-id="0d654-166">MessageText</span><span class="sxs-lookup"><span data-stu-id="0d654-166">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="0d654-167">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="0d654-167">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="0d654-168">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="0d654-168">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
- [<span data-ttu-id="0d654-169">Элементы (NonEmptyArrayOfAllItemsType)</span><span class="sxs-lookup"><span data-stu-id="0d654-169">Items (NonEmptyArrayOfAllItemsType)</span></span>](items-nonemptyarrayofallitemstype.md)
    
## <a name="see-also"></a><span data-ttu-id="0d654-170">См. также</span><span class="sxs-lookup"><span data-stu-id="0d654-170">See also</span></span>



[<span data-ttu-id="0d654-171">CreateItem Operation</span><span class="sxs-lookup"><span data-stu-id="0d654-171">CreateItem operation</span></span>](createitem-operation.md)

