---
title: Emails1
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: cc02bd86-c618-446a-92f0-749423cbc4ee
description: Элемент Emails1 указывает массив значений EmailAddressAttributedValue и идентификаторы их атрибуты источника для связанного пользователя.
ms.openlocfilehash: f1a1223244c91731b1a5a1beb9daed6d680d3bc4
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762296"
---
# <a name="emails1"></a><span data-ttu-id="99e06-103">Emails1</span><span class="sxs-lookup"><span data-stu-id="99e06-103">Emails1</span></span>

<span data-ttu-id="99e06-104">Элемент **Emails1** указывает массив значений **EmailAddressAttributedValue** и идентификаторы их атрибуты источника для связанного пользователя.</span><span class="sxs-lookup"><span data-stu-id="99e06-104">The **Emails1** element specifies an array of **EmailAddressAttributedValue** values and the identifiers of their source attributions for the associated persona.</span></span> 
  
```XML
<Emails1>
    <EmailAddressAttributedValue></EmailAddressAttributedValue>
</Emails1>
```

 <span data-ttu-id="99e06-105">**ArrayOfEmailAddressAttributedValuesType**</span><span class="sxs-lookup"><span data-stu-id="99e06-105">**ArrayOfEmailAddressAttributedValuesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="99e06-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="99e06-106">Attributes and elements</span></span>

<span data-ttu-id="99e06-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="99e06-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="99e06-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="99e06-108">Attributes</span></span>

<span data-ttu-id="99e06-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="99e06-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="99e06-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="99e06-110">Child elements</span></span>

|<span data-ttu-id="99e06-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="99e06-111">**Element**</span></span>|<span data-ttu-id="99e06-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="99e06-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="99e06-113">EmailAddressAttributedValue</span><span class="sxs-lookup"><span data-stu-id="99e06-113">EmailAddressAttributedValue</span></span>](emailaddressattributedvalue.md) <br/> |<span data-ttu-id="99e06-114">Указывает экземпляр массив адресов электронной почты и их связанные атрибуты.</span><span class="sxs-lookup"><span data-stu-id="99e06-114">Specifies an instance of an array of email addresses and their associated attributions.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="99e06-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="99e06-115">Parent elements</span></span>

|<span data-ttu-id="99e06-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="99e06-116">**Element**</span></span>|<span data-ttu-id="99e06-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="99e06-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="99e06-118">Пользователь</span><span class="sxs-lookup"><span data-stu-id="99e06-118">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="99e06-119">Задает набор пользователя данные, возвращаемые запросом **GetPersona** .</span><span class="sxs-lookup"><span data-stu-id="99e06-119">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="99e06-120">Замечания</span><span class="sxs-lookup"><span data-stu-id="99e06-120">Remarks</span></span>

<span data-ttu-id="99e06-121">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="99e06-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="99e06-122">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="99e06-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="99e06-123">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="99e06-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="99e06-124">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="99e06-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="99e06-125">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="99e06-125">Schema Name</span></span>  <br/> |<span data-ttu-id="99e06-126">Схема типа</span><span class="sxs-lookup"><span data-stu-id="99e06-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="99e06-127">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="99e06-127">Validation File</span></span>  <br/> |<span data-ttu-id="99e06-128">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="99e06-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="99e06-129">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="99e06-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="99e06-130">См. также</span><span class="sxs-lookup"><span data-stu-id="99e06-130">See also</span></span>



- [<span data-ttu-id="99e06-131">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="99e06-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

