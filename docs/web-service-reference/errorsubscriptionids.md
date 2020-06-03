---
title: еррорсубскриптионидс
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ErrorSubscriptionIds
api_type:
- schema
ms.assetid: e64e76ff-4d98-4082-9acc-a1114ae45f44
description: Элемент Еррорсубскриптионидс содержит массив недопустимых идентификаторов подписки.
ms.openlocfilehash: bdc5c86560800464d677a9043607bed3f7872e32
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44526188"
---
# <a name="errorsubscriptionids"></a><span data-ttu-id="14332-103">еррорсубскриптионидс</span><span class="sxs-lookup"><span data-stu-id="14332-103">ErrorSubscriptionIds</span></span>

<span data-ttu-id="14332-104">Элемент **еррорсубскриптионидс** содержит массив недопустимых идентификаторов подписки.</span><span class="sxs-lookup"><span data-stu-id="14332-104">The **ErrorSubscriptionIds** element contains an array of invalid subscription IDs.</span></span> 
  
```xml
<ErrorSubscriptionIds>
   <SubscriptionId/>
</ErrorSubscriptionIds>
```

 <span data-ttu-id="14332-105">**нонемптяррайофсубскриптионидстипе**</span><span class="sxs-lookup"><span data-stu-id="14332-105">**NonEmptyArrayOfSubscriptionIdsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="14332-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="14332-106">Attributes and elements</span></span>

<span data-ttu-id="14332-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="14332-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="14332-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="14332-108">Attributes</span></span>

<span data-ttu-id="14332-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="14332-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="14332-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="14332-110">Child elements</span></span>

|<span data-ttu-id="14332-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="14332-111">**Element**</span></span>|<span data-ttu-id="14332-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="14332-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="14332-113">SubscriptionId (Events)</span><span class="sxs-lookup"><span data-stu-id="14332-113">SubscriptionId (GetEvents)</span></span>](subscriptionid-getevents.md) <br/> |<span data-ttu-id="14332-114">Представляет идентификатор подписки.</span><span class="sxs-lookup"><span data-stu-id="14332-114">Represents the identifier for a subscription.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="14332-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="14332-115">Parent elements</span></span>

|<span data-ttu-id="14332-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="14332-116">**Element**</span></span>|<span data-ttu-id="14332-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="14332-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="14332-118">жетстреаминжевентсреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="14332-118">GetStreamingEventsResponseMessage</span></span>](getstreamingeventsresponsemessage.md) <br/> |<span data-ttu-id="14332-119">Содержит состояние и результат одного запроса [операции GetStreamingEvents](getstreamingevents-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="14332-119">Contains the status and result of a single [GetStreamingEvents operation](getstreamingevents-operation.md) request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="14332-120">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="14332-120">Text value</span></span>

<span data-ttu-id="14332-121">Нет.</span><span class="sxs-lookup"><span data-stu-id="14332-121">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="14332-122">Примечания</span><span class="sxs-lookup"><span data-stu-id="14332-122">Remarks</span></span>

<span data-ttu-id="14332-123">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.Этот элемент появился в Exchange Server 2010 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="14332-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="14332-124">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="14332-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="14332-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="14332-125">Namespace</span></span>  <br/> |<span data-ttu-id="14332-126">https://schemas.microsoft.com/exchange/services/2006/messages и https://schemas.microsoft.com/exchange/services/2006/types</span><span class="sxs-lookup"><span data-stu-id="14332-126">https://schemas.microsoft.com/exchange/services/2006/messages and https://schemas.microsoft.com/exchange/services/2006/types</span></span>  <br/> |
|<span data-ttu-id="14332-127">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="14332-127">Schema Name</span></span>  <br/> |<span data-ttu-id="14332-128">Схема сообщений; Схема Types</span><span class="sxs-lookup"><span data-stu-id="14332-128">Messages schema; Types schema</span></span>  <br/> |
|<span data-ttu-id="14332-129">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="14332-129">Validation File</span></span>  <br/> |<span data-ttu-id="14332-130">Messages. xsd; Types. xsd</span><span class="sxs-lookup"><span data-stu-id="14332-130">Messages.xsd; Types.xsd</span></span>  <br/> |
|<span data-ttu-id="14332-131">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="14332-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="14332-132">False</span><span class="sxs-lookup"><span data-stu-id="14332-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="14332-133">См. также</span><span class="sxs-lookup"><span data-stu-id="14332-133">See also</span></span>



[<span data-ttu-id="14332-134">Операция GetStreamingEvents</span><span class="sxs-lookup"><span data-stu-id="14332-134">GetStreamingEvents operation</span></span>](getstreamingevents-operation.md)


- [<span data-ttu-id="14332-135">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="14332-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

