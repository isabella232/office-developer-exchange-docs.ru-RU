---
title: EndDateTime
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- EndDateTime
api_type:
- schema
ms.assetid: 54d14e47-a8f7-400b-a859-c7ea7ce4c6a4
description: Элемент EndDateTime указывает Дата и время окончания для правила или поиска.
ms.openlocfilehash: ad596c6441e7bdb10b4e886a8d0f3ba183c43c3e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762351"
---
# <a name="enddatetime"></a><span data-ttu-id="a8b25-103">EndDateTime</span><span class="sxs-lookup"><span data-stu-id="a8b25-103">EndDateTime</span></span>

<span data-ttu-id="a8b25-104">Элемент **EndDateTime** указывает Дата и время окончания для правила или поиска.</span><span class="sxs-lookup"><span data-stu-id="a8b25-104">The **EndDateTime** element specifies the end date and time for a rule or a search.</span></span> 
  
```XML
<EndDateTime/>
```

 <span data-ttu-id="a8b25-105">**dateTime**</span><span class="sxs-lookup"><span data-stu-id="a8b25-105">**dateTime**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a8b25-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="a8b25-106">Attributes and elements</span></span>

<span data-ttu-id="a8b25-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="a8b25-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a8b25-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="a8b25-108">Attributes</span></span>

<span data-ttu-id="a8b25-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="a8b25-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a8b25-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="a8b25-110">Child elements</span></span>

<span data-ttu-id="a8b25-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="a8b25-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="a8b25-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="a8b25-112">Parent elements</span></span>

|<span data-ttu-id="a8b25-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="a8b25-113">**Element**</span></span>|<span data-ttu-id="a8b25-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="a8b25-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a8b25-115">FindMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="a8b25-115">FindMessageTrackingReport</span></span>](findmessagetrackingreport.md) <br/> |<span data-ttu-id="a8b25-116">Содержит критерии для типов сообщений для поиска.</span><span class="sxs-lookup"><span data-stu-id="a8b25-116">Contains criteria for the types of messages to find.</span></span>  <br/> |
|[<span data-ttu-id="a8b25-117">WithinDateRange</span><span class="sxs-lookup"><span data-stu-id="a8b25-117">WithinDateRange</span></span>](withindaterange.md) <br/> |<span data-ttu-id="a8b25-118">Указывает диапазон дат, в течение которого нужно были получены в порядке для условие или исключение для применения входящих сообщений.</span><span class="sxs-lookup"><span data-stu-id="a8b25-118">Specifies the date range within which incoming messages have to have been received in order for the condition or exception to apply.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="a8b25-119">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="a8b25-119">Text value</span></span>

<span data-ttu-id="a8b25-120">Текстовое значение, представляющее даты/времени является обязательным, если данный элемент используется.</span><span class="sxs-lookup"><span data-stu-id="a8b25-120">A text value that represents a date/time is required if this element is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="a8b25-121">Замечания</span><span class="sxs-lookup"><span data-stu-id="a8b25-121">Remarks</span></span>

<span data-ttu-id="a8b25-122">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="a8b25-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a8b25-123">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="a8b25-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a8b25-124">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="a8b25-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="a8b25-125">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="a8b25-125">Schema Name</span></span>  <br/> |<span data-ttu-id="a8b25-126">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="a8b25-126">Messages schema</span></span>  <br/> |
|<span data-ttu-id="a8b25-127">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="a8b25-127">Validation File</span></span>  <br/> |<span data-ttu-id="a8b25-128">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="a8b25-128">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="a8b25-129">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="a8b25-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="a8b25-130">False</span><span class="sxs-lookup"><span data-stu-id="a8b25-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a8b25-131">См. также</span><span class="sxs-lookup"><span data-stu-id="a8b25-131">See also</span></span>



- [<span data-ttu-id="a8b25-132">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="a8b25-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

