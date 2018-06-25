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
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762295"
---
# <a name="emails2"></a><span data-ttu-id="25b25-103">Emails2</span><span class="sxs-lookup"><span data-stu-id="25b25-103">Emails2</span></span>

<span data-ttu-id="25b25-104">Элемент **Emails2** содержит массив значений **EmailAddressAttributedValue** и идентификаторы их атрибуты источника для связанного пользователя.</span><span class="sxs-lookup"><span data-stu-id="25b25-104">The **Emails2** element contains an array of **EmailAddressAttributedValue** values and the identifiers of their source attributions for the associated persona.</span></span> 
  
```XML
<Emails2>
    <EmailAddressAttributedValue></EmailAddressAttributedValue>
</Emails2>
```

 <span data-ttu-id="25b25-105">**ArrayOfEmailAddressAttributedValuesType**</span><span class="sxs-lookup"><span data-stu-id="25b25-105">**ArrayOfEmailAddressAttributedValuesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="25b25-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="25b25-106">Attributes and elements</span></span>

<span data-ttu-id="25b25-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="25b25-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="25b25-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="25b25-108">Attributes</span></span>

<span data-ttu-id="25b25-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="25b25-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="25b25-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="25b25-110">Child elements</span></span>

|<span data-ttu-id="25b25-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="25b25-111">**Element**</span></span>|<span data-ttu-id="25b25-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="25b25-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="25b25-113">EmailAddressAttributedValue</span><span class="sxs-lookup"><span data-stu-id="25b25-113">EmailAddressAttributedValue</span></span>](emailaddressattributedvalue.md) <br/> |<span data-ttu-id="25b25-114">Указывает экземпляр массив адресов электронной почты и их связанные атрибуты.</span><span class="sxs-lookup"><span data-stu-id="25b25-114">Specifies an instance of an array of email addresses and their associated attributions.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="25b25-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="25b25-115">Parent elements</span></span>

|<span data-ttu-id="25b25-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="25b25-116">**Element**</span></span>|<span data-ttu-id="25b25-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="25b25-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="25b25-118">Пользователь</span><span class="sxs-lookup"><span data-stu-id="25b25-118">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="25b25-119">Задает набор пользователя данные, возвращаемые запросом **GetPersona** .</span><span class="sxs-lookup"><span data-stu-id="25b25-119">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="25b25-120">Замечания</span><span class="sxs-lookup"><span data-stu-id="25b25-120">Remarks</span></span>

<span data-ttu-id="25b25-121">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="25b25-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="25b25-122">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="25b25-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="25b25-123">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="25b25-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="25b25-124">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="25b25-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="25b25-125">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="25b25-125">Schema Name</span></span>  <br/> |<span data-ttu-id="25b25-126">Схема типа</span><span class="sxs-lookup"><span data-stu-id="25b25-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="25b25-127">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="25b25-127">Validation File</span></span>  <br/> |<span data-ttu-id="25b25-128">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="25b25-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="25b25-129">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="25b25-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="25b25-130">См. также</span><span class="sxs-lookup"><span data-stu-id="25b25-130">See also</span></span>



- [<span data-ttu-id="25b25-131">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="25b25-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

