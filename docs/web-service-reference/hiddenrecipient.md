---
title: хидденреЦипиент
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- HiddenRecipient
api_type:
- schema
ms.assetid: a8209f75-0070-4424-8dcd-273cfd192728
description: Элемент ХидденреЦипиент указывает, что получатель был добавлен политикой Организации, которая должна быть скрыта от непривилегированных пользователей.
ms.openlocfilehash: bfe57fabc02ff00c801672b71ccdb0bf1b916bd9
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457643"
---
# <a name="hiddenrecipient"></a><span data-ttu-id="764be-103">хидденреЦипиент</span><span class="sxs-lookup"><span data-stu-id="764be-103">HiddenRecipient</span></span>

<span data-ttu-id="764be-104">Элемент **хидденреЦипиент** указывает, что получатель был добавлен политикой Организации, которая должна быть скрыта от непривилегированных пользователей.</span><span class="sxs-lookup"><span data-stu-id="764be-104">The **HiddenRecipient** element indicates that the recipient was added by an organization policy that should be hidden from unprivileged users.</span></span> 
  
```XML
<HiddenRecipient>true | false</HiddenRecipient>
```

 <span data-ttu-id="764be-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="764be-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="764be-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="764be-106">Attributes and elements</span></span>

<span data-ttu-id="764be-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="764be-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="764be-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="764be-108">Attributes</span></span>

<span data-ttu-id="764be-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="764be-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="764be-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="764be-110">Child elements</span></span>

<span data-ttu-id="764be-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="764be-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="764be-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="764be-112">Parent elements</span></span>

|<span data-ttu-id="764be-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="764be-113">**Element**</span></span>|<span data-ttu-id="764be-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="764be-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="764be-115">реЦипиенттраккинжевент</span><span class="sxs-lookup"><span data-stu-id="764be-115">RecipientTrackingEvent</span></span>](recipienttrackingevent.md) <br/> |<span data-ttu-id="764be-116">Содержит сведения об отдельном событии получателя.</span><span class="sxs-lookup"><span data-stu-id="764be-116">Contains information for a single event for a recipient.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="764be-117">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="764be-117">Text value</span></span>

<span data-ttu-id="764be-118">Этот элемент может иметь **значение true** или **false**.</span><span class="sxs-lookup"><span data-stu-id="764be-118">This element can be either **true** or **false**.</span></span> <span data-ttu-id="764be-119">Значение **true** указывает, что пользователь был добавлен политикой Организации; значение **false** указывает, что пользователь не был добавлен политикой Организации.</span><span class="sxs-lookup"><span data-stu-id="764be-119">A value of **true** indicates that the user was added by an organization policy; a value of **false** indicates that the user was not added by an organization policy.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="764be-120">Примечания</span><span class="sxs-lookup"><span data-stu-id="764be-120">Remarks</span></span>

<span data-ttu-id="764be-121">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="764be-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="764be-122">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="764be-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="764be-123">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="764be-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="764be-124">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="764be-124">Schema Name</span></span>  <br/> |<span data-ttu-id="764be-125">Схема Types</span><span class="sxs-lookup"><span data-stu-id="764be-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="764be-126">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="764be-126">Validation File</span></span>  <br/> |<span data-ttu-id="764be-127">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="764be-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="764be-128">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="764be-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="764be-129">False</span><span class="sxs-lookup"><span data-stu-id="764be-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="764be-130">См. также</span><span class="sxs-lookup"><span data-stu-id="764be-130">See also</span></span>



- [<span data-ttu-id="764be-131">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="764be-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

