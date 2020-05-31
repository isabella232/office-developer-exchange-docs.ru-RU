---
title: контекстфолдерид
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
description: Элемент Контекстфолдерид указывает папку, предназначенную для действий, в которых используются папки. Этот элемент должен присутствовать при копировании, удалении, перемещении и установке состояния чтения элементов беседы в целевой папке.
ms.openlocfilehash: 94428a079be6da8873c777556771579a7110fb62
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/28/2018
ms.locfileid: "21354283"
---
# <a name="contextfolderid"></a><span data-ttu-id="50160-104">контекстфолдерид</span><span class="sxs-lookup"><span data-stu-id="50160-104">ContextFolderId</span></span>

<span data-ttu-id="50160-105">Элемент **контекстфолдерид** указывает папку, предназначенную для действий, в которых используются папки.</span><span class="sxs-lookup"><span data-stu-id="50160-105">The **ContextFolderId** element indicates the folder that is targeted for actions that use folders.</span></span> <span data-ttu-id="50160-106">Этот элемент должен присутствовать при копировании, удалении, перемещении и установке состояния чтения элементов беседы в целевой папке.</span><span class="sxs-lookup"><span data-stu-id="50160-106">This element must be present when copying, deleting, moving, and setting read state on conversation items in a target folder.</span></span> 
  
- [<span data-ttu-id="50160-107">ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="50160-107">ApplyConversationAction</span></span>](applyconversationaction.md) 
- [<span data-ttu-id="50160-108">конверсатионактионс</span><span class="sxs-lookup"><span data-stu-id="50160-108">ConversationActions</span></span>](conversationactions.md)
- [<span data-ttu-id="50160-109">конверсатионактион</span><span class="sxs-lookup"><span data-stu-id="50160-109">ConversationAction</span></span>](conversationaction.md)
- [<span data-ttu-id="50160-110">контекстфолдерид</span><span class="sxs-lookup"><span data-stu-id="50160-110">ContextFolderId</span></span>](contextfolderid.md)
  
```XML
<ContextFolderId>
   <FolderId/>
</ContextFolderId>
```

```XML
<ContextFolderId>
   <DistinguishedFolderId/>
</ContextFolderId>
```


<span data-ttu-id="50160-111">**таржетфолдеридтипе**</span><span class="sxs-lookup"><span data-stu-id="50160-111">**TargetFolderIdType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="50160-112">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="50160-112">Attributes and elements</span></span>

<span data-ttu-id="50160-113">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="50160-113">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="50160-114">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="50160-114">Attributes</span></span>

<span data-ttu-id="50160-115">Нет.</span><span class="sxs-lookup"><span data-stu-id="50160-115">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="50160-116">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="50160-116">Child elements</span></span>

|<span data-ttu-id="50160-117">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="50160-117">**Element**</span></span>|<span data-ttu-id="50160-118">**Описание**</span><span class="sxs-lookup"><span data-stu-id="50160-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="50160-119">FolderId</span><span class="sxs-lookup"><span data-stu-id="50160-119">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="50160-120">Содержит идентификатор и ключ изменения для папки контекста.</span><span class="sxs-lookup"><span data-stu-id="50160-120">Contains the identifier and change key of the context folder.</span></span>  <br/> |
|[<span data-ttu-id="50160-121">дистингуишедфолдерид</span><span class="sxs-lookup"><span data-stu-id="50160-121">DistinguishedFolderId</span></span>](distinguishedfolderid.md) <br/> |<span data-ttu-id="50160-122">Определяет папки, на которые можно ссылаться по имени.</span><span class="sxs-lookup"><span data-stu-id="50160-122">Identifies folders that can be referenced by name.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="50160-123">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="50160-123">Parent elements</span></span>

|<span data-ttu-id="50160-124">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="50160-124">**Element**</span></span>|<span data-ttu-id="50160-125">**Описание**</span><span class="sxs-lookup"><span data-stu-id="50160-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="50160-126">конверсатионактион</span><span class="sxs-lookup"><span data-stu-id="50160-126">ConversationAction</span></span>](conversationaction.md) <br/> |<span data-ttu-id="50160-127">Содержит одно действие, которое будет применено к одной беседе.</span><span class="sxs-lookup"><span data-stu-id="50160-127">Contains a single action to be applied to a single conversation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="50160-128">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="50160-128">Text value</span></span>

<span data-ttu-id="50160-129">Нет.</span><span class="sxs-lookup"><span data-stu-id="50160-129">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="50160-130">Примечания</span><span class="sxs-lookup"><span data-stu-id="50160-130">Remarks</span></span>

<span data-ttu-id="50160-131">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.Этот элемент появился в Exchange Server 2010 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="50160-131">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="50160-132">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="50160-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="50160-133">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="50160-133">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="50160-134">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="50160-134">Schema Name</span></span>  <br/> |<span data-ttu-id="50160-135">Схема Types</span><span class="sxs-lookup"><span data-stu-id="50160-135">Types schema</span></span>  <br/> |
|<span data-ttu-id="50160-136">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="50160-136">Validation File</span></span>  <br/> |<span data-ttu-id="50160-137">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="50160-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="50160-138">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="50160-138">Can be Empty</span></span>  <br/> |<span data-ttu-id="50160-139">False</span><span class="sxs-lookup"><span data-stu-id="50160-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="50160-140">См. также</span><span class="sxs-lookup"><span data-stu-id="50160-140">See also</span></span>

- [<span data-ttu-id="50160-141">Операция ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="50160-141">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)

