---
title: MailTipsEnabled
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MailTipsEnabled
api_type:
- schema
ms.assetid: 737388b3-7b73-42af-94d3-3dbb0659718f
description: Элемент MailTipsEnabled указывает, доступна ли служба советы почты.
ms.openlocfilehash: 4fe2cae1087ab667133ec685c3325b14c4f12088
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19834330"
---
# <a name="mailtipsenabled"></a><span data-ttu-id="e9531-103">MailTipsEnabled</span><span class="sxs-lookup"><span data-stu-id="e9531-103">MailTipsEnabled</span></span>

<span data-ttu-id="e9531-104">Элемент **MailTipsEnabled** указывает, доступна ли служба советы почты.</span><span class="sxs-lookup"><span data-stu-id="e9531-104">The **MailTipsEnabled** element indicates whether the mail tips service is available.</span></span> 
  
```xml
<MailTipsEnabled>true | false</MailTipsEnabled>
```

 <span data-ttu-id="e9531-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="e9531-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e9531-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="e9531-106">Attributes and elements</span></span>

<span data-ttu-id="e9531-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="e9531-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e9531-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="e9531-108">Attributes</span></span>

<span data-ttu-id="e9531-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="e9531-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e9531-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="e9531-110">Child elements</span></span>

<span data-ttu-id="e9531-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="e9531-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="e9531-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="e9531-112">Parent elements</span></span>

|<span data-ttu-id="e9531-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="e9531-113">**Element**</span></span>|<span data-ttu-id="e9531-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="e9531-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e9531-115">MailTipsConfiguration (MailTipsServiceConfiguration)</span><span class="sxs-lookup"><span data-stu-id="e9531-115">MailTipsConfiguration (MailTipsServiceConfiguration)</span></span>](mailtipsconfiguration-mailtipsserviceconfiguration.md) <br/> |<span data-ttu-id="e9531-116">Содержит сведения о конфигурации службы для службы советы почты.</span><span class="sxs-lookup"><span data-stu-id="e9531-116">Contains service configuration information for the mail tips service.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="e9531-117">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="e9531-117">Text value</span></span>

<span data-ttu-id="e9531-118">Текстовое значение этого элемента равно **true** , если доступна служба советы почты.</span><span class="sxs-lookup"><span data-stu-id="e9531-118">The text value of this element is **true** if the mail tips service is available.</span></span> <span data-ttu-id="e9531-119">Значение равно **false** , если служба советы почты недоступен.</span><span class="sxs-lookup"><span data-stu-id="e9531-119">The value is **false** if the mail tips service is not available.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="e9531-120">Замечания</span><span class="sxs-lookup"><span data-stu-id="e9531-120">Remarks</span></span>

<span data-ttu-id="e9531-121">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="e9531-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e9531-122">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="e9531-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e9531-123">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="e9531-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e9531-124">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="e9531-124">Schema Name</span></span>  <br/> |<span data-ttu-id="e9531-125">Схема Types</span><span class="sxs-lookup"><span data-stu-id="e9531-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="e9531-126">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="e9531-126">Validation File</span></span>  <br/> |<span data-ttu-id="e9531-127">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="e9531-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="e9531-128">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="e9531-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="e9531-129">False</span><span class="sxs-lookup"><span data-stu-id="e9531-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e9531-130">См. также</span><span class="sxs-lookup"><span data-stu-id="e9531-130">See also</span></span>



- [<span data-ttu-id="e9531-131">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="e9531-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

