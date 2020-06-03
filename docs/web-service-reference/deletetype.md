---
title: делететипе
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DeleteType
api_type:
- schema
ms.assetid: 6e3136cd-9cb4-493a-aa85-9678f719002d
description: Элемент Делететипе указывает, как удаляются элементы в беседе.
ms.openlocfilehash: 199f7afc29fe866865509d2fb90d24944113d5c0
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44442635"
---
# <a name="deletetype"></a><span data-ttu-id="f83c3-103">делететипе</span><span class="sxs-lookup"><span data-stu-id="f83c3-103">DeleteType</span></span>

<span data-ttu-id="f83c3-104">Элемент **делететипе** указывает, как удаляются элементы в беседе.</span><span class="sxs-lookup"><span data-stu-id="f83c3-104">The **DeleteType** element indicates how items in a conversation are deleted.</span></span> 
  
- [<span data-ttu-id="f83c3-105">ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="f83c3-105">ApplyConversationAction</span></span>](applyconversationaction.md)  
- [<span data-ttu-id="f83c3-106">конверсатионактионс</span><span class="sxs-lookup"><span data-stu-id="f83c3-106">ConversationActions</span></span>](conversationactions.md)  
- [<span data-ttu-id="f83c3-107">конверсатионактион</span><span class="sxs-lookup"><span data-stu-id="f83c3-107">ConversationAction</span></span>](conversationaction.md)  
- [<span data-ttu-id="f83c3-108">делететипе</span><span class="sxs-lookup"><span data-stu-id="f83c3-108">DeleteType</span></span>](deletetype.md)
  
```XML
<DeleteType> HardDelete | MoveToDeletedItems | SoftDelete </DeleteType>
```

 <span data-ttu-id="f83c3-109">**диспосалтипе**</span><span class="sxs-lookup"><span data-stu-id="f83c3-109">**DisposalType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f83c3-110">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="f83c3-110">Attributes and elements</span></span>

<span data-ttu-id="f83c3-111">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="f83c3-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f83c3-112">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="f83c3-112">Attributes</span></span>

<span data-ttu-id="f83c3-113">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="f83c3-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f83c3-114">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="f83c3-114">Child elements</span></span>

<span data-ttu-id="f83c3-115">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="f83c3-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="f83c3-116">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="f83c3-116">Parent elements</span></span>

|<span data-ttu-id="f83c3-117">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="f83c3-117">**Element**</span></span>|<span data-ttu-id="f83c3-118">**Описание**</span><span class="sxs-lookup"><span data-stu-id="f83c3-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f83c3-119">конверсатионактион</span><span class="sxs-lookup"><span data-stu-id="f83c3-119">ConversationAction</span></span>](conversationaction.md) <br/> |<span data-ttu-id="f83c3-120">Содержит одно действие, которое будет применено к одной беседе.</span><span class="sxs-lookup"><span data-stu-id="f83c3-120">Contains a single action to be applied to a single conversation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="f83c3-121">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="f83c3-121">Text value</span></span>

<span data-ttu-id="f83c3-122">Текстовое значение элемента **делететипе** указывает, как удаляются элементы в беседе.</span><span class="sxs-lookup"><span data-stu-id="f83c3-122">The text value of the **DeleteType** element indicates how items in a conversation are deleted.</span></span> <span data-ttu-id="f83c3-123">Ниже приведены возможные текстовые значения.</span><span class="sxs-lookup"><span data-stu-id="f83c3-123">The following are the possible text values:</span></span> 
  
- <span data-ttu-id="f83c3-124">HardDelete — указывает, что элементы в беседе навсегда удаляются из базы данных почтовых ящиков.</span><span class="sxs-lookup"><span data-stu-id="f83c3-124">HardDelete - Indicates that items in a conversation are permanently removed from the mailbox database.</span></span>
    
- <span data-ttu-id="f83c3-125">Моветоделетеитемс — указывает, что элементы в беседе перемещаются в папку "Удаленные".</span><span class="sxs-lookup"><span data-stu-id="f83c3-125">MoveToDeleteItems - Indicates that items in a conversation are moved to the Deleted Items folder.</span></span>
    
- <span data-ttu-id="f83c3-126">SoftDelete — указывает, что элементы в беседе перемещаются в мусорную корзину, если корзина включена.</span><span class="sxs-lookup"><span data-stu-id="f83c3-126">SoftDelete - Indicates that items in a conversation are moved to the dumpster if the dumpster is enabled.</span></span>
    
## <a name="remarks"></a><span data-ttu-id="f83c3-127">Примечания</span><span class="sxs-lookup"><span data-stu-id="f83c3-127">Remarks</span></span>

<span data-ttu-id="f83c3-128">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.Этот элемент появился в Exchange Server 2010 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="f83c3-128">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f83c3-129">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="f83c3-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f83c3-130">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="f83c3-130">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f83c3-131">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="f83c3-131">Schema Name</span></span>  <br/> |<span data-ttu-id="f83c3-132">Схема Types</span><span class="sxs-lookup"><span data-stu-id="f83c3-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="f83c3-133">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="f83c3-133">Validation File</span></span>  <br/> |<span data-ttu-id="f83c3-134">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="f83c3-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="f83c3-135">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="f83c3-135">Can be Empty</span></span>  <br/> |<span data-ttu-id="f83c3-136">False</span><span class="sxs-lookup"><span data-stu-id="f83c3-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f83c3-137">См. также</span><span class="sxs-lookup"><span data-stu-id="f83c3-137">See also</span></span>

- [<span data-ttu-id="f83c3-138">Операция ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="f83c3-138">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)
- [<span data-ttu-id="f83c3-139">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="f83c3-139">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

