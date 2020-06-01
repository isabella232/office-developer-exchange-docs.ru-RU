---
title: хомеаддрессес
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 57fb1b9d-2ba8-4359-ae79-35c0d56a2d0f
description: Элемент Хомеаддрессес указывает массив домашних адресов и идентификаторы их исходных атрибутов для связанного пользователя.
ms.openlocfilehash: d6a1808bf000ac8bca1e2ce7865aa099037c5a5d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460892"
---
# <a name="homeaddresses"></a><span data-ttu-id="e1578-103">хомеаддрессес</span><span class="sxs-lookup"><span data-stu-id="e1578-103">HomeAddresses</span></span>

<span data-ttu-id="e1578-104">Элемент **хомеаддрессес** указывает массив домашних адресов и идентификаторы их исходных атрибутов для связанного пользователя.</span><span class="sxs-lookup"><span data-stu-id="e1578-104">The **HomeAddresses** element specifies an array of home addresses and the identifiers of their source attributions for the associated persona.</span></span> 
  
```XML
<HomeAddresses>
    <PostalAddressAttributedValue/>
</HomeAddresses>
```

 <span data-ttu-id="e1578-105">**аррайофпосталаддрессаттрибутедвалуестипе**</span><span class="sxs-lookup"><span data-stu-id="e1578-105">**ArrayOfPostalAddressAttributedValuesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e1578-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="e1578-106">Attributes and elements</span></span>

<span data-ttu-id="e1578-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="e1578-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e1578-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="e1578-108">Attributes</span></span>

<span data-ttu-id="e1578-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="e1578-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e1578-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="e1578-110">Child elements</span></span>

|<span data-ttu-id="e1578-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="e1578-111">**Element**</span></span>|<span data-ttu-id="e1578-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="e1578-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e1578-113">посталаддрессаттрибутедвалуе</span><span class="sxs-lookup"><span data-stu-id="e1578-113">PostalAddressAttributedValue</span></span>](postaladdressattributedvalue.md) <br/> |<span data-ttu-id="e1578-114">Указывает экземпляр массива почтовых адресов и связанные с ними атрибуты.</span><span class="sxs-lookup"><span data-stu-id="e1578-114">Specifies an instance of an array of postal addresses and their associated attributions.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="e1578-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="e1578-115">Parent elements</span></span>

|<span data-ttu-id="e1578-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="e1578-116">**Element**</span></span>|<span data-ttu-id="e1578-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="e1578-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e1578-118">Роль</span><span class="sxs-lookup"><span data-stu-id="e1578-118">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="e1578-119">Задает набор данных о пользователях, возвращаемых запросом к **другому человеку** .</span><span class="sxs-lookup"><span data-stu-id="e1578-119">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="e1578-120">Примечания</span><span class="sxs-lookup"><span data-stu-id="e1578-120">Remarks</span></span>

<span data-ttu-id="e1578-121">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="e1578-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="e1578-122">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="e1578-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e1578-123">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="e1578-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e1578-124">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="e1578-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e1578-125">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="e1578-125">Schema Name</span></span>  <br/> |<span data-ttu-id="e1578-126">Схема типа</span><span class="sxs-lookup"><span data-stu-id="e1578-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="e1578-127">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="e1578-127">Validation File</span></span>  <br/> |<span data-ttu-id="e1578-128">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="e1578-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="e1578-129">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="e1578-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="e1578-130">См. также</span><span class="sxs-lookup"><span data-stu-id="e1578-130">See also</span></span>



- [<span data-ttu-id="e1578-131">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="e1578-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

