---
title: Offset
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Offset
api_type:
- schema
ms.assetid: dcbb9d85-d90c-4363-b4c9-d081ad03f407
description: Элемент offset описывает смещение из Басеоффсет. В сочетании с элементом Басеоффсет элемент offset определяет, является ли время стандартным или летним.
ms.openlocfilehash: d85fef0d67633733f6aa1943d70413ea70a528d6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834642"
---
# <a name="offset"></a><span data-ttu-id="99626-104">Offset</span><span class="sxs-lookup"><span data-stu-id="99626-104">Offset</span></span>

<span data-ttu-id="99626-105">Элемент **offset** описывает смещение из [басеоффсет](baseoffset.md).</span><span class="sxs-lookup"><span data-stu-id="99626-105">The **Offset** element describes the offset from the [BaseOffset](baseoffset.md).</span></span> <span data-ttu-id="99626-106">В сочетании с элементом **басеоффсет** элемент **offset** определяет, является ли время стандартным или летним.</span><span class="sxs-lookup"><span data-stu-id="99626-106">Together with the **BaseOffset** element, the **Offset** element identifies whether the time is standard or daylight saving time.</span></span> 
  
```xml
<Offset/>
```

 <span data-ttu-id="99626-107">**duration**</span><span class="sxs-lookup"><span data-stu-id="99626-107">**duration**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="99626-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="99626-108">Attributes and elements</span></span>

<span data-ttu-id="99626-109">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="99626-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="99626-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="99626-110">Attributes</span></span>

<span data-ttu-id="99626-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="99626-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="99626-112">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="99626-112">Child elements</span></span>

<span data-ttu-id="99626-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="99626-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="99626-114">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="99626-114">Parent elements</span></span>

|<span data-ttu-id="99626-115">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="99626-115">**Element**</span></span>|<span data-ttu-id="99626-116">**Описание**</span><span class="sxs-lookup"><span data-stu-id="99626-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="99626-117">Переход</span><span class="sxs-lookup"><span data-stu-id="99626-117">Daylight</span></span>](daylight.md) <br/> |<span data-ttu-id="99626-118">Представляет дату и время изменения времени с летнего на стандартное время.</span><span class="sxs-lookup"><span data-stu-id="99626-118">Represents the date and time when the time changes from daylight saving time to standard time.</span></span>  <br/> |
|[<span data-ttu-id="99626-119">Standard</span><span class="sxs-lookup"><span data-stu-id="99626-119">Standard</span></span>](standard.md) <br/> |<span data-ttu-id="99626-120">Представляет дату и время изменения времени с летнего на стандартное время.</span><span class="sxs-lookup"><span data-stu-id="99626-120">Represents the date and time when the time changes from daylight saving time to standard time.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="99626-121">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="99626-121">Text value</span></span>

<span data-ttu-id="99626-122">Текстовое значение представляет смещение от всеобщего скоординированного времени (UTC).</span><span class="sxs-lookup"><span data-stu-id="99626-122">The text value represents the offset from Coordinated Universal Time (UTC).</span></span>
  
## <a name="remarks"></a><span data-ttu-id="99626-123">Примечания</span><span class="sxs-lookup"><span data-stu-id="99626-123">Remarks</span></span>

<span data-ttu-id="99626-124">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="99626-124">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="99626-125">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="99626-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="99626-126">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="99626-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="99626-127">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="99626-127">Schema Name</span></span>  <br/> |<span data-ttu-id="99626-128">Схема Types</span><span class="sxs-lookup"><span data-stu-id="99626-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="99626-129">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="99626-129">Validation File</span></span>  <br/> |<span data-ttu-id="99626-130">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="99626-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="99626-131">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="99626-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="99626-132">False</span><span class="sxs-lookup"><span data-stu-id="99626-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="99626-133">См. также</span><span class="sxs-lookup"><span data-stu-id="99626-133">See also</span></span>



- [<span data-ttu-id="99626-134">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="99626-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

