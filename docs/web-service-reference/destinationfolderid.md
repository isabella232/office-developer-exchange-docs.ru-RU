---
title: дестинатионфолдерид
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DestinationFolderId
api_type:
- schema
ms.assetid: 77d2d222-320b-4aab-88e4-934ef177f55c
description: Элемент Дестинатионфолдерид указывает папку назначения для действий по копированию и перемещению.
ms.openlocfilehash: bfbacb9c82a681c7963ab5164c43cbb648e726cd
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/28/2018
ms.locfileid: "21353380"
---
# <a name="destinationfolderid"></a><span data-ttu-id="33fe4-103">дестинатионфолдерид</span><span class="sxs-lookup"><span data-stu-id="33fe4-103">DestinationFolderId</span></span>

<span data-ttu-id="33fe4-104">Элемент **дестинатионфолдерид** указывает папку назначения для действий по копированию и перемещению.</span><span class="sxs-lookup"><span data-stu-id="33fe4-104">The **DestinationFolderId** element indicates the destination folder for copy and move actions.</span></span> 
  
- [<span data-ttu-id="33fe4-105">ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="33fe4-105">ApplyConversationAction</span></span>](applyconversationaction.md)  
- [<span data-ttu-id="33fe4-106">конверсатионактионс</span><span class="sxs-lookup"><span data-stu-id="33fe4-106">ConversationActions</span></span>](conversationactions.md) 
- [<span data-ttu-id="33fe4-107">конверсатионактион</span><span class="sxs-lookup"><span data-stu-id="33fe4-107">ConversationAction</span></span>](conversationaction.md)  
- [<span data-ttu-id="33fe4-108">дестинатионфолдерид</span><span class="sxs-lookup"><span data-stu-id="33fe4-108">DestinationFolderId</span></span>](destinationfolderid.md)
  
```XML
<DestinationFolderId>
   <FolderId/>
</DestinationFolderId>
```

```XML
<DestinationFolderId>
   <DistinguishedFolderId/>
</DestinationFolderId>
```

<span data-ttu-id="33fe4-109">**таржетфолдеридтипе**</span><span class="sxs-lookup"><span data-stu-id="33fe4-109">**TargetFolderIdType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="33fe4-110">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="33fe4-110">Attributes and elements</span></span>

<span data-ttu-id="33fe4-111">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="33fe4-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="33fe4-112">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="33fe4-112">Attributes</span></span>

<span data-ttu-id="33fe4-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="33fe4-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="33fe4-114">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="33fe4-114">Child elements</span></span>

|<span data-ttu-id="33fe4-115">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="33fe4-115">**Element**</span></span>|<span data-ttu-id="33fe4-116">**Описание**</span><span class="sxs-lookup"><span data-stu-id="33fe4-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="33fe4-117">FolderId</span><span class="sxs-lookup"><span data-stu-id="33fe4-117">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="33fe4-118">Содержит идентификатор и ключ изменения конечной папки.</span><span class="sxs-lookup"><span data-stu-id="33fe4-118">Contains the identifier and change key of the destination folder.</span></span>  <br/> |
|[<span data-ttu-id="33fe4-119">дистингуишедфолдерид</span><span class="sxs-lookup"><span data-stu-id="33fe4-119">DistinguishedFolderId</span></span>](distinguishedfolderid.md) <br/> |<span data-ttu-id="33fe4-120">Определяет папки, на которые можно ссылаться по имени.</span><span class="sxs-lookup"><span data-stu-id="33fe4-120">Identifies folders that can be referenced by name.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="33fe4-121">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="33fe4-121">Parent elements</span></span>

|<span data-ttu-id="33fe4-122">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="33fe4-122">**Element**</span></span>|<span data-ttu-id="33fe4-123">**Описание**</span><span class="sxs-lookup"><span data-stu-id="33fe4-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="33fe4-124">конверсатионактион</span><span class="sxs-lookup"><span data-stu-id="33fe4-124">ConversationAction</span></span>](conversationaction.md) <br/> |<span data-ttu-id="33fe4-125">Содержит одно действие, которое будет применено к одной беседе.</span><span class="sxs-lookup"><span data-stu-id="33fe4-125">Contains a single action to be applied to a single conversation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="33fe4-126">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="33fe4-126">Text value</span></span>

<span data-ttu-id="33fe4-127">Нет.</span><span class="sxs-lookup"><span data-stu-id="33fe4-127">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="33fe4-128">Примечания</span><span class="sxs-lookup"><span data-stu-id="33fe4-128">Remarks</span></span>

<span data-ttu-id="33fe4-129">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.Этот элемент появился в Exchange Server 2010 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="33fe4-129">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="33fe4-130">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="33fe4-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="33fe4-131">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="33fe4-131">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="33fe4-132">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="33fe4-132">Schema Name</span></span>  <br/> |<span data-ttu-id="33fe4-133">Схема Types</span><span class="sxs-lookup"><span data-stu-id="33fe4-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="33fe4-134">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="33fe4-134">Validation File</span></span>  <br/> |<span data-ttu-id="33fe4-135">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="33fe4-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="33fe4-136">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="33fe4-136">Can be Empty</span></span>  <br/> |<span data-ttu-id="33fe4-137">False</span><span class="sxs-lookup"><span data-stu-id="33fe4-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="33fe4-138">См. также</span><span class="sxs-lookup"><span data-stu-id="33fe4-138">See also</span></span>

- [<span data-ttu-id="33fe4-139">Операция ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="33fe4-139">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)

