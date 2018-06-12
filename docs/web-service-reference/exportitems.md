---
title: ExportItems
manager: sethgros
ms.date: 09/17/2015
ms.audience: ITPro
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ExportItems
api_type:
- schema
ms.assetid: bbbc56e4-8cc1-43ae-b70a-9a8d6bb0f399
description: Элемент ExportItems представляет запрос для экспорта элементов из почтового ящика.
ms.openlocfilehash: 055012166bb125dfcf86070f2e23496bf0209b51
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762435"
---
# <a name="exportitems"></a><span data-ttu-id="be3ab-103">ExportItems</span><span class="sxs-lookup"><span data-stu-id="be3ab-103">ExportItems</span></span>

<span data-ttu-id="be3ab-104">Элемент **ExportItems** представляет запрос для экспорта элементов из почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="be3ab-104">The **ExportItems** element represents a request to export items from a mailbox.</span></span> 
  
[<span data-ttu-id="be3ab-105">ExportItems</span><span class="sxs-lookup"><span data-stu-id="be3ab-105">ExportItems</span></span>](exportitems.md)
  
```XML
<ExportItems>
   <ItemIds/>
</ExportItems>
```

 <span data-ttu-id="be3ab-106">**ExportItemsType**</span><span class="sxs-lookup"><span data-stu-id="be3ab-106">**ExportItemsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="be3ab-107">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="be3ab-107">Attributes and elements</span></span>

<span data-ttu-id="be3ab-108">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="be3ab-108">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="be3ab-109">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="be3ab-109">Attributes</span></span>

<span data-ttu-id="be3ab-110">Нет.</span><span class="sxs-lookup"><span data-stu-id="be3ab-110">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="be3ab-111">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="be3ab-111">Child elements</span></span>

|<span data-ttu-id="be3ab-112">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="be3ab-112">**Element**</span></span>|<span data-ttu-id="be3ab-113">**Описание**</span><span class="sxs-lookup"><span data-stu-id="be3ab-113">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="be3ab-114">Что ItemID (NonEmptyArrayOfItemIdsType)</span><span class="sxs-lookup"><span data-stu-id="be3ab-114">ItemIds (NonEmptyArrayOfItemIdsType)</span></span>](itemids-nonemptyarrayofitemidstype.md) <br/> |<span data-ttu-id="be3ab-115">Содержит массив идентификаторов элементов, определите, какие элементы из почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="be3ab-115">Contains an array of item identifiers that identify the items to export from a mailbox.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="be3ab-116">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="be3ab-116">Parent elements</span></span>

<span data-ttu-id="be3ab-117">Нет.</span><span class="sxs-lookup"><span data-stu-id="be3ab-117">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="be3ab-118">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="be3ab-118">Text value</span></span>

<span data-ttu-id="be3ab-119">Нет.</span><span class="sxs-lookup"><span data-stu-id="be3ab-119">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="be3ab-120">Замечания</span><span class="sxs-lookup"><span data-stu-id="be3ab-120">Remarks</span></span>

<span data-ttu-id="be3ab-121">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.Этот элемент появился в Exchange Server 2010 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="be3ab-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="be3ab-122">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="be3ab-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="be3ab-123">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="be3ab-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="be3ab-124">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="be3ab-124">Schema Name</span></span>  <br/> |<span data-ttu-id="be3ab-125">Схема сообщения</span><span class="sxs-lookup"><span data-stu-id="be3ab-125">Message schema</span></span>  <br/> |
|<span data-ttu-id="be3ab-126">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="be3ab-126">Validation File</span></span>  <br/> |<span data-ttu-id="be3ab-127">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="be3ab-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="be3ab-128">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="be3ab-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="be3ab-129">False</span><span class="sxs-lookup"><span data-stu-id="be3ab-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="be3ab-130">См. также</span><span class="sxs-lookup"><span data-stu-id="be3ab-130">See also</span></span>



[<span data-ttu-id="be3ab-131">Операция ExportItems</span><span class="sxs-lookup"><span data-stu-id="be3ab-131">ExportItems operation</span></span>](exportitems-operation.md)
  
[<span data-ttu-id="be3ab-132">Операция UploadItems</span><span class="sxs-lookup"><span data-stu-id="be3ab-132">UploadItems operation</span></span>](uploaditems-operation.md)

