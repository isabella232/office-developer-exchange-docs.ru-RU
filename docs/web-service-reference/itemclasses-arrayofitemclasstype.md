---
title: ItemClasses (ArrayOfItemClassType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 971784d1-6860-4833-bb26-0e930fa11c21
description: Элемент ItemClasses содержит список классов элементов, представляющий все классы элементов из элементов беседы в текущей папке.
ms.openlocfilehash: 62ea5b624025b3f012249afd1763e2b393ef5caa
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19834150"
---
# <a name="itemclasses-arrayofitemclasstype"></a><span data-ttu-id="ee858-103">ItemClasses (ArrayOfItemClassType)</span><span class="sxs-lookup"><span data-stu-id="ee858-103">ItemClasses (ArrayOfItemClassType)</span></span>

<span data-ttu-id="ee858-104">Элемент **ItemClasses** содержит список классов элементов, представляющий все классы элементов из элементов беседы в текущей папке.</span><span class="sxs-lookup"><span data-stu-id="ee858-104">The **ItemClasses** element contains a list of item classes that represents all the item classes of the conversation items in the current folder.</span></span> 
  
[<span data-ttu-id="ee858-105">FindConversationResponse</span><span class="sxs-lookup"><span data-stu-id="ee858-105">FindConversationResponse</span></span>](findconversationresponse.md)
  
[<span data-ttu-id="ee858-106">Conversations</span><span class="sxs-lookup"><span data-stu-id="ee858-106">Conversations</span></span>](conversations-ex15websvcsotherref.md)
  
[<span data-ttu-id="ee858-107">Беседы (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="ee858-107">Conversation (ConversationType)</span></span>](conversation-conversationtype.md)
  
[<span data-ttu-id="ee858-108">ItemClasses (ArrayOfItemClassType)</span><span class="sxs-lookup"><span data-stu-id="ee858-108">ItemClasses (ArrayOfItemClassType)</span></span>](itemclasses-arrayofitemclasstype.md)
  
```XML
<ItemClasses>
    <String/>
</ItemClasses>
```

 <span data-ttu-id="ee858-109">**ArrayOfItemClassType**</span><span class="sxs-lookup"><span data-stu-id="ee858-109">**ArrayOfItemClassType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ee858-110">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="ee858-110">Attributes and elements</span></span>

<span data-ttu-id="ee858-111">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="ee858-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ee858-112">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="ee858-112">Attributes</span></span>

<span data-ttu-id="ee858-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="ee858-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ee858-114">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="ee858-114">Child elements</span></span>

|<span data-ttu-id="ee858-115">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="ee858-115">**Element**</span></span>|<span data-ttu-id="ee858-116">**Описание**</span><span class="sxs-lookup"><span data-stu-id="ee858-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ee858-117">ItemClass</span><span class="sxs-lookup"><span data-stu-id="ee858-117">ItemClass</span></span>](itemclass.md) <br/> |<span data-ttu-id="ee858-118">Представляет класс сообщения элемента.</span><span class="sxs-lookup"><span data-stu-id="ee858-118">Represents the message class of an item.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="ee858-119">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="ee858-119">Parent elements</span></span>

|<span data-ttu-id="ee858-120">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="ee858-120">**Element**</span></span>|<span data-ttu-id="ee858-121">**Описание**</span><span class="sxs-lookup"><span data-stu-id="ee858-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ee858-122">Беседы (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="ee858-122">Conversation (ConversationType)</span></span>](conversation-conversationtype.md) <br/> |<span data-ttu-id="ee858-123">Представляет одну беседу.</span><span class="sxs-lookup"><span data-stu-id="ee858-123">Represents a single conversation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="ee858-124">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="ee858-124">Text value</span></span>

<span data-ttu-id="ee858-125">Нет.</span><span class="sxs-lookup"><span data-stu-id="ee858-125">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="ee858-126">Замечания</span><span class="sxs-lookup"><span data-stu-id="ee858-126">Remarks</span></span>

<span data-ttu-id="ee858-127">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.Этот элемент появился в Exchange Server 2010 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="ee858-127">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ee858-128">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="ee858-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ee858-129">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="ee858-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="ee858-130">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="ee858-130">Schema name</span></span>  <br/> |<span data-ttu-id="ee858-131">Схема Types</span><span class="sxs-lookup"><span data-stu-id="ee858-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="ee858-132">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="ee858-132">Validation file</span></span>  <br/> |<span data-ttu-id="ee858-133">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="ee858-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="ee858-134">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="ee858-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="ee858-135">False</span><span class="sxs-lookup"><span data-stu-id="ee858-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ee858-136">См. также</span><span class="sxs-lookup"><span data-stu-id="ee858-136">See also</span></span>



[<span data-ttu-id="ee858-137">FindConversation Operation</span><span class="sxs-lookup"><span data-stu-id="ee858-137">FindConversation operation</span></span>](findconversation-operation.md)
  
[<span data-ttu-id="ee858-138">Операция ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="ee858-138">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)


[<span data-ttu-id="ee858-139">Conversations in EWS</span><span class="sxs-lookup"><span data-stu-id="ee858-139">Conversations in EWS</span></span>](http://msdn.microsoft.com/library/91e64629-db6c-4c94-9dcb-d386232e8467%28Office.15%29.aspx)

