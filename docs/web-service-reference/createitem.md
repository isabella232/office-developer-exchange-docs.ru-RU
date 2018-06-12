---
title: CreateItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CreateItem
api_type:
- schema
ms.assetid: c3707feb-3fd4-4b8a-a68f-2abadd455163
description: Элемент CreateItem определяет запрос для создания элемента в хранилище Exchange.
ms.openlocfilehash: bb5cddd5ea4fa1b73c424275a0b0219ce3e189e3
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761898"
---
# <a name="createitem"></a><span data-ttu-id="020c3-103">CreateItem</span><span class="sxs-lookup"><span data-stu-id="020c3-103">CreateItem</span></span>

<span data-ttu-id="020c3-104">Элемент **CreateItem** определяет запрос для создания элемента в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="020c3-104">The **CreateItem** element defines a request to create an item in the Exchange store.</span></span> 
  
```xml
<CreateItem MessageDisposition="" SendMeetingInvitations="">
   <SavedItemFolderId/>
   <Items/>
</CreateItem>
```

 <span data-ttu-id="020c3-105">**CreateItemType**</span><span class="sxs-lookup"><span data-stu-id="020c3-105">**CreateItemType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="020c3-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="020c3-106">Attributes and elements</span></span>

<span data-ttu-id="020c3-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="020c3-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="020c3-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="020c3-108">Attributes</span></span>

|<span data-ttu-id="020c3-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="020c3-109">**Attribute**</span></span>|<span data-ttu-id="020c3-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="020c3-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="020c3-111">**MessageDisposition**</span><span class="sxs-lookup"><span data-stu-id="020c3-111">**MessageDisposition**</span></span> <br/> |<span data-ttu-id="020c3-112">Описывает, как будут обрабатываться элемент после его создания.</span><span class="sxs-lookup"><span data-stu-id="020c3-112">Describes how the item will be handled after it is created.</span></span> <span data-ttu-id="020c3-113">Атрибут является обязательным для сообщений электронной почты.</span><span class="sxs-lookup"><span data-stu-id="020c3-113">The attribute is required for e-mail messages.</span></span> <span data-ttu-id="020c3-114">Этот атрибут применим только к сообщениям электронной почты.</span><span class="sxs-lookup"><span data-stu-id="020c3-114">This attribute is only applicable to e-mail messages.</span></span>  <br/> |
|<span data-ttu-id="020c3-115">**SendMeetingInvitations**</span><span class="sxs-lookup"><span data-stu-id="020c3-115">**SendMeetingInvitations**</span></span> <br/> |<span data-ttu-id="020c3-116">Описывает порядок обработки приглашений на собрание после их создания.</span><span class="sxs-lookup"><span data-stu-id="020c3-116">Describes how meeting requests are handled after they are created.</span></span> <span data-ttu-id="020c3-117">Этот атрибут является обязательным для элементов календаря.</span><span class="sxs-lookup"><span data-stu-id="020c3-117">This attribute is required for calendar items.</span></span>  <br/> |
   
#### <a name="messagedisposition-attribute"></a><span data-ttu-id="020c3-118">Атрибут MessageDisposition</span><span class="sxs-lookup"><span data-stu-id="020c3-118">MessageDisposition Attribute</span></span>

|<span data-ttu-id="020c3-119">**Значение**</span><span class="sxs-lookup"><span data-stu-id="020c3-119">**Value**</span></span>|<span data-ttu-id="020c3-120">**Описание**</span><span class="sxs-lookup"><span data-stu-id="020c3-120">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="020c3-121">SaveOnly</span><span class="sxs-lookup"><span data-stu-id="020c3-121">SaveOnly</span></span>  <br/> |<span data-ttu-id="020c3-122">Элемент сообщение сохраняется в папке, указанной с помощью элемента [SavedItemFolderId](saveditemfolderid.md) .</span><span class="sxs-lookup"><span data-stu-id="020c3-122">The message item is saved in the folder that is specified by the [SavedItemFolderId](saveditemfolderid.md) element.</span></span> <span data-ttu-id="020c3-123">Сообщения могут быть отправлены более поздней версии с помощью [операции SendItem](senditem-operation.md).</span><span class="sxs-lookup"><span data-stu-id="020c3-123">Messages can be sent later by using the [SendItem operation](senditem-operation.md).</span></span> <span data-ttu-id="020c3-124">Идентификатор элемента возвращаемого в ответе.</span><span class="sxs-lookup"><span data-stu-id="020c3-124">An item identifier is returned in the response.</span></span> <span data-ttu-id="020c3-125">Идентификаторы элементов не возвращаются для любых типов элементов, за исключением элементы сообщения.</span><span class="sxs-lookup"><span data-stu-id="020c3-125">Item identifiers are not returned for any item types except for message items.</span></span> <span data-ttu-id="020c3-126">Этот компонент включает объекты ответа.</span><span class="sxs-lookup"><span data-stu-id="020c3-126">This includes response objects.</span></span>  <br/> |
|<span data-ttu-id="020c3-127">SendOnly</span><span class="sxs-lookup"><span data-stu-id="020c3-127">SendOnly</span></span>  <br/> |<span data-ttu-id="020c3-128">Элемент отправляется, но копия не сохраняется в папке «Отправленные».</span><span class="sxs-lookup"><span data-stu-id="020c3-128">The item is sent but no copy is saved in the Sent Items folder.</span></span> <span data-ttu-id="020c3-129">Идентификатор элемента не возвращается в ответе.</span><span class="sxs-lookup"><span data-stu-id="020c3-129">An item identifier is not returned in the response.</span></span>  <br/> <span data-ttu-id="020c3-130">> [!NOTE]> **CreateItem** не поддерживает делегированный доступ, когда используется параметр SendOnly, так как этот параметр нельзя использовать папку назначения.</span><span class="sxs-lookup"><span data-stu-id="020c3-130">> [!NOTE]> **CreateItem** does not support delegate access when the SendOnly option is used because a destination folder cannot be specified with this option.</span></span> <span data-ttu-id="020c3-131">Обходным путем является создание элемента, получить идентификатор элемента и затем использовать операцию SendItem для отправки элемента.</span><span class="sxs-lookup"><span data-stu-id="020c3-131">The workaround is to create the item, get the item identifier, and then use the SendItem operation to send the item.</span></span>           |
|<span data-ttu-id="020c3-132">SendAndSaveCopy</span><span class="sxs-lookup"><span data-stu-id="020c3-132">SendAndSaveCopy</span></span>  <br/> |<span data-ttu-id="020c3-133">Элемент отправляется и копия сохраняется в папке, которая определена в элементе [SavedItemFolderId](saveditemfolderid.md) .</span><span class="sxs-lookup"><span data-stu-id="020c3-133">The item is sent and a copy is saved in the folder that is identified by the [SavedItemFolderId](saveditemfolderid.md) element.</span></span> <span data-ttu-id="020c3-134">Идентификатор элемента не возвращается в ответе.</span><span class="sxs-lookup"><span data-stu-id="020c3-134">An item identifier is not returned in the response.</span></span>  <br/> <span data-ttu-id="020c3-135">> [!NOTE]> Приглашения на собрания не сохраняются в папке, заданной свойством [SavedItemFolderId](saveditemfolderid.md) .</span><span class="sxs-lookup"><span data-stu-id="020c3-135">> [!NOTE]> Meeting requests are not saved to the folder that is identified by the [SavedItemFolderId](saveditemfolderid.md) property.</span></span> <span data-ttu-id="020c3-136">Для функции календаря, только сохранения в свойстве **SavedItemFolderId** можно указать расположение элементов календаря.</span><span class="sxs-lookup"><span data-stu-id="020c3-136">For calendaring, only the save location for calendar items can be specified by the **SavedItemFolderId** property.</span></span> <span data-ttu-id="020c3-137">Вы не можете определять, приглашения на собрание элемент был сохранен.</span><span class="sxs-lookup"><span data-stu-id="020c3-137">You cannot control where a meeting request item is saved.</span></span> <span data-ttu-id="020c3-138">Связанных элементов календаря, копируются и сохраняются в папке, заданной свойством **SavedItemFolderId** .</span><span class="sxs-lookup"><span data-stu-id="020c3-138">Only the associated calendar items are copied and saved into the folder that is identified by the **SavedItemFolderId** property.</span></span>           |
   
#### <a name="sendmeetinginvitations-attribute"></a><span data-ttu-id="020c3-139">Атрибут SendMeetingInvitations</span><span class="sxs-lookup"><span data-stu-id="020c3-139">SendMeetingInvitations Attribute</span></span>

|<span data-ttu-id="020c3-140">**Значение**</span><span class="sxs-lookup"><span data-stu-id="020c3-140">**Value**</span></span>|<span data-ttu-id="020c3-141">**Описание**</span><span class="sxs-lookup"><span data-stu-id="020c3-141">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="020c3-142">SendToNone</span><span class="sxs-lookup"><span data-stu-id="020c3-142">SendToNone</span></span>  <br/> |<span data-ttu-id="020c3-143">Если элемент имеет приглашения на собрание, сохраняемый в виде элемента календаря, но не отправляются.</span><span class="sxs-lookup"><span data-stu-id="020c3-143">If the item is a meeting request, it is saved as a calendar item but not sent.</span></span>  <br/> |
|<span data-ttu-id="020c3-144">SendOnlyToAll</span><span class="sxs-lookup"><span data-stu-id="020c3-144">SendOnlyToAll</span></span>  <br/> |<span data-ttu-id="020c3-145">Запрос на собрание отправляется всех участников, но не сохраняются в папке «Отправленные».</span><span class="sxs-lookup"><span data-stu-id="020c3-145">The meeting request is sent to all attendees but is not saved in the Sent Items folder.</span></span>  <br/> |
|<span data-ttu-id="020c3-146">SendToAllAndSaveCopy</span><span class="sxs-lookup"><span data-stu-id="020c3-146">SendToAllAndSaveCopy</span></span>  <br/> |<span data-ttu-id="020c3-147">Всем участникам отправляется запрос на собрание и копия сохраняется в папке, которая определена в элементе [SavedItemFolderId](saveditemfolderid.md) .</span><span class="sxs-lookup"><span data-stu-id="020c3-147">The meeting request is sent to all attendees and a copy is saved in the folder that is identified by the [SavedItemFolderId](saveditemfolderid.md) element.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="020c3-148">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="020c3-148">Child elements</span></span>

|<span data-ttu-id="020c3-149">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="020c3-149">**Element**</span></span>|<span data-ttu-id="020c3-150">**Описание**</span><span class="sxs-lookup"><span data-stu-id="020c3-150">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="020c3-151">SavedItemFolderId</span><span class="sxs-lookup"><span data-stu-id="020c3-151">SavedItemFolderId</span></span>](saveditemfolderid.md) <br/> |<span data-ttu-id="020c3-152">Определяет целевой папке, где можно создать новый элемент.</span><span class="sxs-lookup"><span data-stu-id="020c3-152">Identifies the target folder where a new item can be created.</span></span> <span data-ttu-id="020c3-153">Если атрибут **MessageDisposition** SendOnly, созданного сообщения будут отправляться только.</span><span class="sxs-lookup"><span data-stu-id="020c3-153">If the **MessageDisposition** attribute is set to SendOnly, a created message will only be sent.</span></span> <span data-ttu-id="020c3-154">Сообщение не следует помещать в папке, указанной с помощью элемента [SavedItemFolderId](saveditemfolderid.md) .</span><span class="sxs-lookup"><span data-stu-id="020c3-154">The message will not be put in the folder that is identified by the [SavedItemFolderId](saveditemfolderid.md) element.</span></span>  <br/> |
|[<span data-ttu-id="020c3-155">Элементы (NonEmptyArrayOfAllItemsType)</span><span class="sxs-lookup"><span data-stu-id="020c3-155">Items (NonEmptyArrayOfAllItemsType)</span></span>](items-nonemptyarrayofallitemstype.md) <br/> |<span data-ttu-id="020c3-156">Содержит массив элементов для создания в папке, указанной с помощью элемента [SavedItemFolderId](saveditemfolderid.md) .</span><span class="sxs-lookup"><span data-stu-id="020c3-156">Contains an array of items to create in the folder that is identified by the [SavedItemFolderId](saveditemfolderid.md) element.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="020c3-157">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="020c3-157">Parent elements</span></span>

<span data-ttu-id="020c3-158">Нет.</span><span class="sxs-lookup"><span data-stu-id="020c3-158">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="020c3-159">Замечания</span><span class="sxs-lookup"><span data-stu-id="020c3-159">Remarks</span></span>

<span data-ttu-id="020c3-160">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="020c3-160">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="020c3-161">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="020c3-161">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="020c3-162">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="020c3-162">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="020c3-163">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="020c3-163">Schema Name</span></span>  <br/> |<span data-ttu-id="020c3-164">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="020c3-164">Messages schema</span></span>  <br/> |
|<span data-ttu-id="020c3-165">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="020c3-165">Validation File</span></span>  <br/> |<span data-ttu-id="020c3-166">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="020c3-166">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="020c3-167">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="020c3-167">Can be Empty</span></span>  <br/> |<span data-ttu-id="020c3-168">False</span><span class="sxs-lookup"><span data-stu-id="020c3-168">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="020c3-169">См. также</span><span class="sxs-lookup"><span data-stu-id="020c3-169">See also</span></span>



[<span data-ttu-id="020c3-170">CreateItemResponse</span><span class="sxs-lookup"><span data-stu-id="020c3-170">CreateItemResponse</span></span>](createitemresponse.md)
  
[<span data-ttu-id="020c3-171">CreateItem Operation</span><span class="sxs-lookup"><span data-stu-id="020c3-171">CreateItem operation</span></span>](createitem-operation.md)
  
 <span data-ttu-id="020c3-172">**CreateItemType**</span><span class="sxs-lookup"><span data-stu-id="020c3-172">**CreateItemType**</span></span>


[<span data-ttu-id="020c3-173">Создание сообщения электронной почты</span><span class="sxs-lookup"><span data-stu-id="020c3-173">Creating E-mail Messages</span></span>](http://msdn.microsoft.com/library/05bfb83c-2866-427d-a9fe-14ba3cb02793%28Office.15%29.aspx)
  
[<span data-ttu-id="020c3-174">Создание контактов (веб-служб Exchange)</span><span class="sxs-lookup"><span data-stu-id="020c3-174">Creating Contacts (Exchange Web Services)</span></span>](http://msdn.microsoft.com/library/4845917e-70d1-481c-bbd7-011ec6571789%28Office.15%29.aspx)
  
[<span data-ttu-id="020c3-175">Создание задач</span><span class="sxs-lookup"><span data-stu-id="020c3-175">Creating Tasks</span></span>](http://msdn.microsoft.com/library/0ef97334-e8a0-4f67-a23a-dd9e2bbad49f%28Office.15%29.aspx)
  
[<span data-ttu-id="020c3-176">Создание встреч</span><span class="sxs-lookup"><span data-stu-id="020c3-176">Creating Appointments</span></span>](http://msdn.microsoft.com/library/2385391e-c9e7-4d45-b803-c4ff94d5c94e%28Office.15%29.aspx)

