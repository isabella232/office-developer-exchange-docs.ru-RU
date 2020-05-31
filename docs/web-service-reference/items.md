---
title: Элементы
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Items
api_type:
- schema
ms.assetid: 0811a73e-bf1f-4889-9219-73902dd47639
description: Элемент Items содержит массив элементов.
ms.openlocfilehash: 241a56ee23e87d6a4320b93cc65b1f5aa1f60120
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834163"
---
# <a name="items"></a><span data-ttu-id="952ae-103">Элементы</span><span class="sxs-lookup"><span data-stu-id="952ae-103">Items</span></span>

<span data-ttu-id="952ae-104">Элемент **Items** содержит массив элементов.</span><span class="sxs-lookup"><span data-stu-id="952ae-104">The **Items** element contains an array of items.</span></span> 
  
```xml
<Items>
   <Item/>
   <Message/>
   <CalendarItem/>
   <Contact/>
   <DistributionList/>
   <MeetingMessage/>
   <MeetingRequest/>
   <MeetingResponse/>
   <MeetingCancellation/>
   <Task/>
   <PostItem/>
</Items>
```

 <span data-ttu-id="952ae-105">**аррайофреалитемстипе**</span><span class="sxs-lookup"><span data-stu-id="952ae-105">**ArrayOfRealItemsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="952ae-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="952ae-106">Attributes and elements</span></span>

<span data-ttu-id="952ae-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="952ae-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="952ae-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="952ae-108">Attributes</span></span>

<span data-ttu-id="952ae-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="952ae-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="952ae-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="952ae-110">Child elements</span></span>

|<span data-ttu-id="952ae-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="952ae-111">**Element**</span></span>|<span data-ttu-id="952ae-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="952ae-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="952ae-113">Элемент</span><span class="sxs-lookup"><span data-stu-id="952ae-113">Item</span></span>](item.md) <br/> |<span data-ttu-id="952ae-114">Представляет элемент в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="952ae-114">Represents an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="952ae-115">Message</span><span class="sxs-lookup"><span data-stu-id="952ae-115">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="952ae-116">Представляет сообщение электронной почты Exchange.</span><span class="sxs-lookup"><span data-stu-id="952ae-116">Represents an Exchange e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="952ae-117">календаритем</span><span class="sxs-lookup"><span data-stu-id="952ae-117">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="952ae-118">Представляет элемент календаря Exchange.</span><span class="sxs-lookup"><span data-stu-id="952ae-118">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="952ae-119">Контакт</span><span class="sxs-lookup"><span data-stu-id="952ae-119">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="952ae-120">Представляет элемент контакта Exchange.</span><span class="sxs-lookup"><span data-stu-id="952ae-120">Represents an Exchange contact item.</span></span>  <br/> |
|[<span data-ttu-id="952ae-121">дистрибутионлист</span><span class="sxs-lookup"><span data-stu-id="952ae-121">DistributionList</span></span>](distributionlist.md) <br/> |<span data-ttu-id="952ae-122">Представляет список рассылки.</span><span class="sxs-lookup"><span data-stu-id="952ae-122">Represents a distribution list.</span></span>  <br/> |
|[<span data-ttu-id="952ae-123">митингмессаже</span><span class="sxs-lookup"><span data-stu-id="952ae-123">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="952ae-124">Представляет сообщение о собрании в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="952ae-124">Represents a meeting message in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="952ae-125">Свойство meetingrequest</span><span class="sxs-lookup"><span data-stu-id="952ae-125">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="952ae-126">Представляет приглашение на собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="952ae-126">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="952ae-127">митингреспонсе</span><span class="sxs-lookup"><span data-stu-id="952ae-127">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="952ae-128">Представляет ответ на приглашение на собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="952ae-128">Represents a meeting response in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="952ae-129">митингканцеллатион</span><span class="sxs-lookup"><span data-stu-id="952ae-129">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="952ae-130">Представляет отмену собрания в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="952ae-130">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="952ae-131">Задача</span><span class="sxs-lookup"><span data-stu-id="952ae-131">Task</span></span>](task.md) <br/> |<span data-ttu-id="952ae-132">Представляет задачу в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="952ae-132">Represents a task in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="952ae-133">PostItem</span><span class="sxs-lookup"><span data-stu-id="952ae-133">PostItem</span></span>](postitem.md) <br/> |<span data-ttu-id="952ae-134">Представляет элемент POST в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="952ae-134">Represents a post item in the Exchange store.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="952ae-135">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="952ae-135">Parent elements</span></span>

|<span data-ttu-id="952ae-136">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="952ae-136">**Element**</span></span>|<span data-ttu-id="952ae-137">**Описание**</span><span class="sxs-lookup"><span data-stu-id="952ae-137">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="952ae-138">копитемреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="952ae-138">CopyItemResponseMessage</span></span>](copyitemresponsemessage.md) <br/> |<span data-ttu-id="952ae-139">Содержит состояние и результат запроса [операции CopyItem](copyitem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="952ae-139">Contains the status and result of a [CopyItem operation](copyitem-operation.md) request.</span></span>  <br/> |
|[<span data-ttu-id="952ae-140">креатеитемреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="952ae-140">CreateItemResponseMessage</span></span>](createitemresponsemessage.md) <br/> |<span data-ttu-id="952ae-141">Содержит состояние и результат одного запроса [операции CreateItem](createitem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="952ae-141">Contains the status and result of a single [CreateItem operation](createitem-operation.md) request.</span></span>  <br/> |
|[<span data-ttu-id="952ae-142">жетитемреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="952ae-142">GetItemResponseMessage</span></span>](getitemresponsemessage.md) <br/> |<span data-ttu-id="952ae-143">Содержит состояние и результат запроса [операции GetItem](getitem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="952ae-143">Contains the status and result of a [GetItem operation](getitem-operation.md) request.</span></span>  <br/> |
|[<span data-ttu-id="952ae-144">граупедитемс</span><span class="sxs-lookup"><span data-stu-id="952ae-144">GroupedItems</span></span>](groupeditems.md) <br/> |<span data-ttu-id="952ae-145">Представляет коллекцию элементов, которая является результатом сгруппированного вызова [операции FindItem](finditem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="952ae-145">Represents a collection of items that are the result of a grouped [FindItem operation](finditem-operation.md) call.</span></span>  <br/> |
|[<span data-ttu-id="952ae-146">мовеитемреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="952ae-146">MoveItemResponseMessage</span></span>](moveitemresponsemessage.md) <br/> |<span data-ttu-id="952ae-147">Содержит состояние и результат запроса [операции MoveItem](moveitem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="952ae-147">Contains the status and result of a [MoveItem operation](moveitem-operation.md) request.</span></span>  <br/> |
|[<span data-ttu-id="952ae-148">Рутфолдер (Финдитемреспонсемессаже)</span><span class="sxs-lookup"><span data-stu-id="952ae-148">RootFolder (FindItemResponseMessage)</span></span>](rootfolder-finditemresponsemessage.md) <br/> |<span data-ttu-id="952ae-149">Содержит результаты поиска в одной корневой папке во время [операции FindItem](finditem-operation.md).</span><span class="sxs-lookup"><span data-stu-id="952ae-149">Contains the results of a search of a single root folder during a [FindItem operation](finditem-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="952ae-150">упдатеитемреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="952ae-150">UpdateItemResponseMessage</span></span>](updateitemresponsemessage.md) <br/> |<span data-ttu-id="952ae-151">Содержит состояние и результат запроса [операции UpdateItem](updateitem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="952ae-151">Contains the status and result of an [UpdateItem operation](updateitem-operation.md) request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="952ae-152">Примечания</span><span class="sxs-lookup"><span data-stu-id="952ae-152">Remarks</span></span>

<span data-ttu-id="952ae-153">Сведения о наборе элементов в запросе на [операцию CreateItem](createitem-operation.md) см. в статье [Items (нонемптяррайофаллитемстипе)](items-nonemptyarrayofallitemstype.md).</span><span class="sxs-lookup"><span data-stu-id="952ae-153">For information about the set of items in a [CreateItem operation](createitem-operation.md) request, see [Items (NonEmptyArrayOfAllItemsType)](items-nonemptyarrayofallitemstype.md).</span></span>
  
<span data-ttu-id="952ae-154">Элементы [Message](message-ex15websvcsotherref.md) представляют сообщения электронной почты и все другие элементы, которые не являются строго типизированными схемой веб-служб Exchange (EWS).</span><span class="sxs-lookup"><span data-stu-id="952ae-154">[Message](message-ex15websvcsotherref.md) elements represent e-mail messages and all other items that are not strongly typed by the Exchange Web Services (EWS) schema.</span></span> <span data-ttu-id="952ae-155">Элементы, такие как IPM. Общий доступ и IPM. InfoPath возвращаются в виде элементов **Message** .</span><span class="sxs-lookup"><span data-stu-id="952ae-155">Items such as IPM.Sharing and IPM.InfoPath are returned as **Message** elements.</span></span> <span data-ttu-id="952ae-156">Версии Exchange, начиная с Exchange Server 2010, не возвращают элемент базового [элемента](item.md) в ответах.</span><span class="sxs-lookup"><span data-stu-id="952ae-156">Versions of Exchange starting with Exchange Server 2010 do not return the base [Item](item.md) element in responses.</span></span> 
  
<span data-ttu-id="952ae-157">Схема, описывающая этот элемент, находится в виртуальном каталоге EWS компьютера, на котором запущен Exchange, на котором установлена роль сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="952ae-157">The schema that describes this element is located in the EWS virtual directory of the computer that is running Exchange that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="952ae-158">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="952ae-158">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="952ae-159">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="952ae-159">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="952ae-160">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="952ae-160">Schema Name</span></span>  <br/> |<span data-ttu-id="952ae-161">Схема Types</span><span class="sxs-lookup"><span data-stu-id="952ae-161">Types schema</span></span>  <br/> |
|<span data-ttu-id="952ae-162">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="952ae-162">Validation File</span></span>  <br/> |<span data-ttu-id="952ae-163">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="952ae-163">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="952ae-164">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="952ae-164">Can be Empty</span></span>  <br/> |<span data-ttu-id="952ae-165">False</span><span class="sxs-lookup"><span data-stu-id="952ae-165">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="952ae-166">См. также</span><span class="sxs-lookup"><span data-stu-id="952ae-166">See also</span></span>



[<span data-ttu-id="952ae-167">Справка по службам EWS для Exchange</span><span class="sxs-lookup"><span data-stu-id="952ae-167">EWS reference for Exchange</span></span>](ews-reference-for-exchange.md)
  
- [<span data-ttu-id="952ae-168">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="952ae-168">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

