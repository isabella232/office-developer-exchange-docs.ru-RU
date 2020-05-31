---
title: Create (Итемсинк)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Create
api_type:
- schema
ms.assetid: cb5e64a2-66a5-4447-921e-7c13efb8f6bf
description: Элемент create определяет отдельный элемент для создания в локальном хранилище клиента.
ms.openlocfilehash: d49e54c64f7bd53dcb296d998a856c20570d81be
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/28/2018
ms.locfileid: "21353947"
---
# <a name="create-itemsync"></a><span data-ttu-id="7494d-103">Create (Итемсинк)</span><span class="sxs-lookup"><span data-stu-id="7494d-103">Create (ItemSync)</span></span>

<span data-ttu-id="7494d-104">Элемент **CREATE** определяет отдельный элемент для создания в локальном хранилище клиента.</span><span class="sxs-lookup"><span data-stu-id="7494d-104">The **Create** element identifies a single item to create in the local client store.</span></span> 
  
- [<span data-ttu-id="7494d-105">синкфолдеритемсреспонсе</span><span class="sxs-lookup"><span data-stu-id="7494d-105">SyncFolderItemsResponse</span></span>](syncfolderitemsresponse.md) 
- [<span data-ttu-id="7494d-106">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="7494d-106">ResponseMessages</span></span>](responsemessages.md) 
- [<span data-ttu-id="7494d-107">синкфолдеритемсреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="7494d-107">SyncFolderItemsResponseMessage</span></span>](syncfolderitemsresponsemessage.md) 
- [<span data-ttu-id="7494d-108">Изменения (элементы)</span><span class="sxs-lookup"><span data-stu-id="7494d-108">Changes (Items)</span></span>](changes-items.md) 
- [<span data-ttu-id="7494d-109">Create (Итемсинк)</span><span class="sxs-lookup"><span data-stu-id="7494d-109">Create (ItemSync)</span></span>](create-itemsync.md)
  
```xml
<Create>
   <Item/>
</Create>
```

```xml
<Create>
   <Task/> 
</Create>
```

```xml
<Create>
   <MeetingResponse/>
</Create>
```

```xml
<Create>
   <CalendarItem/>
</Create>
```

```xml
<Create>
   <MeetingMessage/>
</Create>
```

```xml
<Create>
   <DistributionList/>
</Create>
```

```xml
<Create>
   <MeetingCancellation/>
</Create>
```

```xml
<Create>
   <MeetingRequest/> 
</Create>
```

```xml
<Create>
   <Message/> 
</Create>
```

```xml
<Create>
   <Contact/> 
</Create>
```

<span data-ttu-id="7494d-110">**синкфолдеритемскреатеорупдатетипе**</span><span class="sxs-lookup"><span data-stu-id="7494d-110">**SyncFolderItemsCreateOrUpdateType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="7494d-111">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="7494d-111">Attributes and elements</span></span>

<span data-ttu-id="7494d-112">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="7494d-112">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7494d-113">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="7494d-113">Attributes</span></span>

<span data-ttu-id="7494d-114">Нет.</span><span class="sxs-lookup"><span data-stu-id="7494d-114">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7494d-115">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="7494d-115">Child elements</span></span>

|<span data-ttu-id="7494d-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="7494d-116">**Element**</span></span>|<span data-ttu-id="7494d-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="7494d-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7494d-118">Элемент</span><span class="sxs-lookup"><span data-stu-id="7494d-118">Item</span></span>](item.md) <br/> |<span data-ttu-id="7494d-119">Представляет общий элемент Exchange для создания.</span><span class="sxs-lookup"><span data-stu-id="7494d-119">Represents a generic Exchange item to create.</span></span>  <br/> |
|[<span data-ttu-id="7494d-120">Сообщение</span><span class="sxs-lookup"><span data-stu-id="7494d-120">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="7494d-121">Представляет создаваемое сообщение электронной почты Exchange.</span><span class="sxs-lookup"><span data-stu-id="7494d-121">Represents an Exchange e-mail message to create.</span></span>  <br/> |
|[<span data-ttu-id="7494d-122">календаритем</span><span class="sxs-lookup"><span data-stu-id="7494d-122">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="7494d-123">Представляет элемент календаря Exchange, который необходимо создать.</span><span class="sxs-lookup"><span data-stu-id="7494d-123">Represents an Exchange calendar item to create.</span></span>  <br/> |
|<span data-ttu-id="7494d-124">[контакт](contact.md);</span><span class="sxs-lookup"><span data-stu-id="7494d-124">[Contact](contact.md)</span></span> <br/> |<span data-ttu-id="7494d-125">Представляет элемент контакта Exchange, который необходимо создать.</span><span class="sxs-lookup"><span data-stu-id="7494d-125">Represents an Exchange contact item to create.</span></span>  <br/> |
|[<span data-ttu-id="7494d-126">дистрибутионлист</span><span class="sxs-lookup"><span data-stu-id="7494d-126">DistributionList</span></span>](distributionlist.md) <br/> |<span data-ttu-id="7494d-127">Представляет создаваемый список рассылки.</span><span class="sxs-lookup"><span data-stu-id="7494d-127">Represents a distribution list to create.</span></span>  <br/> |
|[<span data-ttu-id="7494d-128">митингмессаже</span><span class="sxs-lookup"><span data-stu-id="7494d-128">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="7494d-129">Представляет создаваемое сообщение о собрании.</span><span class="sxs-lookup"><span data-stu-id="7494d-129">Represents a meeting message to create.</span></span>  <br/> |
|[<span data-ttu-id="7494d-130">Свойство meetingrequest</span><span class="sxs-lookup"><span data-stu-id="7494d-130">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="7494d-131">Представляет приглашение на собрание, которое требуется создать.</span><span class="sxs-lookup"><span data-stu-id="7494d-131">Represents a meeting request to create.</span></span>  <br/> |
|[<span data-ttu-id="7494d-132">митингреспонсе</span><span class="sxs-lookup"><span data-stu-id="7494d-132">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="7494d-133">Представляет ответ на приглашение на собрание, который требуется создать.</span><span class="sxs-lookup"><span data-stu-id="7494d-133">Represents a meeting response to create.</span></span>  <br/> |
|[<span data-ttu-id="7494d-134">митингканцеллатион</span><span class="sxs-lookup"><span data-stu-id="7494d-134">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="7494d-135">Представляет отмену собрания, которое необходимо создать.</span><span class="sxs-lookup"><span data-stu-id="7494d-135">Represents a meeting cancellation to create.</span></span>  <br/> |
|[<span data-ttu-id="7494d-136">Task</span><span class="sxs-lookup"><span data-stu-id="7494d-136">Task</span></span>](task.md) <br/> |<span data-ttu-id="7494d-137">Представляет задачу, которую необходимо создать.</span><span class="sxs-lookup"><span data-stu-id="7494d-137">Represents a task to create.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="7494d-138">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="7494d-138">Parent elements</span></span>

|<span data-ttu-id="7494d-139">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="7494d-139">**Element**</span></span>|<span data-ttu-id="7494d-140">**Описание**</span><span class="sxs-lookup"><span data-stu-id="7494d-140">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7494d-141">Изменения (элементы)</span><span class="sxs-lookup"><span data-stu-id="7494d-141">Changes (Items)</span></span>](changes-items.md) <br/> |<span data-ttu-id="7494d-142">Содержит массив последовательности типов изменений, которые представляют типы различий между элементами на клиенте и элементами на сервере Exchange.</span><span class="sxs-lookup"><span data-stu-id="7494d-142">Contains a sequence array of change types that represent the types of differences between the items on the client and the items on the Exchange server.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="7494d-143">Примечания</span><span class="sxs-lookup"><span data-stu-id="7494d-143">Remarks</span></span>

<span data-ttu-id="7494d-144">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="7494d-144">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7494d-145">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="7494d-145">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7494d-146">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="7494d-146">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="7494d-147">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="7494d-147">Schema name</span></span>  <br/> |<span data-ttu-id="7494d-148">Схема Types</span><span class="sxs-lookup"><span data-stu-id="7494d-148">Types schema</span></span>  <br/> |
|<span data-ttu-id="7494d-149">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="7494d-149">Validation file</span></span>  <br/> |<span data-ttu-id="7494d-150">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="7494d-150">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="7494d-151">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="7494d-151">Can be empty</span></span>  <br/> |<span data-ttu-id="7494d-152">False</span><span class="sxs-lookup"><span data-stu-id="7494d-152">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7494d-153">См. также</span><span class="sxs-lookup"><span data-stu-id="7494d-153">See also</span></span>

- [<span data-ttu-id="7494d-154">Операция SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="7494d-154">SyncFolderItems operation</span></span>](syncfolderitems-operation.md)
- [<span data-ttu-id="7494d-155">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="7494d-155">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

