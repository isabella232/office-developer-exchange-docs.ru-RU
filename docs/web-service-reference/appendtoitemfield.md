---
title: AppendToItemField
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AppendToItemField
api_type:
- schema
ms.assetid: 66dbcb4a-ae6d-4648-8610-67187bdb105c
description: Элемент AppendToItemField определяет данные для добавления к отдельное свойство элемента во время операции UpdateItem.
ms.openlocfilehash: b432399e84ee4a3fd7edc5d3f803079435c79143
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761396"
---
# <a name="appendtoitemfield"></a><span data-ttu-id="d41b5-103">AppendToItemField</span><span class="sxs-lookup"><span data-stu-id="d41b5-103">AppendToItemField</span></span>

<span data-ttu-id="d41b5-104">Элемент **AppendToItemField** определяет данные для добавления к отдельное свойство элемента во время [операции UpdateItem](updateitem-operation.md).</span><span class="sxs-lookup"><span data-stu-id="d41b5-104">The **AppendToItemField** element identifies data to append to a single property of an item during an [UpdateItem operation](updateitem-operation.md).</span></span>
  
- [<span data-ttu-id="d41b5-105">UpdateItem</span><span class="sxs-lookup"><span data-stu-id="d41b5-105">UpdateItem</span></span>](updateitem.md)
  
- [<span data-ttu-id="d41b5-106">ItemChanges</span><span class="sxs-lookup"><span data-stu-id="d41b5-106">ItemChanges</span></span>](itemchanges.md)
  
- [<span data-ttu-id="d41b5-107">ItemChange</span><span class="sxs-lookup"><span data-stu-id="d41b5-107">ItemChange</span></span>](itemchange.md)
  
- [<span data-ttu-id="d41b5-108">Обновления (элемент)</span><span class="sxs-lookup"><span data-stu-id="d41b5-108">Updates (Item)</span></span>](updates-item.md)
  
- [<span data-ttu-id="d41b5-109">AppendToItemField</span><span class="sxs-lookup"><span data-stu-id="d41b5-109">AppendToItemField</span></span>](appendtoitemfield.md)
  
```xml
<AppendToItemField>
   <FieldURI/>
   <Item/>
</AppendToItemField>
```

 <span data-ttu-id="d41b5-110">**AppendToItemFieldType**</span><span class="sxs-lookup"><span data-stu-id="d41b5-110">**AppendToItemFieldType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d41b5-111">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="d41b5-111">Attributes and elements</span></span>

<span data-ttu-id="d41b5-112">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="d41b5-112">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d41b5-113">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="d41b5-113">Attributes</span></span>

<span data-ttu-id="d41b5-114">Нет.</span><span class="sxs-lookup"><span data-stu-id="d41b5-114">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d41b5-115">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="d41b5-115">Child elements</span></span>

|<span data-ttu-id="d41b5-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="d41b5-116">**Element**</span></span>|<span data-ttu-id="d41b5-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d41b5-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d41b5-118">FieldURI</span><span class="sxs-lookup"><span data-stu-id="d41b5-118">FieldURI</span></span>](fielduri.md) <br/> |<span data-ttu-id="d41b5-119">Идентифицирует часто упоминаемые свойства по URI.</span><span class="sxs-lookup"><span data-stu-id="d41b5-119">Identifies frequently referenced properties by URI.</span></span>  <br/> |
|[<span data-ttu-id="d41b5-120">IndexedFieldURI</span><span class="sxs-lookup"><span data-stu-id="d41b5-120">IndexedFieldURI</span></span>](indexedfielduri.md) <br/> |<span data-ttu-id="d41b5-121">Идентифицирует отдельных элементов словаря.</span><span class="sxs-lookup"><span data-stu-id="d41b5-121">Identifies individual members of a dictionary.</span></span>  <br/> |
|[<span data-ttu-id="d41b5-122">ExtendedFieldURI</span><span class="sxs-lookup"><span data-stu-id="d41b5-122">ExtendedFieldURI</span></span>](extendedfielduri.md) <br/> |<span data-ttu-id="d41b5-123">Задает расширенные свойства MAPI для добавления.</span><span class="sxs-lookup"><span data-stu-id="d41b5-123">Identifies extended MAPI properties to append.</span></span>  <br/> |
|[<span data-ttu-id="d41b5-124">Элемент</span><span class="sxs-lookup"><span data-stu-id="d41b5-124">Item</span></span>](item.md) <br/> |<span data-ttu-id="d41b5-125">Представляет элемент в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="d41b5-125">Represents an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="d41b5-126">Message</span><span class="sxs-lookup"><span data-stu-id="d41b5-126">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="d41b5-127">Представляет сообщение электронной почты Exchange.</span><span class="sxs-lookup"><span data-stu-id="d41b5-127">Represents an Exchange e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="d41b5-128">Элемента календаря, имеющего</span><span class="sxs-lookup"><span data-stu-id="d41b5-128">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="d41b5-129">Представляет элемент календаря Exchange.</span><span class="sxs-lookup"><span data-stu-id="d41b5-129">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="d41b5-130">Контакт</span><span class="sxs-lookup"><span data-stu-id="d41b5-130">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="d41b5-131">Представляет элемент контакта Exchange.</span><span class="sxs-lookup"><span data-stu-id="d41b5-131">Represents an Exchange contact item.</span></span>  <br/> |
|[<span data-ttu-id="d41b5-132">DistributionList</span><span class="sxs-lookup"><span data-stu-id="d41b5-132">DistributionList</span></span>](distributionlist.md) <br/> |<span data-ttu-id="d41b5-133">Представляет список рассылки.</span><span class="sxs-lookup"><span data-stu-id="d41b5-133">Represents a distribution list.</span></span>  <br/> |
|[<span data-ttu-id="d41b5-134">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="d41b5-134">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="d41b5-135">Представляет собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="d41b5-135">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="d41b5-136">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="d41b5-136">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="d41b5-137">Представляет ответ на приглашение на собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="d41b5-137">Represents a meeting response in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="d41b5-138">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="d41b5-138">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="d41b5-139">Представляет приглашение на собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="d41b5-139">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="d41b5-140">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="d41b5-140">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="d41b5-141">Представляет отмену собрания в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="d41b5-141">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="d41b5-142">Задача</span><span class="sxs-lookup"><span data-stu-id="d41b5-142">Task</span></span>](task.md) <br/> |<span data-ttu-id="d41b5-143">Представляет задачу в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="d41b5-143">Represents a task in the Exchange store.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d41b5-144">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="d41b5-144">Parent elements</span></span>

|<span data-ttu-id="d41b5-145">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="d41b5-145">**Element**</span></span>|<span data-ttu-id="d41b5-146">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d41b5-146">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d41b5-147">Обновления (элемент)</span><span class="sxs-lookup"><span data-stu-id="d41b5-147">Updates (Item)</span></span>](updates-item.md) <br/> |<span data-ttu-id="d41b5-148">Содержит массив, определяющий добавьте, Установка и удаление изменения свойств элемента.</span><span class="sxs-lookup"><span data-stu-id="d41b5-148">Contains an array that defines append, set, and delete changes to item properties.</span></span>  <br/> <span data-ttu-id="d41b5-149">Ниже приведен выражение XPath для этого элемента.`/UpdateItem/ItemChanges/ItemChange[i]/Updates`</span><span class="sxs-lookup"><span data-stu-id="d41b5-149">The following is the XPath expression to this element:  `/UpdateItem/ItemChanges/ItemChange[i]/Updates`</span></span> <br/> |
   
## <a name="remarks"></a><span data-ttu-id="d41b5-150">Замечания</span><span class="sxs-lookup"><span data-stu-id="d41b5-150">Remarks</span></span>

<span data-ttu-id="d41b5-151">Только определенные свойства поддержка добавления операции.</span><span class="sxs-lookup"><span data-stu-id="d41b5-151">Only certain properties support append operations.</span></span> <span data-ttu-id="d41b5-152">При попытке добавить свойство, которое не поддерживает добавление приведет к ошибке.</span><span class="sxs-lookup"><span data-stu-id="d41b5-152">An attempt to append to a property that does not support appending will result in an error.</span></span>
  
<span data-ttu-id="d41b5-153">Для операции обновления только одно свойство может быть изменено в рамках одного запроса.</span><span class="sxs-lookup"><span data-stu-id="d41b5-153">For update operations, only one property can be modified within a single request.</span></span> <span data-ttu-id="d41b5-154">Что в элементе [путь](path.md) должен указанный отдельное свойство.</span><span class="sxs-lookup"><span data-stu-id="d41b5-154">That single property must be referenced in the [Path](path.md) element.</span></span> <span data-ttu-id="d41b5-155">**Элемент в производные классы** можно только удержание отдельное свойство, который является согласуется единственный элемент **пути** .</span><span class="sxs-lookup"><span data-stu-id="d41b5-155">The **Item** element in the derived classes can then only hold a single property that is in agreement with the single **Path** element.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="d41b5-156">Элемент [пути](path.md) абстрактный.</span><span class="sxs-lookup"><span data-stu-id="d41b5-156">The [Path](path.md) element is abstract.</span></span> <span data-ttu-id="d41b5-157">Он должен быть заменен элемент [FieldURI](fielduri.md), [IndexedFieldURI](indexedfielduri.md)или [ExtendedFieldURI](extendedfielduri.md) .</span><span class="sxs-lookup"><span data-stu-id="d41b5-157">It must be substituted by the [FieldURI](fielduri.md), [IndexedFieldURI](indexedfielduri.md), or [ExtendedFieldURI](extendedfielduri.md) element.</span></span> 
  
<span data-ttu-id="d41b5-158">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="d41b5-158">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d41b5-159">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="d41b5-159">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d41b5-160">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="d41b5-160">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d41b5-161">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="d41b5-161">Schema Name</span></span>  <br/> |<span data-ttu-id="d41b5-162">Схема Types</span><span class="sxs-lookup"><span data-stu-id="d41b5-162">Types schema</span></span>  <br/> |
|<span data-ttu-id="d41b5-163">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="d41b5-163">Validation File</span></span>  <br/> |<span data-ttu-id="d41b5-164">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="d41b5-164">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d41b5-165">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="d41b5-165">Can be Empty</span></span>  <br/> |<span data-ttu-id="d41b5-166">False</span><span class="sxs-lookup"><span data-stu-id="d41b5-166">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d41b5-167">См. также</span><span class="sxs-lookup"><span data-stu-id="d41b5-167">See also</span></span>

- [<span data-ttu-id="d41b5-168">UpdateItem Operation</span><span class="sxs-lookup"><span data-stu-id="d41b5-168">UpdateItem operation</span></span>](updateitem-operation.md)
- [<span data-ttu-id="d41b5-169">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="d41b5-169">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

