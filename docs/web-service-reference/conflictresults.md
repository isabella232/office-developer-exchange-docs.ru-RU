---
title: конфликтресултс
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
description: Элемент Конфликтресултс содержит количество конфликтов в ответе операции UpdateItem.
ms.openlocfilehash: 923c7950e21039adf28e232486f4df5fc04889d1
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460171"
---
# <a name="conflictresults"></a><span data-ttu-id="aa9a6-103">конфликтресултс</span><span class="sxs-lookup"><span data-stu-id="aa9a6-103">ConflictResults</span></span>

<span data-ttu-id="aa9a6-104">Элемент [конфликтресултс](conflictresults.md) содержит количество конфликтов в ответе [операции UpdateItem](updateitem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="aa9a6-104">The [ConflictResults](conflictresults.md) element contains the number of conflicts in an [UpdateItem operation](updateitem-operation.md) response.</span></span> 
  
[<span data-ttu-id="aa9a6-105">упдатеитемреспонсе</span><span class="sxs-lookup"><span data-stu-id="aa9a6-105">UpdateItemResponse</span></span>](updateitemresponse.md)
  
[<span data-ttu-id="aa9a6-106">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="aa9a6-106">ResponseMessages</span></span>](responsemessages.md)
  
[<span data-ttu-id="aa9a6-107">упдатеитемреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="aa9a6-107">UpdateItemResponseMessage</span></span>](updateitemresponsemessage.md)
  
[<span data-ttu-id="aa9a6-108">конфликтресултс</span><span class="sxs-lookup"><span data-stu-id="aa9a6-108">ConflictResults</span></span>](conflictresults.md)
  
```xml
<ConflictResults>
   <Count/>
</ConflictResults>
```

 <span data-ttu-id="aa9a6-109">**конфликтресултстипе**</span><span class="sxs-lookup"><span data-stu-id="aa9a6-109">**ConflictResultsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="aa9a6-110">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="aa9a6-110">Attributes and elements</span></span>

<span data-ttu-id="aa9a6-111">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="aa9a6-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="aa9a6-112">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="aa9a6-112">Attributes</span></span>

<span data-ttu-id="aa9a6-113">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="aa9a6-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="aa9a6-114">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="aa9a6-114">Child elements</span></span>

|<span data-ttu-id="aa9a6-115">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="aa9a6-115">**Element**</span></span>|<span data-ttu-id="aa9a6-116">**Описание**</span><span class="sxs-lookup"><span data-stu-id="aa9a6-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="aa9a6-117">Count</span><span class="sxs-lookup"><span data-stu-id="aa9a6-117">Count</span></span>](count.md) <br/> |<span data-ttu-id="aa9a6-118">Содержит количество конфликтов в отклике [операции UpdateItem](updateitem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="aa9a6-118">Contains the number of conflicts in an [UpdateItem operation](updateitem-operation.md) response.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="aa9a6-119">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="aa9a6-119">Parent elements</span></span>

|<span data-ttu-id="aa9a6-120">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="aa9a6-120">**Element**</span></span>|<span data-ttu-id="aa9a6-121">**Описание**</span><span class="sxs-lookup"><span data-stu-id="aa9a6-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="aa9a6-122">упдатеитемреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="aa9a6-122">UpdateItemResponseMessage</span></span>](updateitemresponsemessage.md) <br/> |<span data-ttu-id="aa9a6-123">Содержит состояние и результат одного запроса [операции UpdateItem](updateitem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="aa9a6-123">Contains the status and result of a single [UpdateItem operation](updateitem-operation.md) request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="aa9a6-124">Примечания</span><span class="sxs-lookup"><span data-stu-id="aa9a6-124">Remarks</span></span>

<span data-ttu-id="aa9a6-125">Схема, описывающая этот элемент, находится в виртуальном каталоге EWS компьютера, на котором установлен сервер Exchange Server с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="aa9a6-125">The schema that describes this element is located in the EWS virtual directory of the computer that is running Exchange Server with the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="aa9a6-126">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="aa9a6-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="aa9a6-127">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="aa9a6-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="aa9a6-128">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="aa9a6-128">Schema Name</span></span>  <br/> |<span data-ttu-id="aa9a6-129">Схема Types</span><span class="sxs-lookup"><span data-stu-id="aa9a6-129">Types schema</span></span>  <br/> |
|<span data-ttu-id="aa9a6-130">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="aa9a6-130">Validation File</span></span>  <br/> |<span data-ttu-id="aa9a6-131">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="aa9a6-131">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="aa9a6-132">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="aa9a6-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="aa9a6-133">False</span><span class="sxs-lookup"><span data-stu-id="aa9a6-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="aa9a6-134">См. также</span><span class="sxs-lookup"><span data-stu-id="aa9a6-134">See also</span></span>



[<span data-ttu-id="aa9a6-135">Операция UpdateItem</span><span class="sxs-lookup"><span data-stu-id="aa9a6-135">UpdateItem operation</span></span>](updateitem-operation.md)
  
 <span data-ttu-id="aa9a6-136">**конфликтресултстипе**</span><span class="sxs-lookup"><span data-stu-id="aa9a6-136">**ConflictResultsType**</span></span>

