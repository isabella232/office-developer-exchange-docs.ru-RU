---
title: конверсатионноде
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: b7f7acd3-ed65-441e-9976-8b4ed5f12c0b
description: Элемент Конверсатионноде указывает узел в беседе.
ms.openlocfilehash: 074209c1b5669db8dd1ea4ba7f9dea064628afbd
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462705"
---
# <a name="conversationnode"></a><span data-ttu-id="d880b-103">конверсатионноде</span><span class="sxs-lookup"><span data-stu-id="d880b-103">ConversationNode</span></span>

<span data-ttu-id="d880b-104">Элемент **конверсатионноде** указывает узел в беседе.</span><span class="sxs-lookup"><span data-stu-id="d880b-104">The **ConversationNode** element specifies a node in a conversation.</span></span> 
  
```XML
<ConversationNode>
    <InternetMessageId></InternetMessageId>
    <ParentInternetMessageId></ParentInternetMessageId>
    <Items></Items>
</ConversationNode>
```

 <span data-ttu-id="d880b-105">**конверсатионнодетипе**</span><span class="sxs-lookup"><span data-stu-id="d880b-105">**ConversationNodeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d880b-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="d880b-106">Attributes and elements</span></span>

<span data-ttu-id="d880b-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="d880b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d880b-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="d880b-108">Attributes</span></span>

<span data-ttu-id="d880b-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="d880b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d880b-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="d880b-110">Child elements</span></span>

|<span data-ttu-id="d880b-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="d880b-111">**Element**</span></span>|<span data-ttu-id="d880b-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d880b-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d880b-113">InternetMessageId</span><span class="sxs-lookup"><span data-stu-id="d880b-113">InternetMessageId</span></span>](internetmessageid.md) <br/> |<span data-ttu-id="d880b-114">Представляет идентификатор сообщения Интернета для элемента.</span><span class="sxs-lookup"><span data-stu-id="d880b-114">Represents the Internet message identifier of an item.</span></span>  <br/> |
|[<span data-ttu-id="d880b-115">парентинтернетмессажеид</span><span class="sxs-lookup"><span data-stu-id="d880b-115">ParentInternetMessageId</span></span>](parentinternetmessageid.md) <br/> |<span data-ttu-id="d880b-116">Задает идентификатор родительского Интернет – сообщения.</span><span class="sxs-lookup"><span data-stu-id="d880b-116">Specifies the identifier of the parent Internet message.</span></span>  <br/> |
|[<span data-ttu-id="d880b-117">Итемидс (Нонемптяррайофитемидстипе)</span><span class="sxs-lookup"><span data-stu-id="d880b-117">ItemIds (NonEmptyArrayOfItemIdsType)</span></span>](itemids-nonemptyarrayofitemidstype.md) <br/> |<span data-ttu-id="d880b-118">Задает все элементы в узле беседы.</span><span class="sxs-lookup"><span data-stu-id="d880b-118">Specifies all the items in the conversation node.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d880b-119">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="d880b-119">Parent elements</span></span>

|<span data-ttu-id="d880b-120">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="d880b-120">**Element**</span></span>|<span data-ttu-id="d880b-121">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d880b-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d880b-122">конверсатионнодес</span><span class="sxs-lookup"><span data-stu-id="d880b-122">ConversationNodes</span></span>](conversationnodes.md) <br/> |<span data-ttu-id="d880b-123">Задает коллекцию узлов беседы.</span><span class="sxs-lookup"><span data-stu-id="d880b-123">Specifies a collection of conversation nodes.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="d880b-124">Примечания</span><span class="sxs-lookup"><span data-stu-id="d880b-124">Remarks</span></span>

<span data-ttu-id="d880b-125">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="d880b-125">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="d880b-126">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="d880b-126">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d880b-127">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="d880b-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d880b-128">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="d880b-128">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d880b-129">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="d880b-129">Schema Name</span></span>  <br/> |<span data-ttu-id="d880b-130">Схема типа</span><span class="sxs-lookup"><span data-stu-id="d880b-130">Type schema</span></span>  <br/> |
|<span data-ttu-id="d880b-131">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="d880b-131">Validation File</span></span>  <br/> |<span data-ttu-id="d880b-132">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="d880b-132">types.xsd</span></span>  <br/> |
|<span data-ttu-id="d880b-133">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="d880b-133">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="d880b-134">См. также</span><span class="sxs-lookup"><span data-stu-id="d880b-134">See also</span></span>



- [<span data-ttu-id="d880b-135">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="d880b-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

