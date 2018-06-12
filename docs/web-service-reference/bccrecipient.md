---
title: BccRecipient
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- BccRecipient
api_type:
- schema
ms.assetid: 4ef0cff5-8a5a-4d76-9d2b-938774d8fc1b
description: Элемент BccRecipient представляет получателя для получения скрытой копии (Bcc) сообщения электронной почты.
ms.openlocfilehash: bed58536263196a61651493e92a4dcd1df3f5ec9
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761550"
---
# <a name="bccrecipient"></a><span data-ttu-id="40cb9-103">BccRecipient</span><span class="sxs-lookup"><span data-stu-id="40cb9-103">BccRecipient</span></span>

<span data-ttu-id="40cb9-104">Элемент **BccRecipient** представляет получателя для получения скрытой копии (Bcc) сообщения электронной почты.</span><span class="sxs-lookup"><span data-stu-id="40cb9-104">The **BccRecipient** element represents a recipient to receive a blind carbon copy (Bcc) of an e-mail message.</span></span> 
  
```XML
<BccRecipient>true | false</BccRecipient>
```

 <span data-ttu-id="40cb9-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="40cb9-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="40cb9-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="40cb9-106">Attributes and elements</span></span>

<span data-ttu-id="40cb9-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="40cb9-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="40cb9-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="40cb9-108">Attributes</span></span>

<span data-ttu-id="40cb9-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="40cb9-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="40cb9-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="40cb9-110">Child elements</span></span>

<span data-ttu-id="40cb9-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="40cb9-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="40cb9-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="40cb9-112">Parent elements</span></span>

|<span data-ttu-id="40cb9-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="40cb9-113">**Element**</span></span>|<span data-ttu-id="40cb9-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="40cb9-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="40cb9-115">RecipientTrackingEvent</span><span class="sxs-lookup"><span data-stu-id="40cb9-115">RecipientTrackingEvent</span></span>](recipienttrackingevent.md) <br/> |<span data-ttu-id="40cb9-116">Содержит сведения для одного события для получателя.</span><span class="sxs-lookup"><span data-stu-id="40cb9-116">Contains information for a single event for a recipient.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="40cb9-117">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="40cb9-117">Text value</span></span>

<span data-ttu-id="40cb9-118">Этот элемент может быть значение **true** или **false**.</span><span class="sxs-lookup"><span data-stu-id="40cb9-118">This element can be either **true** or **false**.</span></span> <span data-ttu-id="40cb9-119">Значение **true** указывает, что получатель является скрытой скрытой копии. значение **false** указывает, что получатель не относится к скрытой выбросов копируются.</span><span class="sxs-lookup"><span data-stu-id="40cb9-119">A value of **true** indicates that the recipient is blind carbon copied; a value of **false** indicates that the recipient is not blind carbon copied.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="40cb9-120">Замечания</span><span class="sxs-lookup"><span data-stu-id="40cb9-120">Remarks</span></span>

<span data-ttu-id="40cb9-121">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="40cb9-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="40cb9-122">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="40cb9-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="40cb9-123">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="40cb9-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="40cb9-124">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="40cb9-124">Schema Name</span></span>  <br/> |<span data-ttu-id="40cb9-125">Схема Types</span><span class="sxs-lookup"><span data-stu-id="40cb9-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="40cb9-126">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="40cb9-126">Validation File</span></span>  <br/> |<span data-ttu-id="40cb9-127">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="40cb9-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="40cb9-128">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="40cb9-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="40cb9-129">False</span><span class="sxs-lookup"><span data-stu-id="40cb9-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="40cb9-130">См. также</span><span class="sxs-lookup"><span data-stu-id="40cb9-130">See also</span></span>



- [<span data-ttu-id="40cb9-131">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="40cb9-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
