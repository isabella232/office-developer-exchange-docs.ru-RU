---
title: Guid
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 49dcf69f-bf8d-4be6-a24c-03bbd13f4fe5
description: Элемент Guid указывает идентификатор почтового ящика.
ms.openlocfilehash: 35307a706523fc5c2916767c7508dec07deb8d09
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833799"
---
# <a name="guid"></a><span data-ttu-id="52cf8-103">Guid</span><span class="sxs-lookup"><span data-stu-id="52cf8-103">Guid</span></span>

<span data-ttu-id="52cf8-104">Элемент **Guid** указывает идентификатор почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="52cf8-104">The **Guid** element specifies the globally unique identifier of the mailbox.</span></span> 
  
```XML
<Guid></Guid>
```

 <span data-ttu-id="52cf8-105">**GuidType**</span><span class="sxs-lookup"><span data-stu-id="52cf8-105">**GuidType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="52cf8-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="52cf8-106">Attributes and elements</span></span>

<span data-ttu-id="52cf8-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="52cf8-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="52cf8-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="52cf8-108">Attributes</span></span>

<span data-ttu-id="52cf8-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="52cf8-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="52cf8-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="52cf8-110">Child elements</span></span>

<span data-ttu-id="52cf8-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="52cf8-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="52cf8-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="52cf8-112">Parent elements</span></span>

|<span data-ttu-id="52cf8-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="52cf8-113">**Element**</span></span>|<span data-ttu-id="52cf8-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="52cf8-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="52cf8-115">SearchableMailbox</span><span class="sxs-lookup"><span data-stu-id="52cf8-115">SearchableMailbox</span></span>](searchablemailbox.md) <br/> |<span data-ttu-id="52cf8-116">Указывает почтового ящика возвращаются из **GetSearchableMailboxes** запроса.</span><span class="sxs-lookup"><span data-stu-id="52cf8-116">Specifies a mailbox returned from a **GetSearchableMailboxes** request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="52cf8-117">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="52cf8-117">Text value</span></span>

<span data-ttu-id="52cf8-118">Текстовое значение элемента **Guid** — это идентификатор GUID, который уникальным образом определяет почтовый ящик.</span><span class="sxs-lookup"><span data-stu-id="52cf8-118">The text value of the **Guid** element is a GUID value that uniquely identifies a mailbox.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="52cf8-119">Замечания</span><span class="sxs-lookup"><span data-stu-id="52cf8-119">Remarks</span></span>

<span data-ttu-id="52cf8-120">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="52cf8-120">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="52cf8-121">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="52cf8-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="52cf8-122">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="52cf8-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="52cf8-123">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="52cf8-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="52cf8-124">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="52cf8-124">Schema Name</span></span>  <br/> |<span data-ttu-id="52cf8-125">Схема типа</span><span class="sxs-lookup"><span data-stu-id="52cf8-125">Type schema</span></span>  <br/> |
|<span data-ttu-id="52cf8-126">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="52cf8-126">Validation File</span></span>  <br/> |<span data-ttu-id="52cf8-127">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="52cf8-127">types.xsd</span></span>  <br/> |
|<span data-ttu-id="52cf8-128">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="52cf8-128">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="52cf8-129">См. также</span><span class="sxs-lookup"><span data-stu-id="52cf8-129">See also</span></span>



- [<span data-ttu-id="52cf8-130">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="52cf8-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

