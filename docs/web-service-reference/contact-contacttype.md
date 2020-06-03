---
title: Контактное лицо (Контакттипе)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 7f7119b7-f5b4-484d-a7de-fa74836d9aee
description: Элемент Contact указывает контакт в едином хранилище контактов.
ms.openlocfilehash: e8ebc28456f8bfc26f5d790ac9ff278930041ea0
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461522"
---
# <a name="contact-contacttype"></a><span data-ttu-id="5844a-103">Контактное лицо (Контакттипе)</span><span class="sxs-lookup"><span data-stu-id="5844a-103">Contact (ContactType)</span></span>

<span data-ttu-id="5844a-104">Элемент **Contact** указывает контакт в едином хранилище контактов.</span><span class="sxs-lookup"><span data-stu-id="5844a-104">The **Contact** element specifies a contact in the Unified Contact Store.</span></span> 
  
```XML
<Contact>
    <PersonName></PersonName>
    <BusinessName></BusinessName>
    <PhoneNumbers></PhoneNumbers>
    <Urls></Urls>
    <EmailAddresses></EmailAddresses>
    <Addresses></Addesses>    <ContactString></ContactString
</Contact>
```

 <span data-ttu-id="5844a-105">**контакттипе**</span><span class="sxs-lookup"><span data-stu-id="5844a-105">**ContactType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5844a-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="5844a-106">Attributes and elements</span></span>

<span data-ttu-id="5844a-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="5844a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5844a-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="5844a-108">Attributes</span></span>

<span data-ttu-id="5844a-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="5844a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5844a-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="5844a-110">Child elements</span></span>

|<span data-ttu-id="5844a-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="5844a-111">**Element**</span></span>|<span data-ttu-id="5844a-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="5844a-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5844a-113">PersonName</span><span class="sxs-lookup"><span data-stu-id="5844a-113">PersonName</span></span>](personname.md) <br/> |<span data-ttu-id="5844a-114">Указывает имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="5844a-114">Specifies the name of an individual.</span></span>  <br/> |
|[<span data-ttu-id="5844a-115">BusinessName</span><span class="sxs-lookup"><span data-stu-id="5844a-115">BusinessName</span></span>](businessname.md) <br/> |<span data-ttu-id="5844a-116">Указывает название организации.</span><span class="sxs-lookup"><span data-stu-id="5844a-116">Specifies the name of a business.</span></span>  <br/> |
|[<span data-ttu-id="5844a-117">PhoneNumbers</span><span class="sxs-lookup"><span data-stu-id="5844a-117">PhoneNumbers</span></span>](phonenumbers.md) <br/> |<span data-ttu-id="5844a-118">Представляет коллекцию телефонных номеров контакта.</span><span class="sxs-lookup"><span data-stu-id="5844a-118">Represents a collection of telephone numbers for a contact.</span></span>  <br/> |
|[<span data-ttu-id="5844a-119">Urls</span><span class="sxs-lookup"><span data-stu-id="5844a-119">Urls</span></span>](urls.md) <br/> |<span data-ttu-id="5844a-120">Указывает массив URL-адресов для пользователя.</span><span class="sxs-lookup"><span data-stu-id="5844a-120">Specifies an array of URLs for a persona.</span></span>  <br/> |
|[<span data-ttu-id="5844a-121">EmailAddresses (Аррайофекстрактедемаиладдрессес)</span><span class="sxs-lookup"><span data-stu-id="5844a-121">EmailAddresses (ArrayOfExtractedEmailAddresses)</span></span>](emailaddresses-arrayofextractedemailaddresses.md) <br/> |<span data-ttu-id="5844a-122">Указывает массив извлеченных адресов электронной почты.</span><span class="sxs-lookup"><span data-stu-id="5844a-122">Specifies an array of extracted email addresses.</span></span>  <br/> |
|[<span data-ttu-id="5844a-123">Адреса (Аррайофаддрессестипе)</span><span class="sxs-lookup"><span data-stu-id="5844a-123">Addresses (ArrayOfAddressesType)</span></span>](addresses-arrayofaddressestype.md) <br/> |<span data-ttu-id="5844a-124">Указывает массив элементов **Address** .</span><span class="sxs-lookup"><span data-stu-id="5844a-124">Specifies an array of **Address** elements.</span></span>  <br/> |
|[<span data-ttu-id="5844a-125">контактстринг</span><span class="sxs-lookup"><span data-stu-id="5844a-125">ContactString</span></span>](contactstring.md) <br/> |<span data-ttu-id="5844a-126">Задает отображаемое имя контакта.</span><span class="sxs-lookup"><span data-stu-id="5844a-126">Specifies the display name of a contact.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="5844a-127">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="5844a-127">Parent elements</span></span>

|<span data-ttu-id="5844a-128">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="5844a-128">**Element**</span></span>|<span data-ttu-id="5844a-129">**Описание**</span><span class="sxs-lookup"><span data-stu-id="5844a-129">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5844a-130">Contacts (Аррайофконтактстипе)</span><span class="sxs-lookup"><span data-stu-id="5844a-130">Contacts (ArrayOfContactsType)</span></span>](contacts-arrayofcontactstype.md) <br/> |<span data-ttu-id="5844a-131">Указывает массив контактов.</span><span class="sxs-lookup"><span data-stu-id="5844a-131">Specifies an array of contacts.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="5844a-132">Примечания</span><span class="sxs-lookup"><span data-stu-id="5844a-132">Remarks</span></span>

<span data-ttu-id="5844a-133">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="5844a-133">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="5844a-134">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="5844a-134">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5844a-135">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="5844a-135">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5844a-136">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="5844a-136">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="5844a-137">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="5844a-137">Schema Name</span></span>  <br/> |<span data-ttu-id="5844a-138">Схема типа</span><span class="sxs-lookup"><span data-stu-id="5844a-138">Type schema</span></span>  <br/> |
|<span data-ttu-id="5844a-139">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="5844a-139">Validation File</span></span>  <br/> |<span data-ttu-id="5844a-140">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="5844a-140">types.xsd</span></span>  <br/> |
|<span data-ttu-id="5844a-141">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="5844a-141">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="5844a-142">См. также</span><span class="sxs-lookup"><span data-stu-id="5844a-142">See also</span></span>



- [<span data-ttu-id="5844a-143">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="5844a-143">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

