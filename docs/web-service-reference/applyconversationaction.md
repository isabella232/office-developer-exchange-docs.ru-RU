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
description: Элемент ApplyConversationAction определяет запрос на применение действий к элементам в беседе.
ms.openlocfilehash: 659b3392778bb1a318c3942a0c8e314f12110c12
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461690"
---
# <a name="applyconversationaction"></a><span data-ttu-id="4b898-103">ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="4b898-103">ApplyConversationAction</span></span>

<span data-ttu-id="4b898-104">Элемент **ApplyConversationAction** определяет запрос на применение действий к элементам в беседе.</span><span class="sxs-lookup"><span data-stu-id="4b898-104">The **ApplyConversationAction** element defines a request to apply actions to items in a conversation.</span></span> 
  
[<span data-ttu-id="4b898-105">ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="4b898-105">ApplyConversationAction</span></span>](applyconversationaction.md)
  
```XML
<ApplyConversationAction>
   <ConversationActions/>
</ApplyConversationAction>
```

 <span data-ttu-id="4b898-106">**аппликонверсатионактионтипе**</span><span class="sxs-lookup"><span data-stu-id="4b898-106">**ApplyConversationActionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4b898-107">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="4b898-107">Attributes and elements</span></span>

<span data-ttu-id="4b898-108">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="4b898-108">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4b898-109">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="4b898-109">Attributes</span></span>

<span data-ttu-id="4b898-110">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="4b898-110">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4b898-111">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="4b898-111">Child elements</span></span>

|<span data-ttu-id="4b898-112">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="4b898-112">**Element**</span></span>|<span data-ttu-id="4b898-113">**Описание**</span><span class="sxs-lookup"><span data-stu-id="4b898-113">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4b898-114">конверсатионактионс</span><span class="sxs-lookup"><span data-stu-id="4b898-114">ConversationActions</span></span>](conversationactions.md) <br/> |<span data-ttu-id="4b898-115">Содержит коллекцию бесед и действий, которые необходимо применить к ним.</span><span class="sxs-lookup"><span data-stu-id="4b898-115">Contains a collection of conversations and the actions to apply to them.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="4b898-116">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="4b898-116">Parent elements</span></span>

<span data-ttu-id="4b898-117">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="4b898-117">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="4b898-118">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="4b898-118">Text value</span></span>

<span data-ttu-id="4b898-119">Нет.</span><span class="sxs-lookup"><span data-stu-id="4b898-119">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="4b898-120">Примечания</span><span class="sxs-lookup"><span data-stu-id="4b898-120">Remarks</span></span>

<span data-ttu-id="4b898-121">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.Этот элемент появился в Exchange Server 2010 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="4b898-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4b898-122">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="4b898-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4b898-123">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="4b898-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="4b898-124">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="4b898-124">Schema Name</span></span>  <br/> |<span data-ttu-id="4b898-125">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="4b898-125">Messages schema</span></span>  <br/> |
|<span data-ttu-id="4b898-126">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="4b898-126">Validation File</span></span>  <br/> |<span data-ttu-id="4b898-127">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="4b898-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="4b898-128">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="4b898-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="4b898-129">False</span><span class="sxs-lookup"><span data-stu-id="4b898-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4b898-130">См. также</span><span class="sxs-lookup"><span data-stu-id="4b898-130">See also</span></span>

- [<span data-ttu-id="4b898-131">Операция ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="4b898-131">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)
- [<span data-ttu-id="4b898-132">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="4b898-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

