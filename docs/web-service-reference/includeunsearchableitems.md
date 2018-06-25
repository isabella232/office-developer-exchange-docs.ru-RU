---
title: IncludeUnsearchableItems
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 9a9bd2dc-f5b9-4b82-a6a0-f643d2951080
description: Элемент IncludeUnsearchableItems указывает, следует ли включать элементы, не удается выполнить поиск.
ms.openlocfilehash: 4c6b9b3752330bf914c9901d2e8f69e93546fec6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833907"
---
# <a name="includeunsearchableitems"></a><span data-ttu-id="cee69-103">IncludeUnsearchableItems</span><span class="sxs-lookup"><span data-stu-id="cee69-103">IncludeUnsearchableItems</span></span>

<span data-ttu-id="cee69-104">Элемент **IncludeUnsearchableItems** указывает, следует ли включать элементы, не удается выполнить поиск.</span><span class="sxs-lookup"><span data-stu-id="cee69-104">The **IncludeUnsearchableItems** element specifies whether to include items that cannot be searched.</span></span> 
  
```XML
<IncludeUnsearchableItems>true | false</IncludeUnsearchableItems>
```

 <span data-ttu-id="cee69-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="cee69-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="cee69-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="cee69-106">Attributes and elements</span></span>

<span data-ttu-id="cee69-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="cee69-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="cee69-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="cee69-108">Attributes</span></span>

<span data-ttu-id="cee69-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="cee69-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="cee69-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="cee69-110">Child elements</span></span>

<span data-ttu-id="cee69-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="cee69-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="cee69-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="cee69-112">Parent elements</span></span>

|<span data-ttu-id="cee69-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="cee69-113">**Element**</span></span>|<span data-ttu-id="cee69-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="cee69-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cee69-115">FindMailboxStatisticsByKeywords</span><span class="sxs-lookup"><span data-stu-id="cee69-115">FindMailboxStatisticsByKeywords</span></span>](findmailboxstatisticsbykeywords.md) <br/> |<span data-ttu-id="cee69-116">Определяет запрос для поиска по ключевым словам статистики почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="cee69-116">Specifies a request to search for mailbox statistics by keyword.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="cee69-117">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="cee69-117">Text value</span></span>

<span data-ttu-id="cee69-118">Текстовое значение **true** для элемента **IncludeUnsearchableItems** указывает, что статистика не включены для элементов, которые не являются с возможностью поиска.</span><span class="sxs-lookup"><span data-stu-id="cee69-118">A text value of **true** for the **IncludeUnsearchableItems** element indicates that statistics are not included for items that are not searchable.</span></span> <span data-ttu-id="cee69-119">Значение **false** указывает, что статистика включены для элементов, которые не являются с возможностью поиска.</span><span class="sxs-lookup"><span data-stu-id="cee69-119">A value of **false** indicates that statistics are included for items that are not searchable.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="cee69-120">Замечания</span><span class="sxs-lookup"><span data-stu-id="cee69-120">Remarks</span></span>

<span data-ttu-id="cee69-121">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="cee69-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="cee69-122">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="cee69-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="cee69-123">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="cee69-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="cee69-124">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="cee69-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="cee69-125">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="cee69-125">Schema Name</span></span>  <br/> |<span data-ttu-id="cee69-126">Схема сообщения</span><span class="sxs-lookup"><span data-stu-id="cee69-126">Message schema</span></span>  <br/> |
|<span data-ttu-id="cee69-127">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="cee69-127">Validation File</span></span>  <br/> |<span data-ttu-id="cee69-128">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="cee69-128">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="cee69-129">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="cee69-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="cee69-130">См. также</span><span class="sxs-lookup"><span data-stu-id="cee69-130">See also</span></span>



- [<span data-ttu-id="cee69-131">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="cee69-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

