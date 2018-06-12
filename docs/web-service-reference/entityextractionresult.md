---
title: EntityExtractionResult
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 643b99ab-ff90-4411-864c-1077623028d6
description: Элемент EntityExtractionResult указывает свойство EntityExtractionResult элемента.
ms.openlocfilehash: ef99629beb95f1e1123569fa99e3f495c1b56e95
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762371"
---
# <a name="entityextractionresult"></a><span data-ttu-id="4cfe1-103">EntityExtractionResult</span><span class="sxs-lookup"><span data-stu-id="4cfe1-103">EntityExtractionResult</span></span>

<span data-ttu-id="4cfe1-104">Элемент **EntityExtractionResult** указывает свойство **EntityExtractionResult** элемента.</span><span class="sxs-lookup"><span data-stu-id="4cfe1-104">The **EntityExtractionResult** element specifies the **EntityExtractionResult** property of an item.</span></span> 
  
```XML
<EntityExtractionResult>
    <Addresses/>
    <MeetingSuggestions/>
    <TaskSuggestions/>
    <EmailAddresses/>
    <Contacts/>
    <Urls/>
    <PhoneNumbers/>
</EntityExtractionResult>
```

 <span data-ttu-id="4cfe1-105">**EntityExtractionResultType**</span><span class="sxs-lookup"><span data-stu-id="4cfe1-105">**EntityExtractionResultType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4cfe1-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="4cfe1-106">Attributes and elements</span></span>

<span data-ttu-id="4cfe1-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="4cfe1-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4cfe1-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="4cfe1-108">Attributes</span></span>

<span data-ttu-id="4cfe1-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="4cfe1-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4cfe1-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="4cfe1-110">Child elements</span></span>

|<span data-ttu-id="4cfe1-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="4cfe1-111">**Element**</span></span>|<span data-ttu-id="4cfe1-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="4cfe1-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4cfe1-113">Адреса (ArrayOfAddressEntitiesType)</span><span class="sxs-lookup"><span data-stu-id="4cfe1-113">Addresses (ArrayOfAddressEntitiesType)</span></span>](addresses-arrayofaddressentitiestype.md) <br/> |<span data-ttu-id="4cfe1-114">Указывает массив элементов **AddressEntity** .</span><span class="sxs-lookup"><span data-stu-id="4cfe1-114">Specifies an array of **AddressEntity** elements.</span></span>  <br/> |
|[<span data-ttu-id="4cfe1-115">MeetingSuggestions</span><span class="sxs-lookup"><span data-stu-id="4cfe1-115">MeetingSuggestions</span></span>](meetingsuggestions.md) <br/> |<span data-ttu-id="4cfe1-116">Указывает массив элементов **MeetingSuggestion** .</span><span class="sxs-lookup"><span data-stu-id="4cfe1-116">Specifies an array of **MeetingSuggestion** elements.</span></span>  <br/> |
|[<span data-ttu-id="4cfe1-117">TaskSuggestions</span><span class="sxs-lookup"><span data-stu-id="4cfe1-117">TaskSuggestions</span></span>](tasksuggestions.md) <br/> |<span data-ttu-id="4cfe1-118">Указывает массив элементов **TaskSuggestion** .</span><span class="sxs-lookup"><span data-stu-id="4cfe1-118">Specifies an array of **TaskSuggestion** elements.</span></span>  <br/> |
|[<span data-ttu-id="4cfe1-119">EmailAddresses (ArrayOfEmailAddressEntitiesType)</span><span class="sxs-lookup"><span data-stu-id="4cfe1-119">EmailAddresses (ArrayOfEmailAddressEntitiesType)</span></span>](emailaddresses-arrayofemailaddressentitiestype.md) <br/> |<span data-ttu-id="4cfe1-120">Указывает массив сущностей, адрес электронной почты.</span><span class="sxs-lookup"><span data-stu-id="4cfe1-120">Specifies an array of email address entities.</span></span>  <br/> |
|[<span data-ttu-id="4cfe1-121">Контакты (ArrayOfContactsType)</span><span class="sxs-lookup"><span data-stu-id="4cfe1-121">Contacts (ArrayOfContactsType)</span></span>](contacts-arrayofcontactstype.md) <br/> |<span data-ttu-id="4cfe1-122">Указывает массив контакты.</span><span class="sxs-lookup"><span data-stu-id="4cfe1-122">Specifies an array of contacts.</span></span>  <br/> |
|[<span data-ttu-id="4cfe1-123">URL-адреса (ArrayOfUrlEntitiesType)</span><span class="sxs-lookup"><span data-stu-id="4cfe1-123">Urls (ArrayOfUrlEntitiesType)</span></span>](urls-arrayofurlentitiestype.md) <br/> |<span data-ttu-id="4cfe1-124">Указывает массив URL-адресов.</span><span class="sxs-lookup"><span data-stu-id="4cfe1-124">Specifies an array of URLs.</span></span>  <br/> |
|[<span data-ttu-id="4cfe1-125">PhoneNumbers (ArrayOfPhoneEntitiesType)</span><span class="sxs-lookup"><span data-stu-id="4cfe1-125">PhoneNumbers (ArrayOfPhoneEntitiesType)</span></span>](phonenumbers-arrayofphoneentitiestype.md) <br/> |<span data-ttu-id="4cfe1-126">Указывает массив телефонных номеров.</span><span class="sxs-lookup"><span data-stu-id="4cfe1-126">Specifies an array of phone numbers.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="4cfe1-127">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="4cfe1-127">Parent elements</span></span>

|<span data-ttu-id="4cfe1-128">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="4cfe1-128">**Element**</span></span>|<span data-ttu-id="4cfe1-129">**Описание**</span><span class="sxs-lookup"><span data-stu-id="4cfe1-129">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4cfe1-130">Элемент</span><span class="sxs-lookup"><span data-stu-id="4cfe1-130">Item</span></span>](item.md) <br/> |<span data-ttu-id="4cfe1-131">Представляет универсальный элемент в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="4cfe1-131">Represents a generic item in the Exchange store.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="4cfe1-132">Замечания</span><span class="sxs-lookup"><span data-stu-id="4cfe1-132">Remarks</span></span>

<span data-ttu-id="4cfe1-133">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="4cfe1-133">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="4cfe1-134">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="4cfe1-134">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4cfe1-135">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="4cfe1-135">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4cfe1-136">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="4cfe1-136">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="4cfe1-137">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="4cfe1-137">Schema Name</span></span>  <br/> |<span data-ttu-id="4cfe1-138">Схема типа</span><span class="sxs-lookup"><span data-stu-id="4cfe1-138">Type schema</span></span>  <br/> |
|<span data-ttu-id="4cfe1-139">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="4cfe1-139">Validation File</span></span>  <br/> |<span data-ttu-id="4cfe1-140">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="4cfe1-140">types.xsd</span></span>  <br/> |
|<span data-ttu-id="4cfe1-141">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="4cfe1-141">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="4cfe1-142">См. также</span><span class="sxs-lookup"><span data-stu-id="4cfe1-142">See also</span></span>



- [<span data-ttu-id="4cfe1-143">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="4cfe1-143">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
