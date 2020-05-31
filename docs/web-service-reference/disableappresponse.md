---
title: дисаблеаппреспонсе
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 11ebe618-d759-4f16-be99-eaaa817ba782
description: Элемент Дисаблеаппреспонсе указывает ответ на запрос DisableApp.
ms.openlocfilehash: 740801fa4b60e217f0b9148bcfcc5b206e96bf31
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762123"
---
# <a name="disableappresponse"></a><span data-ttu-id="6dc59-103">дисаблеаппреспонсе</span><span class="sxs-lookup"><span data-stu-id="6dc59-103">DisableAppResponse</span></span>

<span data-ttu-id="6dc59-104">Элемент **дисаблеаппреспонсе** указывает ответ на запрос **DisableApp** .</span><span class="sxs-lookup"><span data-stu-id="6dc59-104">The **DisableAppResponse** element specifies the response to a **DisableApp** request.</span></span> 
  
```XML
<DisableAppResponse>
    <MessageText></MessageText>
    <ResponseCode></ResponeCode>
    <DescriptiveLinkKey></DescriptiveLinkKey>
    <MessageXml></MessageXml>
</DisableAppResponse>
```

 <span data-ttu-id="6dc59-105">**дисаблеаппреспонсетипе**</span><span class="sxs-lookup"><span data-stu-id="6dc59-105">**DisableAppResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6dc59-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="6dc59-106">Attributes and elements</span></span>

<span data-ttu-id="6dc59-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="6dc59-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6dc59-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="6dc59-108">Attributes</span></span>

<span data-ttu-id="6dc59-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="6dc59-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6dc59-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="6dc59-110">Child elements</span></span>

|<span data-ttu-id="6dc59-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="6dc59-111">**Element**</span></span>|<span data-ttu-id="6dc59-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="6dc59-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6dc59-113">мессажетекст</span><span class="sxs-lookup"><span data-stu-id="6dc59-113">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="6dc59-114">Предоставляет текстовое описание состояния отклика.</span><span class="sxs-lookup"><span data-stu-id="6dc59-114">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="6dc59-115">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="6dc59-115">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="6dc59-116">Предоставляет сведения о состоянии запроса.</span><span class="sxs-lookup"><span data-stu-id="6dc59-116">Provides status information about the request.</span></span>  <br/> |
|[<span data-ttu-id="6dc59-117">дескриптивелинккэй</span><span class="sxs-lookup"><span data-stu-id="6dc59-117">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="6dc59-118">В настоящее время не используется и зарезервировано для будущего использования.</span><span class="sxs-lookup"><span data-stu-id="6dc59-118">Currently unused and reserved for future use.</span></span>  <br/> |
|[<span data-ttu-id="6dc59-119">мессажексмл</span><span class="sxs-lookup"><span data-stu-id="6dc59-119">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="6dc59-120">Предоставляет дополнительные сведения об ошибке.</span><span class="sxs-lookup"><span data-stu-id="6dc59-120">Provides additional error response information.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="6dc59-121">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="6dc59-121">Parent elements</span></span>

<span data-ttu-id="6dc59-122">Нет.</span><span class="sxs-lookup"><span data-stu-id="6dc59-122">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="6dc59-123">Примечания</span><span class="sxs-lookup"><span data-stu-id="6dc59-123">Remarks</span></span>

<span data-ttu-id="6dc59-124">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="6dc59-124">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="6dc59-125">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="6dc59-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6dc59-126">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="6dc59-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6dc59-127">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="6dc59-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="6dc59-128">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="6dc59-128">Schema Name</span></span>  <br/> |<span data-ttu-id="6dc59-129">Схема сообщения</span><span class="sxs-lookup"><span data-stu-id="6dc59-129">Message schema</span></span>  <br/> |
|<span data-ttu-id="6dc59-130">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="6dc59-130">Validation File</span></span>  <br/> |<span data-ttu-id="6dc59-131">messages. xsd</span><span class="sxs-lookup"><span data-stu-id="6dc59-131">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="6dc59-132">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="6dc59-132">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="6dc59-133">См. также</span><span class="sxs-lookup"><span data-stu-id="6dc59-133">See also</span></span>

- [<span data-ttu-id="6dc59-134">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="6dc59-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

