---
title: маилтипсенаблед
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
description: Элемент Маилтипсенаблед указывает, доступна ли служба советов по работе с почтой.
ms.openlocfilehash: 6be923733f1cbd584010ce5f8ee5b96178d5c2c0
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44468014"
---
# <a name="mailtipsenabled"></a><span data-ttu-id="899ef-103">маилтипсенаблед</span><span class="sxs-lookup"><span data-stu-id="899ef-103">MailTipsEnabled</span></span>

<span data-ttu-id="899ef-104">Элемент **маилтипсенаблед** указывает, доступна ли служба советов по работе с почтой.</span><span class="sxs-lookup"><span data-stu-id="899ef-104">The **MailTipsEnabled** element indicates whether the mail tips service is available.</span></span> 
  
```xml
<MailTipsEnabled>true | false</MailTipsEnabled>
```

 <span data-ttu-id="899ef-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="899ef-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="899ef-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="899ef-106">Attributes and elements</span></span>

<span data-ttu-id="899ef-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="899ef-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="899ef-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="899ef-108">Attributes</span></span>

<span data-ttu-id="899ef-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="899ef-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="899ef-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="899ef-110">Child elements</span></span>

<span data-ttu-id="899ef-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="899ef-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="899ef-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="899ef-112">Parent elements</span></span>

|<span data-ttu-id="899ef-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="899ef-113">**Element**</span></span>|<span data-ttu-id="899ef-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="899ef-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="899ef-115">Маилтипсконфигуратион (Маилтипссервицеконфигуратион)</span><span class="sxs-lookup"><span data-stu-id="899ef-115">MailTipsConfiguration (MailTipsServiceConfiguration)</span></span>](mailtipsconfiguration-mailtipsserviceconfiguration.md) <br/> |<span data-ttu-id="899ef-116">Содержит сведения о конфигурации службы для советов почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="899ef-116">Contains service configuration information for the mail tips service.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="899ef-117">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="899ef-117">Text value</span></span>

<span data-ttu-id="899ef-118">Текстовое значение этого элемента равно **true** , если доступна служба советов по почте.</span><span class="sxs-lookup"><span data-stu-id="899ef-118">The text value of this element is **true** if the mail tips service is available.</span></span> <span data-ttu-id="899ef-119">Значение **false** , если служба советов почты недоступна.</span><span class="sxs-lookup"><span data-stu-id="899ef-119">The value is **false** if the mail tips service is not available.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="899ef-120">Примечания</span><span class="sxs-lookup"><span data-stu-id="899ef-120">Remarks</span></span>

<span data-ttu-id="899ef-121">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="899ef-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="899ef-122">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="899ef-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="899ef-123">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="899ef-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="899ef-124">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="899ef-124">Schema Name</span></span>  <br/> |<span data-ttu-id="899ef-125">Схема Types</span><span class="sxs-lookup"><span data-stu-id="899ef-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="899ef-126">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="899ef-126">Validation File</span></span>  <br/> |<span data-ttu-id="899ef-127">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="899ef-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="899ef-128">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="899ef-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="899ef-129">False</span><span class="sxs-lookup"><span data-stu-id="899ef-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="899ef-130">См. также</span><span class="sxs-lookup"><span data-stu-id="899ef-130">See also</span></span>



- [<span data-ttu-id="899ef-131">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="899ef-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

