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
ms.openlocfilehash: 9556e4c1ef405ae66a71d19d99d9a71a61f54efc
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460136"
---
# <a name="enddatetime"></a><span data-ttu-id="23092-103">EndDateTime</span><span class="sxs-lookup"><span data-stu-id="23092-103">EndDateTime</span></span>

<span data-ttu-id="23092-104">Элемент **EndDateTime** указывает дату и время окончания для правила или поиска.</span><span class="sxs-lookup"><span data-stu-id="23092-104">The **EndDateTime** element specifies the end date and time for a rule or a search.</span></span> 
  
```XML
<EndDateTime/>
```

 <span data-ttu-id="23092-105">**дата и время**</span><span class="sxs-lookup"><span data-stu-id="23092-105">**dateTime**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="23092-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="23092-106">Attributes and elements</span></span>

<span data-ttu-id="23092-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="23092-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="23092-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="23092-108">Attributes</span></span>

<span data-ttu-id="23092-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="23092-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="23092-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="23092-110">Child elements</span></span>

<span data-ttu-id="23092-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="23092-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="23092-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="23092-112">Parent elements</span></span>

|<span data-ttu-id="23092-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="23092-113">**Element**</span></span>|<span data-ttu-id="23092-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="23092-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="23092-115">FindMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="23092-115">FindMessageTrackingReport</span></span>](findmessagetrackingreport.md) <br/> |<span data-ttu-id="23092-116">Содержит условия для типов сообщений, которые требуется найти.</span><span class="sxs-lookup"><span data-stu-id="23092-116">Contains criteria for the types of messages to find.</span></span>  <br/> |
|[<span data-ttu-id="23092-117">висиндатеранже</span><span class="sxs-lookup"><span data-stu-id="23092-117">WithinDateRange</span></span>](withindaterange.md) <br/> |<span data-ttu-id="23092-118">Указывает диапазон дат, в течение которого должны быть получены входящие сообщения, чтобы применялось условие или исключение.</span><span class="sxs-lookup"><span data-stu-id="23092-118">Specifies the date range within which incoming messages have to have been received in order for the condition or exception to apply.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="23092-119">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="23092-119">Text value</span></span>

<span data-ttu-id="23092-120">При использовании этого элемента необходимо указать текстовое значение, представляющее дату и время.</span><span class="sxs-lookup"><span data-stu-id="23092-120">A text value that represents a date/time is required if this element is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="23092-121">Примечания</span><span class="sxs-lookup"><span data-stu-id="23092-121">Remarks</span></span>

<span data-ttu-id="23092-122">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="23092-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="23092-123">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="23092-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="23092-124">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="23092-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="23092-125">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="23092-125">Schema Name</span></span>  <br/> |<span data-ttu-id="23092-126">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="23092-126">Messages schema</span></span>  <br/> |
|<span data-ttu-id="23092-127">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="23092-127">Validation File</span></span>  <br/> |<span data-ttu-id="23092-128">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="23092-128">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="23092-129">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="23092-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="23092-130">False</span><span class="sxs-lookup"><span data-stu-id="23092-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="23092-131">См. также</span><span class="sxs-lookup"><span data-stu-id="23092-131">See also</span></span>



- [<span data-ttu-id="23092-132">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="23092-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

