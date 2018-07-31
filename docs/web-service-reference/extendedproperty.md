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
ms.openlocfilehash: 9a6c44e953cab4900e4b75eb42bdf4d8633e58f9
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/28/2018
ms.locfileid: "21353730"
---
# <a name="extendedproperty"></a><span data-ttu-id="d21b7-103">ExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="d21b7-103">ExtendedProperty</span></span>

<span data-ttu-id="d21b7-104">Элемент **ExtendedProperty** задает расширенные свойства MAPI для папок и элементов.</span><span class="sxs-lookup"><span data-stu-id="d21b7-104">The **ExtendedProperty** element identifies extended MAPI properties on folders and items.</span></span> 
  
```xml
<ExtendedProperty>
   <ExtendedFieldURI/>
   <Values/>
</ExtendedProperty>
```

```xml
<ExtendedProperty>
   <ExtendedFieldURI/>
   <Value/>
</ExtendedProperty>
```

<span data-ttu-id="d21b7-105">**ExtendedPropertyType**</span><span class="sxs-lookup"><span data-stu-id="d21b7-105">**ExtendedPropertyType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="d21b7-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="d21b7-106">Attributes and elements</span></span>

<span data-ttu-id="d21b7-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="d21b7-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d21b7-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="d21b7-108">Attributes</span></span>

<span data-ttu-id="d21b7-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="d21b7-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d21b7-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="d21b7-110">Child elements</span></span>

|<span data-ttu-id="d21b7-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="d21b7-111">**Element**</span></span>|<span data-ttu-id="d21b7-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d21b7-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d21b7-113">ExtendedFieldURI</span><span class="sxs-lookup"><span data-stu-id="d21b7-113">ExtendedFieldURI</span></span>](extendedfielduri.md) <br/> |<span data-ttu-id="d21b7-114">Определяет расширенные свойства MAPI для получения, установки или создать.</span><span class="sxs-lookup"><span data-stu-id="d21b7-114">Identifies an extended MAPI property to get, set, or create.</span></span>  <br/> |
|[<span data-ttu-id="d21b7-115">Значения</span><span class="sxs-lookup"><span data-stu-id="d21b7-115">Values</span></span>](values.md) <br/> |<span data-ttu-id="d21b7-116">Содержит коллекцию значений для многозначного расширенные свойства MAPI.</span><span class="sxs-lookup"><span data-stu-id="d21b7-116">Contains a collection of values for a multivalued extended MAPI property.</span></span>  <br/> |
|[<span data-ttu-id="d21b7-117">Значение</span><span class="sxs-lookup"><span data-stu-id="d21b7-117">Value</span></span>](value.md) <br/> |<span data-ttu-id="d21b7-118">Содержит значение расширенных свойств MAPI с одним значением.</span><span class="sxs-lookup"><span data-stu-id="d21b7-118">Contains the value of single-valued MAPI extended property.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d21b7-119">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="d21b7-119">Parent elements</span></span>

|<span data-ttu-id="d21b7-120">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="d21b7-120">**Element**</span></span>|<span data-ttu-id="d21b7-121">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d21b7-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d21b7-122">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="d21b7-122">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="d21b7-123">Представляет элемент календаря Exchange.</span><span class="sxs-lookup"><span data-stu-id="d21b7-123">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="d21b7-124">Контакт</span><span class="sxs-lookup"><span data-stu-id="d21b7-124">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="d21b7-125">Представляет элемент контакта Exchange.</span><span class="sxs-lookup"><span data-stu-id="d21b7-125">Represents an Exchange contact item.</span></span>  <br/> |
|[<span data-ttu-id="d21b7-126">DistributionList</span><span class="sxs-lookup"><span data-stu-id="d21b7-126">DistributionList</span></span>](distributionlist.md) <br/> |<span data-ttu-id="d21b7-127">Представляет список рассылки.</span><span class="sxs-lookup"><span data-stu-id="d21b7-127">Represents a distribution list.</span></span>  <br/> |
|[<span data-ttu-id="d21b7-128">Элемент</span><span class="sxs-lookup"><span data-stu-id="d21b7-128">Item</span></span>](item.md) <br/> |<span data-ttu-id="d21b7-129">Представляет элемент в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="d21b7-129">Represents an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="d21b7-130">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="d21b7-130">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="d21b7-131">Представляет отмену собрания в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="d21b7-131">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="d21b7-132">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="d21b7-132">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="d21b7-133">Представляет собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="d21b7-133">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="d21b7-134">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="d21b7-134">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="d21b7-135">Представляет приглашение на собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="d21b7-135">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="d21b7-136">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="d21b7-136">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="d21b7-137">Представляет ответ на приглашение на собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="d21b7-137">Represents a meeting response in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="d21b7-138">Message</span><span class="sxs-lookup"><span data-stu-id="d21b7-138">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="d21b7-139">Представляет сообщение электронной почты Exchange.</span><span class="sxs-lookup"><span data-stu-id="d21b7-139">Represents an Exchange e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="d21b7-140">RemoveItem</span><span class="sxs-lookup"><span data-stu-id="d21b7-140">RemoveItem</span></span>](removeitem.md) <br/> |<span data-ttu-id="d21b7-141">Удаляет элемент из хранилища Exchange.</span><span class="sxs-lookup"><span data-stu-id="d21b7-141">Removes an item from the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="d21b7-142">Задача</span><span class="sxs-lookup"><span data-stu-id="d21b7-142">Task</span></span>](task.md) <br/> |<span data-ttu-id="d21b7-143">Представляет задачу в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="d21b7-143">Represents a task in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="d21b7-144">CalendarFolder</span><span class="sxs-lookup"><span data-stu-id="d21b7-144">CalendarFolder</span></span>](calendarfolder.md) <br/> |<span data-ttu-id="d21b7-145">Представляет папку, содержащую элементы календаря в первую очередь.</span><span class="sxs-lookup"><span data-stu-id="d21b7-145">Represents a folder that primarily contains calendar items.</span></span>  <br/> |
|[<span data-ttu-id="d21b7-146">ContactsFolder</span><span class="sxs-lookup"><span data-stu-id="d21b7-146">ContactsFolder</span></span>](contactsfolder.md) <br/> |<span data-ttu-id="d21b7-147">Представляет папку контактов в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="d21b7-147">Represents a contacts folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="d21b7-148">Folder</span><span class="sxs-lookup"><span data-stu-id="d21b7-148">Folder</span></span>](folder.md) <br/> |<span data-ttu-id="d21b7-149">Представляет папку на создание, получение, найти, синхронизировать или обновление.</span><span class="sxs-lookup"><span data-stu-id="d21b7-149">Represents a folder to create, get, find, synchronize, or update.</span></span>  <br/> |
|[<span data-ttu-id="d21b7-150">SearchFolder</span><span class="sxs-lookup"><span data-stu-id="d21b7-150">SearchFolder</span></span>](searchfolder.md) <br/> |<span data-ttu-id="d21b7-151">Представляет папку поиска, содержащихся в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="d21b7-151">Represents a search folder that is contained in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="d21b7-152">TasksFolder</span><span class="sxs-lookup"><span data-stu-id="d21b7-152">TasksFolder</span></span>](tasksfolder.md) <br/> |<span data-ttu-id="d21b7-153">Представляет папку задачи, содержащихся в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="d21b7-153">Represents a tasks folder that is contained in a mailbox.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="d21b7-154">Замечания</span><span class="sxs-lookup"><span data-stu-id="d21b7-154">Remarks</span></span>

<span data-ttu-id="d21b7-155">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="d21b7-155">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d21b7-156">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="d21b7-156">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d21b7-157">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="d21b7-157">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d21b7-158">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="d21b7-158">Schema Name</span></span>  <br/> |<span data-ttu-id="d21b7-159">Схема Types</span><span class="sxs-lookup"><span data-stu-id="d21b7-159">Types schema</span></span>  <br/> |
|<span data-ttu-id="d21b7-160">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="d21b7-160">Validation File</span></span>  <br/> |<span data-ttu-id="d21b7-161">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="d21b7-161">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d21b7-162">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="d21b7-162">Can be Empty</span></span>  <br/> |<span data-ttu-id="d21b7-163">False</span><span class="sxs-lookup"><span data-stu-id="d21b7-163">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d21b7-164">См. также</span><span class="sxs-lookup"><span data-stu-id="d21b7-164">See also</span></span>

- [<span data-ttu-id="d21b7-165">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="d21b7-165">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

