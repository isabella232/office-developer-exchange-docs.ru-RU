---
title: Обновление (Итемсинк)
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
description: Элемент Update определяет один элемент для обновления в локальном хранилище клиента.
ms.openlocfilehash: 12248cbbd5d47a19e36d49fcebe6d4753a2e162f
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44468889"
---
# <a name="update-itemsync"></a><span data-ttu-id="d3dc7-103">Обновление (Итемсинк)</span><span class="sxs-lookup"><span data-stu-id="d3dc7-103">Update (ItemSync)</span></span>

<span data-ttu-id="d3dc7-104">Элемент **Update** определяет один элемент для обновления в локальном хранилище клиента.</span><span class="sxs-lookup"><span data-stu-id="d3dc7-104">The **Update** element identifies a single item to update in the local client store.</span></span> 
  
- [<span data-ttu-id="d3dc7-105">синкфолдеритемсреспонсе</span><span class="sxs-lookup"><span data-stu-id="d3dc7-105">SyncFolderItemsResponse</span></span>](syncfolderitemsresponse.md) 
- [<span data-ttu-id="d3dc7-106">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="d3dc7-106">ResponseMessages</span></span>](responsemessages.md)  
- [<span data-ttu-id="d3dc7-107">синкфолдеритемсреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="d3dc7-107">SyncFolderItemsResponseMessage</span></span>](syncfolderitemsresponsemessage.md)  
- [<span data-ttu-id="d3dc7-108">Изменения (элементы)</span><span class="sxs-lookup"><span data-stu-id="d3dc7-108">Changes (Items)</span></span>](changes-items.md)  
- [<span data-ttu-id="d3dc7-109">Обновление (Итемсинк)</span><span class="sxs-lookup"><span data-stu-id="d3dc7-109">Update (ItemSync)</span></span>](update-itemsync.md)
  
```xml
<Update>
   <Item/>
</Update>
```

```xml
<Update>
   <MeetingRequest/>
</Update>
```

```xml
<Update>
   <MeetingCancellation/>
</Update>
```

```xml
<Update>
   <Task/>
</Update>
```

```xml
<Update>
   <CalendarItem/>
</Update>
```

```xml
<Update>
   <MeetingResponse/>
</Update>
```

```xml
<Update>
   <Message/>
</Update>
```

```xml
<Update>
   <DistributionList/>
</Update>
```

```xml
<Update>
   <MeetingMessage/>
</Update>
```

```xml
<Update>
   <Contact/> 
</Update>
```

<span data-ttu-id="d3dc7-110">**синкфолдеритемскреатеорупдатетипе**</span><span class="sxs-lookup"><span data-stu-id="d3dc7-110">**SyncFolderItemsCreateOrUpdateType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="d3dc7-111">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="d3dc7-111">Attributes and elements</span></span>

<span data-ttu-id="d3dc7-112">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="d3dc7-112">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d3dc7-113">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="d3dc7-113">Attributes</span></span>

<span data-ttu-id="d3dc7-114">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="d3dc7-114">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d3dc7-115">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="d3dc7-115">Child elements</span></span>

|<span data-ttu-id="d3dc7-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="d3dc7-116">**Element**</span></span>|<span data-ttu-id="d3dc7-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d3dc7-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d3dc7-118">Ресурс</span><span class="sxs-lookup"><span data-stu-id="d3dc7-118">Item</span></span>](item.md) <br/> |<span data-ttu-id="d3dc7-119">Представляет универсальный элемент Exchange, который необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="d3dc7-119">Represents a generic Exchange item to update.</span></span>  <br/> |
|[<span data-ttu-id="d3dc7-120">Сообщение</span><span class="sxs-lookup"><span data-stu-id="d3dc7-120">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="d3dc7-121">Представляет сообщение электронной почты Exchange, которое требуется обновить.</span><span class="sxs-lookup"><span data-stu-id="d3dc7-121">Represents an Exchange e-mail message to update.</span></span>  <br/> |
|[<span data-ttu-id="d3dc7-122">календаритем</span><span class="sxs-lookup"><span data-stu-id="d3dc7-122">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="d3dc7-123">Представляет элемент календаря Exchange, который необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="d3dc7-123">Represents an Exchange calendar item to update.</span></span>  <br/> |
|<span data-ttu-id="d3dc7-124">[контакт](contact.md);</span><span class="sxs-lookup"><span data-stu-id="d3dc7-124">[Contact](contact.md)</span></span> <br/> |<span data-ttu-id="d3dc7-125">Представляет элемент контакта Exchange, который необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="d3dc7-125">Represents an Exchange contact item to update.</span></span>  <br/> |
|[<span data-ttu-id="d3dc7-126">дистрибутионлист</span><span class="sxs-lookup"><span data-stu-id="d3dc7-126">DistributionList</span></span>](distributionlist.md) <br/> |<span data-ttu-id="d3dc7-127">Представляет список рассылки, который необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="d3dc7-127">Represents a distribution list to update.</span></span>  <br/> |
|[<span data-ttu-id="d3dc7-128">митингмессаже</span><span class="sxs-lookup"><span data-stu-id="d3dc7-128">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="d3dc7-129">Представляет сообщение о собрании, которое необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="d3dc7-129">Represents a meeting message to update.</span></span>  <br/> |
|[<span data-ttu-id="d3dc7-130">Свойство meetingrequest</span><span class="sxs-lookup"><span data-stu-id="d3dc7-130">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="d3dc7-131">Представляет приглашение на собрание, которое требуется обновить.</span><span class="sxs-lookup"><span data-stu-id="d3dc7-131">Represents a meeting request to update.</span></span>  <br/> |
|[<span data-ttu-id="d3dc7-132">митингреспонсе</span><span class="sxs-lookup"><span data-stu-id="d3dc7-132">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="d3dc7-133">Представляет ответ на приглашение на собрание, который необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="d3dc7-133">Represents a meeting response to update.</span></span>  <br/> |
|[<span data-ttu-id="d3dc7-134">митингканцеллатион</span><span class="sxs-lookup"><span data-stu-id="d3dc7-134">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="d3dc7-135">Представляет отмену собрания, которое необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="d3dc7-135">Represents a meeting cancellation to update.</span></span>  <br/> |
|[<span data-ttu-id="d3dc7-136">Task</span><span class="sxs-lookup"><span data-stu-id="d3dc7-136">Task</span></span>](task.md) <br/> |<span data-ttu-id="d3dc7-137">Представляет задачу, которую необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="d3dc7-137">Represents a task to update.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d3dc7-138">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="d3dc7-138">Parent elements</span></span>

|<span data-ttu-id="d3dc7-139">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="d3dc7-139">**Element**</span></span>|<span data-ttu-id="d3dc7-140">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d3dc7-140">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d3dc7-141">Изменения (элементы)</span><span class="sxs-lookup"><span data-stu-id="d3dc7-141">Changes (Items)</span></span>](changes-items.md) <br/> |<span data-ttu-id="d3dc7-142">Содержит массив последовательности типов изменений, представляющих тип различий между элементами на клиенте и элементами на сервере Exchange.</span><span class="sxs-lookup"><span data-stu-id="d3dc7-142">Contains a sequence array of change types that represent the type of differences between the items on the client and the items on the Exchange server.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="d3dc7-143">Примечания</span><span class="sxs-lookup"><span data-stu-id="d3dc7-143">Remarks</span></span>

<span data-ttu-id="d3dc7-144">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="d3dc7-144">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d3dc7-145">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="d3dc7-145">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d3dc7-146">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="d3dc7-146">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d3dc7-147">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="d3dc7-147">Schema name</span></span>  <br/> |<span data-ttu-id="d3dc7-148">Схема Types</span><span class="sxs-lookup"><span data-stu-id="d3dc7-148">Types schema</span></span>  <br/> |
|<span data-ttu-id="d3dc7-149">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="d3dc7-149">Validation file</span></span>  <br/> |<span data-ttu-id="d3dc7-150">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="d3dc7-150">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d3dc7-151">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="d3dc7-151">Can be empty</span></span>  <br/> |<span data-ttu-id="d3dc7-152">False</span><span class="sxs-lookup"><span data-stu-id="d3dc7-152">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d3dc7-153">См. также</span><span class="sxs-lookup"><span data-stu-id="d3dc7-153">See also</span></span>

- [<span data-ttu-id="d3dc7-154">Операция SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="d3dc7-154">SyncFolderItems operation</span></span>](syncfolderitems-operation.md)
- [<span data-ttu-id="d3dc7-155">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="d3dc7-155">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

