---
title: Текст сообщений
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: a71a75f0-0b77-4cb9-8f9d-319de72fc1fd
description: Элемент тела указывает массив элементов BodyContentAttributedValue.
ms.openlocfilehash: 3316d25a567a791301c0e703a912ef28da42fa74
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761580"
---
# <a name="bodies"></a><span data-ttu-id="0c013-103">Текст сообщений</span><span class="sxs-lookup"><span data-stu-id="0c013-103">Bodies</span></span>

<span data-ttu-id="0c013-104">Элемент **тела** указывает массив элементов **BodyContentAttributedValue** .</span><span class="sxs-lookup"><span data-stu-id="0c013-104">The **Bodies** element specifies an array of **BodyContentAttributedValue** elements.</span></span> 
  
```XML
<Bodies>
    <BodyContentAttributedValue></BodyContentAttributedValue>
<Bodies>
```

 <span data-ttu-id="0c013-105">**ArrayOfBodyContentAttributedValuesType**</span><span class="sxs-lookup"><span data-stu-id="0c013-105">**ArrayOfBodyContentAttributedValuesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0c013-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="0c013-106">Attributes and elements</span></span>

<span data-ttu-id="0c013-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="0c013-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0c013-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="0c013-108">Attributes</span></span>

<span data-ttu-id="0c013-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="0c013-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0c013-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="0c013-110">Child elements</span></span>

|<span data-ttu-id="0c013-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="0c013-111">**Element**</span></span>|<span data-ttu-id="0c013-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="0c013-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0c013-113">BodyContentAttributedValue</span><span class="sxs-lookup"><span data-stu-id="0c013-113">BodyContentAttributedValue</span></span>](bodycontentattributedvalue.md) <br/> |<span data-ttu-id="0c013-114">Указывает содержимое основного текста элемента.</span><span class="sxs-lookup"><span data-stu-id="0c013-114">Specifies the body content of an item.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="0c013-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="0c013-115">Parent elements</span></span>

|<span data-ttu-id="0c013-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="0c013-116">**Element**</span></span>|<span data-ttu-id="0c013-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="0c013-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0c013-118">Пользователь</span><span class="sxs-lookup"><span data-stu-id="0c013-118">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="0c013-119">Задает набор пользователя данные, возвращаемые запросом **GetPersona** .</span><span class="sxs-lookup"><span data-stu-id="0c013-119">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="0c013-120">Замечания</span><span class="sxs-lookup"><span data-stu-id="0c013-120">Remarks</span></span>

<span data-ttu-id="0c013-121">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="0c013-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="0c013-122">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="0c013-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0c013-123">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="0c013-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0c013-124">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="0c013-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="0c013-125">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="0c013-125">Schema Name</span></span>  <br/> |<span data-ttu-id="0c013-126">Схема типа</span><span class="sxs-lookup"><span data-stu-id="0c013-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="0c013-127">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="0c013-127">Validation File</span></span>  <br/> |<span data-ttu-id="0c013-128">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="0c013-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="0c013-129">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="0c013-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="0c013-130">См. также</span><span class="sxs-lookup"><span data-stu-id="0c013-130">See also</span></span>



- [<span data-ttu-id="0c013-131">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="0c013-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
