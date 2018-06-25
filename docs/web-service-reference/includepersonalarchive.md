---
title: IncludePersonalArchive
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: b373bb1a-6b1d-4959-98a1-4c4ea62973bc
description: Элемент IncludePersonalArchive указывает, следует ли включать в поиск личного архива.
ms.openlocfilehash: ba2dcaae3befd3595815c7281858e4fa8a738e0a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833905"
---
# <a name="includepersonalarchive"></a><span data-ttu-id="fc996-103">IncludePersonalArchive</span><span class="sxs-lookup"><span data-stu-id="fc996-103">IncludePersonalArchive</span></span>

<span data-ttu-id="fc996-104">Элемент **IncludePersonalArchive** указывает, следует ли включать в поиск личного архива.</span><span class="sxs-lookup"><span data-stu-id="fc996-104">The **IncludePersonalArchive** element specifies whether to include the personal archive in the search.</span></span> 
  
```XML
<IncludePersonalArchive>true | false</IncludePersonalArchive>
```

 <span data-ttu-id="fc996-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="fc996-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="fc996-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="fc996-106">Attributes and elements</span></span>

<span data-ttu-id="fc996-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="fc996-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="fc996-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="fc996-108">Attributes</span></span>

<span data-ttu-id="fc996-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="fc996-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="fc996-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="fc996-110">Child elements</span></span>

<span data-ttu-id="fc996-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="fc996-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="fc996-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="fc996-112">Parent elements</span></span>

|<span data-ttu-id="fc996-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="fc996-113">**Element**</span></span>|<span data-ttu-id="fc996-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="fc996-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fc996-115">FindMailboxStatisticsByKeywords</span><span class="sxs-lookup"><span data-stu-id="fc996-115">FindMailboxStatisticsByKeywords</span></span>](findmailboxstatisticsbykeywords.md) <br/> |<span data-ttu-id="fc996-116">Определяет запрос для поиска по ключевым словам статистики почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="fc996-116">Specifies a request to search for mailbox statistics by keyword.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="fc996-117">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="fc996-117">Text value</span></span>

<span data-ttu-id="fc996-118">Текстовое значение **true** для элемента **IncludePersonalArchive** указывает, что личный архив включен в поиск.</span><span class="sxs-lookup"><span data-stu-id="fc996-118">A text value of **true** for the **IncludePersonalArchive** element indicates that the personal archive is included in the search.</span></span> <span data-ttu-id="fc996-119">Значение **false** указывает, что личный архив не включен в поиск.</span><span class="sxs-lookup"><span data-stu-id="fc996-119">A value of **false** indicates that the personal archive is not included in the search.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="fc996-120">Замечания</span><span class="sxs-lookup"><span data-stu-id="fc996-120">Remarks</span></span>

<span data-ttu-id="fc996-121">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="fc996-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="fc996-122">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="fc996-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="fc996-123">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="fc996-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="fc996-124">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="fc996-124">Schema Name</span></span>  <br/> |<span data-ttu-id="fc996-125">Схема сообщения</span><span class="sxs-lookup"><span data-stu-id="fc996-125">Message schema</span></span>  <br/> |
|<span data-ttu-id="fc996-126">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="fc996-126">Validation File</span></span>  <br/> |<span data-ttu-id="fc996-127">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="fc996-127">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="fc996-128">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="fc996-128">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="fc996-129">См. также</span><span class="sxs-lookup"><span data-stu-id="fc996-129">See also</span></span>



- [<span data-ttu-id="fc996-130">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="fc996-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

