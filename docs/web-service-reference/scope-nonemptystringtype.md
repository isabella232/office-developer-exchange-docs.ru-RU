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
ms.openlocfilehash: f86f6198e84e094e61ee569f6d005549316bbb9b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44466943"
---
# <a name="scope-nonemptystringtype"></a><span data-ttu-id="997e0-103">Область действия (Нонемптистрингтипе)</span><span class="sxs-lookup"><span data-stu-id="997e0-103">Scope (NonEmptyStringType)</span></span>

<span data-ttu-id="997e0-104">Элемент **Scope** определяет область отчета об отслеживании сообщений.</span><span class="sxs-lookup"><span data-stu-id="997e0-104">The **Scope** element specifies the scope of the message tracking report.</span></span> 
  
```XML
<Scope>Organization | Forest | Site</Scope>
```

 <span data-ttu-id="997e0-105">**нонемптистрингтипе**</span><span class="sxs-lookup"><span data-stu-id="997e0-105">**NonEmptyStringType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="997e0-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="997e0-106">Attributes and elements</span></span>

<span data-ttu-id="997e0-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="997e0-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="997e0-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="997e0-108">Attributes</span></span>

<span data-ttu-id="997e0-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="997e0-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="997e0-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="997e0-110">Child elements</span></span>

<span data-ttu-id="997e0-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="997e0-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="997e0-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="997e0-112">Parent elements</span></span>

<span data-ttu-id="997e0-113">[FindMessageTrackingReport](findmessagetrackingreport.md)  |  [GetMessageTrackingReport](getmessagetrackingreport.md)</span><span class="sxs-lookup"><span data-stu-id="997e0-113">[FindMessageTrackingReport](findmessagetrackingreport.md) | [GetMessageTrackingReport](getmessagetrackingreport.md)</span></span>
  
## <a name="text-value"></a><span data-ttu-id="997e0-114">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="997e0-114">Text value</span></span>

<span data-ttu-id="997e0-115">В следующей таблице приведены возможные значения для элемента **Scope** .</span><span class="sxs-lookup"><span data-stu-id="997e0-115">The following table lists the possible values for the **Scope** element.</span></span> 
  
|<span data-ttu-id="997e0-116">**Значение**</span><span class="sxs-lookup"><span data-stu-id="997e0-116">**Value**</span></span>|<span data-ttu-id="997e0-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="997e0-117">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="997e0-118">Организация</span><span class="sxs-lookup"><span data-stu-id="997e0-118">Organization</span></span>  <br/> |<span data-ttu-id="997e0-119">Области отслеживания сообщений охватываются в пределах организации.</span><span class="sxs-lookup"><span data-stu-id="997e0-119">The message tracking scopes spans across an organization.</span></span>  <br/> |
|<span data-ttu-id="997e0-120">Лес</span><span class="sxs-lookup"><span data-stu-id="997e0-120">Forest</span></span>  <br/> |<span data-ttu-id="997e0-121">Области отслеживания сообщений охватываются в пределах леса.</span><span class="sxs-lookup"><span data-stu-id="997e0-121">The message tracking scopes spans across a forest.</span></span>  <br/> |
|<span data-ttu-id="997e0-122">Site</span><span class="sxs-lookup"><span data-stu-id="997e0-122">Site</span></span>  <br/> |<span data-ttu-id="997e0-123">Области отслеживания сообщений охватываются на сайте.</span><span class="sxs-lookup"><span data-stu-id="997e0-123">The message tracking scopes spans across a site.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="997e0-124">Примечания</span><span class="sxs-lookup"><span data-stu-id="997e0-124">Remarks</span></span>

<span data-ttu-id="997e0-125">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="997e0-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="997e0-126">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="997e0-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="997e0-127">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="997e0-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="997e0-128">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="997e0-128">Schema Name</span></span>  <br/> |<span data-ttu-id="997e0-129">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="997e0-129">Messages schema</span></span>  <br/> |
|<span data-ttu-id="997e0-130">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="997e0-130">Validation File</span></span>  <br/> |<span data-ttu-id="997e0-131">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="997e0-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="997e0-132">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="997e0-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="997e0-133">False</span><span class="sxs-lookup"><span data-stu-id="997e0-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="997e0-134">См. также</span><span class="sxs-lookup"><span data-stu-id="997e0-134">See also</span></span>



- [<span data-ttu-id="997e0-135">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="997e0-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

