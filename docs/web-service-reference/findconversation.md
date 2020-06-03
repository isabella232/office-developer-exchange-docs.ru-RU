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
description: Элемент FindConversation определяет запрос на поиск бесед в почтовом ящике.
ms.openlocfilehash: 98d692132ed9375d981c95d24600b0e2c4b1d8c1
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462649"
---
# <a name="findconversation"></a><span data-ttu-id="8d5c2-103">FindConversation</span><span class="sxs-lookup"><span data-stu-id="8d5c2-103">FindConversation</span></span>

<span data-ttu-id="8d5c2-104">Элемент **FindConversation** определяет запрос на поиск бесед в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="8d5c2-104">The **FindConversation** element defines a request to find conversations in a mailbox.</span></span> 
  
[<span data-ttu-id="8d5c2-105">FindConversation</span><span class="sxs-lookup"><span data-stu-id="8d5c2-105">FindConversation</span></span>](findconversation.md)
  
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

 <span data-ttu-id="8d5c2-106">**финдконверсатионтипе**</span><span class="sxs-lookup"><span data-stu-id="8d5c2-106">**FindConversationType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8d5c2-107">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="8d5c2-107">Attributes and elements</span></span>

<span data-ttu-id="8d5c2-108">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="8d5c2-108">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8d5c2-109">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="8d5c2-109">Attributes</span></span>

****

|<span data-ttu-id="8d5c2-110">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="8d5c2-110">**Attribute**</span></span>|<span data-ttu-id="8d5c2-111">**Описание**</span><span class="sxs-lookup"><span data-stu-id="8d5c2-111">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="8d5c2-112">Обход</span><span class="sxs-lookup"><span data-stu-id="8d5c2-112">Traversal</span></span>  <br/> |<span data-ttu-id="8d5c2-113">Определяет типы обхода вложенного дерева.</span><span class="sxs-lookup"><span data-stu-id="8d5c2-113">Identifies the types of sub-tree traversal.</span></span> <span data-ttu-id="8d5c2-114">Этот атрибут является необязательным.</span><span class="sxs-lookup"><span data-stu-id="8d5c2-114">This attribute is optional.</span></span>  <br/> |
|<span data-ttu-id="8d5c2-115">виевфилтер</span><span class="sxs-lookup"><span data-stu-id="8d5c2-115">ViewFilter</span></span>  <br/> |<span data-ttu-id="8d5c2-116">Определяет фильтры представления типов.</span><span class="sxs-lookup"><span data-stu-id="8d5c2-116">Identifies the types view filters.</span></span> <span data-ttu-id="8d5c2-117">Этот атрибут является необязательным.</span><span class="sxs-lookup"><span data-stu-id="8d5c2-117">This attribute is optional.</span></span>  <br/> |
   
#### <a name="traversal-attribute-values"></a><span data-ttu-id="8d5c2-118">Значения атрибутов обхода</span><span class="sxs-lookup"><span data-stu-id="8d5c2-118">Traversal attribute values</span></span>

****

|<span data-ttu-id="8d5c2-119">**Значение**</span><span class="sxs-lookup"><span data-stu-id="8d5c2-119">**Value**</span></span>|<span data-ttu-id="8d5c2-120">**Описание**</span><span class="sxs-lookup"><span data-stu-id="8d5c2-120">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="8d5c2-121">Поверхност</span><span class="sxs-lookup"><span data-stu-id="8d5c2-121">Shallow</span></span>  <br/> |<span data-ttu-id="8d5c2-122">Обозначает неполную обходов.</span><span class="sxs-lookup"><span data-stu-id="8d5c2-122">Indicates a shallow traversal.</span></span>  <br/> |
|<span data-ttu-id="8d5c2-123">Углублен</span><span class="sxs-lookup"><span data-stu-id="8d5c2-123">Deep</span></span>  <br/> |<span data-ttu-id="8d5c2-124">Указывает на глубокий обход.</span><span class="sxs-lookup"><span data-stu-id="8d5c2-124">Indicates a deep traversal.</span></span>  <br/> |
   
#### <a name="viewfilter-attribute-values"></a><span data-ttu-id="8d5c2-125">Значения атрибутов Виевфилтер</span><span class="sxs-lookup"><span data-stu-id="8d5c2-125">ViewFilter attribute values</span></span>

****

|<span data-ttu-id="8d5c2-126">**Значение**</span><span class="sxs-lookup"><span data-stu-id="8d5c2-126">**Value**</span></span>|<span data-ttu-id="8d5c2-127">**Описание**</span><span class="sxs-lookup"><span data-stu-id="8d5c2-127">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="8d5c2-128">Все</span><span class="sxs-lookup"><span data-stu-id="8d5c2-128">All</span></span>  <br/> |<span data-ttu-id="8d5c2-129">Поиск всех бесед.</span><span class="sxs-lookup"><span data-stu-id="8d5c2-129">Find all conversations.</span></span>  <br/> |
|<span data-ttu-id="8d5c2-130">Отмеченные</span><span class="sxs-lookup"><span data-stu-id="8d5c2-130">Flagged</span></span>  <br/> |<span data-ttu-id="8d5c2-131">Поиск помеченных бесед.</span><span class="sxs-lookup"><span data-stu-id="8d5c2-131">Find flagged conversations.</span></span>  <br/> |
|<span data-ttu-id="8d5c2-132">HasAttachment</span><span class="sxs-lookup"><span data-stu-id="8d5c2-132">HasAttachment</span></span>  <br/> |<span data-ttu-id="8d5c2-133">Поиск бесед с вложениями.</span><span class="sxs-lookup"><span data-stu-id="8d5c2-133">Find conversations with attachments.</span></span>  <br/> |
|<span data-ttu-id="8d5c2-134">турккме</span><span class="sxs-lookup"><span data-stu-id="8d5c2-134">ToOrCcMe</span></span>  <br/> |<span data-ttu-id="8d5c2-135">Поиск бесед, адресованных или получателей CC.</span><span class="sxs-lookup"><span data-stu-id="8d5c2-135">Find conversations addressed or cc'd to me.</span></span>  <br/> |
|<span data-ttu-id="8d5c2-136">Unread</span><span class="sxs-lookup"><span data-stu-id="8d5c2-136">Unread</span></span>  <br/> |<span data-ttu-id="8d5c2-137">Поиск непрочитанных бесед.</span><span class="sxs-lookup"><span data-stu-id="8d5c2-137">Find unread conversations.</span></span>  <br/> |
|<span data-ttu-id="8d5c2-138">таскактиве</span><span class="sxs-lookup"><span data-stu-id="8d5c2-138">TaskActive</span></span>  <br/> |<span data-ttu-id="8d5c2-139">Поиск активных задач.</span><span class="sxs-lookup"><span data-stu-id="8d5c2-139">Find active tasks.</span></span>  <br/> |
|<span data-ttu-id="8d5c2-140">тасковердуе</span><span class="sxs-lookup"><span data-stu-id="8d5c2-140">TaskOverdue</span></span>  <br/> |<span data-ttu-id="8d5c2-141">Поиск просроченных задач.</span><span class="sxs-lookup"><span data-stu-id="8d5c2-141">Find overdue tasks.</span></span>  <br/> |
|<span data-ttu-id="8d5c2-142">тасккомплетед</span><span class="sxs-lookup"><span data-stu-id="8d5c2-142">TaskCompleted</span></span>  <br/> |<span data-ttu-id="8d5c2-143">Поиск завершенных задач.</span><span class="sxs-lookup"><span data-stu-id="8d5c2-143">Find completed tasks.</span></span>  <br/> |
|<span data-ttu-id="8d5c2-144">Функция "несрочные"</span><span class="sxs-lookup"><span data-stu-id="8d5c2-144">NoClutter</span></span>  <br/> |<span data-ttu-id="8d5c2-145">Только для внутреннего использования.</span><span class="sxs-lookup"><span data-stu-id="8d5c2-145">For internal use only.</span></span>  <br/> |
|<span data-ttu-id="8d5c2-146">Папка "Несрочные"</span><span class="sxs-lookup"><span data-stu-id="8d5c2-146">Clutter</span></span>  <br/> |<span data-ttu-id="8d5c2-147">Только для внутреннего использования.</span><span class="sxs-lookup"><span data-stu-id="8d5c2-147">For internal use only.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="8d5c2-148">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="8d5c2-148">Child elements</span></span>

|<span data-ttu-id="8d5c2-149">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="8d5c2-149">**Element**</span></span>|<span data-ttu-id="8d5c2-150">**Описание**</span><span class="sxs-lookup"><span data-stu-id="8d5c2-150">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8d5c2-151">индекседпажеитемвиев</span><span class="sxs-lookup"><span data-stu-id="8d5c2-151">IndexedPageItemView</span></span>](indexedpageitemview.md) <br/> |<span data-ttu-id="8d5c2-152">Описывает, как возвращаются сведения о страничной беседе.</span><span class="sxs-lookup"><span data-stu-id="8d5c2-152">Describes how paged conversation information is returned.</span></span>  <br/> |
|[<span data-ttu-id="8d5c2-153">сиктокондитионпажеитемвиев</span><span class="sxs-lookup"><span data-stu-id="8d5c2-153">SeekToConditionPageItemView</span></span>](seektoconditionpageitemview.md) <br/> |<span data-ttu-id="8d5c2-154">Задает условие, используемое для определения конца поиска, начального индекса поиска, максимальных возвращаемых значений и направления поиска для поиска **FindItem** или **FindConversation** .</span><span class="sxs-lookup"><span data-stu-id="8d5c2-154">Specifies the condition that is used to identify the end of a search, the starting index of a search, the maximum entries to return, and the search directions for a **FindItem** or **FindConversation** search.</span></span>  <br/> |
|[<span data-ttu-id="8d5c2-155">SortOrder</span><span class="sxs-lookup"><span data-stu-id="8d5c2-155">SortOrder</span></span>](sortorder.md) <br/> |<span data-ttu-id="8d5c2-156">Определяет порядок сортировки элементов в запросе [операции FindConversation](findconversation-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="8d5c2-156">Defines how items are sorted in a [FindConversation operation](findconversation-operation.md) request.</span></span> <span data-ttu-id="8d5c2-157">Свойство **CONVERSATION: ластделиверитиме** — единственное свойство, которое поддерживается для сортировки при использовании операции **FindConversation** .</span><span class="sxs-lookup"><span data-stu-id="8d5c2-157">The **conversation:LastDeliveryTime** property is the only property that is supported for sorting when the **FindConversation** operation is used.</span></span>  <br/> |
|[<span data-ttu-id="8d5c2-158">ParentFolderId (Таржетфолдеридтипе)</span><span class="sxs-lookup"><span data-stu-id="8d5c2-158">ParentFolderId (TargetFolderIdType)</span></span>](parentfolderid-targetfolderidtype.md) <br/> |<span data-ttu-id="8d5c2-159">Определяет папку для поиска обсуждений.</span><span class="sxs-lookup"><span data-stu-id="8d5c2-159">Identifies the folder to search for conversations.</span></span>  <br/> |
|[<span data-ttu-id="8d5c2-160">маилбоксскопе</span><span class="sxs-lookup"><span data-stu-id="8d5c2-160">MailboxScope</span></span>](mailboxscope.md) <br/> |<span data-ttu-id="8d5c2-161">Указывает, следует ли выполнять поиск или выборку для беседы: в основном почтовом ящике, архивном почтовом ящике или основном и архивном почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="8d5c2-161">Specifies whether a search or fetch for a conversation should span either the primary mailbox, archive mailbox, or both the primary and archive mailbox.</span></span>  <br/> |
|[<span data-ttu-id="8d5c2-162">Строка запроса (Куеристрингтипе)</span><span class="sxs-lookup"><span data-stu-id="8d5c2-162">QueryString (QueryStringType)</span></span>](querystring-querystringtype.md) <br/> |<span data-ttu-id="8d5c2-163">Указывает строку запроса к почтовому ящику на основе расширенного синтаксиса запросов (AQS).</span><span class="sxs-lookup"><span data-stu-id="8d5c2-163">Specifies a mailbox query string based on Advanced Query Syntax (AQS).</span></span>  <br/> |
|[<span data-ttu-id="8d5c2-164">конверсатионшапе</span><span class="sxs-lookup"><span data-stu-id="8d5c2-164">ConversationShape</span></span>](conversationshape.md) <br/> |<span data-ttu-id="8d5c2-165">Определяет значение свойства, возвращаемого в ответе [операции FindConversation](findconversation-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="8d5c2-165">Identifies the property set to return in a [FindConversation operation](findconversation-operation.md) response.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="8d5c2-166">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="8d5c2-166">Parent elements</span></span>

<span data-ttu-id="8d5c2-167">Нет.</span><span class="sxs-lookup"><span data-stu-id="8d5c2-167">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="8d5c2-168">Примечания</span><span class="sxs-lookup"><span data-stu-id="8d5c2-168">Remarks</span></span>

<span data-ttu-id="8d5c2-169">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.Этот элемент появился в Exchange Server 2010 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="8d5c2-169">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8d5c2-170">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="8d5c2-170">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8d5c2-171">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="8d5c2-171">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="8d5c2-172">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="8d5c2-172">Schema Name</span></span>  <br/> |<span data-ttu-id="8d5c2-173">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="8d5c2-173">Messages schema</span></span>  <br/> |
|<span data-ttu-id="8d5c2-174">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="8d5c2-174">Validation File</span></span>  <br/> |<span data-ttu-id="8d5c2-175">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="8d5c2-175">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="8d5c2-176">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="8d5c2-176">Can be Empty</span></span>  <br/> |<span data-ttu-id="8d5c2-177">False</span><span class="sxs-lookup"><span data-stu-id="8d5c2-177">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="8d5c2-178">См. также</span><span class="sxs-lookup"><span data-stu-id="8d5c2-178">See also</span></span>



[<span data-ttu-id="8d5c2-179">Операция FindConversation</span><span class="sxs-lookup"><span data-stu-id="8d5c2-179">FindConversation operation</span></span>](findconversation-operation.md)


- [<span data-ttu-id="8d5c2-180">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="8d5c2-180">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="8d5c2-181">Conversations in EWS</span><span class="sxs-lookup"><span data-stu-id="8d5c2-181">Conversations in EWS</span></span>](https://msdn.microsoft.com/library/91e64629-db6c-4c94-9dcb-d386232e8467%28Office.15%29.aspx)

