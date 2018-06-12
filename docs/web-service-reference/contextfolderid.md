---
title: ContextFolderId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ContextFolderId
api_type:
- schema
ms.assetid: 48de92aa-e124-42b5-89bc-cdce5e93d78b
description: Элемент ContextFolderId указывает папку, предназначенное для действий, использующих папок. Этот элемент должен присутствовать при копирование, удаление, перемещение и настройка состояние чтения элементов беседы в целевой папке.
ms.openlocfilehash: bd863d0395b9b9d7b437833acfb656fec4580985
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761800"
---
# <a name="contextfolderid"></a><span data-ttu-id="3bb14-104">ContextFolderId</span><span class="sxs-lookup"><span data-stu-id="3bb14-104">ContextFolderId</span></span>

<span data-ttu-id="3bb14-105">Элемент **ContextFolderId** указывает папку, предназначенное для действий, использующих папок.</span><span class="sxs-lookup"><span data-stu-id="3bb14-105">The **ContextFolderId** element indicates the folder that is targeted for actions that use folders.</span></span> <span data-ttu-id="3bb14-106">Этот элемент должен присутствовать при копирование, удаление, перемещение и настройка состояние чтения элементов беседы в целевой папке.</span><span class="sxs-lookup"><span data-stu-id="3bb14-106">This element must be present when copying, deleting, moving, and setting read state on conversation items in a target folder.</span></span> 
  
[<span data-ttu-id="3bb14-107">ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="3bb14-107">ApplyConversationAction</span></span>](applyconversationaction.md)
  
[<span data-ttu-id="3bb14-108">ConversationActions</span><span class="sxs-lookup"><span data-stu-id="3bb14-108">ConversationActions</span></span>](conversationactions.md)
  
[<span data-ttu-id="3bb14-109">ConversationAction</span><span class="sxs-lookup"><span data-stu-id="3bb14-109">ConversationAction</span></span>](conversationaction.md)
  
[<span data-ttu-id="3bb14-110">ContextFolderId</span><span class="sxs-lookup"><span data-stu-id="3bb14-110">ContextFolderId</span></span>](contextfolderid.md)
  
```XML
<ContextFolderId>
   <FolderId/>
</ContextFolderId>
```

 <span data-ttu-id="3bb14-111">**TargetFolderIdType**</span><span class="sxs-lookup"><span data-stu-id="3bb14-111">**TargetFolderIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3bb14-112">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="3bb14-112">Attributes and elements</span></span>

<span data-ttu-id="3bb14-113">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="3bb14-113">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3bb14-114">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="3bb14-114">Attributes</span></span>

<span data-ttu-id="3bb14-115">Нет.</span><span class="sxs-lookup"><span data-stu-id="3bb14-115">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3bb14-116">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="3bb14-116">Child elements</span></span>

|<span data-ttu-id="3bb14-117">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="3bb14-117">**Element**</span></span>|<span data-ttu-id="3bb14-118">**Описание**</span><span class="sxs-lookup"><span data-stu-id="3bb14-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3bb14-119">FolderId</span><span class="sxs-lookup"><span data-stu-id="3bb14-119">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="3bb14-120">Содержит идентификатор и меняет ключ контекстной папки.</span><span class="sxs-lookup"><span data-stu-id="3bb14-120">Contains the identifier and change key of the context folder.</span></span>  <br/> |
|[<span data-ttu-id="3bb14-121">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="3bb14-121">DistinguishedFolderId</span></span>](distinguishedfolderid.md) <br/> |<span data-ttu-id="3bb14-122">Идентифицирует папки, которые можно ссылаться по имени.</span><span class="sxs-lookup"><span data-stu-id="3bb14-122">Identifies folders that can be referenced by name.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="3bb14-123">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="3bb14-123">Parent elements</span></span>

|<span data-ttu-id="3bb14-124">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="3bb14-124">**Element**</span></span>|<span data-ttu-id="3bb14-125">**Описание**</span><span class="sxs-lookup"><span data-stu-id="3bb14-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3bb14-126">ConversationAction</span><span class="sxs-lookup"><span data-stu-id="3bb14-126">ConversationAction</span></span>](conversationaction.md) <br/> |<span data-ttu-id="3bb14-127">Содержит одно действие должен применяться к разговора.</span><span class="sxs-lookup"><span data-stu-id="3bb14-127">Contains a single action to be applied to a single conversation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="3bb14-128">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="3bb14-128">Text value</span></span>

<span data-ttu-id="3bb14-129">Нет.</span><span class="sxs-lookup"><span data-stu-id="3bb14-129">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="3bb14-130">Замечания</span><span class="sxs-lookup"><span data-stu-id="3bb14-130">Remarks</span></span>

<span data-ttu-id="3bb14-131">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.Этот элемент появился в Exchange Server 2010 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="3bb14-131">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3bb14-132">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="3bb14-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3bb14-133">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="3bb14-133">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="3bb14-134">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="3bb14-134">Schema Name</span></span>  <br/> |<span data-ttu-id="3bb14-135">Схема Types</span><span class="sxs-lookup"><span data-stu-id="3bb14-135">Types schema</span></span>  <br/> |
|<span data-ttu-id="3bb14-136">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="3bb14-136">Validation File</span></span>  <br/> |<span data-ttu-id="3bb14-137">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="3bb14-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="3bb14-138">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="3bb14-138">Can be Empty</span></span>  <br/> |<span data-ttu-id="3bb14-139">False</span><span class="sxs-lookup"><span data-stu-id="3bb14-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3bb14-140">См. также</span><span class="sxs-lookup"><span data-stu-id="3bb14-140">See also</span></span>



[<span data-ttu-id="3bb14-141">Операция ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="3bb14-141">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)

