---
title: ExchangeStoreId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 5acceb42-a757-4c74-ab1c-b1abf7bf1e0a
description: Элемент ExchangeStoreId указывает обмена мгновенными сообщениями идентификатор группы обмена Мгновенными сообщениями.
ms.openlocfilehash: 815e9c2f368558ea38efce3671dbdc33d4d97168
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762419"
---
# <a name="exchangestoreid"></a><span data-ttu-id="df061-103">ExchangeStoreId</span><span class="sxs-lookup"><span data-stu-id="df061-103">ExchangeStoreId</span></span>

<span data-ttu-id="df061-104">Элемент **ExchangeStoreId** указывает обмена мгновенными сообщениями идентификатор группы обмена Мгновенными сообщениями.</span><span class="sxs-lookup"><span data-stu-id="df061-104">The **ExchangeStoreId** element specifies the instant messaging (IM) group identifier.</span></span> 
  
```XML
<ExchangeStoreId Id="" ChangeKey=""/>
```

 <span data-ttu-id="df061-105">**ItemIdType**</span><span class="sxs-lookup"><span data-stu-id="df061-105">**ItemIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="df061-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="df061-106">Attributes and elements</span></span>

<span data-ttu-id="df061-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="df061-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="df061-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="df061-108">Attributes</span></span>

|<span data-ttu-id="df061-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="df061-109">**Attribute**</span></span>|<span data-ttu-id="df061-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="df061-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="df061-111">Id</span><span class="sxs-lookup"><span data-stu-id="df061-111">Id</span></span>  <br/> |<span data-ttu-id="df061-112">Текстовое значение атрибута **Id** является идентификатор группы.</span><span class="sxs-lookup"><span data-stu-id="df061-112">The text value of the **Id** attribute is the identifier of the group.</span></span>  <br/> |
|<span data-ttu-id="df061-113">ChangeKey</span><span class="sxs-lookup"><span data-stu-id="df061-113">ChangeKey</span></span>  <br/> |<span data-ttu-id="df061-114">Текстовое значение атрибута **ChangeKey** — это ключ изменения группы.</span><span class="sxs-lookup"><span data-stu-id="df061-114">The text value of the **ChangeKey** attribute is the change key of the group.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="df061-115">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="df061-115">Child elements</span></span>

<span data-ttu-id="df061-116">Нет.</span><span class="sxs-lookup"><span data-stu-id="df061-116">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="df061-117">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="df061-117">Parent elements</span></span>

|<span data-ttu-id="df061-118">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="df061-118">**Element**</span></span>|<span data-ttu-id="df061-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="df061-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="df061-120">ImGroup</span><span class="sxs-lookup"><span data-stu-id="df061-120">ImGroup</span></span>](imgroup.md) <br/> |<span data-ttu-id="df061-121">Представляет группу мгновенного обмена сообщениями.</span><span class="sxs-lookup"><span data-stu-id="df061-121">Represents an instant messaging group.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="df061-122">Замечания</span><span class="sxs-lookup"><span data-stu-id="df061-122">Remarks</span></span>

<span data-ttu-id="df061-123">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="df061-123">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="df061-124">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="df061-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="df061-125">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="df061-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="df061-126">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="df061-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="df061-127">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="df061-127">Schema Name</span></span>  <br/> |<span data-ttu-id="df061-128">Схема типа</span><span class="sxs-lookup"><span data-stu-id="df061-128">Type schema</span></span>  <br/> |
|<span data-ttu-id="df061-129">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="df061-129">Validation File</span></span>  <br/> |<span data-ttu-id="df061-130">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="df061-130">types.xsd</span></span>  <br/> |
|<span data-ttu-id="df061-131">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="df061-131">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="df061-132">См. также</span><span class="sxs-lookup"><span data-stu-id="df061-132">See also</span></span>



- [<span data-ttu-id="df061-133">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="df061-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

