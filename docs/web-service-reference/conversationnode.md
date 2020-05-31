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
ms.openlocfilehash: c8289e5f30bfd25eb12d54e3be0c561786308dc6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761821"
---
# <a name="conversationnode"></a><span data-ttu-id="f5461-103">конверсатионноде</span><span class="sxs-lookup"><span data-stu-id="f5461-103">ConversationNode</span></span>

<span data-ttu-id="f5461-104">Элемент **конверсатионноде** указывает узел в беседе.</span><span class="sxs-lookup"><span data-stu-id="f5461-104">The **ConversationNode** element specifies a node in a conversation.</span></span> 
  
```XML
<ConversationNode>
    <InternetMessageId></InternetMessageId>
    <ParentInternetMessageId></ParentInternetMessageId>
    <Items></Items>
</ConversationNode>
```

 <span data-ttu-id="f5461-105">**конверсатионнодетипе**</span><span class="sxs-lookup"><span data-stu-id="f5461-105">**ConversationNodeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f5461-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="f5461-106">Attributes and elements</span></span>

<span data-ttu-id="f5461-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="f5461-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f5461-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="f5461-108">Attributes</span></span>

<span data-ttu-id="f5461-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="f5461-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f5461-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="f5461-110">Child elements</span></span>

|<span data-ttu-id="f5461-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="f5461-111">**Element**</span></span>|<span data-ttu-id="f5461-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="f5461-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f5461-113">InternetMessageId</span><span class="sxs-lookup"><span data-stu-id="f5461-113">InternetMessageId</span></span>](internetmessageid.md) <br/> |<span data-ttu-id="f5461-114">Представляет идентификатор сообщения Интернета для элемента.</span><span class="sxs-lookup"><span data-stu-id="f5461-114">Represents the Internet message identifier of an item.</span></span>  <br/> |
|[<span data-ttu-id="f5461-115">парентинтернетмессажеид</span><span class="sxs-lookup"><span data-stu-id="f5461-115">ParentInternetMessageId</span></span>](parentinternetmessageid.md) <br/> |<span data-ttu-id="f5461-116">Задает идентификатор родительского Интернет – сообщения.</span><span class="sxs-lookup"><span data-stu-id="f5461-116">Specifies the identifier of the parent Internet message.</span></span>  <br/> |
|[<span data-ttu-id="f5461-117">Итемидс (Нонемптяррайофитемидстипе)</span><span class="sxs-lookup"><span data-stu-id="f5461-117">ItemIds (NonEmptyArrayOfItemIdsType)</span></span>](itemids-nonemptyarrayofitemidstype.md) <br/> |<span data-ttu-id="f5461-118">Задает все элементы в узле беседы.</span><span class="sxs-lookup"><span data-stu-id="f5461-118">Specifies all the items in the conversation node.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f5461-119">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="f5461-119">Parent elements</span></span>

|<span data-ttu-id="f5461-120">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="f5461-120">**Element**</span></span>|<span data-ttu-id="f5461-121">**Описание**</span><span class="sxs-lookup"><span data-stu-id="f5461-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f5461-122">конверсатионнодес</span><span class="sxs-lookup"><span data-stu-id="f5461-122">ConversationNodes</span></span>](conversationnodes.md) <br/> |<span data-ttu-id="f5461-123">Задает коллекцию узлов беседы.</span><span class="sxs-lookup"><span data-stu-id="f5461-123">Specifies a collection of conversation nodes.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="f5461-124">Примечания</span><span class="sxs-lookup"><span data-stu-id="f5461-124">Remarks</span></span>

<span data-ttu-id="f5461-125">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="f5461-125">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="f5461-126">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="f5461-126">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f5461-127">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="f5461-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f5461-128">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="f5461-128">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f5461-129">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="f5461-129">Schema Name</span></span>  <br/> |<span data-ttu-id="f5461-130">Схема типа</span><span class="sxs-lookup"><span data-stu-id="f5461-130">Type schema</span></span>  <br/> |
|<span data-ttu-id="f5461-131">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="f5461-131">Validation File</span></span>  <br/> |<span data-ttu-id="f5461-132">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="f5461-132">types.xsd</span></span>  <br/> |
|<span data-ttu-id="f5461-133">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="f5461-133">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="f5461-134">См. также</span><span class="sxs-lookup"><span data-stu-id="f5461-134">See also</span></span>



- [<span data-ttu-id="f5461-135">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="f5461-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

