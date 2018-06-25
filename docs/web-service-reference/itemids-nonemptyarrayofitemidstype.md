---
title: Что ItemID (NonEmptyArrayOfItemIdsType)
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
description: Что ItemID элемент содержит массив идентификаторов элементов, определите, какие элементы из почтового ящика.
ms.openlocfilehash: c6d48832c5435080c7cec8e43093ea60825b604a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834151"
---
# <a name="itemids-nonemptyarrayofitemidstype"></a><span data-ttu-id="9e97a-103">Что ItemID (NonEmptyArrayOfItemIdsType)</span><span class="sxs-lookup"><span data-stu-id="9e97a-103">ItemIds (NonEmptyArrayOfItemIdsType)</span></span>

<span data-ttu-id="9e97a-104">**Что ItemID** элемент содержит массив идентификаторов элементов, определите, какие элементы из почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="9e97a-104">The **ItemIds** element contains an array of item identifiers that identify the items to export from a mailbox.</span></span> 
  
[<span data-ttu-id="9e97a-105">ExportItems</span><span class="sxs-lookup"><span data-stu-id="9e97a-105">ExportItems</span></span>](exportitems.md)
  
[<span data-ttu-id="9e97a-106">Что ItemID (NonEmptyArrayOfItemIdsType)</span><span class="sxs-lookup"><span data-stu-id="9e97a-106">ItemIds (NonEmptyArrayOfItemIdsType)</span></span>](itemids-nonemptyarrayofitemidstype.md)
  
```XML
<ItemIds>
   <ItemId/>
</ItemIds>
```

 <span data-ttu-id="9e97a-107">**NonEmptyArrayOfItemIdsType**</span><span class="sxs-lookup"><span data-stu-id="9e97a-107">**NonEmptyArrayOfItemIdsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9e97a-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="9e97a-108">Attributes and elements</span></span>

<span data-ttu-id="9e97a-109">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="9e97a-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9e97a-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="9e97a-110">Attributes</span></span>

<span data-ttu-id="9e97a-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="9e97a-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9e97a-112">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="9e97a-112">Child elements</span></span>

|<span data-ttu-id="9e97a-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="9e97a-113">**Element**</span></span>|<span data-ttu-id="9e97a-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="9e97a-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9e97a-115">Идентификатор элемента</span><span class="sxs-lookup"><span data-stu-id="9e97a-115">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="9e97a-116">Содержит уникальный идентификатор и меняет ключ элемента в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="9e97a-116">Contains the unique identifier and change key of an item in the Exchange store.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="9e97a-117">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="9e97a-117">Parent elements</span></span>

|<span data-ttu-id="9e97a-118">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="9e97a-118">**Element**</span></span>|<span data-ttu-id="9e97a-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="9e97a-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9e97a-120">ExportItems</span><span class="sxs-lookup"><span data-stu-id="9e97a-120">ExportItems</span></span>](exportitems.md) <br/> |<span data-ttu-id="9e97a-121">Представляет запрос для экспорта элементов из почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="9e97a-121">Represents a request to export items from a mailbox.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="9e97a-122">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="9e97a-122">Text value</span></span>

<span data-ttu-id="9e97a-123">Нет.</span><span class="sxs-lookup"><span data-stu-id="9e97a-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="9e97a-124">Замечания</span><span class="sxs-lookup"><span data-stu-id="9e97a-124">Remarks</span></span>

<span data-ttu-id="9e97a-125">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.Этот элемент появился в Exchange Server 2010 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="9e97a-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9e97a-126">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="9e97a-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9e97a-127">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="9e97a-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="9e97a-128">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="9e97a-128">Schema Name</span></span>  <br/> |<span data-ttu-id="9e97a-129">Схема сообщения</span><span class="sxs-lookup"><span data-stu-id="9e97a-129">Message schema</span></span>  <br/> |
|<span data-ttu-id="9e97a-130">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="9e97a-130">Validation File</span></span>  <br/> |<span data-ttu-id="9e97a-131">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="9e97a-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="9e97a-132">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="9e97a-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="9e97a-133">False</span><span class="sxs-lookup"><span data-stu-id="9e97a-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9e97a-134">См. также</span><span class="sxs-lookup"><span data-stu-id="9e97a-134">See also</span></span>



[<span data-ttu-id="9e97a-135">Операция ExportItems</span><span class="sxs-lookup"><span data-stu-id="9e97a-135">ExportItems operation</span></span>](exportitems-operation.md)
  
[<span data-ttu-id="9e97a-136">Операция UploadItems</span><span class="sxs-lookup"><span data-stu-id="9e97a-136">UploadItems operation</span></span>](uploaditems-operation.md)

