---
title: SetItemField
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SetItemField
api_type:
- schema
ms.assetid: 85284fcb-bd1e-4fda-9dab-cb4cd637cd5b
description: Элемент SetItemField представляет отдельное свойство элемента в рамках одной операции UpdateItem обновление.
ms.openlocfilehash: 012e6ae21af653b4bf12588e5a97334a62884059
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19835439"
---
# <a name="setitemfield"></a><span data-ttu-id="b0a66-103">SetItemField</span><span class="sxs-lookup"><span data-stu-id="b0a66-103">SetItemField</span></span>

<span data-ttu-id="b0a66-104">Элемент **SetItemField** представляет отдельное свойство элемента в рамках одной [операции UpdateItem](updateitem-operation.md)обновление.</span><span class="sxs-lookup"><span data-stu-id="b0a66-104">The **SetItemField** element represents an update to a single property of an item in an [UpdateItem operation](updateitem-operation.md).</span></span>
  
```xml
<SetItemField>
   <FieldURI/>
   <Item/>
</SetItemField>
```

 <span data-ttu-id="b0a66-105">**SetItemFieldType**</span><span class="sxs-lookup"><span data-stu-id="b0a66-105">**SetItemFieldType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b0a66-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="b0a66-106">Attributes and elements</span></span>

<span data-ttu-id="b0a66-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="b0a66-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b0a66-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="b0a66-108">Attributes</span></span>

<span data-ttu-id="b0a66-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="b0a66-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b0a66-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="b0a66-110">Child elements</span></span>

|<span data-ttu-id="b0a66-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="b0a66-111">**Element**</span></span>|<span data-ttu-id="b0a66-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="b0a66-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b0a66-113">FieldURI</span><span class="sxs-lookup"><span data-stu-id="b0a66-113">FieldURI</span></span>](fielduri.md) <br/> |<span data-ttu-id="b0a66-114">Идентифицирует часто упоминаемые свойства по URI.</span><span class="sxs-lookup"><span data-stu-id="b0a66-114">Identifies frequently referenced properties by URI.</span></span>  <br/> |
|[<span data-ttu-id="b0a66-115">IndexedFieldURI</span><span class="sxs-lookup"><span data-stu-id="b0a66-115">IndexedFieldURI</span></span>](indexedfielduri.md) <br/> |<span data-ttu-id="b0a66-116">Идентифицирует отдельных элементов словаря.</span><span class="sxs-lookup"><span data-stu-id="b0a66-116">Identifies individual members of a dictionary.</span></span>  <br/> |
|[<span data-ttu-id="b0a66-117">ExtendedFieldURI</span><span class="sxs-lookup"><span data-stu-id="b0a66-117">ExtendedFieldURI</span></span>](extendedfielduri.md) <br/> |<span data-ttu-id="b0a66-118">Задает расширенные свойства MAPI для установки.</span><span class="sxs-lookup"><span data-stu-id="b0a66-118">Identifies extended MAPI properties to set.</span></span>  <br/> |
|[<span data-ttu-id="b0a66-119">Элемент</span><span class="sxs-lookup"><span data-stu-id="b0a66-119">Item</span></span>](item.md) <br/> |<span data-ttu-id="b0a66-120">Представляет элемент в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="b0a66-120">Represents an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="b0a66-121">Message</span><span class="sxs-lookup"><span data-stu-id="b0a66-121">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="b0a66-122">Представляет сообщение электронной почты Exchange для обновления.</span><span class="sxs-lookup"><span data-stu-id="b0a66-122">Represents an Exchange e-mail message to update.</span></span>  <br/> |
|[<span data-ttu-id="b0a66-123">Элемента календаря, имеющего</span><span class="sxs-lookup"><span data-stu-id="b0a66-123">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="b0a66-124">Представляет элемент календаря Exchange для обновления.</span><span class="sxs-lookup"><span data-stu-id="b0a66-124">Represents an Exchange calendar item to update.</span></span>  <br/> |
|[<span data-ttu-id="b0a66-125">Контакт</span><span class="sxs-lookup"><span data-stu-id="b0a66-125">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="b0a66-126">Представляет элемент контакта Exchange для обновления.</span><span class="sxs-lookup"><span data-stu-id="b0a66-126">Represents an Exchange contact item to update.</span></span>  <br/> |
|[<span data-ttu-id="b0a66-127">DistributionList</span><span class="sxs-lookup"><span data-stu-id="b0a66-127">DistributionList</span></span>](distributionlist.md) <br/> |<span data-ttu-id="b0a66-128">Представляет список рассылки, чтобы обновить.</span><span class="sxs-lookup"><span data-stu-id="b0a66-128">Represents a distribution list to update.</span></span>  <br/> |
|[<span data-ttu-id="b0a66-129">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="b0a66-129">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="b0a66-130">Представляет сообщение собрания для обновления.</span><span class="sxs-lookup"><span data-stu-id="b0a66-130">Represents a meeting message to update.</span></span>  <br/> |
|[<span data-ttu-id="b0a66-131">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="b0a66-131">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="b0a66-132">Представляет приглашения на собрание для обновления.</span><span class="sxs-lookup"><span data-stu-id="b0a66-132">Represents a meeting request to update.</span></span>  <br/> |
|[<span data-ttu-id="b0a66-133">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="b0a66-133">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="b0a66-134">Представляет ответ на приглашение для обновления.</span><span class="sxs-lookup"><span data-stu-id="b0a66-134">Represents a meeting response to update.</span></span>  <br/> |
|[<span data-ttu-id="b0a66-135">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="b0a66-135">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="b0a66-136">Представляет отмены собрания для обновления.</span><span class="sxs-lookup"><span data-stu-id="b0a66-136">Represents a meeting cancellation to update.</span></span>  <br/> |
|[<span data-ttu-id="b0a66-137">Задача</span><span class="sxs-lookup"><span data-stu-id="b0a66-137">Task</span></span>](task.md) <br/> |<span data-ttu-id="b0a66-138">Представляет задачу для обновления.</span><span class="sxs-lookup"><span data-stu-id="b0a66-138">Represents a task to update.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="b0a66-139">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="b0a66-139">Parent elements</span></span>

|<span data-ttu-id="b0a66-140">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="b0a66-140">**Element**</span></span>|<span data-ttu-id="b0a66-141">**Описание**</span><span class="sxs-lookup"><span data-stu-id="b0a66-141">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b0a66-142">Обновления (элемент)</span><span class="sxs-lookup"><span data-stu-id="b0a66-142">Updates (Item)</span></span>](updates-item.md) <br/> |<span data-ttu-id="b0a66-143">Содержит набор элементов, которые определяют добавьте, Установка и удаление изменения свойств элемента.</span><span class="sxs-lookup"><span data-stu-id="b0a66-143">Contains a set of elements that define append, set, and delete changes to item properties.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="b0a66-144">Замечания</span><span class="sxs-lookup"><span data-stu-id="b0a66-144">Remarks</span></span>

<span data-ttu-id="b0a66-145">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="b0a66-145">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b0a66-146">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="b0a66-146">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b0a66-147">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="b0a66-147">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="b0a66-148">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="b0a66-148">Schema Name</span></span>  <br/> |<span data-ttu-id="b0a66-149">Схема Types</span><span class="sxs-lookup"><span data-stu-id="b0a66-149">Types schema</span></span>  <br/> |
|<span data-ttu-id="b0a66-150">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="b0a66-150">Validation File</span></span>  <br/> |<span data-ttu-id="b0a66-151">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="b0a66-151">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="b0a66-152">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="b0a66-152">Can be Empty</span></span>  <br/> |<span data-ttu-id="b0a66-153">False</span><span class="sxs-lookup"><span data-stu-id="b0a66-153">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b0a66-154">См. также</span><span class="sxs-lookup"><span data-stu-id="b0a66-154">See also</span></span>



[<span data-ttu-id="b0a66-155">UpdateItem Operation</span><span class="sxs-lookup"><span data-stu-id="b0a66-155">UpdateItem operation</span></span>](updateitem-operation.md)

