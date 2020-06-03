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
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460892"
---
# <a name="homeaddresses"></a><span data-ttu-id="a2b7d-103">хомеаддрессес</span><span class="sxs-lookup"><span data-stu-id="a2b7d-103">HomeAddresses</span></span>

<span data-ttu-id="a2b7d-104">Элемент **хомеаддрессес** указывает массив домашних адресов и идентификаторы их исходных атрибутов для связанного пользователя.</span><span class="sxs-lookup"><span data-stu-id="a2b7d-104">The **HomeAddresses** element specifies an array of home addresses and the identifiers of their source attributions for the associated persona.</span></span> 
  
```XML
<HomeAddresses>
    <PostalAddressAttributedValue/>
</HomeAddresses>
```

 <span data-ttu-id="a2b7d-105">**аррайофпосталаддрессаттрибутедвалуестипе**</span><span class="sxs-lookup"><span data-stu-id="a2b7d-105">**ArrayOfPostalAddressAttributedValuesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a2b7d-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="a2b7d-106">Attributes and elements</span></span>

<span data-ttu-id="a2b7d-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="a2b7d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a2b7d-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="a2b7d-108">Attributes</span></span>

<span data-ttu-id="a2b7d-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="a2b7d-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a2b7d-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="a2b7d-110">Child elements</span></span>

|<span data-ttu-id="a2b7d-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="a2b7d-111">**Element**</span></span>|<span data-ttu-id="a2b7d-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="a2b7d-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a2b7d-113">посталаддрессаттрибутедвалуе</span><span class="sxs-lookup"><span data-stu-id="a2b7d-113">PostalAddressAttributedValue</span></span>](postaladdressattributedvalue.md) <br/> |<span data-ttu-id="a2b7d-114">Указывает экземпляр массива почтовых адресов и связанные с ними атрибуты.</span><span class="sxs-lookup"><span data-stu-id="a2b7d-114">Specifies an instance of an array of postal addresses and their associated attributions.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="a2b7d-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="a2b7d-115">Parent elements</span></span>

|<span data-ttu-id="a2b7d-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="a2b7d-116">**Element**</span></span>|<span data-ttu-id="a2b7d-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="a2b7d-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a2b7d-118">Роль</span><span class="sxs-lookup"><span data-stu-id="a2b7d-118">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="a2b7d-119">Задает набор данных о пользователях, возвращаемых запросом к **другому человеку** .</span><span class="sxs-lookup"><span data-stu-id="a2b7d-119">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="a2b7d-120">Примечания</span><span class="sxs-lookup"><span data-stu-id="a2b7d-120">Remarks</span></span>

<span data-ttu-id="a2b7d-121">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="a2b7d-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="a2b7d-122">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="a2b7d-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a2b7d-123">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="a2b7d-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a2b7d-124">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="a2b7d-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="a2b7d-125">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="a2b7d-125">Schema Name</span></span>  <br/> |<span data-ttu-id="a2b7d-126">Схема типа</span><span class="sxs-lookup"><span data-stu-id="a2b7d-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="a2b7d-127">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="a2b7d-127">Validation File</span></span>  <br/> |<span data-ttu-id="a2b7d-128">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="a2b7d-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="a2b7d-129">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="a2b7d-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="a2b7d-130">См. также</span><span class="sxs-lookup"><span data-stu-id="a2b7d-130">See also</span></span>



- [<span data-ttu-id="a2b7d-131">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="a2b7d-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

