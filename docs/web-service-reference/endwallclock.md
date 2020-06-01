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
ms.openlocfilehash: 48b762d0bfe367b966b6f1790230f6a2118c3fd6
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462973"
---
# <a name="endwallclock"></a><span data-ttu-id="ec1d5-103">ендваллклокк</span><span class="sxs-lookup"><span data-stu-id="ec1d5-103">EndWallClock</span></span>

<span data-ttu-id="ec1d5-104">Элемент **ендваллклокк** указывает время окончания собрания в часовом поясе, где выполняется собрание.</span><span class="sxs-lookup"><span data-stu-id="ec1d5-104">The **EndWallClock** element specifies the end time of a meeting in the time zone of the location in which the meeting takes place.</span></span> 
  
```XML
<EndWallClock></EndWallClock>
```

 <span data-ttu-id="ec1d5-105">**дата и время**</span><span class="sxs-lookup"><span data-stu-id="ec1d5-105">**dateTime**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ec1d5-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="ec1d5-106">Attributes and elements</span></span>

<span data-ttu-id="ec1d5-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="ec1d5-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ec1d5-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="ec1d5-108">Attributes</span></span>

<span data-ttu-id="ec1d5-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="ec1d5-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ec1d5-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="ec1d5-110">Child elements</span></span>

<span data-ttu-id="ec1d5-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="ec1d5-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="ec1d5-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="ec1d5-112">Parent elements</span></span>

|<span data-ttu-id="ec1d5-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="ec1d5-113">**Element**</span></span>|<span data-ttu-id="ec1d5-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="ec1d5-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ec1d5-115">Роль</span><span class="sxs-lookup"><span data-stu-id="ec1d5-115">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="ec1d5-116">Задает набор данных о пользователях, возвращаемых запросом к **другому человеку** .</span><span class="sxs-lookup"><span data-stu-id="ec1d5-116">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="ec1d5-117">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="ec1d5-117">Text value</span></span>

<span data-ttu-id="ec1d5-118">Текстовое значение элемента **ендваллклокк** — это строковое значение, задающее идентификатор часового пояса.</span><span class="sxs-lookup"><span data-stu-id="ec1d5-118">The text value of the **EndWallClock** element is a string value that specifies the time zone identifier.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="ec1d5-119">Примечания</span><span class="sxs-lookup"><span data-stu-id="ec1d5-119">Remarks</span></span>

<span data-ttu-id="ec1d5-120">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="ec1d5-120">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="ec1d5-121">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="ec1d5-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ec1d5-122">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="ec1d5-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ec1d5-123">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="ec1d5-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="ec1d5-124">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="ec1d5-124">Schema Name</span></span>  <br/> |<span data-ttu-id="ec1d5-125">Схема типа</span><span class="sxs-lookup"><span data-stu-id="ec1d5-125">Type schema</span></span>  <br/> |
|<span data-ttu-id="ec1d5-126">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="ec1d5-126">Validation File</span></span>  <br/> |<span data-ttu-id="ec1d5-127">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="ec1d5-127">types.xsd</span></span>  <br/> |
|<span data-ttu-id="ec1d5-128">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="ec1d5-128">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="ec1d5-129">См. также</span><span class="sxs-lookup"><span data-stu-id="ec1d5-129">See also</span></span>



- [<span data-ttu-id="ec1d5-130">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="ec1d5-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

