---
title: Emails2
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 6ad95936-f61b-431a-9d86-df160b5d4b2d
description: Элемент Emails2 содержит массив значений EmailAddressAttributedValue и идентификаторы их атрибуты источника для связанного пользователя.
ms.openlocfilehash: 1767d6bfaee335717e33e0345c605025a073335c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762295"
---
# <a name="emails2"></a><span data-ttu-id="2230c-103">Emails2</span><span class="sxs-lookup"><span data-stu-id="2230c-103">Emails2</span></span>

<span data-ttu-id="2230c-104">Элемент **Emails2** содержит массив значений **EmailAddressAttributedValue** и идентификаторы их атрибуты источника для связанного пользователя.</span><span class="sxs-lookup"><span data-stu-id="2230c-104">The **Emails2** element contains an array of **EmailAddressAttributedValue** values and the identifiers of their source attributions for the associated persona.</span></span> 
  
```XML
<Emails2>
    <EmailAddressAttributedValue></EmailAddressAttributedValue>
</Emails2>
```

 <span data-ttu-id="2230c-105">**ArrayOfEmailAddressAttributedValuesType**</span><span class="sxs-lookup"><span data-stu-id="2230c-105">**ArrayOfEmailAddressAttributedValuesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2230c-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="2230c-106">Attributes and elements</span></span>

<span data-ttu-id="2230c-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="2230c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2230c-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="2230c-108">Attributes</span></span>

<span data-ttu-id="2230c-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="2230c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2230c-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="2230c-110">Child elements</span></span>

|<span data-ttu-id="2230c-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="2230c-111">**Element**</span></span>|<span data-ttu-id="2230c-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="2230c-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2230c-113">EmailAddressAttributedValue</span><span class="sxs-lookup"><span data-stu-id="2230c-113">EmailAddressAttributedValue</span></span>](emailaddressattributedvalue.md) <br/> |<span data-ttu-id="2230c-114">Указывает экземпляр массив адресов электронной почты и их связанные атрибуты.</span><span class="sxs-lookup"><span data-stu-id="2230c-114">Specifies an instance of an array of email addresses and their associated attributions.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="2230c-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="2230c-115">Parent elements</span></span>

|<span data-ttu-id="2230c-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="2230c-116">**Element**</span></span>|<span data-ttu-id="2230c-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="2230c-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2230c-118">Пользователь</span><span class="sxs-lookup"><span data-stu-id="2230c-118">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="2230c-119">Задает набор пользователя данные, возвращаемые запросом **GetPersona** .</span><span class="sxs-lookup"><span data-stu-id="2230c-119">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="2230c-120">Замечания</span><span class="sxs-lookup"><span data-stu-id="2230c-120">Remarks</span></span>

<span data-ttu-id="2230c-121">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="2230c-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="2230c-122">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="2230c-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2230c-123">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="2230c-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2230c-124">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="2230c-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="2230c-125">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="2230c-125">Schema Name</span></span>  <br/> |<span data-ttu-id="2230c-126">Схема типа</span><span class="sxs-lookup"><span data-stu-id="2230c-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="2230c-127">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="2230c-127">Validation File</span></span>  <br/> |<span data-ttu-id="2230c-128">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="2230c-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="2230c-129">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="2230c-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="2230c-130">См. также</span><span class="sxs-lookup"><span data-stu-id="2230c-130">See also</span></span>



- [<span data-ttu-id="2230c-131">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="2230c-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

