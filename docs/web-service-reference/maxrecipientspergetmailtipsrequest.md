---
title: MaxRecipientsPerGetMailTipsRequest
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MaxRecipientsPerGetMailTipsRequest
api_type:
- schema
ms.assetid: 8ff5df18-1989-4217-b4c0-599232911d0c
description: Элемент MaxRecipientsPerGetMailTipsRequest указывает максимальное количество получателей, которые могут передаваться GetMailTips операции.
ms.openlocfilehash: 4c873fe534582e582bf5b1c1d5fd2789616e056a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19834386"
---
# <a name="maxrecipientspergetmailtipsrequest"></a><span data-ttu-id="14366-103">MaxRecipientsPerGetMailTipsRequest</span><span class="sxs-lookup"><span data-stu-id="14366-103">MaxRecipientsPerGetMailTipsRequest</span></span>

<span data-ttu-id="14366-104">Элемент **MaxRecipientsPerGetMailTipsRequest** указывает максимальное количество получателей, которые могут передаваться [GetMailTips операции](getmailtips-operation.md).</span><span class="sxs-lookup"><span data-stu-id="14366-104">The **MaxRecipientsPerGetMailTipsRequest** element indicates the maximum number of recipients that can be passed to the [GetMailTips operation](getmailtips-operation.md).</span></span>
  
```XML
<MaxRecipientsPerGetMailTipsRequest/>
```

 <span data-ttu-id="14366-105">**int**</span><span class="sxs-lookup"><span data-stu-id="14366-105">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="14366-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="14366-106">Attributes and elements</span></span>

<span data-ttu-id="14366-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="14366-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="14366-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="14366-108">Attributes</span></span>

<span data-ttu-id="14366-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="14366-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="14366-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="14366-110">Child elements</span></span>

<span data-ttu-id="14366-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="14366-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="14366-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="14366-112">Parent elements</span></span>

|<span data-ttu-id="14366-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="14366-113">**Element**</span></span>|<span data-ttu-id="14366-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="14366-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="14366-115">MailTipsConfiguration (MailTipsServiceConfiguration)</span><span class="sxs-lookup"><span data-stu-id="14366-115">MailTipsConfiguration (MailTipsServiceConfiguration)</span></span>](mailtipsconfiguration-mailtipsserviceconfiguration.md) <br/> |<span data-ttu-id="14366-116">Содержит сведения о конфигурации службы для службы советы почты.</span><span class="sxs-lookup"><span data-stu-id="14366-116">Contains service configuration information for the mail tips service.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="14366-117">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="14366-117">Text value</span></span>

<span data-ttu-id="14366-118">Текстовое значение представляет собой целое число, который представляет максимальное количество получателей, которые могут передаваться [GetMailTips операции](getmailtips-operation.md).</span><span class="sxs-lookup"><span data-stu-id="14366-118">The text value is an integer that represents the maximum number of recipients that can be passed to the [GetMailTips operation](getmailtips-operation.md).</span></span>
  
## <a name="remarks"></a><span data-ttu-id="14366-119">Замечания</span><span class="sxs-lookup"><span data-stu-id="14366-119">Remarks</span></span>

<span data-ttu-id="14366-120">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="14366-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="14366-121">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="14366-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="14366-122">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="14366-122">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="14366-123">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="14366-123">Schema Name</span></span>  <br/> |<span data-ttu-id="14366-124">Схема Types</span><span class="sxs-lookup"><span data-stu-id="14366-124">Types schema</span></span>  <br/> |
|<span data-ttu-id="14366-125">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="14366-125">Validation File</span></span>  <br/> |<span data-ttu-id="14366-126">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="14366-126">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="14366-127">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="14366-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="14366-128">False</span><span class="sxs-lookup"><span data-stu-id="14366-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="14366-129">См. также</span><span class="sxs-lookup"><span data-stu-id="14366-129">See also</span></span>



[<span data-ttu-id="14366-130">Операция GetMailTips</span><span class="sxs-lookup"><span data-stu-id="14366-130">GetMailTips operation</span></span>](getmailtips-operation.md)


- [<span data-ttu-id="14366-131">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="14366-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

