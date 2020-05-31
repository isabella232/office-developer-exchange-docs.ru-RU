---
title: Область действия (Нонемптистрингтипе)
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
description: Элемент SCOPE определяет область отчета об отслеживании сообщений.
ms.openlocfilehash: 534ed23916a60b246c7cb5be4a59d086980a7c37
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835280"
---
# <a name="scope-nonemptystringtype"></a><span data-ttu-id="7f9d1-103">Область действия (Нонемптистрингтипе)</span><span class="sxs-lookup"><span data-stu-id="7f9d1-103">Scope (NonEmptyStringType)</span></span>

<span data-ttu-id="7f9d1-104">Элемент **Scope** определяет область отчета об отслеживании сообщений.</span><span class="sxs-lookup"><span data-stu-id="7f9d1-104">The **Scope** element specifies the scope of the message tracking report.</span></span> 
  
```XML
<Scope>Organization | Forest | Site</Scope>
```

 <span data-ttu-id="7f9d1-105">**нонемптистрингтипе**</span><span class="sxs-lookup"><span data-stu-id="7f9d1-105">**NonEmptyStringType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7f9d1-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="7f9d1-106">Attributes and elements</span></span>

<span data-ttu-id="7f9d1-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="7f9d1-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7f9d1-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="7f9d1-108">Attributes</span></span>

<span data-ttu-id="7f9d1-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="7f9d1-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7f9d1-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="7f9d1-110">Child elements</span></span>

<span data-ttu-id="7f9d1-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="7f9d1-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="7f9d1-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="7f9d1-112">Parent elements</span></span>

<span data-ttu-id="7f9d1-113">[FindMessageTrackingReport](findmessagetrackingreport.md) | [GetMessageTrackingReport](getmessagetrackingreport.md)</span><span class="sxs-lookup"><span data-stu-id="7f9d1-113">[FindMessageTrackingReport](findmessagetrackingreport.md) | [GetMessageTrackingReport](getmessagetrackingreport.md)</span></span>
  
## <a name="text-value"></a><span data-ttu-id="7f9d1-114">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="7f9d1-114">Text value</span></span>

<span data-ttu-id="7f9d1-115">В следующей таблице приведены возможные значения для элемента **Scope** .</span><span class="sxs-lookup"><span data-stu-id="7f9d1-115">The following table lists the possible values for the **Scope** element.</span></span> 
  
|<span data-ttu-id="7f9d1-116">**Значение**</span><span class="sxs-lookup"><span data-stu-id="7f9d1-116">**Value**</span></span>|<span data-ttu-id="7f9d1-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="7f9d1-117">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="7f9d1-118">Организация</span><span class="sxs-lookup"><span data-stu-id="7f9d1-118">Organization</span></span>  <br/> |<span data-ttu-id="7f9d1-119">Области отслеживания сообщений охватываются в пределах организации.</span><span class="sxs-lookup"><span data-stu-id="7f9d1-119">The message tracking scopes spans across an organization.</span></span>  <br/> |
|<span data-ttu-id="7f9d1-120">Лес</span><span class="sxs-lookup"><span data-stu-id="7f9d1-120">Forest</span></span>  <br/> |<span data-ttu-id="7f9d1-121">Области отслеживания сообщений охватываются в пределах леса.</span><span class="sxs-lookup"><span data-stu-id="7f9d1-121">The message tracking scopes spans across a forest.</span></span>  <br/> |
|<span data-ttu-id="7f9d1-122">Site</span><span class="sxs-lookup"><span data-stu-id="7f9d1-122">Site</span></span>  <br/> |<span data-ttu-id="7f9d1-123">Области отслеживания сообщений охватываются на сайте.</span><span class="sxs-lookup"><span data-stu-id="7f9d1-123">The message tracking scopes spans across a site.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="7f9d1-124">Примечания</span><span class="sxs-lookup"><span data-stu-id="7f9d1-124">Remarks</span></span>

<span data-ttu-id="7f9d1-125">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="7f9d1-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7f9d1-126">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="7f9d1-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7f9d1-127">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="7f9d1-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="7f9d1-128">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="7f9d1-128">Schema Name</span></span>  <br/> |<span data-ttu-id="7f9d1-129">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="7f9d1-129">Messages schema</span></span>  <br/> |
|<span data-ttu-id="7f9d1-130">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="7f9d1-130">Validation File</span></span>  <br/> |<span data-ttu-id="7f9d1-131">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="7f9d1-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="7f9d1-132">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="7f9d1-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="7f9d1-133">False</span><span class="sxs-lookup"><span data-stu-id="7f9d1-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7f9d1-134">См. также</span><span class="sxs-lookup"><span data-stu-id="7f9d1-134">See also</span></span>



- [<span data-ttu-id="7f9d1-135">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="7f9d1-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

