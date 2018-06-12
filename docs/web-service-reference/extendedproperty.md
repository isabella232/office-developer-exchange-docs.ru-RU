---
title: ExtendedProperty
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ExtendedProperty
api_type:
- schema
ms.assetid: f9701409-b620-4afe-b9ee-4c1e95507af7
description: Элемент ExtendedProperty задает расширенные свойства MAPI для папок и элементов.
ms.openlocfilehash: 6a0aecc732ef634c2258127fca89b19461e25762
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762467"
---
# <a name="extendedproperty"></a><span data-ttu-id="9112a-103">ExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="9112a-103">ExtendedProperty</span></span>

<span data-ttu-id="9112a-104">Элемент **ExtendedProperty** задает расширенные свойства MAPI для папок и элементов.</span><span class="sxs-lookup"><span data-stu-id="9112a-104">The **ExtendedProperty** element identifies extended MAPI properties on folders and items.</span></span> 
  
```xml
<ExtendedProperty>
   <ExtendedFieldURI/>
   <Values/>
</ExtendedProperty>
```

 <span data-ttu-id="9112a-105">**ExtendedPropertyType**</span><span class="sxs-lookup"><span data-stu-id="9112a-105">**ExtendedPropertyType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9112a-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="9112a-106">Attributes and elements</span></span>

<span data-ttu-id="9112a-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="9112a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9112a-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="9112a-108">Attributes</span></span>

<span data-ttu-id="9112a-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="9112a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9112a-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="9112a-110">Child elements</span></span>

|<span data-ttu-id="9112a-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="9112a-111">**Element**</span></span>|<span data-ttu-id="9112a-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="9112a-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9112a-113">ExtendedFieldURI</span><span class="sxs-lookup"><span data-stu-id="9112a-113">ExtendedFieldURI</span></span>](extendedfielduri.md) <br/> |<span data-ttu-id="9112a-114">Определяет расширенные свойства MAPI для получения, установки или создать.</span><span class="sxs-lookup"><span data-stu-id="9112a-114">Identifies an extended MAPI property to get, set, or create.</span></span>  <br/> |
|[<span data-ttu-id="9112a-115">Значения</span><span class="sxs-lookup"><span data-stu-id="9112a-115">Values</span></span>](values.md) <br/> |<span data-ttu-id="9112a-116">Содержит коллекцию значений для многозначного расширенные свойства MAPI.</span><span class="sxs-lookup"><span data-stu-id="9112a-116">Contains a collection of values for a multivalued extended MAPI property.</span></span>  <br/> |
|[<span data-ttu-id="9112a-117">Значение</span><span class="sxs-lookup"><span data-stu-id="9112a-117">Value</span></span>](value.md) <br/> |<span data-ttu-id="9112a-118">Содержит значение расширенных свойств MAPI с одним значением.</span><span class="sxs-lookup"><span data-stu-id="9112a-118">Contains the value of single-valued MAPI extended property.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="9112a-119">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="9112a-119">Parent elements</span></span>

|<span data-ttu-id="9112a-120">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="9112a-120">**Element**</span></span>|<span data-ttu-id="9112a-121">**Описание**</span><span class="sxs-lookup"><span data-stu-id="9112a-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9112a-122">Элемента календаря, имеющего</span><span class="sxs-lookup"><span data-stu-id="9112a-122">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="9112a-123">Представляет элемент календаря Exchange.</span><span class="sxs-lookup"><span data-stu-id="9112a-123">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="9112a-124">Контакт</span><span class="sxs-lookup"><span data-stu-id="9112a-124">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="9112a-125">Представляет элемент контакта Exchange.</span><span class="sxs-lookup"><span data-stu-id="9112a-125">Represents an Exchange contact item.</span></span>  <br/> |
|[<span data-ttu-id="9112a-126">DistributionList</span><span class="sxs-lookup"><span data-stu-id="9112a-126">DistributionList</span></span>](distributionlist.md) <br/> |<span data-ttu-id="9112a-127">Представляет список рассылки.</span><span class="sxs-lookup"><span data-stu-id="9112a-127">Represents a distribution list.</span></span>  <br/> |
|[<span data-ttu-id="9112a-128">Элемент</span><span class="sxs-lookup"><span data-stu-id="9112a-128">Item</span></span>](item.md) <br/> |<span data-ttu-id="9112a-129">Представляет элемент в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="9112a-129">Represents an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="9112a-130">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="9112a-130">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="9112a-131">Представляет отмену собрания в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="9112a-131">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="9112a-132">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="9112a-132">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="9112a-133">Представляет собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="9112a-133">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="9112a-134">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="9112a-134">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="9112a-135">Представляет приглашение на собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="9112a-135">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="9112a-136">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="9112a-136">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="9112a-137">Представляет ответ на приглашение на собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="9112a-137">Represents a meeting response in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="9112a-138">Message</span><span class="sxs-lookup"><span data-stu-id="9112a-138">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="9112a-139">Представляет сообщение электронной почты Exchange.</span><span class="sxs-lookup"><span data-stu-id="9112a-139">Represents an Exchange e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="9112a-140">RemoveItem</span><span class="sxs-lookup"><span data-stu-id="9112a-140">RemoveItem</span></span>](removeitem.md) <br/> |<span data-ttu-id="9112a-141">Удаляет элемент из хранилища Exchange.</span><span class="sxs-lookup"><span data-stu-id="9112a-141">Removes an item from the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="9112a-142">Задача</span><span class="sxs-lookup"><span data-stu-id="9112a-142">Task</span></span>](task.md) <br/> |<span data-ttu-id="9112a-143">Представляет задачу в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="9112a-143">Represents a task in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="9112a-144">CalendarFolder</span><span class="sxs-lookup"><span data-stu-id="9112a-144">CalendarFolder</span></span>](calendarfolder.md) <br/> |<span data-ttu-id="9112a-145">Представляет папку, содержащую элементы календаря в первую очередь.</span><span class="sxs-lookup"><span data-stu-id="9112a-145">Represents a folder that primarily contains calendar items.</span></span>  <br/> |
|[<span data-ttu-id="9112a-146">ContactsFolder</span><span class="sxs-lookup"><span data-stu-id="9112a-146">ContactsFolder</span></span>](contactsfolder.md) <br/> |<span data-ttu-id="9112a-147">Представляет папку контактов в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="9112a-147">Represents a contacts folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="9112a-148">Folder</span><span class="sxs-lookup"><span data-stu-id="9112a-148">Folder</span></span>](folder.md) <br/> |<span data-ttu-id="9112a-149">Представляет папку на создание, получение, найти, синхронизировать или обновление.</span><span class="sxs-lookup"><span data-stu-id="9112a-149">Represents a folder to create, get, find, synchronize, or update.</span></span>  <br/> |
|[<span data-ttu-id="9112a-150">SearchFolder</span><span class="sxs-lookup"><span data-stu-id="9112a-150">SearchFolder</span></span>](searchfolder.md) <br/> |<span data-ttu-id="9112a-151">Представляет папку поиска, содержащихся в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="9112a-151">Represents a search folder that is contained in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="9112a-152">TasksFolder</span><span class="sxs-lookup"><span data-stu-id="9112a-152">TasksFolder</span></span>](tasksfolder.md) <br/> |<span data-ttu-id="9112a-153">Представляет папку задачи, содержащихся в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="9112a-153">Represents a tasks folder that is contained in a mailbox.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="9112a-154">Замечания</span><span class="sxs-lookup"><span data-stu-id="9112a-154">Remarks</span></span>

<span data-ttu-id="9112a-155">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="9112a-155">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9112a-156">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="9112a-156">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9112a-157">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="9112a-157">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="9112a-158">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="9112a-158">Schema Name</span></span>  <br/> |<span data-ttu-id="9112a-159">Схема Types</span><span class="sxs-lookup"><span data-stu-id="9112a-159">Types schema</span></span>  <br/> |
|<span data-ttu-id="9112a-160">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="9112a-160">Validation File</span></span>  <br/> |<span data-ttu-id="9112a-161">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="9112a-161">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="9112a-162">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="9112a-162">Can be Empty</span></span>  <br/> |<span data-ttu-id="9112a-163">False</span><span class="sxs-lookup"><span data-stu-id="9112a-163">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9112a-164">См. также</span><span class="sxs-lookup"><span data-stu-id="9112a-164">See also</span></span>



- [<span data-ttu-id="9112a-165">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="9112a-165">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
