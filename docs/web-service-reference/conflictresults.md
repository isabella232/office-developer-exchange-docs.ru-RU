---
title: ConflictResults
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ConflictResults
api_type:
- schema
ms.assetid: 08cdd547-4de7-4c7a-b60f-e618dc217d20
description: Элемент ConflictResults содержит число конфликтов в ответ UpdateItem операции.
ms.openlocfilehash: faa6dc6c5fbbe874438a89c810a12fa675e8a1c9
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761715"
---
# <a name="conflictresults"></a><span data-ttu-id="a8d34-103">ConflictResults</span><span class="sxs-lookup"><span data-stu-id="a8d34-103">ConflictResults</span></span>

<span data-ttu-id="a8d34-104">Элемент [ConflictResults](conflictresults.md) содержит число конфликтов в ответ [UpdateItem операции](updateitem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="a8d34-104">The [ConflictResults](conflictresults.md) element contains the number of conflicts in an [UpdateItem operation](updateitem-operation.md) response.</span></span> 
  
[<span data-ttu-id="a8d34-105">UpdateItemResponse</span><span class="sxs-lookup"><span data-stu-id="a8d34-105">UpdateItemResponse</span></span>](updateitemresponse.md)
  
[<span data-ttu-id="a8d34-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="a8d34-106">ResponseMessages</span></span>](responsemessages.md)
  
[<span data-ttu-id="a8d34-107">UpdateItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="a8d34-107">UpdateItemResponseMessage</span></span>](updateitemresponsemessage.md)
  
[<span data-ttu-id="a8d34-108">ConflictResults</span><span class="sxs-lookup"><span data-stu-id="a8d34-108">ConflictResults</span></span>](conflictresults.md)
  
```xml
<ConflictResults>
   <Count/>
</ConflictResults>
```

 <span data-ttu-id="a8d34-109">**ConflictResultsType**</span><span class="sxs-lookup"><span data-stu-id="a8d34-109">**ConflictResultsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a8d34-110">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="a8d34-110">Attributes and elements</span></span>

<span data-ttu-id="a8d34-111">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="a8d34-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a8d34-112">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="a8d34-112">Attributes</span></span>

<span data-ttu-id="a8d34-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="a8d34-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a8d34-114">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="a8d34-114">Child elements</span></span>

|<span data-ttu-id="a8d34-115">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="a8d34-115">**Element**</span></span>|<span data-ttu-id="a8d34-116">**Описание**</span><span class="sxs-lookup"><span data-stu-id="a8d34-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a8d34-117">Count</span><span class="sxs-lookup"><span data-stu-id="a8d34-117">Count</span></span>](count.md) <br/> |<span data-ttu-id="a8d34-118">Содержит число конфликтов в ответ [UpdateItem операции](updateitem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="a8d34-118">Contains the number of conflicts in an [UpdateItem operation](updateitem-operation.md) response.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="a8d34-119">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="a8d34-119">Parent elements</span></span>

|<span data-ttu-id="a8d34-120">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="a8d34-120">**Element**</span></span>|<span data-ttu-id="a8d34-121">**Описание**</span><span class="sxs-lookup"><span data-stu-id="a8d34-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a8d34-122">UpdateItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="a8d34-122">UpdateItemResponseMessage</span></span>](updateitemresponsemessage.md) <br/> |<span data-ttu-id="a8d34-123">Содержит состояние и результат одного запроса [UpdateItem операции](updateitem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="a8d34-123">Contains the status and result of a single [UpdateItem operation](updateitem-operation.md) request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="a8d34-124">Замечания</span><span class="sxs-lookup"><span data-stu-id="a8d34-124">Remarks</span></span>

<span data-ttu-id="a8d34-125">Схема, описывающая этот элемент находится в виртуальном каталоге EWS компьютера, на котором работает Exchange Server с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="a8d34-125">The schema that describes this element is located in the EWS virtual directory of the computer that is running Exchange Server with the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a8d34-126">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="a8d34-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a8d34-127">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="a8d34-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="a8d34-128">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="a8d34-128">Schema Name</span></span>  <br/> |<span data-ttu-id="a8d34-129">Схема Types</span><span class="sxs-lookup"><span data-stu-id="a8d34-129">Types schema</span></span>  <br/> |
|<span data-ttu-id="a8d34-130">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="a8d34-130">Validation File</span></span>  <br/> |<span data-ttu-id="a8d34-131">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="a8d34-131">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="a8d34-132">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="a8d34-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="a8d34-133">False</span><span class="sxs-lookup"><span data-stu-id="a8d34-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a8d34-134">См. также</span><span class="sxs-lookup"><span data-stu-id="a8d34-134">See also</span></span>



[<span data-ttu-id="a8d34-135">UpdateItem Operation</span><span class="sxs-lookup"><span data-stu-id="a8d34-135">UpdateItem operation</span></span>](updateitem-operation.md)
  
 <span data-ttu-id="a8d34-136">**ConflictResultsType**</span><span class="sxs-lookup"><span data-stu-id="a8d34-136">**ConflictResultsType**</span></span>

