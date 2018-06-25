---
title: BusinessAddresses
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 828f8f62-7abf-44d4-8d58-f706d595a812
description: Элемент BusinessAddresses указывает массив business адресов и идентификаторы их атрибуты источника для связанного пользователя.
ms.openlocfilehash: bc7ad948572c24f913ae02abb9e8fc5a7b1e0b0d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761597"
---
# <a name="businessaddresses"></a><span data-ttu-id="b93a3-103">BusinessAddresses</span><span class="sxs-lookup"><span data-stu-id="b93a3-103">BusinessAddresses</span></span>

<span data-ttu-id="b93a3-104">Элемент **BusinessAddresses** указывает массив business адресов и идентификаторы их атрибуты источника для связанного пользователя.</span><span class="sxs-lookup"><span data-stu-id="b93a3-104">The **BusinessAddresses** element specifies an array of business addresses and the identifiers of their source attributions for the associated persona.</span></span> 
  
```XML
<BusinessAddresses>
    <PostalAddressAttributedValue></PostalAddressAttributedValue>
</BusinessAddresses
```

 <span data-ttu-id="b93a3-105">**ArrayOfPostalAddressAttributedValuesType**</span><span class="sxs-lookup"><span data-stu-id="b93a3-105">**ArrayOfPostalAddressAttributedValuesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b93a3-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="b93a3-106">Attributes and elements</span></span>

<span data-ttu-id="b93a3-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="b93a3-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b93a3-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="b93a3-108">Attributes</span></span>

<span data-ttu-id="b93a3-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="b93a3-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b93a3-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="b93a3-110">Child elements</span></span>

|<span data-ttu-id="b93a3-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="b93a3-111">**Element**</span></span>|<span data-ttu-id="b93a3-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="b93a3-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b93a3-113">PostalAddressAttributedValue</span><span class="sxs-lookup"><span data-stu-id="b93a3-113">PostalAddressAttributedValue</span></span>](postaladdressattributedvalue.md) <br/> |<span data-ttu-id="b93a3-114">Указывает экземпляр массив почтовых адресов и их связанные атрибуты.</span><span class="sxs-lookup"><span data-stu-id="b93a3-114">Specifies an instance of an array of postal addresses and their associated attributions.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="b93a3-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="b93a3-115">Parent elements</span></span>

|<span data-ttu-id="b93a3-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="b93a3-116">**Element**</span></span>|<span data-ttu-id="b93a3-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="b93a3-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b93a3-118">Пользователь</span><span class="sxs-lookup"><span data-stu-id="b93a3-118">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="b93a3-119">Задает набор пользователя данные, возвращаемые запросом **GetPersona** .</span><span class="sxs-lookup"><span data-stu-id="b93a3-119">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="b93a3-120">Замечания</span><span class="sxs-lookup"><span data-stu-id="b93a3-120">Remarks</span></span>

<span data-ttu-id="b93a3-121">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="b93a3-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="b93a3-122">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="b93a3-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b93a3-123">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="b93a3-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b93a3-124">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="b93a3-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="b93a3-125">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="b93a3-125">Schema Name</span></span>  <br/> |<span data-ttu-id="b93a3-126">Схема типа</span><span class="sxs-lookup"><span data-stu-id="b93a3-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="b93a3-127">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="b93a3-127">Validation File</span></span>  <br/> |<span data-ttu-id="b93a3-128">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="b93a3-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="b93a3-129">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="b93a3-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="b93a3-130">См. также</span><span class="sxs-lookup"><span data-stu-id="b93a3-130">See also</span></span>



- [<span data-ttu-id="b93a3-131">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="b93a3-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

