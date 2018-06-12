---
title: PermanentDelete
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- PermanentDelete
api_type:
- schema
ms.assetid: 1a0e0f46-1472-4eb7-bb54-f193a2603587
description: Элемент PermanentDelete указывает ли сообщений для окончательного удаления и не сохраняются в папку «Удаленные».
ms.openlocfilehash: 40cf80e054bb70a3f6d687e8d4361f1d4331a7f8
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19834724"
---
# <a name="permanentdelete"></a><span data-ttu-id="cc124-103">PermanentDelete</span><span class="sxs-lookup"><span data-stu-id="cc124-103">PermanentDelete</span></span>

<span data-ttu-id="cc124-104">Элемент **PermanentDelete** указывает ли сообщений для окончательного удаления и не сохраняются в папку «Удаленные».</span><span class="sxs-lookup"><span data-stu-id="cc124-104">The **PermanentDelete** element indicates whether messages are to be permanently deleted and not saved to the Deleted Items folder.</span></span> 
  
```XML
<PermanentDelete>true | false</PermanentDelete>
```

 <span data-ttu-id="cc124-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="cc124-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="cc124-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="cc124-106">Attributes and elements</span></span>

<span data-ttu-id="cc124-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="cc124-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="cc124-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="cc124-108">Attributes</span></span>

<span data-ttu-id="cc124-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="cc124-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="cc124-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="cc124-110">Child elements</span></span>

<span data-ttu-id="cc124-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="cc124-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="cc124-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="cc124-112">Parent elements</span></span>

|<span data-ttu-id="cc124-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="cc124-113">**Element**</span></span>|<span data-ttu-id="cc124-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="cc124-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cc124-115">Действия</span><span class="sxs-lookup"><span data-stu-id="cc124-115">Actions</span></span>](actions.md) <br/> |<span data-ttu-id="cc124-116">Представляет набор действий, которые доступны для выполнения на сообщение при условия будут выполнены.</span><span class="sxs-lookup"><span data-stu-id="cc124-116">Represents the set of actions that are available to be taken on a message when the conditions are fulfilled.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="cc124-117">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="cc124-117">Text value</span></span>

<span data-ttu-id="cc124-118">Текстовое значение **true,** указывает, что сообщения должны быть отмечены будут окончательно удалены.</span><span class="sxs-lookup"><span data-stu-id="cc124-118">A text value of **true** indicates that the message must be marked to be permanently deleted.</span></span> <span data-ttu-id="cc124-119">Значение **false** указывает, что сообщение не должны быть отмечены будут окончательно удалены.</span><span class="sxs-lookup"><span data-stu-id="cc124-119">A value of **false** indicates that the message must not be marked to be permanently deleted.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="cc124-120">Замечания</span><span class="sxs-lookup"><span data-stu-id="cc124-120">Remarks</span></span>

<span data-ttu-id="cc124-121">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="cc124-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="cc124-122">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="cc124-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="cc124-123">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="cc124-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="cc124-124">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="cc124-124">Schema Name</span></span>  <br/> |<span data-ttu-id="cc124-125">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="cc124-125">Messages schema</span></span>  <br/> |
|<span data-ttu-id="cc124-126">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="cc124-126">Validation File</span></span>  <br/> |<span data-ttu-id="cc124-127">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="cc124-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="cc124-128">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="cc124-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="cc124-129">True</span><span class="sxs-lookup"><span data-stu-id="cc124-129">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="cc124-130">См. также</span><span class="sxs-lookup"><span data-stu-id="cc124-130">See also</span></span>



- [<span data-ttu-id="cc124-131">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="cc124-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

