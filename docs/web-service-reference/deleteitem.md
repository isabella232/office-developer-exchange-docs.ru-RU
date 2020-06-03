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
description: Элемент DeleteItem определяет запрос на удаление элемента из почтового ящика в хранилище Exchange.
ms.openlocfilehash: ed13ee32b487f49740aed80e8705257d3e2e6938
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529205"
---
# <a name="deleteitem"></a><span data-ttu-id="3a470-103">DeleteItem</span><span class="sxs-lookup"><span data-stu-id="3a470-103">DeleteItem</span></span>

<span data-ttu-id="3a470-104">Элемент **DeleteItem** определяет запрос на удаление элемента из почтового ящика в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="3a470-104">The **DeleteItem** element defines a request to delete an item from a mailbox in the Exchange store.</span></span> 
  
```XML
<DeleteItem DeleteType="" SendMeetingCancellations="" AffectedTaskOccurrences="" SuppressReadReceipts="">
   <ItemIds/>
</DeleteItem>
```

 <span data-ttu-id="3a470-105">**делетеитемтипе**</span><span class="sxs-lookup"><span data-stu-id="3a470-105">**DeleteItemType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3a470-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="3a470-106">Attributes and elements</span></span>

<span data-ttu-id="3a470-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="3a470-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3a470-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="3a470-108">Attributes</span></span>

|<span data-ttu-id="3a470-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="3a470-109">**Attribute**</span></span>|<span data-ttu-id="3a470-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="3a470-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="3a470-111">**делететипе**</span><span class="sxs-lookup"><span data-stu-id="3a470-111">**DeleteType**</span></span> <br/> |<span data-ttu-id="3a470-112">Описывает способ удаления элемента.</span><span class="sxs-lookup"><span data-stu-id="3a470-112">Describes how an item is deleted.</span></span> <span data-ttu-id="3a470-113">Этот атрибут является обязательным.</span><span class="sxs-lookup"><span data-stu-id="3a470-113">This attribute is required.</span></span>  <br/> |
|<span data-ttu-id="3a470-114">**сендмитингканцеллатионс**</span><span class="sxs-lookup"><span data-stu-id="3a470-114">**SendMeetingCancellations**</span></span> <br/> |<span data-ttu-id="3a470-115">Указывает, сообщается ли об удалении элемента календаря участникам.</span><span class="sxs-lookup"><span data-stu-id="3a470-115">Describes whether a calendar item deletion is communicated to attendees.</span></span> <span data-ttu-id="3a470-116">Этот атрибут необходим при удалении элементов календаря.</span><span class="sxs-lookup"><span data-stu-id="3a470-116">This attribute is required when calendar items are deleted.</span></span> <span data-ttu-id="3a470-117">Этот атрибут является необязательным при удалении элементов, не относящихся к календарю.</span><span class="sxs-lookup"><span data-stu-id="3a470-117">This attribute is optional if non-calendar items are deleted.</span></span>  <br/> |
|<span data-ttu-id="3a470-118">**аффектедтаскоккурренцес**</span><span class="sxs-lookup"><span data-stu-id="3a470-118">**AffectedTaskOccurrences**</span></span> <br/> |<span data-ttu-id="3a470-119">Указывает, удален ли экземпляр задачи или хозяин задач с помощью [операции DeleteItem](deleteitem-operation.md).</span><span class="sxs-lookup"><span data-stu-id="3a470-119">Describes whether a task instance or a task master is deleted by a [DeleteItem operation](deleteitem-operation.md).</span></span> <span data-ttu-id="3a470-120">Этот атрибут является обязательным при удалении задач.</span><span class="sxs-lookup"><span data-stu-id="3a470-120">This attribute is required when tasks are deleted.</span></span> <span data-ttu-id="3a470-121">Этот атрибут является необязательным при удалении элементов, не являющихся задачами.</span><span class="sxs-lookup"><span data-stu-id="3a470-121">This attribute is optional when non-task items are deleted.</span></span>  <br/> |
|<span data-ttu-id="3a470-122">**суппрессреадрецеиптс**</span><span class="sxs-lookup"><span data-stu-id="3a470-122">**SuppressReadReceipts**</span></span> <br/> |<span data-ttu-id="3a470-123">Указывает, подавляются ли уведомления о прочтении для удаленного элемента.</span><span class="sxs-lookup"><span data-stu-id="3a470-123">Indicates whether read receipts for the deleted item are suppressed.</span></span> <span data-ttu-id="3a470-124">Текстовое значение **true**указывает, что уведомления о прочтении подавляются.</span><span class="sxs-lookup"><span data-stu-id="3a470-124">A text value of **true**, indicates that the read receipts are suppressed.</span></span> <span data-ttu-id="3a470-125">Значение **false** указывает, что уведомления о прочтении отправляются отправителю.</span><span class="sxs-lookup"><span data-stu-id="3a470-125">A value of **false** indicates that the read receipts are sent to the sender.</span></span> <span data-ttu-id="3a470-126">Этот атрибут является необязательным.</span><span class="sxs-lookup"><span data-stu-id="3a470-126">This attribute is optional.</span></span>  <br/> |
   
#### <a name="deletetype-attribute"></a><span data-ttu-id="3a470-127">Атрибут Делететипе</span><span class="sxs-lookup"><span data-stu-id="3a470-127">DeleteType attribute</span></span>

|<span data-ttu-id="3a470-128">**Значение**</span><span class="sxs-lookup"><span data-stu-id="3a470-128">**Value**</span></span>|<span data-ttu-id="3a470-129">**Описание**</span><span class="sxs-lookup"><span data-stu-id="3a470-129">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="3a470-130">HardDelete</span><span class="sxs-lookup"><span data-stu-id="3a470-130">HardDelete</span></span>  <br/> |<span data-ttu-id="3a470-131">Элемент окончательно удаляется из хранилища.</span><span class="sxs-lookup"><span data-stu-id="3a470-131">An item is permanently removed from the store.</span></span>  <br/> |
|<span data-ttu-id="3a470-132">SoftDelete</span><span class="sxs-lookup"><span data-stu-id="3a470-132">SoftDelete</span></span>  <br/> |<span data-ttu-id="3a470-133">При включенной корзине элемент перемещается в корзину.</span><span class="sxs-lookup"><span data-stu-id="3a470-133">An item is moved to the dumpster if the dumpster is enabled.</span></span>  <br/> |
|<span data-ttu-id="3a470-134">MoveToDeletedItems</span><span class="sxs-lookup"><span data-stu-id="3a470-134">MoveToDeletedItems</span></span>  <br/> |<span data-ttu-id="3a470-135">Сообщение перемещено в папку "Удаленные".</span><span class="sxs-lookup"><span data-stu-id="3a470-135">An item is moved to the Deleted Items folder.</span></span>  <br/> |
   
#### <a name="sendmeetingcancellations-attribute"></a><span data-ttu-id="3a470-136">Атрибут Сендмитингканцеллатионс</span><span class="sxs-lookup"><span data-stu-id="3a470-136">SendMeetingCancellations attribute</span></span>

|<span data-ttu-id="3a470-137">**Значение**</span><span class="sxs-lookup"><span data-stu-id="3a470-137">**Value**</span></span>|<span data-ttu-id="3a470-138">**Описание**</span><span class="sxs-lookup"><span data-stu-id="3a470-138">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="3a470-139">сендтононе</span><span class="sxs-lookup"><span data-stu-id="3a470-139">SendToNone</span></span>  <br/> |<span data-ttu-id="3a470-140">Элемент календаря удаляется без отправки сообщения об отмене.</span><span class="sxs-lookup"><span data-stu-id="3a470-140">A calendar item is deleted without sending a cancellation message.</span></span>  <br/> |
|<span data-ttu-id="3a470-141">сендонлитоалл</span><span class="sxs-lookup"><span data-stu-id="3a470-141">SendOnlyToAll</span></span>  <br/> |<span data-ttu-id="3a470-142">Элемент календаря удален и сообщение об отмене отправляется всем участникам.</span><span class="sxs-lookup"><span data-stu-id="3a470-142">A calendar item is deleted and a cancellation message is sent to all attendees.</span></span>  <br/> |
|<span data-ttu-id="3a470-143">сендтоалландсавекопи</span><span class="sxs-lookup"><span data-stu-id="3a470-143">SendToAllAndSaveCopy</span></span>  <br/> |<span data-ttu-id="3a470-144">Элемент календаря удален и сообщение об отмене отправляется всем участникам.</span><span class="sxs-lookup"><span data-stu-id="3a470-144">A calendar item is deleted and a cancellation message is sent to all attendees.</span></span> <span data-ttu-id="3a470-145">Копия сообщения об отмене сохраняется в папке "Отправленные".</span><span class="sxs-lookup"><span data-stu-id="3a470-145">A copy of the cancellation message is saved in the Sent Items folder.</span></span>  <br/> |
   
#### <a name="affectedtaskoccurrences-attribute"></a><span data-ttu-id="3a470-146">Атрибут Аффектедтаскоккурренцес</span><span class="sxs-lookup"><span data-stu-id="3a470-146">AffectedTaskOccurrences attribute</span></span>

|<span data-ttu-id="3a470-147">**Значение**</span><span class="sxs-lookup"><span data-stu-id="3a470-147">**Value**</span></span>|<span data-ttu-id="3a470-148">**Описание**</span><span class="sxs-lookup"><span data-stu-id="3a470-148">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="3a470-149">аллоккурренцес</span><span class="sxs-lookup"><span data-stu-id="3a470-149">AllOccurrences</span></span>  <br/> |<span data-ttu-id="3a470-150">Запрос на удаление элемента удаляет главную задачу и поэтому все повторяющиеся задачи, связанные с главной задачей.</span><span class="sxs-lookup"><span data-stu-id="3a470-150">A delete item request deletes the master task, and therefore all recurring tasks that are associated with the master task.</span></span>  <br/> |
|<span data-ttu-id="3a470-151">спеЦифиедоккурренцеонли</span><span class="sxs-lookup"><span data-stu-id="3a470-151">SpecifiedOccurrenceOnly</span></span>  <br/> |<span data-ttu-id="3a470-152">Запрос на удаление элемента удаляет только определенные экземпляры задачи.</span><span class="sxs-lookup"><span data-stu-id="3a470-152">A delete item request deletes only specific occurrences of a task.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="3a470-153">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="3a470-153">Child elements</span></span>

|<span data-ttu-id="3a470-154">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="3a470-154">**Element**</span></span>|<span data-ttu-id="3a470-155">**Описание**</span><span class="sxs-lookup"><span data-stu-id="3a470-155">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3a470-156">итемидс</span><span class="sxs-lookup"><span data-stu-id="3a470-156">ItemIds</span></span>](itemids.md) <br/> |<span data-ttu-id="3a470-157">Содержит массив элементов, элементов вхождений и повторяющихся элементов шаблона, которые необходимо удалить из почтового ящика в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="3a470-157">Contains an array of items, occurrence items, and recurring master items to delete from a mailbox in the Exchange store.</span></span> <span data-ttu-id="3a470-158">[Операцию DeleteItem](deleteitem-operation.md) можно выполнить для любого типа элемента.</span><span class="sxs-lookup"><span data-stu-id="3a470-158">The [DeleteItem operation](deleteitem-operation.md) can be performed on any item type.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="3a470-159">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="3a470-159">Parent elements</span></span>

<span data-ttu-id="3a470-160">Нет.</span><span class="sxs-lookup"><span data-stu-id="3a470-160">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="3a470-161">Примечания</span><span class="sxs-lookup"><span data-stu-id="3a470-161">Remarks</span></span>

<span data-ttu-id="3a470-162">Параметры **MoveToDeletedItems** и **HardDelete** являются транзакционными, что означает, что по завершении вызова веб-службы база данных переместит элемент в папку "Удаленные" или окончательно удалил его из базы данных Exchange.</span><span class="sxs-lookup"><span data-stu-id="3a470-162">The **MoveToDeletedItems** and **HardDelete** options are transactional, which means that by the time a Web service call completes, the database has moved the item to the Deleted Items folder or permanently removed the item from the Exchange database.</span></span> <span data-ttu-id="3a470-163">Это одно и то же поведение для Майкрософт Exchange Server 2007 и Exchange Server 2010.</span><span class="sxs-lookup"><span data-stu-id="3a470-163">This behavior is the same for MicrosoftExchange Server 2007 and Exchange Server 2010.</span></span> 
  
<span data-ttu-id="3a470-164">Параметр **SoftDelete** работает по-разному для разных целевых версий Exchange.</span><span class="sxs-lookup"><span data-stu-id="3a470-164">The **SoftDelete** option works differently for different target versions of Exchange.</span></span> <span data-ttu-id="3a470-165">**SoftDelete** для Exchange 2007 устанавливает бит для элемента, указывающего на базу данных Exchange, в которую элемент будет перемещен в папку корзины одновременно в будущем.</span><span class="sxs-lookup"><span data-stu-id="3a470-165">**SoftDelete** for Exchange 2007 sets a bit on the item that indicates to the Exchange database that the item will be moved to the dumpster folder at an indeterminate time in the future.</span></span> <span data-ttu-id="3a470-166">**SoftDelete** для Exchange 2010 немедленно перемещает элемент в корзину.</span><span class="sxs-lookup"><span data-stu-id="3a470-166">**SoftDelete** for Exchange 2010 immediately moves the item to the dumpster.</span></span> <span data-ttu-id="3a470-167">**SoftDelete** не является возможностью удаления папок.</span><span class="sxs-lookup"><span data-stu-id="3a470-167">**SoftDelete** is not an option for folder deletion.</span></span> <span data-ttu-id="3a470-168">Поиск по элементам и папкам **SoftDelete** не возвратит результаты.</span><span class="sxs-lookup"><span data-stu-id="3a470-168">**SoftDelete** traversal searches for items and folders will not return any results.</span></span> 
  
<span data-ttu-id="3a470-169">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="3a470-169">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3a470-170">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="3a470-170">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3a470-171">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="3a470-171">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="3a470-172">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="3a470-172">Schema Name</span></span>  <br/> |<span data-ttu-id="3a470-173">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="3a470-173">Messages schema</span></span>  <br/> |
|<span data-ttu-id="3a470-174">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="3a470-174">Validation File</span></span>  <br/> |<span data-ttu-id="3a470-175">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="3a470-175">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="3a470-176">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="3a470-176">Can be Empty</span></span>  <br/> |<span data-ttu-id="3a470-177">False</span><span class="sxs-lookup"><span data-stu-id="3a470-177">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3a470-178">См. также</span><span class="sxs-lookup"><span data-stu-id="3a470-178">See also</span></span>

- [<span data-ttu-id="3a470-179">делетеитемреспонсе</span><span class="sxs-lookup"><span data-stu-id="3a470-179">DeleteItemResponse</span></span>](deleteitemresponse.md)  
- [<span data-ttu-id="3a470-180">Операция DeleteItem</span><span class="sxs-lookup"><span data-stu-id="3a470-180">DeleteItem operation</span></span>](deleteitem-operation.md)

