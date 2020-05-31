---
title: ConversationId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ConversationId
api_type:
- schema
ms.assetid: d5f1ddb3-9af3-4677-a6ba-111b304a951e
description: Элемент ConversationId содержит идентификатор элемента или беседы.
ms.openlocfilehash: 1f82e6ade60fb70db4a9f026fd72d9f11cc63821
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761814"
---
# <a name="conversationid"></a><span data-ttu-id="2afa8-103">ConversationId</span><span class="sxs-lookup"><span data-stu-id="2afa8-103">ConversationId</span></span>

<span data-ttu-id="2afa8-104">Элемент **ConversationId** содержит идентификатор элемента или беседы.</span><span class="sxs-lookup"><span data-stu-id="2afa8-104">The **ConversationId** element contains the identifier of an item or conversation.</span></span> 
  
```XML
<ConversationId Id="" ChangeKey="" />
```

 <span data-ttu-id="2afa8-105">**итемидтипе**</span><span class="sxs-lookup"><span data-stu-id="2afa8-105">**ItemIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2afa8-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="2afa8-106">Attributes and elements</span></span>

<span data-ttu-id="2afa8-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="2afa8-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2afa8-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="2afa8-108">Attributes</span></span>

|<span data-ttu-id="2afa8-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="2afa8-109">**Attribute**</span></span>|<span data-ttu-id="2afa8-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="2afa8-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="2afa8-111">**Id**</span><span class="sxs-lookup"><span data-stu-id="2afa8-111">**Id**</span></span> <br/> |<span data-ttu-id="2afa8-112">Определяет определенный элемент в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="2afa8-112">Identifies a specific item in the Exchange store.</span></span>  <br/> |
|<span data-ttu-id="2afa8-113">**чанжекэй**</span><span class="sxs-lookup"><span data-stu-id="2afa8-113">**ChangeKey**</span></span> <br/> | <span data-ttu-id="2afa8-114">Определяет определенную версию элемента.</span><span class="sxs-lookup"><span data-stu-id="2afa8-114">Identifies a specific version of an item.</span></span> <span data-ttu-id="2afa8-115">**Чанжекэй** является обязательным для следующих сценариев:</span><span class="sxs-lookup"><span data-stu-id="2afa8-115">A **ChangeKey** is required for the following scenarios:</span></span>  <br/><br/><span data-ttu-id="2afa8-116">-Для элемента [UpdateItem](updateitem.md) требуется **чанжекэй** , если для атрибута **Конфликтресолутион** задано значение автоматического разрешения.</span><span class="sxs-lookup"><span data-stu-id="2afa8-116">- The [UpdateItem](updateitem.md) element requires a **ChangeKey** if the **ConflictResolution** attribute is set to AutoResolve.</span></span> <span data-ttu-id="2afa8-117">Параметр "Авторазрешение" является значением по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="2afa8-117">AutoResolve is a default value.</span></span> <span data-ttu-id="2afa8-118">Если атрибут **чанжекэй** не включен, ответ вернет значение [респонсекоде](responsecode.md) , равное **еррорчанжекэйрекуиред**.</span><span class="sxs-lookup"><span data-stu-id="2afa8-118">If the **ChangeKey** attribute is not included, the response will return a [ResponseCode](responsecode.md) value equal to **ErrorChangeKeyRequired**.</span></span><br/><br/><span data-ttu-id="2afa8-119">- Для элементов [SendItem](senditem.md), [DeleteItem](deleteitem.md)и [DeleteFolder](deletefolder.md) требуется **чанжекэй** , чтобы проверить, будет ли Предпринятая операция действовать в последней версии элемента.</span><span class="sxs-lookup"><span data-stu-id="2afa8-119">- [SendItem](senditem.md), [DeleteItem](deleteitem.md), and [DeleteFolder](deletefolder.md) elements require a **ChangeKey** to test whether the attempted operation will act upon the most recent version of an item.</span></span> <span data-ttu-id="2afa8-120">Если атрибут **чанжекэй** не включен в идентификатор **ItemId** или **чанжекэй** пуст, то ответ вернет значение [респонсекоде](responsecode.md) , равное **еррорсталеобжект**.</span><span class="sxs-lookup"><span data-stu-id="2afa8-120">If the **ChangeKey** attribute is not included in the **ItemId** or if the **ChangeKey** is empty, the response will return a [ResponseCode](responsecode.md) value equal to **ErrorStaleObject**.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="2afa8-121">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="2afa8-121">Child elements</span></span>

<span data-ttu-id="2afa8-122">Нет.</span><span class="sxs-lookup"><span data-stu-id="2afa8-122">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="2afa8-123">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="2afa8-123">Parent elements</span></span>

|<span data-ttu-id="2afa8-124">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="2afa8-124">**Element**</span></span>|<span data-ttu-id="2afa8-125">**Описание**</span><span class="sxs-lookup"><span data-stu-id="2afa8-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2afa8-126">календаритем</span><span class="sxs-lookup"><span data-stu-id="2afa8-126">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="2afa8-127">Представляет элемент календаря Exchange.</span><span class="sxs-lookup"><span data-stu-id="2afa8-127">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="2afa8-128">Контакт</span><span class="sxs-lookup"><span data-stu-id="2afa8-128">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="2afa8-129">Представляет элемент контакта Exchange.</span><span class="sxs-lookup"><span data-stu-id="2afa8-129">Represents an Exchange contact item.</span></span>  <br/> |
|[<span data-ttu-id="2afa8-130">конверсатионактион</span><span class="sxs-lookup"><span data-stu-id="2afa8-130">ConversationAction</span></span>](conversationaction.md) <br/> |<span data-ttu-id="2afa8-131">Представляет одно действие, которое будет применено к одной беседе.</span><span class="sxs-lookup"><span data-stu-id="2afa8-131">Represents a single action to be applied to a single conversation.</span></span>  <br/> |
|[<span data-ttu-id="2afa8-132">дистрибутионлист</span><span class="sxs-lookup"><span data-stu-id="2afa8-132">DistributionList</span></span>](distributionlist.md) <br/> |<span data-ttu-id="2afa8-133">Представляет список рассылки.</span><span class="sxs-lookup"><span data-stu-id="2afa8-133">Represents a distribution list.</span></span>  <br/> |
|[<span data-ttu-id="2afa8-134">Элемент</span><span class="sxs-lookup"><span data-stu-id="2afa8-134">Item</span></span>](item.md) <br/> |<span data-ttu-id="2afa8-135">Представляет элемент в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="2afa8-135">Represents an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="2afa8-136">митингканцеллатион</span><span class="sxs-lookup"><span data-stu-id="2afa8-136">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="2afa8-137">Представляет отмену собрания в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="2afa8-137">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="2afa8-138">митингмессаже</span><span class="sxs-lookup"><span data-stu-id="2afa8-138">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="2afa8-139">Представляет собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="2afa8-139">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="2afa8-140">Свойство meetingrequest</span><span class="sxs-lookup"><span data-stu-id="2afa8-140">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="2afa8-141">Представляет приглашение на собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="2afa8-141">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="2afa8-142">митингреспонсе</span><span class="sxs-lookup"><span data-stu-id="2afa8-142">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="2afa8-143">Представляет ответ на приглашение на собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="2afa8-143">Represents a meeting response in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="2afa8-144">Message</span><span class="sxs-lookup"><span data-stu-id="2afa8-144">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="2afa8-145">Представляет сообщение электронной почты Exchange.</span><span class="sxs-lookup"><span data-stu-id="2afa8-145">Represents an Exchange e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="2afa8-146">PostItem</span><span class="sxs-lookup"><span data-stu-id="2afa8-146">PostItem</span></span>](postitem.md) <br/> |<span data-ttu-id="2afa8-147">Представляет элемент POST в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="2afa8-147">Represents a post item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="2afa8-148">RemoveItem</span><span class="sxs-lookup"><span data-stu-id="2afa8-148">RemoveItem</span></span>](removeitem.md) <br/> |<span data-ttu-id="2afa8-149">Удаляет элемент из хранилища Exchange.</span><span class="sxs-lookup"><span data-stu-id="2afa8-149">Removes an item from the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="2afa8-150">Задача</span><span class="sxs-lookup"><span data-stu-id="2afa8-150">Task</span></span>](task.md) <br/> |<span data-ttu-id="2afa8-151">Представляет задачу в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="2afa8-151">Represents a task in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="2afa8-152">Беседы (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="2afa8-152">Conversation (ConversationType)</span></span>](conversation-conversationtype.md) <br/> |<span data-ttu-id="2afa8-153">Представляет одну беседу.</span><span class="sxs-lookup"><span data-stu-id="2afa8-153">Represents a single conversation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="2afa8-154">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="2afa8-154">Text value</span></span>

<span data-ttu-id="2afa8-155">Нет.</span><span class="sxs-lookup"><span data-stu-id="2afa8-155">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="2afa8-156">Примечания</span><span class="sxs-lookup"><span data-stu-id="2afa8-156">Remarks</span></span>

<span data-ttu-id="2afa8-157">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="2afa8-157">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2afa8-158">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="2afa8-158">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2afa8-159">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="2afa8-159">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="2afa8-160">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="2afa8-160">Schema Name</span></span>  <br/> |<span data-ttu-id="2afa8-161">Схема Types</span><span class="sxs-lookup"><span data-stu-id="2afa8-161">Types schema</span></span>  <br/> |
|<span data-ttu-id="2afa8-162">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="2afa8-162">Validation File</span></span>  <br/> |<span data-ttu-id="2afa8-163">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="2afa8-163">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="2afa8-164">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="2afa8-164">Can be Empty</span></span>  <br/> |<span data-ttu-id="2afa8-165">False</span><span class="sxs-lookup"><span data-stu-id="2afa8-165">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="2afa8-166">См. также</span><span class="sxs-lookup"><span data-stu-id="2afa8-166">See also</span></span>

- [<span data-ttu-id="2afa8-167">Операция FindConversation</span><span class="sxs-lookup"><span data-stu-id="2afa8-167">FindConversation operation</span></span>](findconversation-operation.md)
- [<span data-ttu-id="2afa8-168">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="2afa8-168">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

