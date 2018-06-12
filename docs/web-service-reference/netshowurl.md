---
title: NetShowUrl
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- NetShowUrl
api_type:
- schema
ms.assetid: a5d48fc1-b141-422c-bcb0-05d0f9ba90dd
description: Элемент NetShowUrl указывает URL-адрес для Microsoft NetShow собрание по сети.
ms.openlocfilehash: 2440e6c1501331d715d0e5ceb31b3b928122f927
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19834519"
---
# <a name="netshowurl"></a><span data-ttu-id="b2ecb-103">NetShowUrl</span><span class="sxs-lookup"><span data-stu-id="b2ecb-103">NetShowUrl</span></span>

<span data-ttu-id="b2ecb-104">Элемент **NetShowUrl** указывает URL-адрес для Microsoft NetShow собрание по сети.</span><span class="sxs-lookup"><span data-stu-id="b2ecb-104">The **NetShowUrl** element specifies the URL for a Microsoft NetShow online meeting.</span></span> 
  
```xml
<NetShowUrl/>
```

 <span data-ttu-id="b2ecb-105">**string**</span><span class="sxs-lookup"><span data-stu-id="b2ecb-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b2ecb-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="b2ecb-106">Attributes and elements</span></span>

<span data-ttu-id="b2ecb-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="b2ecb-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b2ecb-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="b2ecb-108">Attributes</span></span>

<span data-ttu-id="b2ecb-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="b2ecb-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b2ecb-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="b2ecb-110">Child elements</span></span>

<span data-ttu-id="b2ecb-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="b2ecb-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="b2ecb-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="b2ecb-112">Parent elements</span></span>

|<span data-ttu-id="b2ecb-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="b2ecb-113">**Element**</span></span>|<span data-ttu-id="b2ecb-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="b2ecb-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b2ecb-115">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="b2ecb-115">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="b2ecb-116">Представляет собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="b2ecb-116">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="b2ecb-117">Элемента календаря, имеющего</span><span class="sxs-lookup"><span data-stu-id="b2ecb-117">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="b2ecb-118">Представляет элемент календаря Exchange.</span><span class="sxs-lookup"><span data-stu-id="b2ecb-118">Represents an Exchange calendar item.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="b2ecb-119">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="b2ecb-119">Text value</span></span>

<span data-ttu-id="b2ecb-120">Текстовое значение, представляющее URL-адрес является обязательным, если данный элемент используется.</span><span class="sxs-lookup"><span data-stu-id="b2ecb-120">A text value that represents a URL is required if this element is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="b2ecb-121">Замечания</span><span class="sxs-lookup"><span data-stu-id="b2ecb-121">Remarks</span></span>

<span data-ttu-id="b2ecb-122">Это свойство NetShowUrl чтения записи для организатора элемента календаря.</span><span class="sxs-lookup"><span data-stu-id="b2ecb-122">This NetShowUrl property is read-writable for the organizer's calendar item.</span></span> <span data-ttu-id="b2ecb-123">Оно доступно только для чтения, для приглашений на собрания и участников.</span><span class="sxs-lookup"><span data-stu-id="b2ecb-123">It is read-only for meeting requests and for attendees.</span></span>
  
<span data-ttu-id="b2ecb-124">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="b2ecb-124">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b2ecb-125">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="b2ecb-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b2ecb-126">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="b2ecb-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="b2ecb-127">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="b2ecb-127">Schema name</span></span>  <br/> |<span data-ttu-id="b2ecb-128">Схема Types</span><span class="sxs-lookup"><span data-stu-id="b2ecb-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="b2ecb-129">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="b2ecb-129">Validation file</span></span>  <br/> |<span data-ttu-id="b2ecb-130">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="b2ecb-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="b2ecb-131">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="b2ecb-131">Can be empty</span></span>  <br/> |<span data-ttu-id="b2ecb-132">False</span><span class="sxs-lookup"><span data-stu-id="b2ecb-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b2ecb-133">См. также</span><span class="sxs-lookup"><span data-stu-id="b2ecb-133">See also</span></span>



- [<span data-ttu-id="b2ecb-134">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="b2ecb-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

