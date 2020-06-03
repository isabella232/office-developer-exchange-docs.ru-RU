---
title: емаиладдрессентити
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 20049467-c01a-4c7d-8ada-ca1801cc95ed
description: Элемент Емаиладдрессентити указывает одну сущность адреса электронной почты.
ms.openlocfilehash: b76b08f93e60c8492906f3cc94e60f5725c8a9dc
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44526223"
---
# <a name="emailaddressentity"></a><span data-ttu-id="ced44-103">емаиладдрессентити</span><span class="sxs-lookup"><span data-stu-id="ced44-103">EmailAddressEntity</span></span>

<span data-ttu-id="ced44-104">Элемент **емаиладдрессентити** указывает одну сущность адреса электронной почты.</span><span class="sxs-lookup"><span data-stu-id="ced44-104">The **EmailAddressEntity** element specifies a single email address entity.</span></span> 
  
```XML
<EmailAddressEntity>
    <EmailAddress></EmailAddress>
</EmailAddressEntity>
```

 <span data-ttu-id="ced44-105">**емаиладдрессентититипе**</span><span class="sxs-lookup"><span data-stu-id="ced44-105">**EmailAddressEntityType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ced44-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="ced44-106">Attributes and elements</span></span>

<span data-ttu-id="ced44-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="ced44-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ced44-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="ced44-108">Attributes</span></span>

<span data-ttu-id="ced44-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="ced44-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ced44-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="ced44-110">Child elements</span></span>

|<span data-ttu-id="ced44-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="ced44-111">**Element**</span></span>|<span data-ttu-id="ced44-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="ced44-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ced44-113">EmailAddress (строка)</span><span class="sxs-lookup"><span data-stu-id="ced44-113">EmailAddress (string)</span></span>](emailaddress-string.md) <br/> |<span data-ttu-id="ced44-114">Задает один адрес электронной почты.</span><span class="sxs-lookup"><span data-stu-id="ced44-114">Specifies a single email address.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="ced44-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="ced44-115">Parent elements</span></span>

|<span data-ttu-id="ced44-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="ced44-116">**Element**</span></span>|<span data-ttu-id="ced44-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="ced44-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ced44-118">EmailAddresses (Аррайофемаиладдрессентитиестипе)</span><span class="sxs-lookup"><span data-stu-id="ced44-118">EmailAddresses (ArrayOfEmailAddressEntitiesType)</span></span>](emailaddresses-arrayofemailaddressentitiestype.md) <br/> |<span data-ttu-id="ced44-119">Указывает массив сущностей адресов электронной почты.</span><span class="sxs-lookup"><span data-stu-id="ced44-119">Specifies an array of email address entities.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="ced44-120">Примечания</span><span class="sxs-lookup"><span data-stu-id="ced44-120">Remarks</span></span>

<span data-ttu-id="ced44-121">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="ced44-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="ced44-122">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="ced44-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ced44-123">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="ced44-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ced44-124">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="ced44-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="ced44-125">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="ced44-125">Schema Name</span></span>  <br/> |<span data-ttu-id="ced44-126">Схема типа</span><span class="sxs-lookup"><span data-stu-id="ced44-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="ced44-127">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="ced44-127">Validation File</span></span>  <br/> |<span data-ttu-id="ced44-128">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="ced44-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="ced44-129">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="ced44-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="ced44-130">См. также</span><span class="sxs-lookup"><span data-stu-id="ced44-130">See also</span></span>



- [<span data-ttu-id="ced44-131">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="ced44-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

