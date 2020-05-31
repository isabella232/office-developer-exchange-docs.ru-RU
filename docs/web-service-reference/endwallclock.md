---
title: ендваллклокк
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: bc04e44e-e6d1-4355-a2b1-feb6663dc647
description: Элемент Ендваллклокк указывает время окончания собрания в часовом поясе, где выполняется собрание.
ms.openlocfilehash: 10e4a2bde50354b2f2752751c01a6a70aa084d05
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762356"
---
# <a name="endwallclock"></a><span data-ttu-id="c9350-103">ендваллклокк</span><span class="sxs-lookup"><span data-stu-id="c9350-103">EndWallClock</span></span>

<span data-ttu-id="c9350-104">Элемент **ендваллклокк** указывает время окончания собрания в часовом поясе, где выполняется собрание.</span><span class="sxs-lookup"><span data-stu-id="c9350-104">The **EndWallClock** element specifies the end time of a meeting in the time zone of the location in which the meeting takes place.</span></span> 
  
```XML
<EndWallClock></EndWallClock>
```

 <span data-ttu-id="c9350-105">**дата и время**</span><span class="sxs-lookup"><span data-stu-id="c9350-105">**dateTime**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c9350-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="c9350-106">Attributes and elements</span></span>

<span data-ttu-id="c9350-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="c9350-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c9350-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="c9350-108">Attributes</span></span>

<span data-ttu-id="c9350-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="c9350-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c9350-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="c9350-110">Child elements</span></span>

<span data-ttu-id="c9350-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="c9350-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="c9350-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="c9350-112">Parent elements</span></span>

|<span data-ttu-id="c9350-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="c9350-113">**Element**</span></span>|<span data-ttu-id="c9350-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="c9350-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c9350-115">Роль</span><span class="sxs-lookup"><span data-stu-id="c9350-115">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="c9350-116">Задает набор данных о пользователях, возвращаемых запросом к **другому человеку** .</span><span class="sxs-lookup"><span data-stu-id="c9350-116">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="c9350-117">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="c9350-117">Text value</span></span>

<span data-ttu-id="c9350-118">Текстовое значение элемента **ендваллклокк** — это строковое значение, задающее идентификатор часового пояса.</span><span class="sxs-lookup"><span data-stu-id="c9350-118">The text value of the **EndWallClock** element is a string value that specifies the time zone identifier.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="c9350-119">Примечания</span><span class="sxs-lookup"><span data-stu-id="c9350-119">Remarks</span></span>

<span data-ttu-id="c9350-120">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="c9350-120">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="c9350-121">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="c9350-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c9350-122">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="c9350-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c9350-123">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="c9350-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="c9350-124">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="c9350-124">Schema Name</span></span>  <br/> |<span data-ttu-id="c9350-125">Схема типа</span><span class="sxs-lookup"><span data-stu-id="c9350-125">Type schema</span></span>  <br/> |
|<span data-ttu-id="c9350-126">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="c9350-126">Validation File</span></span>  <br/> |<span data-ttu-id="c9350-127">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="c9350-127">types.xsd</span></span>  <br/> |
|<span data-ttu-id="c9350-128">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="c9350-128">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="c9350-129">См. также</span><span class="sxs-lookup"><span data-stu-id="c9350-129">See also</span></span>



- [<span data-ttu-id="c9350-130">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="c9350-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

