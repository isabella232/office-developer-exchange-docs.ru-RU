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
ms.openlocfilehash: cc28abf644247339e1226cd0e13824cc5f5669be
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44455648"
---
# <a name="disableappresponse"></a><span data-ttu-id="bcecf-103">дисаблеаппреспонсе</span><span class="sxs-lookup"><span data-stu-id="bcecf-103">DisableAppResponse</span></span>

<span data-ttu-id="bcecf-104">Элемент **дисаблеаппреспонсе** указывает ответ на запрос **DisableApp** .</span><span class="sxs-lookup"><span data-stu-id="bcecf-104">The **DisableAppResponse** element specifies the response to a **DisableApp** request.</span></span> 
  
```XML
<DisableAppResponse>
    <MessageText></MessageText>
    <ResponseCode></ResponeCode>
    <DescriptiveLinkKey></DescriptiveLinkKey>
    <MessageXml></MessageXml>
</DisableAppResponse>
```

 <span data-ttu-id="bcecf-105">**дисаблеаппреспонсетипе**</span><span class="sxs-lookup"><span data-stu-id="bcecf-105">**DisableAppResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="bcecf-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="bcecf-106">Attributes and elements</span></span>

<span data-ttu-id="bcecf-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="bcecf-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="bcecf-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="bcecf-108">Attributes</span></span>

<span data-ttu-id="bcecf-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="bcecf-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="bcecf-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="bcecf-110">Child elements</span></span>

|<span data-ttu-id="bcecf-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="bcecf-111">**Element**</span></span>|<span data-ttu-id="bcecf-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="bcecf-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bcecf-113">мессажетекст</span><span class="sxs-lookup"><span data-stu-id="bcecf-113">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="bcecf-114">Предоставляет текстовое описание состояния отклика.</span><span class="sxs-lookup"><span data-stu-id="bcecf-114">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="bcecf-115">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="bcecf-115">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="bcecf-116">Предоставляет сведения о состоянии запроса.</span><span class="sxs-lookup"><span data-stu-id="bcecf-116">Provides status information about the request.</span></span>  <br/> |
|[<span data-ttu-id="bcecf-117">дескриптивелинккэй</span><span class="sxs-lookup"><span data-stu-id="bcecf-117">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="bcecf-118">В настоящее время не используется и зарезервировано для будущего использования.</span><span class="sxs-lookup"><span data-stu-id="bcecf-118">Currently unused and reserved for future use.</span></span>  <br/> |
|[<span data-ttu-id="bcecf-119">мессажексмл</span><span class="sxs-lookup"><span data-stu-id="bcecf-119">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="bcecf-120">Предоставляет дополнительные сведения об ошибке.</span><span class="sxs-lookup"><span data-stu-id="bcecf-120">Provides additional error response information.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="bcecf-121">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="bcecf-121">Parent elements</span></span>

<span data-ttu-id="bcecf-122">Нет.</span><span class="sxs-lookup"><span data-stu-id="bcecf-122">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="bcecf-123">Примечания</span><span class="sxs-lookup"><span data-stu-id="bcecf-123">Remarks</span></span>

<span data-ttu-id="bcecf-124">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="bcecf-124">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="bcecf-125">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="bcecf-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="bcecf-126">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="bcecf-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="bcecf-127">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="bcecf-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="bcecf-128">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="bcecf-128">Schema Name</span></span>  <br/> |<span data-ttu-id="bcecf-129">Схема сообщения</span><span class="sxs-lookup"><span data-stu-id="bcecf-129">Message schema</span></span>  <br/> |
|<span data-ttu-id="bcecf-130">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="bcecf-130">Validation File</span></span>  <br/> |<span data-ttu-id="bcecf-131">messages. xsd</span><span class="sxs-lookup"><span data-stu-id="bcecf-131">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="bcecf-132">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="bcecf-132">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="bcecf-133">См. также</span><span class="sxs-lookup"><span data-stu-id="bcecf-133">See also</span></span>

- [<span data-ttu-id="bcecf-134">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="bcecf-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

