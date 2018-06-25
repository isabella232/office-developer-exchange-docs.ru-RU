---
title: ApplyConversationAction
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ApplyConversationAction
api_type:
- schema
ms.assetid: e0ee8f30-529b-4d87-8bc0-b6616e75fb6b
description: Элемент ApplyConversationAction определяет запрос для выполнения определенных действий к элементам в беседе.
ms.openlocfilehash: 1b672c6e6d2f60e50215417be7100e9cd77e2a58
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761471"
---
# <a name="applyconversationaction"></a><span data-ttu-id="cf78e-103">ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="cf78e-103">ApplyConversationAction</span></span>

<span data-ttu-id="cf78e-104">Элемент **ApplyConversationAction** определяет запрос для выполнения определенных действий к элементам в беседе.</span><span class="sxs-lookup"><span data-stu-id="cf78e-104">The **ApplyConversationAction** element defines a request to apply actions to items in a conversation.</span></span> 
  
[<span data-ttu-id="cf78e-105">ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="cf78e-105">ApplyConversationAction</span></span>](applyconversationaction.md)
  
```XML
<ApplyConversationAction>
   <ConversationActions/>
</ApplyConversationAction>
```

 <span data-ttu-id="cf78e-106">**ApplyConversationActionType**</span><span class="sxs-lookup"><span data-stu-id="cf78e-106">**ApplyConversationActionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="cf78e-107">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="cf78e-107">Attributes and elements</span></span>

<span data-ttu-id="cf78e-108">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="cf78e-108">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="cf78e-109">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="cf78e-109">Attributes</span></span>

<span data-ttu-id="cf78e-110">Нет.</span><span class="sxs-lookup"><span data-stu-id="cf78e-110">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="cf78e-111">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="cf78e-111">Child elements</span></span>

|<span data-ttu-id="cf78e-112">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="cf78e-112">**Element**</span></span>|<span data-ttu-id="cf78e-113">**Описание**</span><span class="sxs-lookup"><span data-stu-id="cf78e-113">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cf78e-114">ConversationActions</span><span class="sxs-lookup"><span data-stu-id="cf78e-114">ConversationActions</span></span>](conversationactions.md) <br/> |<span data-ttu-id="cf78e-115">Содержит коллекцию бесед и действий для применения к ним.</span><span class="sxs-lookup"><span data-stu-id="cf78e-115">Contains a collection of conversations and the actions to apply to them.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="cf78e-116">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="cf78e-116">Parent elements</span></span>

<span data-ttu-id="cf78e-117">Нет.</span><span class="sxs-lookup"><span data-stu-id="cf78e-117">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="cf78e-118">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="cf78e-118">Text value</span></span>

<span data-ttu-id="cf78e-119">Нет.</span><span class="sxs-lookup"><span data-stu-id="cf78e-119">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="cf78e-120">Замечания</span><span class="sxs-lookup"><span data-stu-id="cf78e-120">Remarks</span></span>

<span data-ttu-id="cf78e-121">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.Этот элемент появился в Exchange Server 2010 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="cf78e-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="cf78e-122">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="cf78e-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="cf78e-123">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="cf78e-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="cf78e-124">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="cf78e-124">Schema Name</span></span>  <br/> |<span data-ttu-id="cf78e-125">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="cf78e-125">Messages schema</span></span>  <br/> |
|<span data-ttu-id="cf78e-126">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="cf78e-126">Validation File</span></span>  <br/> |<span data-ttu-id="cf78e-127">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="cf78e-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="cf78e-128">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="cf78e-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="cf78e-129">False</span><span class="sxs-lookup"><span data-stu-id="cf78e-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="cf78e-130">См. также</span><span class="sxs-lookup"><span data-stu-id="cf78e-130">See also</span></span>

- [<span data-ttu-id="cf78e-131">Операция ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="cf78e-131">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)
- [<span data-ttu-id="cf78e-132">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="cf78e-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

