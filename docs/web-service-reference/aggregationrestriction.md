---
title: аггрегатионрестриктион
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: d05044f9-d2ff-4aca-956c-20c9cb2f7709
description: Элемент Аггрегатионрестриктион указывает значение, которое применяется к набору свойств пользователя, полученному при запросе FindPeople, и фильтрует результат в соответствии с указанным ограничением.
ms.openlocfilehash: f07e54235cf13b43da26ed1c56596d3c7c357bf2
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463526"
---
# <a name="aggregationrestriction"></a><span data-ttu-id="86b98-103">аггрегатионрестриктион</span><span class="sxs-lookup"><span data-stu-id="86b98-103">AggregationRestriction</span></span>

<span data-ttu-id="86b98-104">Элемент **аггрегатионрестриктион** указывает значение, которое применяется к набору свойств пользователя, полученному при запросе FindPeople, и фильтрует результат в соответствии с указанным ограничением.</span><span class="sxs-lookup"><span data-stu-id="86b98-104">The **AggregationRestriction** element specifies a value that is applied to a set of Persona properties resulting from a FindPeople request and filters the result according to the specified restriction.</span></span> 
  
```XML
<AggregationRestriction>
   <SearchExpression/>
</AggregationRestriction>
```

 <span data-ttu-id="86b98-105">**рестриктионтипе**</span><span class="sxs-lookup"><span data-stu-id="86b98-105">**RestrictionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="86b98-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="86b98-106">Attributes and elements</span></span>

<span data-ttu-id="86b98-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="86b98-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="86b98-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="86b98-108">Attributes</span></span>

<span data-ttu-id="86b98-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="86b98-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="86b98-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="86b98-110">Child elements</span></span>

[<span data-ttu-id="86b98-111">сеарчекспрессион</span><span class="sxs-lookup"><span data-stu-id="86b98-111">SearchExpression</span></span>](searchexpression.md)
  
### <a name="parent-elements"></a><span data-ttu-id="86b98-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="86b98-112">Parent elements</span></span>

[<span data-ttu-id="86b98-113">FindPeople</span><span class="sxs-lookup"><span data-stu-id="86b98-113">FindPeople</span></span>](findpeople.md)
  
## <a name="remarks"></a><span data-ttu-id="86b98-114">Примечания</span><span class="sxs-lookup"><span data-stu-id="86b98-114">Remarks</span></span>

<span data-ttu-id="86b98-115">Элемент **аггрегатионрестриктион** может содержать любой дочерний элемент, в котором используется группа подстановки **сеарчекспрессион** .</span><span class="sxs-lookup"><span data-stu-id="86b98-115">The **AggregationRestriction** element can contain any child element that uses the **SearchExpression** substitution group.</span></span> <span data-ttu-id="86b98-116">Элементами, которые являются частью группы подстановки **сеарчекспрессион** : [Contains](contains.md), [Exclude](excludes.md), [Exists](exists.md), [Not](not.md), [or](or.md) [и](and.md), [исекуалто](isequalto.md), [иснотекуалто](isnotequalto.md), [исгреатерсан](isgreaterthan.md), [исгреатерсанорекуалто](isgreaterthanorequalto.md), [ислесссан](islessthan.md)и [IsLessThanOrEqualTo](islessthanorequalto.md).</span><span class="sxs-lookup"><span data-stu-id="86b98-116">The elements that are a part of the **SearchExpression** substitution group are: [Contains](contains.md), [Excludes](excludes.md), [Exists](exists.md), [Not](not.md), [Or](or.md), [And](and.md), [IsEqualTo](isequalto.md), [IsNotEqualTo](isnotequalto.md), [IsGreaterThan](isgreaterthan.md), [IsGreaterThanOrEqualTo](isgreaterthanorequalto.md), [IsLessThan](islessthan.md), and [IsLessThanOrEqualTo](islessthanorequalto.md).</span></span>
  
<span data-ttu-id="86b98-117">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="86b98-117">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="86b98-118">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="86b98-118">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="86b98-119">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="86b98-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="86b98-120">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="86b98-120">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="86b98-121">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="86b98-121">Schema name</span></span>  <br/> |<span data-ttu-id="86b98-122">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="86b98-122">Messages schema</span></span>  <br/> |
|<span data-ttu-id="86b98-123">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="86b98-123">Validation file</span></span>  <br/> |<span data-ttu-id="86b98-124">messages. xsd</span><span class="sxs-lookup"><span data-stu-id="86b98-124">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="86b98-125">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="86b98-125">Can be empty</span></span>  <br/> |<span data-ttu-id="86b98-126">false</span><span class="sxs-lookup"><span data-stu-id="86b98-126">false</span></span>  <br/> |
   

