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
ms.openlocfilehash: bf560f18184151a3f17d7016d05cdb725db934ae
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/28/2018
ms.locfileid: "21353632"
---
# <a name="update-itemsync"></a><span data-ttu-id="f5c4c-103">Обновление (Итемсинк)</span><span class="sxs-lookup"><span data-stu-id="f5c4c-103">Update (ItemSync)</span></span>

<span data-ttu-id="f5c4c-104">Элемент **Update** определяет один элемент для обновления в локальном хранилище клиента.</span><span class="sxs-lookup"><span data-stu-id="f5c4c-104">The **Update** element identifies a single item to update in the local client store.</span></span> 
  
- [<span data-ttu-id="f5c4c-105">синкфолдеритемсреспонсе</span><span class="sxs-lookup"><span data-stu-id="f5c4c-105">SyncFolderItemsResponse</span></span>](syncfolderitemsresponse.md) 
- [<span data-ttu-id="f5c4c-106">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="f5c4c-106">ResponseMessages</span></span>](responsemessages.md)  
- [<span data-ttu-id="f5c4c-107">синкфолдеритемсреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="f5c4c-107">SyncFolderItemsResponseMessage</span></span>](syncfolderitemsresponsemessage.md)  
- [<span data-ttu-id="f5c4c-108">Изменения (элементы)</span><span class="sxs-lookup"><span data-stu-id="f5c4c-108">Changes (Items)</span></span>](changes-items.md)  
- [<span data-ttu-id="f5c4c-109">Обновление (Итемсинк)</span><span class="sxs-lookup"><span data-stu-id="f5c4c-109">Update (ItemSync)</span></span>](update-itemsync.md)
  
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

<span data-ttu-id="f5c4c-110">**синкфолдеритемскреатеорупдатетипе**</span><span class="sxs-lookup"><span data-stu-id="f5c4c-110">**SyncFolderItemsCreateOrUpdateType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="f5c4c-111">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="f5c4c-111">Attributes and elements</span></span>

<span data-ttu-id="f5c4c-112">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="f5c4c-112">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f5c4c-113">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="f5c4c-113">Attributes</span></span>

<span data-ttu-id="f5c4c-114">Нет.</span><span class="sxs-lookup"><span data-stu-id="f5c4c-114">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f5c4c-115">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="f5c4c-115">Child elements</span></span>

|<span data-ttu-id="f5c4c-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="f5c4c-116">**Element**</span></span>|<span data-ttu-id="f5c4c-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="f5c4c-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f5c4c-118">Элемент</span><span class="sxs-lookup"><span data-stu-id="f5c4c-118">Item</span></span>](item.md) <br/> |<span data-ttu-id="f5c4c-119">Представляет универсальный элемент Exchange, который необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="f5c4c-119">Represents a generic Exchange item to update.</span></span>  <br/> |
|[<span data-ttu-id="f5c4c-120">Сообщение</span><span class="sxs-lookup"><span data-stu-id="f5c4c-120">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="f5c4c-121">Представляет сообщение электронной почты Exchange, которое требуется обновить.</span><span class="sxs-lookup"><span data-stu-id="f5c4c-121">Represents an Exchange e-mail message to update.</span></span>  <br/> |
|[<span data-ttu-id="f5c4c-122">календаритем</span><span class="sxs-lookup"><span data-stu-id="f5c4c-122">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="f5c4c-123">Представляет элемент календаря Exchange, который необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="f5c4c-123">Represents an Exchange calendar item to update.</span></span>  <br/> |
|<span data-ttu-id="f5c4c-124">[контакт](contact.md);</span><span class="sxs-lookup"><span data-stu-id="f5c4c-124">[Contact](contact.md)</span></span> <br/> |<span data-ttu-id="f5c4c-125">Представляет элемент контакта Exchange, который необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="f5c4c-125">Represents an Exchange contact item to update.</span></span>  <br/> |
|[<span data-ttu-id="f5c4c-126">дистрибутионлист</span><span class="sxs-lookup"><span data-stu-id="f5c4c-126">DistributionList</span></span>](distributionlist.md) <br/> |<span data-ttu-id="f5c4c-127">Представляет список рассылки, который необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="f5c4c-127">Represents a distribution list to update.</span></span>  <br/> |
|[<span data-ttu-id="f5c4c-128">митингмессаже</span><span class="sxs-lookup"><span data-stu-id="f5c4c-128">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="f5c4c-129">Представляет сообщение о собрании, которое необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="f5c4c-129">Represents a meeting message to update.</span></span>  <br/> |
|[<span data-ttu-id="f5c4c-130">Свойство meetingrequest</span><span class="sxs-lookup"><span data-stu-id="f5c4c-130">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="f5c4c-131">Представляет приглашение на собрание, которое требуется обновить.</span><span class="sxs-lookup"><span data-stu-id="f5c4c-131">Represents a meeting request to update.</span></span>  <br/> |
|[<span data-ttu-id="f5c4c-132">митингреспонсе</span><span class="sxs-lookup"><span data-stu-id="f5c4c-132">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="f5c4c-133">Представляет ответ на приглашение на собрание, который необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="f5c4c-133">Represents a meeting response to update.</span></span>  <br/> |
|[<span data-ttu-id="f5c4c-134">митингканцеллатион</span><span class="sxs-lookup"><span data-stu-id="f5c4c-134">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="f5c4c-135">Представляет отмену собрания, которое необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="f5c4c-135">Represents a meeting cancellation to update.</span></span>  <br/> |
|[<span data-ttu-id="f5c4c-136">Task</span><span class="sxs-lookup"><span data-stu-id="f5c4c-136">Task</span></span>](task.md) <br/> |<span data-ttu-id="f5c4c-137">Представляет задачу, которую необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="f5c4c-137">Represents a task to update.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f5c4c-138">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="f5c4c-138">Parent elements</span></span>

|<span data-ttu-id="f5c4c-139">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="f5c4c-139">**Element**</span></span>|<span data-ttu-id="f5c4c-140">**Описание**</span><span class="sxs-lookup"><span data-stu-id="f5c4c-140">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f5c4c-141">Изменения (элементы)</span><span class="sxs-lookup"><span data-stu-id="f5c4c-141">Changes (Items)</span></span>](changes-items.md) <br/> |<span data-ttu-id="f5c4c-142">Содержит массив последовательности типов изменений, представляющих тип различий между элементами на клиенте и элементами на сервере Exchange.</span><span class="sxs-lookup"><span data-stu-id="f5c4c-142">Contains a sequence array of change types that represent the type of differences between the items on the client and the items on the Exchange server.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="f5c4c-143">Примечания</span><span class="sxs-lookup"><span data-stu-id="f5c4c-143">Remarks</span></span>

<span data-ttu-id="f5c4c-144">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="f5c4c-144">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f5c4c-145">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="f5c4c-145">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f5c4c-146">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="f5c4c-146">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f5c4c-147">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="f5c4c-147">Schema name</span></span>  <br/> |<span data-ttu-id="f5c4c-148">Схема Types</span><span class="sxs-lookup"><span data-stu-id="f5c4c-148">Types schema</span></span>  <br/> |
|<span data-ttu-id="f5c4c-149">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="f5c4c-149">Validation file</span></span>  <br/> |<span data-ttu-id="f5c4c-150">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="f5c4c-150">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="f5c4c-151">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="f5c4c-151">Can be empty</span></span>  <br/> |<span data-ttu-id="f5c4c-152">False</span><span class="sxs-lookup"><span data-stu-id="f5c4c-152">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f5c4c-153">См. также</span><span class="sxs-lookup"><span data-stu-id="f5c4c-153">See also</span></span>

- [<span data-ttu-id="f5c4c-154">Операция SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="f5c4c-154">SyncFolderItems operation</span></span>](syncfolderitems-operation.md)
- [<span data-ttu-id="f5c4c-155">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="f5c4c-155">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

