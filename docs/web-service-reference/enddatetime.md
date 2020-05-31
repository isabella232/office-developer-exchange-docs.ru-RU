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
description: Элемент EndDateTime указывает дату и время окончания для правила или поиска.
ms.openlocfilehash: ad596c6441e7bdb10b4e886a8d0f3ba183c43c3e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762351"
---
# <a name="enddatetime"></a><span data-ttu-id="3a17b-103">EndDateTime</span><span class="sxs-lookup"><span data-stu-id="3a17b-103">EndDateTime</span></span>

<span data-ttu-id="3a17b-104">Элемент **EndDateTime** указывает дату и время окончания для правила или поиска.</span><span class="sxs-lookup"><span data-stu-id="3a17b-104">The **EndDateTime** element specifies the end date and time for a rule or a search.</span></span> 
  
```XML
<EndDateTime/>
```

 <span data-ttu-id="3a17b-105">**дата и время**</span><span class="sxs-lookup"><span data-stu-id="3a17b-105">**dateTime**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3a17b-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="3a17b-106">Attributes and elements</span></span>

<span data-ttu-id="3a17b-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="3a17b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3a17b-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="3a17b-108">Attributes</span></span>

<span data-ttu-id="3a17b-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="3a17b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3a17b-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="3a17b-110">Child elements</span></span>

<span data-ttu-id="3a17b-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="3a17b-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="3a17b-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="3a17b-112">Parent elements</span></span>

|<span data-ttu-id="3a17b-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="3a17b-113">**Element**</span></span>|<span data-ttu-id="3a17b-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="3a17b-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3a17b-115">FindMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="3a17b-115">FindMessageTrackingReport</span></span>](findmessagetrackingreport.md) <br/> |<span data-ttu-id="3a17b-116">Содержит условия для типов сообщений, которые требуется найти.</span><span class="sxs-lookup"><span data-stu-id="3a17b-116">Contains criteria for the types of messages to find.</span></span>  <br/> |
|[<span data-ttu-id="3a17b-117">висиндатеранже</span><span class="sxs-lookup"><span data-stu-id="3a17b-117">WithinDateRange</span></span>](withindaterange.md) <br/> |<span data-ttu-id="3a17b-118">Указывает диапазон дат, в течение которого должны быть получены входящие сообщения, чтобы применялось условие или исключение.</span><span class="sxs-lookup"><span data-stu-id="3a17b-118">Specifies the date range within which incoming messages have to have been received in order for the condition or exception to apply.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="3a17b-119">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="3a17b-119">Text value</span></span>

<span data-ttu-id="3a17b-120">При использовании этого элемента необходимо указать текстовое значение, представляющее дату и время.</span><span class="sxs-lookup"><span data-stu-id="3a17b-120">A text value that represents a date/time is required if this element is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="3a17b-121">Примечания</span><span class="sxs-lookup"><span data-stu-id="3a17b-121">Remarks</span></span>

<span data-ttu-id="3a17b-122">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="3a17b-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3a17b-123">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="3a17b-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3a17b-124">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="3a17b-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="3a17b-125">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="3a17b-125">Schema Name</span></span>  <br/> |<span data-ttu-id="3a17b-126">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="3a17b-126">Messages schema</span></span>  <br/> |
|<span data-ttu-id="3a17b-127">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="3a17b-127">Validation File</span></span>  <br/> |<span data-ttu-id="3a17b-128">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="3a17b-128">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="3a17b-129">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="3a17b-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="3a17b-130">False</span><span class="sxs-lookup"><span data-stu-id="3a17b-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3a17b-131">См. также</span><span class="sxs-lookup"><span data-stu-id="3a17b-131">See also</span></span>



- [<span data-ttu-id="3a17b-132">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="3a17b-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

