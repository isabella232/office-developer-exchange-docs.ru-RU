---
title: Атрибуты (Аррайофперсонааттрибутионстипе)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f61d843c-bca5-4c88-9667-fd03d2a963a1
description: Элемент "атрибуты" определяет массив сведений о сопоставлении для одного или нескольких контактов или получателей Active Directory, собранных в связанный с ним пользователь.
ms.openlocfilehash: a9883e06a8adbd5c9d3bc7e1edd28c62418df653
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460325"
---
# <a name="attributions-arrayofpersonaattributionstype"></a><span data-ttu-id="d0d1c-103">Атрибуты (Аррайофперсонааттрибутионстипе)</span><span class="sxs-lookup"><span data-stu-id="d0d1c-103">Attributions (ArrayOfPersonaAttributionsType)</span></span>

<span data-ttu-id="d0d1c-104">Элемент " **атрибуты** " определяет массив сведений о сопоставлении для одного или нескольких контактов или получателей Active Directory, собранных в связанный с ним пользователь.</span><span class="sxs-lookup"><span data-stu-id="d0d1c-104">The **Attributions** element specifies an array of attribution information for one or more of the contacts or Active Directory recipients aggregated into the associated persona.</span></span> 
  
```XML
<Attributions>
    <Attribution></Attribution>
</Attributions>
```

 <span data-ttu-id="d0d1c-105">**аррайофперсонааттрибутионстипе**</span><span class="sxs-lookup"><span data-stu-id="d0d1c-105">**ArrayOfPersonaAttributionsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d0d1c-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="d0d1c-106">Attributes and elements</span></span>

<span data-ttu-id="d0d1c-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="d0d1c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d0d1c-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="d0d1c-108">Attributes</span></span>

<span data-ttu-id="d0d1c-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="d0d1c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d0d1c-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="d0d1c-110">Child elements</span></span>

|<span data-ttu-id="d0d1c-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="d0d1c-111">**Element**</span></span>|<span data-ttu-id="d0d1c-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d0d1c-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d0d1c-113">Атрибуты (Персонааттрибутионтипе)</span><span class="sxs-lookup"><span data-stu-id="d0d1c-113">Attribution (PersonaAttributionType)</span></span>](attribution-personaattributiontype.md) <br/> |<span data-ttu-id="d0d1c-114">Указывает экземпляр в массиве атрибутов для элемента **персонатипе** .</span><span class="sxs-lookup"><span data-stu-id="d0d1c-114">Specifies an instance in an array of attributes for a **PersonaType** element.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d0d1c-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="d0d1c-115">Parent elements</span></span>

|<span data-ttu-id="d0d1c-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="d0d1c-116">**Element**</span></span>|<span data-ttu-id="d0d1c-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d0d1c-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d0d1c-118">Роль</span><span class="sxs-lookup"><span data-stu-id="d0d1c-118">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="d0d1c-119">Задает набор данных о пользователях, возвращаемых запросом к **другому человеку** .</span><span class="sxs-lookup"><span data-stu-id="d0d1c-119">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="d0d1c-120">Примечания</span><span class="sxs-lookup"><span data-stu-id="d0d1c-120">Remarks</span></span>

<span data-ttu-id="d0d1c-121">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="d0d1c-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="d0d1c-122">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="d0d1c-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d0d1c-123">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="d0d1c-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d0d1c-124">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="d0d1c-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d0d1c-125">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="d0d1c-125">Schema Name</span></span>  <br/> |<span data-ttu-id="d0d1c-126">Схема типа</span><span class="sxs-lookup"><span data-stu-id="d0d1c-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="d0d1c-127">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="d0d1c-127">Validation File</span></span>  <br/> |<span data-ttu-id="d0d1c-128">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="d0d1c-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="d0d1c-129">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="d0d1c-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="d0d1c-130">См. также</span><span class="sxs-lookup"><span data-stu-id="d0d1c-130">See also</span></span>

- [<span data-ttu-id="d0d1c-131">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="d0d1c-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

