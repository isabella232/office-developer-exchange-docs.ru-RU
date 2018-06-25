---
title: DisableAppResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 11ebe618-d759-4f16-be99-eaaa817ba782
description: Элемент DisableAppResponse указывает ответ на запрос DisableApp.
ms.openlocfilehash: 740801fa4b60e217f0b9148bcfcc5b206e96bf31
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762123"
---
# <a name="disableappresponse"></a><span data-ttu-id="e0367-103">DisableAppResponse</span><span class="sxs-lookup"><span data-stu-id="e0367-103">DisableAppResponse</span></span>

<span data-ttu-id="e0367-104">Элемент **DisableAppResponse** указывает ответ на запрос **DisableApp** .</span><span class="sxs-lookup"><span data-stu-id="e0367-104">The **DisableAppResponse** element specifies the response to a **DisableApp** request.</span></span> 
  
```XML
<DisableAppResponse>
    <MessageText></MessageText>
    <ResponseCode></ResponeCode>
    <DescriptiveLinkKey></DescriptiveLinkKey>
    <MessageXml></MessageXml>
</DisableAppResponse>
```

 <span data-ttu-id="e0367-105">**DisableAppResponseType**</span><span class="sxs-lookup"><span data-stu-id="e0367-105">**DisableAppResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e0367-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="e0367-106">Attributes and elements</span></span>

<span data-ttu-id="e0367-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="e0367-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e0367-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="e0367-108">Attributes</span></span>

<span data-ttu-id="e0367-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="e0367-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e0367-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="e0367-110">Child elements</span></span>

|<span data-ttu-id="e0367-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="e0367-111">**Element**</span></span>|<span data-ttu-id="e0367-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="e0367-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e0367-113">MessageText</span><span class="sxs-lookup"><span data-stu-id="e0367-113">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="e0367-114">Предоставляет текстовое описание состояния ответа.</span><span class="sxs-lookup"><span data-stu-id="e0367-114">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="e0367-115">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="e0367-115">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="e0367-116">Предоставляет сведения о состоянии о запросе.</span><span class="sxs-lookup"><span data-stu-id="e0367-116">Provides status information about the request.</span></span>  <br/> |
|[<span data-ttu-id="e0367-117">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="e0367-117">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="e0367-118">В настоящее время используется и зарезервировано для будущего использования.</span><span class="sxs-lookup"><span data-stu-id="e0367-118">Currently unused and reserved for future use.</span></span>  <br/> |
|[<span data-ttu-id="e0367-119">MessageXml</span><span class="sxs-lookup"><span data-stu-id="e0367-119">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="e0367-120">Предоставляет дополнительные сведения об ошибке ответа.</span><span class="sxs-lookup"><span data-stu-id="e0367-120">Provides additional error response information.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="e0367-121">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="e0367-121">Parent elements</span></span>

<span data-ttu-id="e0367-122">Нет.</span><span class="sxs-lookup"><span data-stu-id="e0367-122">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="e0367-123">Замечания</span><span class="sxs-lookup"><span data-stu-id="e0367-123">Remarks</span></span>

<span data-ttu-id="e0367-124">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="e0367-124">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="e0367-125">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="e0367-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e0367-126">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="e0367-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e0367-127">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="e0367-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="e0367-128">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="e0367-128">Schema Name</span></span>  <br/> |<span data-ttu-id="e0367-129">Схема сообщения</span><span class="sxs-lookup"><span data-stu-id="e0367-129">Message schema</span></span>  <br/> |
|<span data-ttu-id="e0367-130">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="e0367-130">Validation File</span></span>  <br/> |<span data-ttu-id="e0367-131">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="e0367-131">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="e0367-132">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="e0367-132">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="e0367-133">См. также</span><span class="sxs-lookup"><span data-stu-id="e0367-133">See also</span></span>

- [<span data-ttu-id="e0367-134">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="e0367-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

