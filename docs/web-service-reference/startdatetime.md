---
title: StartDateTime
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- StartDateTime
api_type:
- schema
ms.assetid: 6fd41b7b-6c83-43b6-8b16-0bdb3d173d73
description: Элемент StartDateTime указывает дату и время начала для правила или поиска.
ms.openlocfilehash: 28b78fad87abb1148cfe49fee4f9bb98f822eae5
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462845"
---
# <a name="startdatetime"></a><span data-ttu-id="12f8e-103">StartDateTime</span><span class="sxs-lookup"><span data-stu-id="12f8e-103">StartDateTime</span></span>

<span data-ttu-id="12f8e-104">Элемент **StartDateTime** указывает дату и время начала для правила или поиска.</span><span class="sxs-lookup"><span data-stu-id="12f8e-104">The **StartDateTime** element specifies the start date and time for a rule or a search.</span></span> 
  
```XML
<StartDate/>
```

<span data-ttu-id="12f8e-105">**дата и время**</span><span class="sxs-lookup"><span data-stu-id="12f8e-105">**dateTime**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="12f8e-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="12f8e-106">Attributes and elements</span></span>

<span data-ttu-id="12f8e-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="12f8e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="12f8e-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="12f8e-108">Attributes</span></span>

<span data-ttu-id="12f8e-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="12f8e-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="12f8e-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="12f8e-110">Child elements</span></span>

<span data-ttu-id="12f8e-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="12f8e-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="12f8e-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="12f8e-112">Parent elements</span></span>

|<span data-ttu-id="12f8e-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="12f8e-113">**Element**</span></span>|<span data-ttu-id="12f8e-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="12f8e-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="12f8e-115">FindMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="12f8e-115">FindMessageTrackingReport</span></span>](findmessagetrackingreport.md) <br/> |<span data-ttu-id="12f8e-116">Задает условия для типов сообщений, которые требуется найти.</span><span class="sxs-lookup"><span data-stu-id="12f8e-116">Specifies criteria for the types of messages to find.</span></span>  <br/> |
|[<span data-ttu-id="12f8e-117">висиндатеранже</span><span class="sxs-lookup"><span data-stu-id="12f8e-117">WithinDateRange</span></span>](withindaterange.md) <br/> |<span data-ttu-id="12f8e-118">Указывает диапазон дат, в течение которого должны быть получены входящие сообщения, чтобы применялось условие или исключение.</span><span class="sxs-lookup"><span data-stu-id="12f8e-118">Specifies the date range within which incoming messages have to have been received in order for the condition or exception to apply.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="12f8e-119">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="12f8e-119">Text value</span></span>

 <span data-ttu-id="12f8e-120">При использовании этого элемента необходимо указать текстовое значение, представляющее дату и время.</span><span class="sxs-lookup"><span data-stu-id="12f8e-120">A text value that represents a date/time is required if this element is used.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="12f8e-121">Примечания</span><span class="sxs-lookup"><span data-stu-id="12f8e-121">Remarks</span></span>

<span data-ttu-id="12f8e-122">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="12f8e-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="12f8e-123">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="12f8e-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="12f8e-124">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="12f8e-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="12f8e-125">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="12f8e-125">Schema Name</span></span>  <br/> |<span data-ttu-id="12f8e-126">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="12f8e-126">Messages schema</span></span>  <br/> |
|<span data-ttu-id="12f8e-127">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="12f8e-127">Validation File</span></span>  <br/> |<span data-ttu-id="12f8e-128">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="12f8e-128">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="12f8e-129">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="12f8e-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="12f8e-130">False</span><span class="sxs-lookup"><span data-stu-id="12f8e-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="12f8e-131">См. также</span><span class="sxs-lookup"><span data-stu-id="12f8e-131">See also</span></span>

- [<span data-ttu-id="12f8e-132">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="12f8e-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

