---
title: Правила
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Rules
api_type:
- schema
ms.assetid: 53f59054-8f68-4eaa-be9c-ccfc9383bcf2
description: Элемент rules содержит массив правил защиты.
ms.openlocfilehash: 5d511f977f3eb3273dc43f56356a059985b2a929
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835269"
---
# <a name="rules"></a><span data-ttu-id="c5c97-103">Правила</span><span class="sxs-lookup"><span data-stu-id="c5c97-103">Rules</span></span>

<span data-ttu-id="c5c97-104">Элемент **Rules** содержит массив правил защиты.</span><span class="sxs-lookup"><span data-stu-id="c5c97-104">The **Rules** element contains an array of protection rules.</span></span> 
  
```xml
<Rules>   <Rule/></Rules>
```

 <span data-ttu-id="c5c97-105">**аррайофпротектионрулестипе**</span><span class="sxs-lookup"><span data-stu-id="c5c97-105">**ArrayOfProtectionRulesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c5c97-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="c5c97-106">Attributes and elements</span></span>

<span data-ttu-id="c5c97-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="c5c97-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c5c97-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="c5c97-108">Attributes</span></span>

<span data-ttu-id="c5c97-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="c5c97-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c5c97-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="c5c97-110">Child elements</span></span>

|<span data-ttu-id="c5c97-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="c5c97-111">**Element**</span></span>|<span data-ttu-id="c5c97-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="c5c97-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c5c97-113">Rule</span><span class="sxs-lookup"><span data-stu-id="c5c97-113">Rule</span></span>](rule.md) <br/> |<span data-ttu-id="c5c97-114">Содержит одно правило защиты.</span><span class="sxs-lookup"><span data-stu-id="c5c97-114">Contains a single protection rule.</span></span> <span data-ttu-id="c5c97-115">Этот элемент может встретиться ноль или более раз.</span><span class="sxs-lookup"><span data-stu-id="c5c97-115">This element can occur zero or more times.</span></span> <span data-ttu-id="c5c97-116">Этот элемент происходит в нулевое время, если в Организации не определены правила защиты.</span><span class="sxs-lookup"><span data-stu-id="c5c97-116">This element occurs zero times when no protection rules are defined by the organization.</span></span> <span data-ttu-id="c5c97-117">Он возникает один или несколько раз, если организация определила по крайней мере одно правило.</span><span class="sxs-lookup"><span data-stu-id="c5c97-117">It occurs one or more times if at least one rule is defined by the organization.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="c5c97-118">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="c5c97-118">Parent elements</span></span>

|<span data-ttu-id="c5c97-119">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="c5c97-119">**Element**</span></span>|<span data-ttu-id="c5c97-120">**Описание**</span><span class="sxs-lookup"><span data-stu-id="c5c97-120">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c5c97-121">протектионрулесконфигуратион</span><span class="sxs-lookup"><span data-stu-id="c5c97-121">ProtectionRulesConfiguration</span></span>](protectionrulesconfiguration.md) <br/> |<span data-ttu-id="c5c97-122">Содержит конфигурацию службы для службы правил защиты.</span><span class="sxs-lookup"><span data-stu-id="c5c97-122">Contains service configuration for the protection rules service.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="c5c97-123">Примечания</span><span class="sxs-lookup"><span data-stu-id="c5c97-123">Remarks</span></span>

<span data-ttu-id="c5c97-124">Схема, описывающая этот элемент, находится в виртуальном каталоге EWS компьютера под управлением Microsoft Exchange Server 2010, на котором установлена роль сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="c5c97-124">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c5c97-125">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="c5c97-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c5c97-126">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="c5c97-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="c5c97-127">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="c5c97-127">Schema Name</span></span>  <br/> |<span data-ttu-id="c5c97-128">Схема Types</span><span class="sxs-lookup"><span data-stu-id="c5c97-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="c5c97-129">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="c5c97-129">Validation File</span></span>  <br/> |<span data-ttu-id="c5c97-130">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="c5c97-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="c5c97-131">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="c5c97-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="c5c97-132">False</span><span class="sxs-lookup"><span data-stu-id="c5c97-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c5c97-133">См. также</span><span class="sxs-lookup"><span data-stu-id="c5c97-133">See also</span></span>



- [<span data-ttu-id="c5c97-134">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="c5c97-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

