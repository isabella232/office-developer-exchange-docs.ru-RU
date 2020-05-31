---
title: нетшовурл
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
description: Элемент Нетшовурл указывает URL-адрес собрания Microsoft NetShow Online.
ms.openlocfilehash: 2440e6c1501331d715d0e5ceb31b3b928122f927
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834519"
---
# <a name="netshowurl"></a><span data-ttu-id="bf537-103">нетшовурл</span><span class="sxs-lookup"><span data-stu-id="bf537-103">NetShowUrl</span></span>

<span data-ttu-id="bf537-104">Элемент **нетшовурл** указывает URL-адрес собрания Microsoft NetShow Online.</span><span class="sxs-lookup"><span data-stu-id="bf537-104">The **NetShowUrl** element specifies the URL for a Microsoft NetShow online meeting.</span></span> 
  
```xml
<NetShowUrl/>
```

 <span data-ttu-id="bf537-105">**строка**</span><span class="sxs-lookup"><span data-stu-id="bf537-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="bf537-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="bf537-106">Attributes and elements</span></span>

<span data-ttu-id="bf537-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="bf537-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="bf537-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="bf537-108">Attributes</span></span>

<span data-ttu-id="bf537-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="bf537-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="bf537-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="bf537-110">Child elements</span></span>

<span data-ttu-id="bf537-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="bf537-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="bf537-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="bf537-112">Parent elements</span></span>

|<span data-ttu-id="bf537-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="bf537-113">**Element**</span></span>|<span data-ttu-id="bf537-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="bf537-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bf537-115">Свойство meetingrequest</span><span class="sxs-lookup"><span data-stu-id="bf537-115">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="bf537-116">Представляет собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="bf537-116">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="bf537-117">календаритем</span><span class="sxs-lookup"><span data-stu-id="bf537-117">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="bf537-118">Представляет элемент календаря Exchange.</span><span class="sxs-lookup"><span data-stu-id="bf537-118">Represents an Exchange calendar item.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="bf537-119">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="bf537-119">Text value</span></span>

<span data-ttu-id="bf537-120">При использовании этого элемента необходимо указать текстовое значение, представляющее URL-адрес.</span><span class="sxs-lookup"><span data-stu-id="bf537-120">A text value that represents a URL is required if this element is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="bf537-121">Примечания</span><span class="sxs-lookup"><span data-stu-id="bf537-121">Remarks</span></span>

<span data-ttu-id="bf537-122">Это свойство Нетшовурл доступно для записи в элементе календаря организатора.</span><span class="sxs-lookup"><span data-stu-id="bf537-122">This NetShowUrl property is read-writable for the organizer's calendar item.</span></span> <span data-ttu-id="bf537-123">Он доступен только для чтения для приглашений на собрания и участников.</span><span class="sxs-lookup"><span data-stu-id="bf537-123">It is read-only for meeting requests and for attendees.</span></span>
  
<span data-ttu-id="bf537-124">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="bf537-124">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="bf537-125">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="bf537-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="bf537-126">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="bf537-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="bf537-127">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="bf537-127">Schema name</span></span>  <br/> |<span data-ttu-id="bf537-128">Схема Types</span><span class="sxs-lookup"><span data-stu-id="bf537-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="bf537-129">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="bf537-129">Validation file</span></span>  <br/> |<span data-ttu-id="bf537-130">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="bf537-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="bf537-131">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="bf537-131">Can be empty</span></span>  <br/> |<span data-ttu-id="bf537-132">False</span><span class="sxs-lookup"><span data-stu-id="bf537-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="bf537-133">См. также</span><span class="sxs-lookup"><span data-stu-id="bf537-133">See also</span></span>



- [<span data-ttu-id="bf537-134">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="bf537-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

