---
title: Language (Дисковерисеарчконфигуратионтипе)
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 34eab81c-d832-4925-9f76-d69f24b36931
description: Элемент Language (Дисковерисеарчконфигуратионтипе) определяет язык и региональные параметры, используемые для форматирования диапазонов дат для определенного языка и региональных параметров. Он также определяет язык, используемый в поисковом запросе.
ms.openlocfilehash: 1e904ac4d7f525b2d12cfe83f0da33b9ed474066
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834197"
---
# <a name="language-discoverysearchconfigurationtype"></a><span data-ttu-id="888bb-104">Language (Дисковерисеарчконфигуратионтипе)</span><span class="sxs-lookup"><span data-stu-id="888bb-104">Language (DiscoverySearchConfigurationType)</span></span>

<span data-ttu-id="888bb-105">Элемент **Language (дисковерисеарчконфигуратионтипе)** определяет язык и региональные параметры, используемые для форматирования диапазонов дат для определенного языка и региональных параметров.</span><span class="sxs-lookup"><span data-stu-id="888bb-105">The **Language (DiscoverySearchConfigurationType)** element identifies the culture to be used for the culture-specific format of date ranges.</span></span> <span data-ttu-id="888bb-106">Он также определяет язык, используемый в поисковом запросе.</span><span class="sxs-lookup"><span data-stu-id="888bb-106">It also specifies the language used in a search query.</span></span> 
  
```XML
<Language />
```

 <span data-ttu-id="888bb-107">**строка**</span><span class="sxs-lookup"><span data-stu-id="888bb-107">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="888bb-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="888bb-108">Attributes and elements</span></span>

<span data-ttu-id="888bb-109">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="888bb-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="888bb-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="888bb-110">Attributes</span></span>

<span data-ttu-id="888bb-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="888bb-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="888bb-112">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="888bb-112">Child elements</span></span>

<span data-ttu-id="888bb-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="888bb-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="888bb-114">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="888bb-114">Parent elements</span></span>

[<span data-ttu-id="888bb-115">дисковерисеарчконфигуратион</span><span class="sxs-lookup"><span data-stu-id="888bb-115">DiscoverySearchConfiguration</span></span>](discoverysearchconfiguration.md)
  
## <a name="text-value"></a><span data-ttu-id="888bb-116">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="888bb-116">Text value</span></span>

<span data-ttu-id="888bb-117">Текстовое значение элемента **Language (дисковерисеарчконфигуратионтипе)** — это язык и региональные параметры или язык.</span><span class="sxs-lookup"><span data-stu-id="888bb-117">The text value of the **Language (DiscoverySearchConfigurationType)** element is a culture or language.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="888bb-118">Примечания</span><span class="sxs-lookup"><span data-stu-id="888bb-118">Remarks</span></span>

<span data-ttu-id="888bb-119">Этот элемент указывает формат диапазонов дат, указанных в [операции SearchMailboxes](searchmailboxes-operation.md) или [SetHoldOnMailboxes](setholdonmailboxes-operation.md).</span><span class="sxs-lookup"><span data-stu-id="888bb-119">This element specifies the format of date ranges specified in the [SearchMailboxes operation](searchmailboxes-operation.md) or the [SetHoldOnMailboxes operation](setholdonmailboxes-operation.md).</span></span>
  
<span data-ttu-id="888bb-120">Этот элемент появился в Exchange Server 2013 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="888bb-120">This element was introduced in Exchange Server 2013 Service Pack 1 (SP1).</span></span>
  
<span data-ttu-id="888bb-121">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="888bb-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="888bb-122">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="888bb-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="888bb-123">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="888bb-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="888bb-124">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="888bb-124">Schema Name</span></span>  <br/> |<span data-ttu-id="888bb-125">Схема Types</span><span class="sxs-lookup"><span data-stu-id="888bb-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="888bb-126">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="888bb-126">Validation File</span></span>  <br/> |<span data-ttu-id="888bb-127">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="888bb-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="888bb-128">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="888bb-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="888bb-129">True</span><span class="sxs-lookup"><span data-stu-id="888bb-129">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="888bb-130">См. также</span><span class="sxs-lookup"><span data-stu-id="888bb-130">See also</span></span>



[<span data-ttu-id="888bb-131">дисковерисеарчконфигуратион</span><span class="sxs-lookup"><span data-stu-id="888bb-131">DiscoverySearchConfiguration</span></span>](discoverysearchconfiguration.md)


- [<span data-ttu-id="888bb-132">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="888bb-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

