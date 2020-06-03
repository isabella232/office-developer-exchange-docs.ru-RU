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
description: Элемент CreateItem определяет запрос на создание элемента в хранилище Exchange.
ms.openlocfilehash: 235664b7baeceeccb14135fd346123f0f7d99346
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44527063"
---
# <a name="createitem"></a><span data-ttu-id="378cc-103">CreateItem</span><span class="sxs-lookup"><span data-stu-id="378cc-103">CreateItem</span></span>

<span data-ttu-id="378cc-104">Элемент **CreateItem** определяет запрос на создание элемента в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="378cc-104">The **CreateItem** element defines a request to create an item in the Exchange store.</span></span> 
  
```xml
<CreateItem MessageDisposition="" SendMeetingInvitations="">
   <SavedItemFolderId/>
   <Items/>
</CreateItem>
```

<span data-ttu-id="378cc-105">**креатеитемтипе**</span><span class="sxs-lookup"><span data-stu-id="378cc-105">**CreateItemType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="378cc-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="378cc-106">Attributes and elements</span></span>

<span data-ttu-id="378cc-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="378cc-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="378cc-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="378cc-108">Attributes</span></span>

|<span data-ttu-id="378cc-109">Атрибут</span><span class="sxs-lookup"><span data-stu-id="378cc-109">Attribute</span></span>|<span data-ttu-id="378cc-110">Описание</span><span class="sxs-lookup"><span data-stu-id="378cc-110">Description</span></span>|
|:-----|:-----|
|<span data-ttu-id="378cc-111">**мессажедиспоситион**</span><span class="sxs-lookup"><span data-stu-id="378cc-111">**MessageDisposition**</span></span> <br/> |<span data-ttu-id="378cc-112">Описывает, как будет обрабатываться элемент после его создания.</span><span class="sxs-lookup"><span data-stu-id="378cc-112">Describes how the item will be handled after it is created.</span></span> <span data-ttu-id="378cc-113">Этот атрибут необходим для сообщений электронной почты.</span><span class="sxs-lookup"><span data-stu-id="378cc-113">The attribute is required for e-mail messages.</span></span> <span data-ttu-id="378cc-114">Этот атрибут применяется только к сообщениям электронной почты.</span><span class="sxs-lookup"><span data-stu-id="378cc-114">This attribute is only applicable to e-mail messages.</span></span>  <br/> |
|<span data-ttu-id="378cc-115">**сендмитингинвитатионс**</span><span class="sxs-lookup"><span data-stu-id="378cc-115">**SendMeetingInvitations**</span></span> <br/> |<span data-ttu-id="378cc-116">Описывает, как обрабатываются приглашения на собрания после их создания.</span><span class="sxs-lookup"><span data-stu-id="378cc-116">Describes how meeting requests are handled after they are created.</span></span> <span data-ttu-id="378cc-117">Этот атрибут необходим для элементов календаря.</span><span class="sxs-lookup"><span data-stu-id="378cc-117">This attribute is required for calendar items.</span></span>  <br/> |
   
#### <a name="messagedisposition-attribute"></a><span data-ttu-id="378cc-118">Атрибут Мессажедиспоситион</span><span class="sxs-lookup"><span data-stu-id="378cc-118">MessageDisposition Attribute</span></span>

|<span data-ttu-id="378cc-119">Значение</span><span class="sxs-lookup"><span data-stu-id="378cc-119">Value</span></span>|<span data-ttu-id="378cc-120">Описание</span><span class="sxs-lookup"><span data-stu-id="378cc-120">Description</span></span>|
|:-----|:-----|
|<span data-ttu-id="378cc-121">савеонли</span><span class="sxs-lookup"><span data-stu-id="378cc-121">SaveOnly</span></span>  <br/> |<span data-ttu-id="378cc-122">Элемент Message сохраняется в папке, указанной элементом [саведитемфолдерид](saveditemfolderid.md) .</span><span class="sxs-lookup"><span data-stu-id="378cc-122">The message item is saved in the folder that is specified by the [SavedItemFolderId](saveditemfolderid.md) element.</span></span> <span data-ttu-id="378cc-123">Сообщения можно отправить позже с помощью [операции SendItem](senditem-operation.md).</span><span class="sxs-lookup"><span data-stu-id="378cc-123">Messages can be sent later by using the [SendItem operation](senditem-operation.md).</span></span> <span data-ttu-id="378cc-124">В отклике возвращается идентификатор элемента.</span><span class="sxs-lookup"><span data-stu-id="378cc-124">An item identifier is returned in the response.</span></span> <span data-ttu-id="378cc-125">Идентификаторы элементов не возвращаются для всех типов элементов, кроме элементов сообщения.</span><span class="sxs-lookup"><span data-stu-id="378cc-125">Item identifiers are not returned for any item types except for message items.</span></span> <span data-ttu-id="378cc-126">Это относится и к объектам Response.</span><span class="sxs-lookup"><span data-stu-id="378cc-126">This includes response objects.</span></span>  <br/> |
|<span data-ttu-id="378cc-127">сендонли</span><span class="sxs-lookup"><span data-stu-id="378cc-127">SendOnly</span></span>  <br/> |<span data-ttu-id="378cc-128">Элемент отправляется, но копия не сохраняется в папке "Отправленные".</span><span class="sxs-lookup"><span data-stu-id="378cc-128">The item is sent but no copy is saved in the Sent Items folder.</span></span> <span data-ttu-id="378cc-129">Идентификатор элемента не возвращается в ответе.</span><span class="sxs-lookup"><span data-stu-id="378cc-129">An item identifier is not returned in the response.</span></span><br/><br/><span data-ttu-id="378cc-130">**Note**: функция **CreateItem** не поддерживает делегированный доступ, если используется параметр сендонли, так как Целевая папка не может быть указана с помощью этого параметра.</span><span class="sxs-lookup"><span data-stu-id="378cc-130">**NOTE**: **CreateItem** does not support delegate access when the SendOnly option is used because a destination folder cannot be specified with this option.</span></span> <span data-ttu-id="378cc-131">Чтобы устранить эту операцию, необходимо создать элемент, получить идентификатор элемента и затем использовать операцию SendItem для отправки элемента.</span><span class="sxs-lookup"><span data-stu-id="378cc-131">The workaround is to create the item, get the item identifier, and then use the SendItem operation to send the item.</span></span>           |
|<span data-ttu-id="378cc-132">SendAndSaveCopy</span><span class="sxs-lookup"><span data-stu-id="378cc-132">SendAndSaveCopy</span></span>  <br/> |<span data-ttu-id="378cc-133">Элемент отправляется, а копия сохраняется в папке, указанной с помощью элемента [саведитемфолдерид](saveditemfolderid.md) .</span><span class="sxs-lookup"><span data-stu-id="378cc-133">The item is sent and a copy is saved in the folder that is identified by the [SavedItemFolderId](saveditemfolderid.md) element.</span></span> <span data-ttu-id="378cc-134">Идентификатор элемента не возвращается в ответе.</span><span class="sxs-lookup"><span data-stu-id="378cc-134">An item identifier is not returned in the response.</span></span><br/><br/><span data-ttu-id="378cc-135">**Note**: приглашения на собрания не сохраняются в папке, определяемой свойством [саведитемфолдерид](saveditemfolderid.md) .</span><span class="sxs-lookup"><span data-stu-id="378cc-135">**NOTE**: Meeting requests are not saved to the folder that is identified by the [SavedItemFolderId](saveditemfolderid.md) property.</span></span> <span data-ttu-id="378cc-136">Для календаря можно указать только расположение для сохранения элементов календаря в свойстве **саведитемфолдерид** .</span><span class="sxs-lookup"><span data-stu-id="378cc-136">For calendaring, only the save location for calendar items can be specified by the **SavedItemFolderId** property.</span></span> <span data-ttu-id="378cc-137">Вы не можете управлять местом сохранения элемента приглашения на собрание.</span><span class="sxs-lookup"><span data-stu-id="378cc-137">You cannot control where a meeting request item is saved.</span></span> <span data-ttu-id="378cc-138">Только связанные элементы календаря копируются и сохраняются в папку, определяемую свойством **саведитемфолдерид** .</span><span class="sxs-lookup"><span data-stu-id="378cc-138">Only the associated calendar items are copied and saved into the folder that is identified by the **SavedItemFolderId** property.</span></span>           |
   
#### <a name="sendmeetinginvitations-attribute"></a><span data-ttu-id="378cc-139">Атрибут Сендмитингинвитатионс</span><span class="sxs-lookup"><span data-stu-id="378cc-139">SendMeetingInvitations Attribute</span></span>

|<span data-ttu-id="378cc-140">Значение</span><span class="sxs-lookup"><span data-stu-id="378cc-140">Value</span></span>|<span data-ttu-id="378cc-141">Описание</span><span class="sxs-lookup"><span data-stu-id="378cc-141">Description</span></span>|
|:-----|:-----|
|<span data-ttu-id="378cc-142">сендтононе</span><span class="sxs-lookup"><span data-stu-id="378cc-142">SendToNone</span></span>  <br/> |<span data-ttu-id="378cc-143">Если элемент является приглашением на собрание, он сохраняется как элемент календаря, но не отправляется.</span><span class="sxs-lookup"><span data-stu-id="378cc-143">If the item is a meeting request, it is saved as a calendar item but not sent.</span></span>  <br/> |
|<span data-ttu-id="378cc-144">сендонлитоалл</span><span class="sxs-lookup"><span data-stu-id="378cc-144">SendOnlyToAll</span></span>  <br/> |<span data-ttu-id="378cc-145">Приглашение на собрание отправляется всем участникам, но не сохраняется в папке "Отправленные".</span><span class="sxs-lookup"><span data-stu-id="378cc-145">The meeting request is sent to all attendees but is not saved in the Sent Items folder.</span></span>  <br/> |
|<span data-ttu-id="378cc-146">сендтоалландсавекопи</span><span class="sxs-lookup"><span data-stu-id="378cc-146">SendToAllAndSaveCopy</span></span>  <br/> |<span data-ttu-id="378cc-147">Приглашение на собрание отправляется всем участникам, а копия сохраняется в папке, указанной с помощью элемента [саведитемфолдерид](saveditemfolderid.md) .</span><span class="sxs-lookup"><span data-stu-id="378cc-147">The meeting request is sent to all attendees and a copy is saved in the folder that is identified by the [SavedItemFolderId](saveditemfolderid.md) element.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="378cc-148">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="378cc-148">Child elements</span></span>

|<span data-ttu-id="378cc-149">Элемент</span><span class="sxs-lookup"><span data-stu-id="378cc-149">Element</span></span>|<span data-ttu-id="378cc-150">Описание</span><span class="sxs-lookup"><span data-stu-id="378cc-150">Description</span></span>|
|:-----|:-----|
|[<span data-ttu-id="378cc-151">саведитемфолдерид</span><span class="sxs-lookup"><span data-stu-id="378cc-151">SavedItemFolderId</span></span>](saveditemfolderid.md) <br/> |<span data-ttu-id="378cc-152">Указывает целевую папку, в которой можно создать новый элемент.</span><span class="sxs-lookup"><span data-stu-id="378cc-152">Identifies the target folder where a new item can be created.</span></span> <span data-ttu-id="378cc-153">Если для атрибута **мессажедиспоситион** задано значение сендонли, будет отправлено созданное сообщение.</span><span class="sxs-lookup"><span data-stu-id="378cc-153">If the **MessageDisposition** attribute is set to SendOnly, a created message will only be sent.</span></span> <span data-ttu-id="378cc-154">Сообщение не будет помещено в папку, определяемую элементом [саведитемфолдерид](saveditemfolderid.md) .</span><span class="sxs-lookup"><span data-stu-id="378cc-154">The message will not be put in the folder that is identified by the [SavedItemFolderId](saveditemfolderid.md) element.</span></span>  <br/> |
|[<span data-ttu-id="378cc-155">Элементы (Нонемптяррайофаллитемстипе)</span><span class="sxs-lookup"><span data-stu-id="378cc-155">Items (NonEmptyArrayOfAllItemsType)</span></span>](items-nonemptyarrayofallitemstype.md) <br/> |<span data-ttu-id="378cc-156">Содержит массив элементов для создания в папке, определяемой элементом [саведитемфолдерид](saveditemfolderid.md) .</span><span class="sxs-lookup"><span data-stu-id="378cc-156">Contains an array of items to create in the folder that is identified by the [SavedItemFolderId](saveditemfolderid.md) element.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="378cc-157">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="378cc-157">Parent elements</span></span>

<span data-ttu-id="378cc-158">Нет.</span><span class="sxs-lookup"><span data-stu-id="378cc-158">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="378cc-159">Примечания</span><span class="sxs-lookup"><span data-stu-id="378cc-159">Remarks</span></span>

<span data-ttu-id="378cc-160">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="378cc-160">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="378cc-161">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="378cc-161">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="378cc-162">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="378cc-162">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="378cc-163">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="378cc-163">Schema Name</span></span>  <br/> |<span data-ttu-id="378cc-164">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="378cc-164">Messages schema</span></span>  <br/> |
|<span data-ttu-id="378cc-165">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="378cc-165">Validation File</span></span>  <br/> |<span data-ttu-id="378cc-166">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="378cc-166">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="378cc-167">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="378cc-167">Can be Empty</span></span>  <br/> |<span data-ttu-id="378cc-168">False</span><span class="sxs-lookup"><span data-stu-id="378cc-168">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="378cc-169">См. также</span><span class="sxs-lookup"><span data-stu-id="378cc-169">See also</span></span>

- [<span data-ttu-id="378cc-170">креатеитемреспонсе</span><span class="sxs-lookup"><span data-stu-id="378cc-170">CreateItemResponse</span></span>](createitemresponse.md)  
- [<span data-ttu-id="378cc-171">Операция CreateItem</span><span class="sxs-lookup"><span data-stu-id="378cc-171">CreateItem operation</span></span>](createitem-operation.md)
- [<span data-ttu-id="378cc-172">Создание сообщений электронной почты</span><span class="sxs-lookup"><span data-stu-id="378cc-172">Creating E-mail Messages</span></span>](https://msdn.microsoft.com/library/05bfb83c-2866-427d-a9fe-14ba3cb02793%28Office.15%29.aspx) 
- [<span data-ttu-id="378cc-173">Создание контактов (веб-службы Exchange)</span><span class="sxs-lookup"><span data-stu-id="378cc-173">Creating Contacts (Exchange Web Services)</span></span>](https://msdn.microsoft.com/library/4845917e-70d1-481c-bbd7-011ec6571789%28Office.15%29.aspx)  
- [<span data-ttu-id="378cc-174">Создание задач</span><span class="sxs-lookup"><span data-stu-id="378cc-174">Creating Tasks</span></span>](https://msdn.microsoft.com/library/0ef97334-e8a0-4f67-a23a-dd9e2bbad49f%28Office.15%29.aspx) 
- [<span data-ttu-id="378cc-175">Создание встреч</span><span class="sxs-lookup"><span data-stu-id="378cc-175">Creating Appointments</span></span>](https://msdn.microsoft.com/library/2385391e-c9e7-4d45-b803-c4ff94d5c94e%28Office.15%29.aspx)

