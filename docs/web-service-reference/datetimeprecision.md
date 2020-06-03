---
title: датетимепреЦисион
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 822dc5a6-2d57-474b-8a7d-da150898e5b6
description: Элемент ДатетимепреЦисион указывает точность возвращаемых значений даты и времени.
ms.openlocfilehash: 9d245dfb0123daae42ba9b9b4e98aff872b67d80
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529226"
---
# <a name="datetimeprecision"></a><span data-ttu-id="78b6f-103">датетимепреЦисион</span><span class="sxs-lookup"><span data-stu-id="78b6f-103">DateTimePrecision</span></span>

<span data-ttu-id="78b6f-104">Элемент **датетимепреЦисион** указывает точность возвращаемых значений даты и времени.</span><span class="sxs-lookup"><span data-stu-id="78b6f-104">The **DateTimePrecision** element specifies the precision for returned date/time values.</span></span> 
  
```XML
<DateTimePrecision />
```

<span data-ttu-id="78b6f-105">**датетимепреЦисионтипе**</span><span class="sxs-lookup"><span data-stu-id="78b6f-105">**DateTimePrecisionType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="78b6f-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="78b6f-106">Attributes and elements</span></span>

<span data-ttu-id="78b6f-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="78b6f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="78b6f-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="78b6f-108">Attributes</span></span>

<span data-ttu-id="78b6f-109">Нет</span><span class="sxs-lookup"><span data-stu-id="78b6f-109">None</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="78b6f-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="78b6f-110">Child elements</span></span>

<span data-ttu-id="78b6f-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="78b6f-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="78b6f-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="78b6f-112">Parent elements</span></span>

<span data-ttu-id="78b6f-113">Элемент **датетимепреЦисион** находится в заголовке SOAP.</span><span class="sxs-lookup"><span data-stu-id="78b6f-113">The **DateTimePrecision** element is located in the SOAP header.</span></span> 
  
## <a name="text-value"></a><span data-ttu-id="78b6f-114">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="78b6f-114">Text value</span></span>

<span data-ttu-id="78b6f-115">Необходимо указать текстовое значение.</span><span class="sxs-lookup"><span data-stu-id="78b6f-115">A text value is required.</span></span> <span data-ttu-id="78b6f-116">Ниже перечислены возможные значения.</span><span class="sxs-lookup"><span data-stu-id="78b6f-116">The following are the possible values:</span></span>
  
- <span data-ttu-id="78b6f-117">Секунды</span><span class="sxs-lookup"><span data-stu-id="78b6f-117">Seconds</span></span>
    
- <span data-ttu-id="78b6f-118">Миллисекундах</span><span class="sxs-lookup"><span data-stu-id="78b6f-118">Milliseconds</span></span>
    
## <a name="remarks"></a><span data-ttu-id="78b6f-119">Примечания</span><span class="sxs-lookup"><span data-stu-id="78b6f-119">Remarks</span></span>

<span data-ttu-id="78b6f-120">Если используется заголовок SOAP с элементом **датетимепреЦисион** , для которого задано значение "секунды", значения даты и времени возвращаются к ближайшей секунде (00:00:00).</span><span class="sxs-lookup"><span data-stu-id="78b6f-120">When a SOAP header with the **DateTimePrecision** element set to "Seconds" is used, date/time values are returned to the nearest seconds (00:00:00).</span></span> <span data-ttu-id="78b6f-121">При использовании параметра "миллисекунды" значения даты и времени возвращаются до ближайшей миллисекунды (00:00:00.0000).</span><span class="sxs-lookup"><span data-stu-id="78b6f-121">When "Milliseconds" is used, date/time values are returned to the nearest millisecond (00:00:00.0000).</span></span> 
  
<span data-ttu-id="78b6f-122">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="78b6f-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
<span data-ttu-id="78b6f-123">Этот элемент появился в Exchange Server 2010 с пакетом обновления 2 (SP2).</span><span class="sxs-lookup"><span data-stu-id="78b6f-123">This element was introduced in Exchange Server 2010 Service Pack 2 (SP2).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="78b6f-124">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="78b6f-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="78b6f-125">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="78b6f-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="78b6f-126">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="78b6f-126">Schema Name</span></span>  <br/> |<span data-ttu-id="78b6f-127">Схема Types</span><span class="sxs-lookup"><span data-stu-id="78b6f-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="78b6f-128">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="78b6f-128">Validation File</span></span>  <br/> |<span data-ttu-id="78b6f-129">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="78b6f-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="78b6f-130">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="78b6f-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="78b6f-131">False</span><span class="sxs-lookup"><span data-stu-id="78b6f-131">False</span></span>  <br/> |
   

