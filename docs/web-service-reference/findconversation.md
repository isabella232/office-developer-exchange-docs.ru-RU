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
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762555"
---
# <a name="findconversation"></a><span data-ttu-id="9074e-103">FindConversation</span><span class="sxs-lookup"><span data-stu-id="9074e-103">FindConversation</span></span>

<span data-ttu-id="9074e-104">Элемент **FindConversation** определяет запрос на поиск бесед в почтовый ящик.</span><span class="sxs-lookup"><span data-stu-id="9074e-104">The **FindConversation** element defines a request to find conversations in a mailbox.</span></span> 
  
[<span data-ttu-id="9074e-105">FindConversation</span><span class="sxs-lookup"><span data-stu-id="9074e-105">FindConversation</span></span>](findconversation.md)
  
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

 <span data-ttu-id="9074e-106">**FindConversationType**</span><span class="sxs-lookup"><span data-stu-id="9074e-106">**FindConversationType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9074e-107">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="9074e-107">Attributes and elements</span></span>

<span data-ttu-id="9074e-108">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="9074e-108">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9074e-109">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="9074e-109">Attributes</span></span>

****

|<span data-ttu-id="9074e-110">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="9074e-110">**Attribute**</span></span>|<span data-ttu-id="9074e-111">**Описание**</span><span class="sxs-lookup"><span data-stu-id="9074e-111">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="9074e-112">Обход</span><span class="sxs-lookup"><span data-stu-id="9074e-112">Traversal</span></span>  <br/> |<span data-ttu-id="9074e-113">Определяет типы поддерева обхода.</span><span class="sxs-lookup"><span data-stu-id="9074e-113">Identifies the types of sub-tree traversal.</span></span> <span data-ttu-id="9074e-114">Этот атрибут является необязательным.</span><span class="sxs-lookup"><span data-stu-id="9074e-114">This attribute is optional.</span></span>  <br/> |
|<span data-ttu-id="9074e-115">ViewFilter</span><span class="sxs-lookup"><span data-stu-id="9074e-115">ViewFilter</span></span>  <br/> |<span data-ttu-id="9074e-116">Определяет типы фильтры представления.</span><span class="sxs-lookup"><span data-stu-id="9074e-116">Identifies the types view filters.</span></span> <span data-ttu-id="9074e-117">Этот атрибут является необязательным.</span><span class="sxs-lookup"><span data-stu-id="9074e-117">This attribute is optional.</span></span>  <br/> |
   
#### <a name="traversal-attribute-values"></a><span data-ttu-id="9074e-118">Значения атрибутов обхода</span><span class="sxs-lookup"><span data-stu-id="9074e-118">Traversal attribute values</span></span>

****

|<span data-ttu-id="9074e-119">**Значение**</span><span class="sxs-lookup"><span data-stu-id="9074e-119">**Value**</span></span>|<span data-ttu-id="9074e-120">**Описание**</span><span class="sxs-lookup"><span data-stu-id="9074e-120">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="9074e-121">Неполная</span><span class="sxs-lookup"><span data-stu-id="9074e-121">Shallow</span></span>  <br/> |<span data-ttu-id="9074e-122">Указывает частичного обхода.</span><span class="sxs-lookup"><span data-stu-id="9074e-122">Indicates a shallow traversal.</span></span>  <br/> |
|<span data-ttu-id="9074e-123">Глубокое</span><span class="sxs-lookup"><span data-stu-id="9074e-123">Deep</span></span>  <br/> |<span data-ttu-id="9074e-124">Указывает глубину обхода.</span><span class="sxs-lookup"><span data-stu-id="9074e-124">Indicates a deep traversal.</span></span>  <br/> |
   
#### <a name="viewfilter-attribute-values"></a><span data-ttu-id="9074e-125">Значения атрибутов ViewFilter</span><span class="sxs-lookup"><span data-stu-id="9074e-125">ViewFilter attribute values</span></span>

****

|<span data-ttu-id="9074e-126">**Значение**</span><span class="sxs-lookup"><span data-stu-id="9074e-126">**Value**</span></span>|<span data-ttu-id="9074e-127">**Описание**</span><span class="sxs-lookup"><span data-stu-id="9074e-127">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="9074e-128">Все</span><span class="sxs-lookup"><span data-stu-id="9074e-128">All</span></span>  <br/> |<span data-ttu-id="9074e-129">Поиск всех бесед.</span><span class="sxs-lookup"><span data-stu-id="9074e-129">Find all conversations.</span></span>  <br/> |
|<span data-ttu-id="9074e-130">Отмеченные</span><span class="sxs-lookup"><span data-stu-id="9074e-130">Flagged</span></span>  <br/> |<span data-ttu-id="9074e-131">Поиск отмеченного бесед.</span><span class="sxs-lookup"><span data-stu-id="9074e-131">Find flagged conversations.</span></span>  <br/> |
|<span data-ttu-id="9074e-132">HasAttachment</span><span class="sxs-lookup"><span data-stu-id="9074e-132">HasAttachment</span></span>  <br/> |<span data-ttu-id="9074e-133">Поиск бесед с вложениями.</span><span class="sxs-lookup"><span data-stu-id="9074e-133">Find conversations with attachments.</span></span>  <br/> |
|<span data-ttu-id="9074e-134">ToOrCcMe</span><span class="sxs-lookup"><span data-stu-id="9074e-134">ToOrCcMe</span></span>  <br/> |<span data-ttu-id="9074e-135">Найдите адресованное беседы или «копия» будет мне.</span><span class="sxs-lookup"><span data-stu-id="9074e-135">Find conversations addressed or cc'd to me.</span></span>  <br/> |
|<span data-ttu-id="9074e-136">Unread</span><span class="sxs-lookup"><span data-stu-id="9074e-136">Unread</span></span>  <br/> |<span data-ttu-id="9074e-137">Поиск непрочитанных бесед.</span><span class="sxs-lookup"><span data-stu-id="9074e-137">Find unread conversations.</span></span>  <br/> |
|<span data-ttu-id="9074e-138">TaskActive</span><span class="sxs-lookup"><span data-stu-id="9074e-138">TaskActive</span></span>  <br/> |<span data-ttu-id="9074e-139">Поиск активных задач.</span><span class="sxs-lookup"><span data-stu-id="9074e-139">Find active tasks.</span></span>  <br/> |
|<span data-ttu-id="9074e-140">TaskOverdue</span><span class="sxs-lookup"><span data-stu-id="9074e-140">TaskOverdue</span></span>  <br/> |<span data-ttu-id="9074e-141">Найдите просроченные задачи.</span><span class="sxs-lookup"><span data-stu-id="9074e-141">Find overdue tasks.</span></span>  <br/> |
|<span data-ttu-id="9074e-142">TaskCompleted</span><span class="sxs-lookup"><span data-stu-id="9074e-142">TaskCompleted</span></span>  <br/> |<span data-ttu-id="9074e-143">Найдите завершенные задачи.</span><span class="sxs-lookup"><span data-stu-id="9074e-143">Find completed tasks.</span></span>  <br/> |
|<span data-ttu-id="9074e-144">NoClutter</span><span class="sxs-lookup"><span data-stu-id="9074e-144">NoClutter</span></span>  <br/> |<span data-ttu-id="9074e-145">Только для внутреннего использования.</span><span class="sxs-lookup"><span data-stu-id="9074e-145">For internal use only.</span></span>  <br/> |
|<span data-ttu-id="9074e-146">Засорение</span><span class="sxs-lookup"><span data-stu-id="9074e-146">Clutter</span></span>  <br/> |<span data-ttu-id="9074e-147">Только для внутреннего использования.</span><span class="sxs-lookup"><span data-stu-id="9074e-147">For internal use only.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="9074e-148">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="9074e-148">Child elements</span></span>

|<span data-ttu-id="9074e-149">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="9074e-149">**Element**</span></span>|<span data-ttu-id="9074e-150">**Описание**</span><span class="sxs-lookup"><span data-stu-id="9074e-150">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9074e-151">IndexedPageItemView</span><span class="sxs-lookup"><span data-stu-id="9074e-151">IndexedPageItemView</span></span>](indexedpageitemview.md) <br/> |<span data-ttu-id="9074e-152">Описывает как выгружаемый беседы возвращаются данные.</span><span class="sxs-lookup"><span data-stu-id="9074e-152">Describes how paged conversation information is returned.</span></span>  <br/> |
|[<span data-ttu-id="9074e-153">SeekToConditionPageItemView</span><span class="sxs-lookup"><span data-stu-id="9074e-153">SeekToConditionPageItemView</span></span>](seektoconditionpageitemview.md) <br/> |<span data-ttu-id="9074e-154">Указывает условие, используемый для идентификации в конце поиска, начальный индекс поиска, максимальное записей для возвращения и указания поиска для поиска **FindItem** или **FindConversation** .</span><span class="sxs-lookup"><span data-stu-id="9074e-154">Specifies the condition that is used to identify the end of a search, the starting index of a search, the maximum entries to return, and the search directions for a **FindItem** or **FindConversation** search.</span></span>  <br/> |
|[<span data-ttu-id="9074e-155">SortOrder</span><span class="sxs-lookup"><span data-stu-id="9074e-155">SortOrder</span></span>](sortorder.md) <br/> |<span data-ttu-id="9074e-156">Определяет порядок сортировки элементов в [FindConversation операции](findconversation-operation.md) запроса.</span><span class="sxs-lookup"><span data-stu-id="9074e-156">Defines how items are sorted in a [FindConversation operation](findconversation-operation.md) request.</span></span> <span data-ttu-id="9074e-157">Свойство **Беседы: LastDeliveryTime** — это единственный параметр, который поддерживается для сортировки при использовании операции **FindConversation** .</span><span class="sxs-lookup"><span data-stu-id="9074e-157">The **conversation:LastDeliveryTime** property is the only property that is supported for sorting when the **FindConversation** operation is used.</span></span>  <br/> |
|[<span data-ttu-id="9074e-158">ParentFolderId (TargetFolderIdType)</span><span class="sxs-lookup"><span data-stu-id="9074e-158">ParentFolderId (TargetFolderIdType)</span></span>](parentfolderid-targetfolderidtype.md) <br/> |<span data-ttu-id="9074e-159">Указывает папку для поиска бесед.</span><span class="sxs-lookup"><span data-stu-id="9074e-159">Identifies the folder to search for conversations.</span></span>  <br/> |
|[<span data-ttu-id="9074e-160">MailboxScope</span><span class="sxs-lookup"><span data-stu-id="9074e-160">MailboxScope</span></span>](mailboxscope.md) <br/> |<span data-ttu-id="9074e-161">Разрешение поиска или выборки для беседы должны охватывать основной почтовый ящик, архивного почтового ящика или обеих основной и архивировать почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="9074e-161">Specifies whether a search or fetch for a conversation should span either the primary mailbox, archive mailbox, or both the primary and archive mailbox.</span></span>  <br/> |
|[<span data-ttu-id="9074e-162">Строка запроса (QueryStringType)</span><span class="sxs-lookup"><span data-stu-id="9074e-162">QueryString (QueryStringType)</span></span>](querystring-querystringtype.md) <br/> |<span data-ttu-id="9074e-163">Указывает строку запроса почтовых ящиков на основе на расширенный синтаксис запроса (AQS).</span><span class="sxs-lookup"><span data-stu-id="9074e-163">Specifies a mailbox query string based on Advanced Query Syntax (AQS).</span></span>  <br/> |
|[<span data-ttu-id="9074e-164">ConversationShape</span><span class="sxs-lookup"><span data-stu-id="9074e-164">ConversationShape</span></span>](conversationshape.md) <br/> |<span data-ttu-id="9074e-165">Определяет свойство, задайте для возврата в ответ на [операцию FindConversation](findconversation-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="9074e-165">Identifies the property set to return in a [FindConversation operation](findconversation-operation.md) response.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="9074e-166">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="9074e-166">Parent elements</span></span>

<span data-ttu-id="9074e-167">Нет.</span><span class="sxs-lookup"><span data-stu-id="9074e-167">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="9074e-168">Замечания</span><span class="sxs-lookup"><span data-stu-id="9074e-168">Remarks</span></span>

<span data-ttu-id="9074e-169">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.Этот элемент появился в Exchange Server 2010 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="9074e-169">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9074e-170">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="9074e-170">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9074e-171">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="9074e-171">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="9074e-172">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="9074e-172">Schema Name</span></span>  <br/> |<span data-ttu-id="9074e-173">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="9074e-173">Messages schema</span></span>  <br/> |
|<span data-ttu-id="9074e-174">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="9074e-174">Validation File</span></span>  <br/> |<span data-ttu-id="9074e-175">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="9074e-175">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="9074e-176">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="9074e-176">Can be Empty</span></span>  <br/> |<span data-ttu-id="9074e-177">False</span><span class="sxs-lookup"><span data-stu-id="9074e-177">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9074e-178">См. также</span><span class="sxs-lookup"><span data-stu-id="9074e-178">See also</span></span>



[<span data-ttu-id="9074e-179">FindConversation Operation</span><span class="sxs-lookup"><span data-stu-id="9074e-179">FindConversation operation</span></span>](findconversation-operation.md)


- [<span data-ttu-id="9074e-180">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="9074e-180">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="9074e-181">Conversations in EWS</span><span class="sxs-lookup"><span data-stu-id="9074e-181">Conversations in EWS</span></span>](http://msdn.microsoft.com/library/91e64629-db6c-4c94-9dcb-d386232e8467%28Office.15%29.aspx)

