---
title: пропосеневтиме
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 6d5977ac-484e-4e53-92ba-58a868eb3395
description: Элемент Пропосеневтиме указывает объект Response, указывающий на то, что участник собрания может предложить новое время проведения собрания.
ms.openlocfilehash: 76f590db760826aa2cd26938947a9b0e02a603f7
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465543"
---
# <a name="proposenewtime"></a><span data-ttu-id="e0cf5-103">пропосеневтиме</span><span class="sxs-lookup"><span data-stu-id="e0cf5-103">ProposeNewTime</span></span>

<span data-ttu-id="e0cf5-104">Элемент **пропосеневтиме** указывает объект Response, указывающий на то, что участник собрания может предложить новое время проведения собрания.</span><span class="sxs-lookup"><span data-stu-id="e0cf5-104">The **ProposeNewTime** element specifies a response object that indicates that the meeting attendee can propose a new meeting time.</span></span> 
  
```XML
<ProposeNewTime ObjectName=""></ProposeNewTime>
```

 <span data-ttu-id="e0cf5-105">**пропосеневтиметипе**</span><span class="sxs-lookup"><span data-stu-id="e0cf5-105">**ProposeNewTimeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e0cf5-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="e0cf5-106">Attributes and elements</span></span>

<span data-ttu-id="e0cf5-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="e0cf5-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e0cf5-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="e0cf5-108">Attributes</span></span>

****

|<span data-ttu-id="e0cf5-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="e0cf5-109">**Attribute**</span></span>|<span data-ttu-id="e0cf5-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="e0cf5-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="e0cf5-111">ObjectName</span><span class="sxs-lookup"><span data-stu-id="e0cf5-111">ObjectName</span></span>  <br/> |<span data-ttu-id="e0cf5-112">Имя объекта ответа.</span><span class="sxs-lookup"><span data-stu-id="e0cf5-112">The name of the response object.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="e0cf5-113">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="e0cf5-113">Child elements</span></span>

<span data-ttu-id="e0cf5-114">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="e0cf5-114">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="e0cf5-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="e0cf5-115">Parent elements</span></span>

[<span data-ttu-id="e0cf5-116">респонсеобжектс</span><span class="sxs-lookup"><span data-stu-id="e0cf5-116">ResponseObjects</span></span>](responseobjects.md)
  
## <a name="remarks"></a><span data-ttu-id="e0cf5-117">Примечания</span><span class="sxs-lookup"><span data-stu-id="e0cf5-117">Remarks</span></span>

<span data-ttu-id="e0cf5-118">Этот элемент появился в Exchange Server 2013 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="e0cf5-118">This element was introduced in Exchange Server 2013 Service Pack 1 (SP1).</span></span>
  
<span data-ttu-id="e0cf5-119">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="e0cf5-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e0cf5-120">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="e0cf5-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e0cf5-121">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="e0cf5-121">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e0cf5-122">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="e0cf5-122">Schema Name</span></span>  <br/> |<span data-ttu-id="e0cf5-123">Схема Types</span><span class="sxs-lookup"><span data-stu-id="e0cf5-123">Types schema</span></span>  <br/> |
|<span data-ttu-id="e0cf5-124">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="e0cf5-124">Validation File</span></span>  <br/> |<span data-ttu-id="e0cf5-125">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="e0cf5-125">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="e0cf5-126">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="e0cf5-126">Can be Empty</span></span>  <br/> |<span data-ttu-id="e0cf5-127">True</span><span class="sxs-lookup"><span data-stu-id="e0cf5-127">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e0cf5-128">См. также</span><span class="sxs-lookup"><span data-stu-id="e0cf5-128">See also</span></span>



[<span data-ttu-id="e0cf5-129">респонсеобжектс</span><span class="sxs-lookup"><span data-stu-id="e0cf5-129">ResponseObjects</span></span>](responseobjects.md)


- [<span data-ttu-id="e0cf5-130">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="e0cf5-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

