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
ms.openlocfilehash: a9d4ceafcac9cf0809668871b4df932b31525ac8
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833817"
---
# <a name="homeaddresses"></a><span data-ttu-id="8260c-103">хомеаддрессес</span><span class="sxs-lookup"><span data-stu-id="8260c-103">HomeAddresses</span></span>

<span data-ttu-id="8260c-104">Элемент **хомеаддрессес** указывает массив домашних адресов и идентификаторы их исходных атрибутов для связанного пользователя.</span><span class="sxs-lookup"><span data-stu-id="8260c-104">The **HomeAddresses** element specifies an array of home addresses and the identifiers of their source attributions for the associated persona.</span></span> 
  
```XML
<HomeAddresses>
    <PostalAddressAttributedValue/>
</HomeAddresses>
```

 <span data-ttu-id="8260c-105">**аррайофпосталаддрессаттрибутедвалуестипе**</span><span class="sxs-lookup"><span data-stu-id="8260c-105">**ArrayOfPostalAddressAttributedValuesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8260c-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="8260c-106">Attributes and elements</span></span>

<span data-ttu-id="8260c-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="8260c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8260c-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="8260c-108">Attributes</span></span>

<span data-ttu-id="8260c-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="8260c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8260c-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="8260c-110">Child elements</span></span>

|<span data-ttu-id="8260c-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="8260c-111">**Element**</span></span>|<span data-ttu-id="8260c-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="8260c-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8260c-113">посталаддрессаттрибутедвалуе</span><span class="sxs-lookup"><span data-stu-id="8260c-113">PostalAddressAttributedValue</span></span>](postaladdressattributedvalue.md) <br/> |<span data-ttu-id="8260c-114">Указывает экземпляр массива почтовых адресов и связанные с ними атрибуты.</span><span class="sxs-lookup"><span data-stu-id="8260c-114">Specifies an instance of an array of postal addresses and their associated attributions.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="8260c-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="8260c-115">Parent elements</span></span>

|<span data-ttu-id="8260c-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="8260c-116">**Element**</span></span>|<span data-ttu-id="8260c-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="8260c-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8260c-118">Роль</span><span class="sxs-lookup"><span data-stu-id="8260c-118">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="8260c-119">Задает набор данных о пользователях, возвращаемых запросом к **другому человеку** .</span><span class="sxs-lookup"><span data-stu-id="8260c-119">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="8260c-120">Примечания</span><span class="sxs-lookup"><span data-stu-id="8260c-120">Remarks</span></span>

<span data-ttu-id="8260c-121">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="8260c-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="8260c-122">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="8260c-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8260c-123">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="8260c-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8260c-124">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="8260c-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="8260c-125">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="8260c-125">Schema Name</span></span>  <br/> |<span data-ttu-id="8260c-126">Схема типа</span><span class="sxs-lookup"><span data-stu-id="8260c-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="8260c-127">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="8260c-127">Validation File</span></span>  <br/> |<span data-ttu-id="8260c-128">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="8260c-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="8260c-129">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="8260c-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="8260c-130">См. также</span><span class="sxs-lookup"><span data-stu-id="8260c-130">See also</span></span>



- [<span data-ttu-id="8260c-131">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="8260c-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

