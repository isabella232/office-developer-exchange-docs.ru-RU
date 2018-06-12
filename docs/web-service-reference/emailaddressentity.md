---
title: EmailAddressEntity
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 20049467-c01a-4c7d-8ada-ca1801cc95ed
description: Элемент EmailAddressEntity указывает адрес сущностям одного адреса электронной почты.
ms.openlocfilehash: c149ee69c1ed08c33d0341c8dfdac3bcda040afb
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762290"
---
# <a name="emailaddressentity"></a><span data-ttu-id="46d68-103">EmailAddressEntity</span><span class="sxs-lookup"><span data-stu-id="46d68-103">EmailAddressEntity</span></span>

<span data-ttu-id="46d68-104">Элемент **EmailAddressEntity** указывает адрес сущностям одного адреса электронной почты.</span><span class="sxs-lookup"><span data-stu-id="46d68-104">The **EmailAddressEntity** element specifies a single email address entity.</span></span> 
  
```XML
<EmailAddressEntity>
    <EmailAddress></EmailAddress>
</EmailAddressEntity>
```

 <span data-ttu-id="46d68-105">**EmailAddressEntityType**</span><span class="sxs-lookup"><span data-stu-id="46d68-105">**EmailAddressEntityType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="46d68-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="46d68-106">Attributes and elements</span></span>

<span data-ttu-id="46d68-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="46d68-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="46d68-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="46d68-108">Attributes</span></span>

<span data-ttu-id="46d68-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="46d68-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="46d68-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="46d68-110">Child elements</span></span>

|<span data-ttu-id="46d68-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="46d68-111">**Element**</span></span>|<span data-ttu-id="46d68-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="46d68-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="46d68-113">EmailAddress (строка)</span><span class="sxs-lookup"><span data-stu-id="46d68-113">EmailAddress (string)</span></span>](emailaddress-string.md) <br/> |<span data-ttu-id="46d68-114">Указывает отдельный адрес электронной почты.</span><span class="sxs-lookup"><span data-stu-id="46d68-114">Specifies a single email address.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="46d68-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="46d68-115">Parent elements</span></span>

|<span data-ttu-id="46d68-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="46d68-116">**Element**</span></span>|<span data-ttu-id="46d68-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="46d68-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="46d68-118">EmailAddresses (ArrayOfEmailAddressEntitiesType)</span><span class="sxs-lookup"><span data-stu-id="46d68-118">EmailAddresses (ArrayOfEmailAddressEntitiesType)</span></span>](emailaddresses-arrayofemailaddressentitiestype.md) <br/> |<span data-ttu-id="46d68-119">Указывает массив сущностей, адрес электронной почты.</span><span class="sxs-lookup"><span data-stu-id="46d68-119">Specifies an array of email address entities.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="46d68-120">Замечания</span><span class="sxs-lookup"><span data-stu-id="46d68-120">Remarks</span></span>

<span data-ttu-id="46d68-121">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="46d68-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="46d68-122">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="46d68-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="46d68-123">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="46d68-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="46d68-124">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="46d68-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="46d68-125">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="46d68-125">Schema Name</span></span>  <br/> |<span data-ttu-id="46d68-126">Схема типа</span><span class="sxs-lookup"><span data-stu-id="46d68-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="46d68-127">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="46d68-127">Validation File</span></span>  <br/> |<span data-ttu-id="46d68-128">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="46d68-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="46d68-129">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="46d68-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="46d68-130">См. также</span><span class="sxs-lookup"><span data-stu-id="46d68-130">See also</span></span>



- [<span data-ttu-id="46d68-131">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="46d68-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

