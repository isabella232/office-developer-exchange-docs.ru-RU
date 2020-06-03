---
title: ассистантнамес
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 4e69022d-1cef-4744-877c-848a0b5c4f40
description: Элемент Ассистантнамес указывает массив имен помощников и идентификаторы их исходных сопоставлений для соответствующего пользователя.
ms.openlocfilehash: cb3722e07da97ed472f9ae50180d61ed761413c1
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461543"
---
# <a name="assistantnames"></a><span data-ttu-id="c1b18-103">ассистантнамес</span><span class="sxs-lookup"><span data-stu-id="c1b18-103">AssistantNames</span></span>

<span data-ttu-id="c1b18-104">Элемент **ассистантнамес** указывает массив имен помощников и идентификаторы их исходных сопоставлений для соответствующего пользователя.</span><span class="sxs-lookup"><span data-stu-id="c1b18-104">The **AssistantNames** element specifies an array of assistant names and the identifiers of their source attributions for the associated persona.</span></span> 
  
```XML
<AssistantNames>
    <StringAttributedValue></StringAttributedValue>
</AssistantNames>
```

 <span data-ttu-id="c1b18-105">**аррайофстрингаттрибутедвалуестипе**</span><span class="sxs-lookup"><span data-stu-id="c1b18-105">**ArrayOfStringAttributedValuesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c1b18-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="c1b18-106">Attributes and elements</span></span>

<span data-ttu-id="c1b18-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="c1b18-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c1b18-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="c1b18-108">Attributes</span></span>

<span data-ttu-id="c1b18-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="c1b18-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c1b18-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="c1b18-110">Child elements</span></span>

|<span data-ttu-id="c1b18-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="c1b18-111">**Element**</span></span>|<span data-ttu-id="c1b18-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="c1b18-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c1b18-113">стрингаттрибутедвалуе</span><span class="sxs-lookup"><span data-stu-id="c1b18-113">StringAttributedValue</span></span>](stringattributedvalue.md) <br/> |<span data-ttu-id="c1b18-114">Указывает экземпляр в массиве атрибутов, связанных с элементом персоны.</span><span class="sxs-lookup"><span data-stu-id="c1b18-114">Specifies an instance in an array of attributes associated with a persona element.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="c1b18-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="c1b18-115">Parent elements</span></span>

|<span data-ttu-id="c1b18-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="c1b18-116">**Element**</span></span>|<span data-ttu-id="c1b18-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="c1b18-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c1b18-118">Роль</span><span class="sxs-lookup"><span data-stu-id="c1b18-118">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="c1b18-119">Задает набор данных о пользователях, возвращаемых запросом к **другому человеку** .</span><span class="sxs-lookup"><span data-stu-id="c1b18-119">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="c1b18-120">Примечания</span><span class="sxs-lookup"><span data-stu-id="c1b18-120">Remarks</span></span>

<span data-ttu-id="c1b18-121">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="c1b18-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="c1b18-122">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="c1b18-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c1b18-123">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="c1b18-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c1b18-124">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="c1b18-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="c1b18-125">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="c1b18-125">Schema Name</span></span>  <br/> |<span data-ttu-id="c1b18-126">Схема типа</span><span class="sxs-lookup"><span data-stu-id="c1b18-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="c1b18-127">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="c1b18-127">Validation File</span></span>  <br/> |<span data-ttu-id="c1b18-128">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="c1b18-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="c1b18-129">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="c1b18-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="c1b18-130">См. также</span><span class="sxs-lookup"><span data-stu-id="c1b18-130">See also</span></span>

- [<span data-ttu-id="c1b18-131">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="c1b18-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

