---
title: FindConversation
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FindConversation
api_type:
- schema
ms.assetid: 94b7083c-60cf-478b-a9af-a88f7acb30fb
description: Элемент FindConversation определяет запрос на поиск бесед в почтовый ящик.
ms.openlocfilehash: 990e15f468f836d51977329c524acb439014da95
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762555"
---
# <a name="findconversation"></a><span data-ttu-id="6196c-103">FindConversation</span><span class="sxs-lookup"><span data-stu-id="6196c-103">FindConversation</span></span>

<span data-ttu-id="6196c-104">Элемент **FindConversation** определяет запрос на поиск бесед в почтовый ящик.</span><span class="sxs-lookup"><span data-stu-id="6196c-104">The **FindConversation** element defines a request to find conversations in a mailbox.</span></span> 
  
[<span data-ttu-id="6196c-105">FindConversation</span><span class="sxs-lookup"><span data-stu-id="6196c-105">FindConversation</span></span>](findconversation.md)
  
```XML
<FindConversation Traversal="" ViewFilter="">
   <IndexedPageItemView/>
   <SeekToConditionPageItemView/>
   <SortOrder/>
   <ParentFolderId/>
   <MailboxScope/>
   <QueryString/>
   <ConversationShape/>
</FindConversation>
```

 <span data-ttu-id="6196c-106">**FindConversationType**</span><span class="sxs-lookup"><span data-stu-id="6196c-106">**FindConversationType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6196c-107">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="6196c-107">Attributes and elements</span></span>

<span data-ttu-id="6196c-108">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="6196c-108">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6196c-109">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="6196c-109">Attributes</span></span>

****

|<span data-ttu-id="6196c-110">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="6196c-110">**Attribute**</span></span>|<span data-ttu-id="6196c-111">**Описание**</span><span class="sxs-lookup"><span data-stu-id="6196c-111">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="6196c-112">Обход</span><span class="sxs-lookup"><span data-stu-id="6196c-112">Traversal</span></span>  <br/> |<span data-ttu-id="6196c-113">Определяет типы поддерева обхода.</span><span class="sxs-lookup"><span data-stu-id="6196c-113">Identifies the types of sub-tree traversal.</span></span> <span data-ttu-id="6196c-114">Этот атрибут является необязательным.</span><span class="sxs-lookup"><span data-stu-id="6196c-114">This attribute is optional.</span></span>  <br/> |
|<span data-ttu-id="6196c-115">ViewFilter</span><span class="sxs-lookup"><span data-stu-id="6196c-115">ViewFilter</span></span>  <br/> |<span data-ttu-id="6196c-116">Определяет типы фильтры представления.</span><span class="sxs-lookup"><span data-stu-id="6196c-116">Identifies the types view filters.</span></span> <span data-ttu-id="6196c-117">Этот атрибут является необязательным.</span><span class="sxs-lookup"><span data-stu-id="6196c-117">This attribute is optional.</span></span>  <br/> |
   
#### <a name="traversal-attribute-values"></a><span data-ttu-id="6196c-118">Значения атрибутов обхода</span><span class="sxs-lookup"><span data-stu-id="6196c-118">Traversal attribute values</span></span>

****

|<span data-ttu-id="6196c-119">**Значение**</span><span class="sxs-lookup"><span data-stu-id="6196c-119">**Value**</span></span>|<span data-ttu-id="6196c-120">**Описание**</span><span class="sxs-lookup"><span data-stu-id="6196c-120">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="6196c-121">Неполная</span><span class="sxs-lookup"><span data-stu-id="6196c-121">Shallow</span></span>  <br/> |<span data-ttu-id="6196c-122">Указывает частичного обхода.</span><span class="sxs-lookup"><span data-stu-id="6196c-122">Indicates a shallow traversal.</span></span>  <br/> |
|<span data-ttu-id="6196c-123">Глубокое</span><span class="sxs-lookup"><span data-stu-id="6196c-123">Deep</span></span>  <br/> |<span data-ttu-id="6196c-124">Указывает глубину обхода.</span><span class="sxs-lookup"><span data-stu-id="6196c-124">Indicates a deep traversal.</span></span>  <br/> |
   
#### <a name="viewfilter-attribute-values"></a><span data-ttu-id="6196c-125">Значения атрибутов ViewFilter</span><span class="sxs-lookup"><span data-stu-id="6196c-125">ViewFilter attribute values</span></span>

****

|<span data-ttu-id="6196c-126">**Значение**</span><span class="sxs-lookup"><span data-stu-id="6196c-126">**Value**</span></span>|<span data-ttu-id="6196c-127">**Описание**</span><span class="sxs-lookup"><span data-stu-id="6196c-127">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="6196c-128">Все</span><span class="sxs-lookup"><span data-stu-id="6196c-128">All</span></span>  <br/> |<span data-ttu-id="6196c-129">Поиск всех бесед.</span><span class="sxs-lookup"><span data-stu-id="6196c-129">Find all conversations.</span></span>  <br/> |
|<span data-ttu-id="6196c-130">Отмеченные</span><span class="sxs-lookup"><span data-stu-id="6196c-130">Flagged</span></span>  <br/> |<span data-ttu-id="6196c-131">Поиск отмеченного бесед.</span><span class="sxs-lookup"><span data-stu-id="6196c-131">Find flagged conversations.</span></span>  <br/> |
|<span data-ttu-id="6196c-132">HasAttachment</span><span class="sxs-lookup"><span data-stu-id="6196c-132">HasAttachment</span></span>  <br/> |<span data-ttu-id="6196c-133">Поиск бесед с вложениями.</span><span class="sxs-lookup"><span data-stu-id="6196c-133">Find conversations with attachments.</span></span>  <br/> |
|<span data-ttu-id="6196c-134">ToOrCcMe</span><span class="sxs-lookup"><span data-stu-id="6196c-134">ToOrCcMe</span></span>  <br/> |<span data-ttu-id="6196c-135">Найдите адресованное беседы или «копия» будет мне.</span><span class="sxs-lookup"><span data-stu-id="6196c-135">Find conversations addressed or cc'd to me.</span></span>  <br/> |
|<span data-ttu-id="6196c-136">Unread</span><span class="sxs-lookup"><span data-stu-id="6196c-136">Unread</span></span>  <br/> |<span data-ttu-id="6196c-137">Поиск непрочитанных бесед.</span><span class="sxs-lookup"><span data-stu-id="6196c-137">Find unread conversations.</span></span>  <br/> |
|<span data-ttu-id="6196c-138">TaskActive</span><span class="sxs-lookup"><span data-stu-id="6196c-138">TaskActive</span></span>  <br/> |<span data-ttu-id="6196c-139">Поиск активных задач.</span><span class="sxs-lookup"><span data-stu-id="6196c-139">Find active tasks.</span></span>  <br/> |
|<span data-ttu-id="6196c-140">TaskOverdue</span><span class="sxs-lookup"><span data-stu-id="6196c-140">TaskOverdue</span></span>  <br/> |<span data-ttu-id="6196c-141">Найдите просроченные задачи.</span><span class="sxs-lookup"><span data-stu-id="6196c-141">Find overdue tasks.</span></span>  <br/> |
|<span data-ttu-id="6196c-142">TaskCompleted</span><span class="sxs-lookup"><span data-stu-id="6196c-142">TaskCompleted</span></span>  <br/> |<span data-ttu-id="6196c-143">Найдите завершенные задачи.</span><span class="sxs-lookup"><span data-stu-id="6196c-143">Find completed tasks.</span></span>  <br/> |
|<span data-ttu-id="6196c-144">NoClutter</span><span class="sxs-lookup"><span data-stu-id="6196c-144">NoClutter</span></span>  <br/> |<span data-ttu-id="6196c-145">Только для внутреннего использования.</span><span class="sxs-lookup"><span data-stu-id="6196c-145">For internal use only.</span></span>  <br/> |
|<span data-ttu-id="6196c-146">Засорение</span><span class="sxs-lookup"><span data-stu-id="6196c-146">Clutter</span></span>  <br/> |<span data-ttu-id="6196c-147">Только для внутреннего использования.</span><span class="sxs-lookup"><span data-stu-id="6196c-147">For internal use only.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="6196c-148">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="6196c-148">Child elements</span></span>

|<span data-ttu-id="6196c-149">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="6196c-149">**Element**</span></span>|<span data-ttu-id="6196c-150">**Описание**</span><span class="sxs-lookup"><span data-stu-id="6196c-150">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6196c-151">IndexedPageItemView</span><span class="sxs-lookup"><span data-stu-id="6196c-151">IndexedPageItemView</span></span>](indexedpageitemview.md) <br/> |<span data-ttu-id="6196c-152">Описывает как выгружаемый беседы возвращаются данные.</span><span class="sxs-lookup"><span data-stu-id="6196c-152">Describes how paged conversation information is returned.</span></span>  <br/> |
|[<span data-ttu-id="6196c-153">SeekToConditionPageItemView</span><span class="sxs-lookup"><span data-stu-id="6196c-153">SeekToConditionPageItemView</span></span>](seektoconditionpageitemview.md) <br/> |<span data-ttu-id="6196c-154">Указывает условие, используемый для идентификации в конце поиска, начальный индекс поиска, максимальное записей для возвращения и указания поиска для поиска **FindItem** или **FindConversation** .</span><span class="sxs-lookup"><span data-stu-id="6196c-154">Specifies the condition that is used to identify the end of a search, the starting index of a search, the maximum entries to return, and the search directions for a **FindItem** or **FindConversation** search.</span></span>  <br/> |
|[<span data-ttu-id="6196c-155">SortOrder</span><span class="sxs-lookup"><span data-stu-id="6196c-155">SortOrder</span></span>](sortorder.md) <br/> |<span data-ttu-id="6196c-156">Определяет порядок сортировки элементов в [FindConversation операции](findconversation-operation.md) запроса.</span><span class="sxs-lookup"><span data-stu-id="6196c-156">Defines how items are sorted in a [FindConversation operation](findconversation-operation.md) request.</span></span> <span data-ttu-id="6196c-157">Свойство **Беседы: LastDeliveryTime** — это единственный параметр, который поддерживается для сортировки при использовании операции **FindConversation** .</span><span class="sxs-lookup"><span data-stu-id="6196c-157">The **conversation:LastDeliveryTime** property is the only property that is supported for sorting when the **FindConversation** operation is used.</span></span>  <br/> |
|[<span data-ttu-id="6196c-158">ParentFolderId (TargetFolderIdType)</span><span class="sxs-lookup"><span data-stu-id="6196c-158">ParentFolderId (TargetFolderIdType)</span></span>](parentfolderid-targetfolderidtype.md) <br/> |<span data-ttu-id="6196c-159">Указывает папку для поиска бесед.</span><span class="sxs-lookup"><span data-stu-id="6196c-159">Identifies the folder to search for conversations.</span></span>  <br/> |
|[<span data-ttu-id="6196c-160">MailboxScope</span><span class="sxs-lookup"><span data-stu-id="6196c-160">MailboxScope</span></span>](mailboxscope.md) <br/> |<span data-ttu-id="6196c-161">Разрешение поиска или выборки для беседы должны охватывать основной почтовый ящик, архивного почтового ящика или обеих основной и архивировать почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="6196c-161">Specifies whether a search or fetch for a conversation should span either the primary mailbox, archive mailbox, or both the primary and archive mailbox.</span></span>  <br/> |
|[<span data-ttu-id="6196c-162">Строка запроса (QueryStringType)</span><span class="sxs-lookup"><span data-stu-id="6196c-162">QueryString (QueryStringType)</span></span>](querystring-querystringtype.md) <br/> |<span data-ttu-id="6196c-163">Указывает строку запроса почтовых ящиков на основе на расширенный синтаксис запроса (AQS).</span><span class="sxs-lookup"><span data-stu-id="6196c-163">Specifies a mailbox query string based on Advanced Query Syntax (AQS).</span></span>  <br/> |
|[<span data-ttu-id="6196c-164">ConversationShape</span><span class="sxs-lookup"><span data-stu-id="6196c-164">ConversationShape</span></span>](conversationshape.md) <br/> |<span data-ttu-id="6196c-165">Определяет свойство, задайте для возврата в ответ на [операцию FindConversation](findconversation-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="6196c-165">Identifies the property set to return in a [FindConversation operation](findconversation-operation.md) response.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="6196c-166">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="6196c-166">Parent elements</span></span>

<span data-ttu-id="6196c-167">Нет.</span><span class="sxs-lookup"><span data-stu-id="6196c-167">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="6196c-168">Замечания</span><span class="sxs-lookup"><span data-stu-id="6196c-168">Remarks</span></span>

<span data-ttu-id="6196c-169">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.Этот элемент появился в Exchange Server 2010 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="6196c-169">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6196c-170">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="6196c-170">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6196c-171">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="6196c-171">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="6196c-172">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="6196c-172">Schema Name</span></span>  <br/> |<span data-ttu-id="6196c-173">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="6196c-173">Messages schema</span></span>  <br/> |
|<span data-ttu-id="6196c-174">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="6196c-174">Validation File</span></span>  <br/> |<span data-ttu-id="6196c-175">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="6196c-175">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="6196c-176">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="6196c-176">Can be Empty</span></span>  <br/> |<span data-ttu-id="6196c-177">False</span><span class="sxs-lookup"><span data-stu-id="6196c-177">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6196c-178">См. также</span><span class="sxs-lookup"><span data-stu-id="6196c-178">See also</span></span>



[<span data-ttu-id="6196c-179">FindConversation Operation</span><span class="sxs-lookup"><span data-stu-id="6196c-179">FindConversation operation</span></span>](findconversation-operation.md)


- [<span data-ttu-id="6196c-180">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="6196c-180">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="6196c-181">Conversations in EWS</span><span class="sxs-lookup"><span data-stu-id="6196c-181">Conversations in EWS</span></span>](http://msdn.microsoft.com/library/91e64629-db6c-4c94-9dcb-d386232e8467%28Office.15%29.aspx)

