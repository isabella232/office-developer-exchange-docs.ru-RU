---
title: Итемидс (Нонемптяррайофитемидстипе)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ItemIds
api_type:
- schema
ms.assetid: e895782a-74fe-4216-8ac2-c3c88c4b232d
description: Элемент Итемидс содержит массив идентификаторов элементов, определяющих элементы для экспорта из почтового ящика.
ms.openlocfilehash: c6d48832c5435080c7cec8e43093ea60825b604a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834151"
---
# <a name="itemids-nonemptyarrayofitemidstype"></a><span data-ttu-id="dfc6d-103">Итемидс (Нонемптяррайофитемидстипе)</span><span class="sxs-lookup"><span data-stu-id="dfc6d-103">ItemIds (NonEmptyArrayOfItemIdsType)</span></span>

<span data-ttu-id="dfc6d-104">Элемент **итемидс** содержит массив идентификаторов элементов, определяющих элементы для экспорта из почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="dfc6d-104">The **ItemIds** element contains an array of item identifiers that identify the items to export from a mailbox.</span></span> 
  
[<span data-ttu-id="dfc6d-105">ExportItems</span><span class="sxs-lookup"><span data-stu-id="dfc6d-105">ExportItems</span></span>](exportitems.md)
  
[<span data-ttu-id="dfc6d-106">Итемидс (Нонемптяррайофитемидстипе)</span><span class="sxs-lookup"><span data-stu-id="dfc6d-106">ItemIds (NonEmptyArrayOfItemIdsType)</span></span>](itemids-nonemptyarrayofitemidstype.md)
  
```XML
<ItemIds>
   <ItemId/>
</ItemIds>
```

 <span data-ttu-id="dfc6d-107">**нонемптяррайофитемидстипе**</span><span class="sxs-lookup"><span data-stu-id="dfc6d-107">**NonEmptyArrayOfItemIdsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="dfc6d-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="dfc6d-108">Attributes and elements</span></span>

<span data-ttu-id="dfc6d-109">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="dfc6d-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="dfc6d-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="dfc6d-110">Attributes</span></span>

<span data-ttu-id="dfc6d-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="dfc6d-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="dfc6d-112">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="dfc6d-112">Child elements</span></span>

|<span data-ttu-id="dfc6d-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="dfc6d-113">**Element**</span></span>|<span data-ttu-id="dfc6d-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="dfc6d-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="dfc6d-115">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="dfc6d-115">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="dfc6d-116">Содержит уникальный идентификатор и ключ изменения элемента в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="dfc6d-116">Contains the unique identifier and change key of an item in the Exchange store.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="dfc6d-117">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="dfc6d-117">Parent elements</span></span>

|<span data-ttu-id="dfc6d-118">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="dfc6d-118">**Element**</span></span>|<span data-ttu-id="dfc6d-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="dfc6d-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="dfc6d-120">ExportItems</span><span class="sxs-lookup"><span data-stu-id="dfc6d-120">ExportItems</span></span>](exportitems.md) <br/> |<span data-ttu-id="dfc6d-121">Представляет запрос на экспорт элементов из почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="dfc6d-121">Represents a request to export items from a mailbox.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="dfc6d-122">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="dfc6d-122">Text value</span></span>

<span data-ttu-id="dfc6d-123">Нет.</span><span class="sxs-lookup"><span data-stu-id="dfc6d-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="dfc6d-124">Примечания</span><span class="sxs-lookup"><span data-stu-id="dfc6d-124">Remarks</span></span>

<span data-ttu-id="dfc6d-125">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.Этот элемент появился в Exchange Server 2010 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="dfc6d-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="dfc6d-126">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="dfc6d-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="dfc6d-127">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="dfc6d-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="dfc6d-128">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="dfc6d-128">Schema Name</span></span>  <br/> |<span data-ttu-id="dfc6d-129">Схема сообщения</span><span class="sxs-lookup"><span data-stu-id="dfc6d-129">Message schema</span></span>  <br/> |
|<span data-ttu-id="dfc6d-130">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="dfc6d-130">Validation File</span></span>  <br/> |<span data-ttu-id="dfc6d-131">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="dfc6d-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="dfc6d-132">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="dfc6d-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="dfc6d-133">False</span><span class="sxs-lookup"><span data-stu-id="dfc6d-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="dfc6d-134">См. также</span><span class="sxs-lookup"><span data-stu-id="dfc6d-134">See also</span></span>



[<span data-ttu-id="dfc6d-135">Операция ExportItems</span><span class="sxs-lookup"><span data-stu-id="dfc6d-135">ExportItems operation</span></span>](exportitems-operation.md)
  
[<span data-ttu-id="dfc6d-136">Операция UploadItems</span><span class="sxs-lookup"><span data-stu-id="dfc6d-136">UploadItems operation</span></span>](uploaditems-operation.md)

