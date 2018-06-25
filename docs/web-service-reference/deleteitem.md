---
title: DeleteItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DeleteItem
api_type:
- schema
ms.assetid: 055cdee8-3c7d-47db-9f27-740f4a674729
description: Элемент DeleteItem определяет запрос для удаления элемента из почтового ящика в хранилище Exchange.
ms.openlocfilehash: de64787750c88c8a47bb69daddc0a1d2ebe8bde9
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762048"
---
# <a name="deleteitem"></a><span data-ttu-id="d382b-103">DeleteItem</span><span class="sxs-lookup"><span data-stu-id="d382b-103">DeleteItem</span></span>

<span data-ttu-id="d382b-104">Элемент **DeleteItem** определяет запрос для удаления элемента из почтового ящика в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="d382b-104">The **DeleteItem** element defines a request to delete an item from a mailbox in the Exchange store.</span></span> 
  
```XML
<DeleteItem DeleteType="" SendMeetingCancellations="" AffectedTaskOccurrences="" SuppressReadReceipts="">
   <ItemIds/>
</DeleteItem>
```

 <span data-ttu-id="d382b-105">**DeleteItemType**</span><span class="sxs-lookup"><span data-stu-id="d382b-105">**DeleteItemType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d382b-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="d382b-106">Attributes and elements</span></span>

<span data-ttu-id="d382b-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="d382b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d382b-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="d382b-108">Attributes</span></span>

|<span data-ttu-id="d382b-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="d382b-109">**Attribute**</span></span>|<span data-ttu-id="d382b-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d382b-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="d382b-111">**DeleteType**</span><span class="sxs-lookup"><span data-stu-id="d382b-111">**DeleteType**</span></span> <br/> |<span data-ttu-id="d382b-112">Описывает, как удалить элемент.</span><span class="sxs-lookup"><span data-stu-id="d382b-112">Describes how an item is deleted.</span></span> <span data-ttu-id="d382b-113">Этот атрибут является обязательным.</span><span class="sxs-lookup"><span data-stu-id="d382b-113">This attribute is required.</span></span>  <br/> |
|<span data-ttu-id="d382b-114">**SendMeetingCancellations**</span><span class="sxs-lookup"><span data-stu-id="d382b-114">**SendMeetingCancellations**</span></span> <br/> |<span data-ttu-id="d382b-115">Описание, передается ли участникам удаления элемента календаря.</span><span class="sxs-lookup"><span data-stu-id="d382b-115">Describes whether a calendar item deletion is communicated to attendees.</span></span> <span data-ttu-id="d382b-116">Этот атрибут является обязательным, при удалении элементов календаря.</span><span class="sxs-lookup"><span data-stu-id="d382b-116">This attribute is required when calendar items are deleted.</span></span> <span data-ttu-id="d382b-117">Этот атрибут является необязательным, если удалить некалендарные элементы.</span><span class="sxs-lookup"><span data-stu-id="d382b-117">This attribute is optional if non-calendar items are deleted.</span></span>  <br/> |
|<span data-ttu-id="d382b-118">**AffectedTaskOccurrences**</span><span class="sxs-lookup"><span data-stu-id="d382b-118">**AffectedTaskOccurrences**</span></span> <br/> |<span data-ttu-id="d382b-119">Описывает удалит ли [операция DeleteItem](deleteitem-operation.md)экземпляра задачи или шаблон задач.</span><span class="sxs-lookup"><span data-stu-id="d382b-119">Describes whether a task instance or a task master is deleted by a [DeleteItem operation](deleteitem-operation.md).</span></span> <span data-ttu-id="d382b-120">Этот атрибут является обязательным, при удалении задачи.</span><span class="sxs-lookup"><span data-stu-id="d382b-120">This attribute is required when tasks are deleted.</span></span> <span data-ttu-id="d382b-121">Этот атрибут является необязательным при удалении элементов не задач.</span><span class="sxs-lookup"><span data-stu-id="d382b-121">This attribute is optional when non-task items are deleted.</span></span>  <br/> |
|<span data-ttu-id="d382b-122">**SuppressReadReceipts**</span><span class="sxs-lookup"><span data-stu-id="d382b-122">**SuppressReadReceipts**</span></span> <br/> |<span data-ttu-id="d382b-123">Указывает, подавляются ли прочтении для удаленных элементов.</span><span class="sxs-lookup"><span data-stu-id="d382b-123">Indicates whether read receipts for the deleted item are suppressed.</span></span> <span data-ttu-id="d382b-124">Текстовое значение **true**, указывает, что прочтении подавляются.</span><span class="sxs-lookup"><span data-stu-id="d382b-124">A text value of **true**, indicates that the read receipts are suppressed.</span></span> <span data-ttu-id="d382b-125">Значение **false** указывает, что прочтении отправляются отправителю.</span><span class="sxs-lookup"><span data-stu-id="d382b-125">A value of **false** indicates that the read receipts are sent to the sender.</span></span> <span data-ttu-id="d382b-126">Этот атрибут является необязательным.</span><span class="sxs-lookup"><span data-stu-id="d382b-126">This attribute is optional.</span></span>  <br/> |
   
#### <a name="deletetype-attribute"></a><span data-ttu-id="d382b-127">Атрибут DeleteType</span><span class="sxs-lookup"><span data-stu-id="d382b-127">DeleteType attribute</span></span>

|<span data-ttu-id="d382b-128">**Значение**</span><span class="sxs-lookup"><span data-stu-id="d382b-128">**Value**</span></span>|<span data-ttu-id="d382b-129">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d382b-129">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="d382b-130">HardDelete</span><span class="sxs-lookup"><span data-stu-id="d382b-130">HardDelete</span></span>  <br/> |<span data-ttu-id="d382b-131">Элемент окончательно удалить из хранилища.</span><span class="sxs-lookup"><span data-stu-id="d382b-131">An item is permanently removed from the store.</span></span>  <br/> |
|<span data-ttu-id="d382b-132">SoftDelete</span><span class="sxs-lookup"><span data-stu-id="d382b-132">SoftDelete</span></span>  <br/> |<span data-ttu-id="d382b-133">Перемещено в корзину Если корзина включена.</span><span class="sxs-lookup"><span data-stu-id="d382b-133">An item is moved to the dumpster if the dumpster is enabled.</span></span>  <br/> |
|<span data-ttu-id="d382b-134">MoveToDeletedItems</span><span class="sxs-lookup"><span data-stu-id="d382b-134">MoveToDeletedItems</span></span>  <br/> |<span data-ttu-id="d382b-135">Сообщение перемещено в папку «Удаленные».</span><span class="sxs-lookup"><span data-stu-id="d382b-135">An item is moved to the Deleted Items folder.</span></span>  <br/> |
   
#### <a name="sendmeetingcancellations-attribute"></a><span data-ttu-id="d382b-136">Атрибут SendMeetingCancellations</span><span class="sxs-lookup"><span data-stu-id="d382b-136">SendMeetingCancellations attribute</span></span>

|<span data-ttu-id="d382b-137">**Значение**</span><span class="sxs-lookup"><span data-stu-id="d382b-137">**Value**</span></span>|<span data-ttu-id="d382b-138">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d382b-138">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="d382b-139">SendToNone</span><span class="sxs-lookup"><span data-stu-id="d382b-139">SendToNone</span></span>  <br/> |<span data-ttu-id="d382b-140">Элемент календаря удаляется без отправки сообщения об отмене.</span><span class="sxs-lookup"><span data-stu-id="d382b-140">A calendar item is deleted without sending a cancellation message.</span></span>  <br/> |
|<span data-ttu-id="d382b-141">SendOnlyToAll</span><span class="sxs-lookup"><span data-stu-id="d382b-141">SendOnlyToAll</span></span>  <br/> |<span data-ttu-id="d382b-142">Удаленного элемента календаря и отмены сообщение отправляется всем участникам.</span><span class="sxs-lookup"><span data-stu-id="d382b-142">A calendar item is deleted and a cancellation message is sent to all attendees.</span></span>  <br/> |
|<span data-ttu-id="d382b-143">SendToAllAndSaveCopy</span><span class="sxs-lookup"><span data-stu-id="d382b-143">SendToAllAndSaveCopy</span></span>  <br/> |<span data-ttu-id="d382b-144">Удаленного элемента календаря и отмены сообщение отправляется всем участникам.</span><span class="sxs-lookup"><span data-stu-id="d382b-144">A calendar item is deleted and a cancellation message is sent to all attendees.</span></span> <span data-ttu-id="d382b-145">Копия сообщения отмены сохраняется в папке «Отправленные».</span><span class="sxs-lookup"><span data-stu-id="d382b-145">A copy of the cancellation message is saved in the Sent Items folder.</span></span>  <br/> |
   
#### <a name="affectedtaskoccurrences-attribute"></a><span data-ttu-id="d382b-146">Атрибут AffectedTaskOccurrences</span><span class="sxs-lookup"><span data-stu-id="d382b-146">AffectedTaskOccurrences attribute</span></span>

|<span data-ttu-id="d382b-147">**Значение**</span><span class="sxs-lookup"><span data-stu-id="d382b-147">**Value**</span></span>|<span data-ttu-id="d382b-148">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d382b-148">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="d382b-149">AllOccurrences</span><span class="sxs-lookup"><span data-stu-id="d382b-149">AllOccurrences</span></span>  <br/> |<span data-ttu-id="d382b-150">Запрос delete элемента удаляет главных задач и поэтому все повторяющиеся задачи, которые связаны с главной задачи.</span><span class="sxs-lookup"><span data-stu-id="d382b-150">A delete item request deletes the master task, and therefore all recurring tasks that are associated with the master task.</span></span>  <br/> |
|<span data-ttu-id="d382b-151">SpecifiedOccurrenceOnly</span><span class="sxs-lookup"><span data-stu-id="d382b-151">SpecifiedOccurrenceOnly</span></span>  <br/> |<span data-ttu-id="d382b-152">Запрос delete элемента удаляет конкретных вхождений задачи.</span><span class="sxs-lookup"><span data-stu-id="d382b-152">A delete item request deletes only specific occurrences of a task.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="d382b-153">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="d382b-153">Child elements</span></span>

|<span data-ttu-id="d382b-154">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="d382b-154">**Element**</span></span>|<span data-ttu-id="d382b-155">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d382b-155">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d382b-156">Что ItemID</span><span class="sxs-lookup"><span data-stu-id="d382b-156">ItemIds</span></span>](itemids.md) <br/> |<span data-ttu-id="d382b-157">Содержит массив элементов, элементы вхождений и повторяющиеся основные элементы для удаления из почтового ящика в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="d382b-157">Contains an array of items, occurrence items, and recurring master items to delete from a mailbox in the Exchange store.</span></span> <span data-ttu-id="d382b-158">[DeleteItem операции](deleteitem-operation.md) можно выполнить на любой тип элемента.</span><span class="sxs-lookup"><span data-stu-id="d382b-158">The [DeleteItem operation](deleteitem-operation.md) can be performed on any item type.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d382b-159">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="d382b-159">Parent elements</span></span>

<span data-ttu-id="d382b-160">Нет.</span><span class="sxs-lookup"><span data-stu-id="d382b-160">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="d382b-161">Замечания</span><span class="sxs-lookup"><span data-stu-id="d382b-161">Remarks</span></span>

<span data-ttu-id="d382b-162">Параметры **MoveToDeletedItems** и **HardDelete** являются транзакций, это означает, что с на время завершения вызова веб-службы, базы данных переместить элемент папки «Удаленные» или окончательно удалить элемент из базы данных Exchange.</span><span class="sxs-lookup"><span data-stu-id="d382b-162">The **MoveToDeletedItems** and **HardDelete** options are transactional, which means that by the time a Web service call completes, the database has moved the item to the Deleted Items folder or permanently removed the item from the Exchange database.</span></span> <span data-ttu-id="d382b-163">Это поведение не зависит от MicrosoftExchange Server 2007 и Exchange Server 2010.</span><span class="sxs-lookup"><span data-stu-id="d382b-163">This behavior is the same for MicrosoftExchange Server 2007 and Exchange Server 2010.</span></span> 
  
<span data-ttu-id="d382b-164">Параметр **SoftDelete** работает по-разному для различных целевых версий Exchange.</span><span class="sxs-lookup"><span data-stu-id="d382b-164">The **SoftDelete** option works differently for different target versions of Exchange.</span></span> <span data-ttu-id="d382b-165">**SoftDelete** для Exchange Server 2007 немного задает для элемента, которое указывает, к базе данных Exchange, элемент перемещается в корзину папки в неопределенное время в будущем.</span><span class="sxs-lookup"><span data-stu-id="d382b-165">**SoftDelete** for Exchange 2007 sets a bit on the item that indicates to the Exchange database that the item will be moved to the dumpster folder at an indeterminate time in the future.</span></span> <span data-ttu-id="d382b-166">**SoftDelete** для Exchange 2010 задает немедленное перемещение элемента в корзину.</span><span class="sxs-lookup"><span data-stu-id="d382b-166">**SoftDelete** for Exchange 2010 immediately moves the item to the dumpster.</span></span> <span data-ttu-id="d382b-167">**SoftDelete** недоступно для удаления папки.</span><span class="sxs-lookup"><span data-stu-id="d382b-167">**SoftDelete** is not an option for folder deletion.</span></span> <span data-ttu-id="d382b-168">Выполняет обход **SoftDelete** элементов и папок не возвращает результатов.</span><span class="sxs-lookup"><span data-stu-id="d382b-168">**SoftDelete** traversal searches for items and folders will not return any results.</span></span> 
  
<span data-ttu-id="d382b-169">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="d382b-169">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d382b-170">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="d382b-170">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d382b-171">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="d382b-171">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="d382b-172">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="d382b-172">Schema Name</span></span>  <br/> |<span data-ttu-id="d382b-173">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="d382b-173">Messages schema</span></span>  <br/> |
|<span data-ttu-id="d382b-174">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="d382b-174">Validation File</span></span>  <br/> |<span data-ttu-id="d382b-175">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="d382b-175">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="d382b-176">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="d382b-176">Can be Empty</span></span>  <br/> |<span data-ttu-id="d382b-177">False</span><span class="sxs-lookup"><span data-stu-id="d382b-177">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d382b-178">См. также</span><span class="sxs-lookup"><span data-stu-id="d382b-178">See also</span></span>

- [<span data-ttu-id="d382b-179">DeleteItemResponse</span><span class="sxs-lookup"><span data-stu-id="d382b-179">DeleteItemResponse</span></span>](deleteitemresponse.md)  
- [<span data-ttu-id="d382b-180">Операция DeleteItem</span><span class="sxs-lookup"><span data-stu-id="d382b-180">DeleteItem operation</span></span>](deleteitem-operation.md)

