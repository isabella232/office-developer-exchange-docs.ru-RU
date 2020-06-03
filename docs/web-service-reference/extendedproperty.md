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
description: Элемент ExtendedProperty определяет расширенные свойства MAPI для папок и элементов.
ms.openlocfilehash: 99ede097d803d6fbf534cde0e77c08cec054bfa3
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530609"
---
# <a name="extendedproperty"></a><span data-ttu-id="050d1-103">ExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="050d1-103">ExtendedProperty</span></span>

<span data-ttu-id="050d1-104">Элемент **ExtendedProperty** определяет расширенные свойства MAPI для папок и элементов.</span><span class="sxs-lookup"><span data-stu-id="050d1-104">The **ExtendedProperty** element identifies extended MAPI properties on folders and items.</span></span> 
  
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

<span data-ttu-id="050d1-105">**екстендедпропертитипе**</span><span class="sxs-lookup"><span data-stu-id="050d1-105">**ExtendedPropertyType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="050d1-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="050d1-106">Attributes and elements</span></span>

<span data-ttu-id="050d1-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="050d1-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="050d1-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="050d1-108">Attributes</span></span>

<span data-ttu-id="050d1-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="050d1-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="050d1-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="050d1-110">Child elements</span></span>

|<span data-ttu-id="050d1-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="050d1-111">**Element**</span></span>|<span data-ttu-id="050d1-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="050d1-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="050d1-113">екстендедфиелдури</span><span class="sxs-lookup"><span data-stu-id="050d1-113">ExtendedFieldURI</span></span>](extendedfielduri.md) <br/> |<span data-ttu-id="050d1-114">Указывает расширенное свойство MAPI, которое необходимо получить, задать или создать.</span><span class="sxs-lookup"><span data-stu-id="050d1-114">Identifies an extended MAPI property to get, set, or create.</span></span>  <br/> |
|[<span data-ttu-id="050d1-115">Values</span><span class="sxs-lookup"><span data-stu-id="050d1-115">Values</span></span>](values.md) <br/> |<span data-ttu-id="050d1-116">Содержит коллекцию значений для многозначного расширенного свойства MAPI.</span><span class="sxs-lookup"><span data-stu-id="050d1-116">Contains a collection of values for a multivalued extended MAPI property.</span></span>  <br/> |
|[<span data-ttu-id="050d1-117">Значение</span><span class="sxs-lookup"><span data-stu-id="050d1-117">Value</span></span>](value.md) <br/> |<span data-ttu-id="050d1-118">Содержит значение расширенного свойства MAPI с одним значением.</span><span class="sxs-lookup"><span data-stu-id="050d1-118">Contains the value of single-valued MAPI extended property.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="050d1-119">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="050d1-119">Parent elements</span></span>

|<span data-ttu-id="050d1-120">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="050d1-120">**Element**</span></span>|<span data-ttu-id="050d1-121">**Описание**</span><span class="sxs-lookup"><span data-stu-id="050d1-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="050d1-122">календаритем</span><span class="sxs-lookup"><span data-stu-id="050d1-122">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="050d1-123">Представляет элемент календаря Exchange.</span><span class="sxs-lookup"><span data-stu-id="050d1-123">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="050d1-124">Контакт</span><span class="sxs-lookup"><span data-stu-id="050d1-124">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="050d1-125">Представляет элемент контакта Exchange.</span><span class="sxs-lookup"><span data-stu-id="050d1-125">Represents an Exchange contact item.</span></span>  <br/> |
|[<span data-ttu-id="050d1-126">дистрибутионлист</span><span class="sxs-lookup"><span data-stu-id="050d1-126">DistributionList</span></span>](distributionlist.md) <br/> |<span data-ttu-id="050d1-127">Представляет список рассылки.</span><span class="sxs-lookup"><span data-stu-id="050d1-127">Represents a distribution list.</span></span>  <br/> |
|[<span data-ttu-id="050d1-128">Элемент</span><span class="sxs-lookup"><span data-stu-id="050d1-128">Item</span></span>](item.md) <br/> |<span data-ttu-id="050d1-129">Представляет элемент в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="050d1-129">Represents an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="050d1-130">митингканцеллатион</span><span class="sxs-lookup"><span data-stu-id="050d1-130">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="050d1-131">Представляет отмену собрания в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="050d1-131">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="050d1-132">митингмессаже</span><span class="sxs-lookup"><span data-stu-id="050d1-132">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="050d1-133">Представляет собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="050d1-133">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="050d1-134">Свойство meetingrequest</span><span class="sxs-lookup"><span data-stu-id="050d1-134">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="050d1-135">Представляет приглашение на собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="050d1-135">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="050d1-136">митингреспонсе</span><span class="sxs-lookup"><span data-stu-id="050d1-136">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="050d1-137">Представляет ответ на приглашение на собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="050d1-137">Represents a meeting response in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="050d1-138">Message</span><span class="sxs-lookup"><span data-stu-id="050d1-138">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="050d1-139">Представляет сообщение электронной почты Exchange.</span><span class="sxs-lookup"><span data-stu-id="050d1-139">Represents an Exchange e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="050d1-140">RemoveItem</span><span class="sxs-lookup"><span data-stu-id="050d1-140">RemoveItem</span></span>](removeitem.md) <br/> |<span data-ttu-id="050d1-141">Удаляет элемент из хранилища Exchange.</span><span class="sxs-lookup"><span data-stu-id="050d1-141">Removes an item from the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="050d1-142">Задача</span><span class="sxs-lookup"><span data-stu-id="050d1-142">Task</span></span>](task.md) <br/> |<span data-ttu-id="050d1-143">Представляет задачу в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="050d1-143">Represents a task in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="050d1-144">календарфолдер</span><span class="sxs-lookup"><span data-stu-id="050d1-144">CalendarFolder</span></span>](calendarfolder.md) <br/> |<span data-ttu-id="050d1-145">Представляет папку, в которой в основном содержатся элементы календаря.</span><span class="sxs-lookup"><span data-stu-id="050d1-145">Represents a folder that primarily contains calendar items.</span></span>  <br/> |
|[<span data-ttu-id="050d1-146">контактсфолдер</span><span class="sxs-lookup"><span data-stu-id="050d1-146">ContactsFolder</span></span>](contactsfolder.md) <br/> |<span data-ttu-id="050d1-147">Представляет папку "Контакты" в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="050d1-147">Represents a contacts folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="050d1-148">Folder</span><span class="sxs-lookup"><span data-stu-id="050d1-148">Folder</span></span>](folder.md) <br/> |<span data-ttu-id="050d1-149">Представляет папку для создания, получения, поиска, синхронизации или обновления.</span><span class="sxs-lookup"><span data-stu-id="050d1-149">Represents a folder to create, get, find, synchronize, or update.</span></span>  <br/> |
|[<span data-ttu-id="050d1-150">SearchFolder</span><span class="sxs-lookup"><span data-stu-id="050d1-150">SearchFolder</span></span>](searchfolder.md) <br/> |<span data-ttu-id="050d1-151">Представляет папку поиска, содержащуюся в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="050d1-151">Represents a search folder that is contained in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="050d1-152">тасксфолдер</span><span class="sxs-lookup"><span data-stu-id="050d1-152">TasksFolder</span></span>](tasksfolder.md) <br/> |<span data-ttu-id="050d1-153">Представляет папку Tasks, содержащуюся в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="050d1-153">Represents a tasks folder that is contained in a mailbox.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="050d1-154">Примечания</span><span class="sxs-lookup"><span data-stu-id="050d1-154">Remarks</span></span>

<span data-ttu-id="050d1-155">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="050d1-155">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="050d1-156">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="050d1-156">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="050d1-157">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="050d1-157">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="050d1-158">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="050d1-158">Schema Name</span></span>  <br/> |<span data-ttu-id="050d1-159">Схема Types</span><span class="sxs-lookup"><span data-stu-id="050d1-159">Types schema</span></span>  <br/> |
|<span data-ttu-id="050d1-160">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="050d1-160">Validation File</span></span>  <br/> |<span data-ttu-id="050d1-161">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="050d1-161">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="050d1-162">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="050d1-162">Can be Empty</span></span>  <br/> |<span data-ttu-id="050d1-163">False</span><span class="sxs-lookup"><span data-stu-id="050d1-163">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="050d1-164">См. также</span><span class="sxs-lookup"><span data-stu-id="050d1-164">See also</span></span>

- [<span data-ttu-id="050d1-165">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="050d1-165">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

