---
title: Область (NonEmptyStringType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Scope
api_type:
- schema
ms.assetid: 7efb6fd9-1615-469e-96f6-0f7846ad9b44
description: Элемент области область отчета отслеживания сообщений.
ms.openlocfilehash: 534ed23916a60b246c7cb5be4a59d086980a7c37
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19835280"
---
# <a name="scope-nonemptystringtype"></a><span data-ttu-id="2e643-103">Область (NonEmptyStringType)</span><span class="sxs-lookup"><span data-stu-id="2e643-103">Scope (NonEmptyStringType)</span></span>

<span data-ttu-id="2e643-104">Элемент **области** область отчета отслеживания сообщений.</span><span class="sxs-lookup"><span data-stu-id="2e643-104">The **Scope** element specifies the scope of the message tracking report.</span></span> 
  
```XML
<Scope>Organization | Forest | Site</Scope>
```

 <span data-ttu-id="2e643-105">**NonEmptyStringType**</span><span class="sxs-lookup"><span data-stu-id="2e643-105">**NonEmptyStringType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2e643-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="2e643-106">Attributes and elements</span></span>

<span data-ttu-id="2e643-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="2e643-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2e643-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="2e643-108">Attributes</span></span>

<span data-ttu-id="2e643-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="2e643-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2e643-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="2e643-110">Child elements</span></span>

<span data-ttu-id="2e643-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="2e643-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="2e643-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="2e643-112">Parent elements</span></span>

<span data-ttu-id="2e643-113">[FindMessageTrackingReport](findmessagetrackingreport.md) | [GetMessageTrackingReport](getmessagetrackingreport.md)</span><span class="sxs-lookup"><span data-stu-id="2e643-113">[FindMessageTrackingReport](findmessagetrackingreport.md) | [GetMessageTrackingReport](getmessagetrackingreport.md)</span></span>
  
## <a name="text-value"></a><span data-ttu-id="2e643-114">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="2e643-114">Text value</span></span>

<span data-ttu-id="2e643-115">В следующей таблице перечислены возможные значения для элемента **области** .</span><span class="sxs-lookup"><span data-stu-id="2e643-115">The following table lists the possible values for the **Scope** element.</span></span> 
  
|<span data-ttu-id="2e643-116">**Значение**</span><span class="sxs-lookup"><span data-stu-id="2e643-116">**Value**</span></span>|<span data-ttu-id="2e643-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="2e643-117">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="2e643-118">Организация</span><span class="sxs-lookup"><span data-stu-id="2e643-118">Organization</span></span>  <br/> |<span data-ttu-id="2e643-119">Отслеживание областей сообщений диапазонов в организации.</span><span class="sxs-lookup"><span data-stu-id="2e643-119">The message tracking scopes spans across an organization.</span></span>  <br/> |
|<span data-ttu-id="2e643-120">Лес</span><span class="sxs-lookup"><span data-stu-id="2e643-120">Forest</span></span>  <br/> |<span data-ttu-id="2e643-121">Отслеживание областей сообщений охватывает лесу.</span><span class="sxs-lookup"><span data-stu-id="2e643-121">The message tracking scopes spans across a forest.</span></span>  <br/> |
|<span data-ttu-id="2e643-122">Сайт</span><span class="sxs-lookup"><span data-stu-id="2e643-122">Site</span></span>  <br/> |<span data-ttu-id="2e643-123">Отслеживание областей сообщений охватывает сайта.</span><span class="sxs-lookup"><span data-stu-id="2e643-123">The message tracking scopes spans across a site.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="2e643-124">Замечания</span><span class="sxs-lookup"><span data-stu-id="2e643-124">Remarks</span></span>

<span data-ttu-id="2e643-125">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="2e643-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2e643-126">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="2e643-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2e643-127">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="2e643-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="2e643-128">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="2e643-128">Schema Name</span></span>  <br/> |<span data-ttu-id="2e643-129">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="2e643-129">Messages schema</span></span>  <br/> |
|<span data-ttu-id="2e643-130">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="2e643-130">Validation File</span></span>  <br/> |<span data-ttu-id="2e643-131">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="2e643-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="2e643-132">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="2e643-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="2e643-133">False</span><span class="sxs-lookup"><span data-stu-id="2e643-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="2e643-134">См. также</span><span class="sxs-lookup"><span data-stu-id="2e643-134">See also</span></span>



- [<span data-ttu-id="2e643-135">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="2e643-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

