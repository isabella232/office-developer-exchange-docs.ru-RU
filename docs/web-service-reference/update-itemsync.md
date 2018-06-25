---
title: Обновление (ItemSync)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Update
api_type:
- schema
ms.assetid: 4e204446-1c80-44f9-b93b-77ce630a01a5
description: Элемент обновления определяет один элемент для обновления в локальном хранилище клиента.
ms.openlocfilehash: ef1bd46906152affbe54372472766afc2a6ae8c1
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19840315"
---
# <a name="update-itemsync"></a><span data-ttu-id="007ba-103">Обновление (ItemSync)</span><span class="sxs-lookup"><span data-stu-id="007ba-103">Update (ItemSync)</span></span>

<span data-ttu-id="007ba-104">**Обновить** элемент определяет один элемент для обновления в локальном хранилище клиента.</span><span class="sxs-lookup"><span data-stu-id="007ba-104">The **Update** element identifies a single item to update in the local client store.</span></span> 
  
[<span data-ttu-id="007ba-105">SyncFolderItemsResponse</span><span class="sxs-lookup"><span data-stu-id="007ba-105">SyncFolderItemsResponse</span></span>](syncfolderitemsresponse.md)
  
[<span data-ttu-id="007ba-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="007ba-106">ResponseMessages</span></span>](responsemessages.md)
  
[<span data-ttu-id="007ba-107">SyncFolderItemsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="007ba-107">SyncFolderItemsResponseMessage</span></span>](syncfolderitemsresponsemessage.md)
  
[<span data-ttu-id="007ba-108">Изменения (элементы)</span><span class="sxs-lookup"><span data-stu-id="007ba-108">Changes (Items)</span></span>](changes-items.md)
  
[<span data-ttu-id="007ba-109">Обновление (ItemSync)</span><span class="sxs-lookup"><span data-stu-id="007ba-109">Update (ItemSync)</span></span>](update-itemsync.md)
  
```xml
<Update>
   <Item/>
</Update>
```

 <span data-ttu-id="007ba-110">**SyncFolderItemsCreateOrUpdateType**</span><span class="sxs-lookup"><span data-stu-id="007ba-110">**SyncFolderItemsCreateOrUpdateType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="007ba-111">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="007ba-111">Attributes and elements</span></span>

<span data-ttu-id="007ba-112">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="007ba-112">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="007ba-113">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="007ba-113">Attributes</span></span>

<span data-ttu-id="007ba-114">Нет.</span><span class="sxs-lookup"><span data-stu-id="007ba-114">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="007ba-115">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="007ba-115">Child elements</span></span>

|<span data-ttu-id="007ba-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="007ba-116">**Element**</span></span>|<span data-ttu-id="007ba-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="007ba-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="007ba-118">Элемент</span><span class="sxs-lookup"><span data-stu-id="007ba-118">Item</span></span>](item.md) <br/> |<span data-ttu-id="007ba-119">Представляет универсальный элемент Exchange для обновления.</span><span class="sxs-lookup"><span data-stu-id="007ba-119">Represents a generic Exchange item to update.</span></span>  <br/> |
|[<span data-ttu-id="007ba-120">Message</span><span class="sxs-lookup"><span data-stu-id="007ba-120">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="007ba-121">Представляет сообщение электронной почты Exchange для обновления.</span><span class="sxs-lookup"><span data-stu-id="007ba-121">Represents an Exchange e-mail message to update.</span></span>  <br/> |
|[<span data-ttu-id="007ba-122">Элемента календаря, имеющего</span><span class="sxs-lookup"><span data-stu-id="007ba-122">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="007ba-123">Представляет элемент календаря Exchange для обновления.</span><span class="sxs-lookup"><span data-stu-id="007ba-123">Represents an Exchange calendar item to update.</span></span>  <br/> |
|[<span data-ttu-id="007ba-124">Контакт</span><span class="sxs-lookup"><span data-stu-id="007ba-124">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="007ba-125">Представляет элемент контакта Exchange для обновления.</span><span class="sxs-lookup"><span data-stu-id="007ba-125">Represents an Exchange contact item to update.</span></span>  <br/> |
|[<span data-ttu-id="007ba-126">DistributionList</span><span class="sxs-lookup"><span data-stu-id="007ba-126">DistributionList</span></span>](distributionlist.md) <br/> |<span data-ttu-id="007ba-127">Представляет список рассылки, чтобы обновить.</span><span class="sxs-lookup"><span data-stu-id="007ba-127">Represents a distribution list to update.</span></span>  <br/> |
|[<span data-ttu-id="007ba-128">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="007ba-128">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="007ba-129">Представляет сообщение собрания для обновления.</span><span class="sxs-lookup"><span data-stu-id="007ba-129">Represents a meeting message to update.</span></span>  <br/> |
|[<span data-ttu-id="007ba-130">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="007ba-130">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="007ba-131">Представляет приглашения на собрание для обновления.</span><span class="sxs-lookup"><span data-stu-id="007ba-131">Represents a meeting request to update.</span></span>  <br/> |
|[<span data-ttu-id="007ba-132">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="007ba-132">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="007ba-133">Представляет ответ на приглашение для обновления.</span><span class="sxs-lookup"><span data-stu-id="007ba-133">Represents a meeting response to update.</span></span>  <br/> |
|[<span data-ttu-id="007ba-134">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="007ba-134">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="007ba-135">Представляет отмены собрания для обновления.</span><span class="sxs-lookup"><span data-stu-id="007ba-135">Represents a meeting cancellation to update.</span></span>  <br/> |
|[<span data-ttu-id="007ba-136">Задача</span><span class="sxs-lookup"><span data-stu-id="007ba-136">Task</span></span>](task.md) <br/> |<span data-ttu-id="007ba-137">Представляет задачу для обновления.</span><span class="sxs-lookup"><span data-stu-id="007ba-137">Represents a task to update.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="007ba-138">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="007ba-138">Parent elements</span></span>

|<span data-ttu-id="007ba-139">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="007ba-139">**Element**</span></span>|<span data-ttu-id="007ba-140">**Описание**</span><span class="sxs-lookup"><span data-stu-id="007ba-140">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="007ba-141">Изменения (элементы)</span><span class="sxs-lookup"><span data-stu-id="007ba-141">Changes (Items)</span></span>](changes-items.md) <br/> |<span data-ttu-id="007ba-142">Содержит массив последовательности типов изменений, которые представляют тип различия между элементами на стороне клиента и элементов на сервере Exchange.</span><span class="sxs-lookup"><span data-stu-id="007ba-142">Contains a sequence array of change types that represent the type of differences between the items on the client and the items on the Exchange server.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="007ba-143">Замечания</span><span class="sxs-lookup"><span data-stu-id="007ba-143">Remarks</span></span>

<span data-ttu-id="007ba-144">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="007ba-144">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="007ba-145">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="007ba-145">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="007ba-146">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="007ba-146">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="007ba-147">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="007ba-147">Schema name</span></span>  <br/> |<span data-ttu-id="007ba-148">Схема Types</span><span class="sxs-lookup"><span data-stu-id="007ba-148">Types schema</span></span>  <br/> |
|<span data-ttu-id="007ba-149">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="007ba-149">Validation file</span></span>  <br/> |<span data-ttu-id="007ba-150">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="007ba-150">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="007ba-151">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="007ba-151">Can be empty</span></span>  <br/> |<span data-ttu-id="007ba-152">False</span><span class="sxs-lookup"><span data-stu-id="007ba-152">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="007ba-153">См. также</span><span class="sxs-lookup"><span data-stu-id="007ba-153">See also</span></span>



[<span data-ttu-id="007ba-154">Операция SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="007ba-154">SyncFolderItems operation</span></span>](syncfolderitems-operation.md)


- [<span data-ttu-id="007ba-155">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="007ba-155">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

