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
description: Элемент StartDateTime указывает дату начала и время для правила или поиска.
ms.openlocfilehash: 4bc32ed5626d692fc73dfa8bd7c46923aba72f9e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19835552"
---
# <a name="startdatetime"></a><span data-ttu-id="8b4e5-103">StartDateTime</span><span class="sxs-lookup"><span data-stu-id="8b4e5-103">StartDateTime</span></span>

<span data-ttu-id="8b4e5-104">Элемент **StartDateTime** указывает дату начала и время для правила или поиска.</span><span class="sxs-lookup"><span data-stu-id="8b4e5-104">The **StartDateTime** element specifies the start date and time for a rule or a search.</span></span> 
  
```XML
<StartDate/>
```

<span data-ttu-id="8b4e5-105">**dateTime**</span><span class="sxs-lookup"><span data-stu-id="8b4e5-105">**dateTime**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="8b4e5-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="8b4e5-106">Attributes and elements</span></span>

<span data-ttu-id="8b4e5-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="8b4e5-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8b4e5-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="8b4e5-108">Attributes</span></span>

<span data-ttu-id="8b4e5-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="8b4e5-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8b4e5-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="8b4e5-110">Child elements</span></span>

<span data-ttu-id="8b4e5-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="8b4e5-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="8b4e5-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="8b4e5-112">Parent elements</span></span>

|<span data-ttu-id="8b4e5-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="8b4e5-113">**Element**</span></span>|<span data-ttu-id="8b4e5-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="8b4e5-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8b4e5-115">FindMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="8b4e5-115">FindMessageTrackingReport</span></span>](findmessagetrackingreport.md) <br/> |<span data-ttu-id="8b4e5-116">Задает условия типам сообщений для поиска.</span><span class="sxs-lookup"><span data-stu-id="8b4e5-116">Specifies criteria for the types of messages to find.</span></span>  <br/> |
|[<span data-ttu-id="8b4e5-117">WithinDateRange</span><span class="sxs-lookup"><span data-stu-id="8b4e5-117">WithinDateRange</span></span>](withindaterange.md) <br/> |<span data-ttu-id="8b4e5-118">Указывает диапазон дат, в течение которого нужно были получены в порядке для условие или исключение для применения входящих сообщений.</span><span class="sxs-lookup"><span data-stu-id="8b4e5-118">Specifies the date range within which incoming messages have to have been received in order for the condition or exception to apply.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="8b4e5-119">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="8b4e5-119">Text value</span></span>

 <span data-ttu-id="8b4e5-120">Текстовое значение, представляющее даты/времени является обязательным, если данный элемент используется.</span><span class="sxs-lookup"><span data-stu-id="8b4e5-120">A text value that represents a date/time is required if this element is used.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="8b4e5-121">Замечания</span><span class="sxs-lookup"><span data-stu-id="8b4e5-121">Remarks</span></span>

<span data-ttu-id="8b4e5-122">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="8b4e5-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8b4e5-123">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="8b4e5-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8b4e5-124">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="8b4e5-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="8b4e5-125">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="8b4e5-125">Schema Name</span></span>  <br/> |<span data-ttu-id="8b4e5-126">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="8b4e5-126">Messages schema</span></span>  <br/> |
|<span data-ttu-id="8b4e5-127">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="8b4e5-127">Validation File</span></span>  <br/> |<span data-ttu-id="8b4e5-128">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="8b4e5-128">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="8b4e5-129">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="8b4e5-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="8b4e5-130">False</span><span class="sxs-lookup"><span data-stu-id="8b4e5-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="8b4e5-131">См. также</span><span class="sxs-lookup"><span data-stu-id="8b4e5-131">See also</span></span>

- [<span data-ttu-id="8b4e5-132">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="8b4e5-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

