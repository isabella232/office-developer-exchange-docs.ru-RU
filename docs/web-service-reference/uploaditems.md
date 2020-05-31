---
title: UploadItems
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UploadItems
api_type:
- schema
ms.assetid: fd2b9545-7213-4427-95ae-71a155b75971
description: Элемент UploadItems представляет запрос на отправку элементов в почтовый ящик.
ms.openlocfilehash: d3cd69cdb744431daeede736c2e156c8ab92a79b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19840388"
---
# <a name="uploaditems"></a><span data-ttu-id="44af8-103">UploadItems</span><span class="sxs-lookup"><span data-stu-id="44af8-103">UploadItems</span></span>

<span data-ttu-id="44af8-104">Элемент **UploadItems** представляет запрос на отправку элементов в почтовый ящик.</span><span class="sxs-lookup"><span data-stu-id="44af8-104">The **UploadItems** element represents a request to upload items into a mailbox.</span></span> 
  
[<span data-ttu-id="44af8-105">UploadItems</span><span class="sxs-lookup"><span data-stu-id="44af8-105">UploadItems</span></span>](uploaditems.md)
  
```XML
<UploadItems>
   <Items/>
</UploadItems>
```

 <span data-ttu-id="44af8-106">**уплоадитемстипе**</span><span class="sxs-lookup"><span data-stu-id="44af8-106">**UploadItemsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="44af8-107">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="44af8-107">Attributes and elements</span></span>

<span data-ttu-id="44af8-108">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="44af8-108">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="44af8-109">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="44af8-109">Attributes</span></span>

<span data-ttu-id="44af8-110">Нет.</span><span class="sxs-lookup"><span data-stu-id="44af8-110">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="44af8-111">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="44af8-111">Child elements</span></span>

|<span data-ttu-id="44af8-112">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="44af8-112">**Element**</span></span>|<span data-ttu-id="44af8-113">**Описание**</span><span class="sxs-lookup"><span data-stu-id="44af8-113">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="44af8-114">Элементы (Нонемптяррайофуплоадитемстипе)</span><span class="sxs-lookup"><span data-stu-id="44af8-114">Items (NonEmptyArrayOfUploadItemsType)</span></span>](items-nonemptyarrayofuploaditemstype.md) <br/> |<span data-ttu-id="44af8-115">Содержит массив элементов для отправки в почтовый ящик.</span><span class="sxs-lookup"><span data-stu-id="44af8-115">Contains an array of items to upload into a mailbox.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="44af8-116">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="44af8-116">Parent elements</span></span>

<span data-ttu-id="44af8-117">Нет.</span><span class="sxs-lookup"><span data-stu-id="44af8-117">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="44af8-118">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="44af8-118">Text value</span></span>

<span data-ttu-id="44af8-119">Нет.</span><span class="sxs-lookup"><span data-stu-id="44af8-119">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="44af8-120">Примечания</span><span class="sxs-lookup"><span data-stu-id="44af8-120">Remarks</span></span>

<span data-ttu-id="44af8-121">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.Этот элемент появился в Exchange Server 2010 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="44af8-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="44af8-122">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="44af8-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="44af8-123">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="44af8-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="44af8-124">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="44af8-124">Schema Name</span></span>  <br/> |<span data-ttu-id="44af8-125">Схема сообщения</span><span class="sxs-lookup"><span data-stu-id="44af8-125">Message schema</span></span>  <br/> |
|<span data-ttu-id="44af8-126">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="44af8-126">Validation File</span></span>  <br/> |<span data-ttu-id="44af8-127">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="44af8-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="44af8-128">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="44af8-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="44af8-129">False</span><span class="sxs-lookup"><span data-stu-id="44af8-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="44af8-130">См. также</span><span class="sxs-lookup"><span data-stu-id="44af8-130">See also</span></span>



[<span data-ttu-id="44af8-131">Операция ExportItems</span><span class="sxs-lookup"><span data-stu-id="44af8-131">ExportItems operation</span></span>](exportitems-operation.md)
  
[<span data-ttu-id="44af8-132">Операция UploadItems</span><span class="sxs-lookup"><span data-stu-id="44af8-132">UploadItems operation</span></span>](uploaditems-operation.md)

