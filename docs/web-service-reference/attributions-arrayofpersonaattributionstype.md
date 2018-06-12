---
title: Атрибуты (ArrayOfPersonaAttributionsType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f61d843c-bca5-4c88-9667-fd03d2a963a1
description: Атрибуты элемента указывает массив сведений атрибуты для одного или нескольких контактов или объединить в связанного пользователя Active Directory получателей.
ms.openlocfilehash: 52fecb4e4381d5e9dbbaf7134fa18068ba15f6ec
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761522"
---
# <a name="attributions-arrayofpersonaattributionstype"></a><span data-ttu-id="a19c0-103">Атрибуты (ArrayOfPersonaAttributionsType)</span><span class="sxs-lookup"><span data-stu-id="a19c0-103">Attributions (ArrayOfPersonaAttributionsType)</span></span>

<span data-ttu-id="a19c0-104">**Атрибуты** элемента указывает массив сведений атрибуты для одного или нескольких контактов или объединить в связанного пользователя Active Directory получателей.</span><span class="sxs-lookup"><span data-stu-id="a19c0-104">The **Attributions** element specifies an array of attribution information for one or more of the contacts or Active Directory recipients aggregated into the associated persona.</span></span> 
  
```XML
<Attributions>
    <Attribution></Attribution>
</Attributions>
```

 <span data-ttu-id="a19c0-105">**ArrayOfPersonaAttributionsType**</span><span class="sxs-lookup"><span data-stu-id="a19c0-105">**ArrayOfPersonaAttributionsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a19c0-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="a19c0-106">Attributes and elements</span></span>

<span data-ttu-id="a19c0-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="a19c0-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a19c0-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="a19c0-108">Attributes</span></span>

<span data-ttu-id="a19c0-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="a19c0-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a19c0-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="a19c0-110">Child elements</span></span>

|<span data-ttu-id="a19c0-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="a19c0-111">**Element**</span></span>|<span data-ttu-id="a19c0-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="a19c0-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a19c0-113">Атрибуты (PersonaAttributionType)</span><span class="sxs-lookup"><span data-stu-id="a19c0-113">Attribution (PersonaAttributionType)</span></span>](attribution-personaattributiontype.md) <br/> |<span data-ttu-id="a19c0-114">Задает экземпляр в массиве атрибутов элемента **PersonaType** .</span><span class="sxs-lookup"><span data-stu-id="a19c0-114">Specifies an instance in an array of attributes for a **PersonaType** element.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="a19c0-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="a19c0-115">Parent elements</span></span>

|<span data-ttu-id="a19c0-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="a19c0-116">**Element**</span></span>|<span data-ttu-id="a19c0-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="a19c0-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a19c0-118">Пользователь</span><span class="sxs-lookup"><span data-stu-id="a19c0-118">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="a19c0-119">Задает набор пользователя данные, возвращаемые запросом **GetPersona** .</span><span class="sxs-lookup"><span data-stu-id="a19c0-119">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="a19c0-120">Замечания</span><span class="sxs-lookup"><span data-stu-id="a19c0-120">Remarks</span></span>

<span data-ttu-id="a19c0-121">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="a19c0-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="a19c0-122">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="a19c0-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a19c0-123">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="a19c0-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a19c0-124">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="a19c0-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="a19c0-125">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="a19c0-125">Schema Name</span></span>  <br/> |<span data-ttu-id="a19c0-126">Схема типа</span><span class="sxs-lookup"><span data-stu-id="a19c0-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="a19c0-127">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="a19c0-127">Validation File</span></span>  <br/> |<span data-ttu-id="a19c0-128">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="a19c0-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="a19c0-129">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="a19c0-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="a19c0-130">См. также</span><span class="sxs-lookup"><span data-stu-id="a19c0-130">See also</span></span>

- [<span data-ttu-id="a19c0-131">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="a19c0-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
