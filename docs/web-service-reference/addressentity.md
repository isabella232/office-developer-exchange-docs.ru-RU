---
title: аддрессентити
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: ead22eab-f1e7-48b4-a165-db0e49fe86a8
description: Элемент Аддрессентити указывает один объект Address.
ms.openlocfilehash: 6a46a64c9824efdd8df6a08fe1a159e7e42b3731
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761366"
---
# <a name="addressentity"></a><span data-ttu-id="abdef-103">аддрессентити</span><span class="sxs-lookup"><span data-stu-id="abdef-103">AddressEntity</span></span>

<span data-ttu-id="abdef-104">Элемент **аддрессентити** указывает один объект Address.</span><span class="sxs-lookup"><span data-stu-id="abdef-104">The **AddressEntity** element specifies a single address entity.</span></span> 
  
```XML
<AddressEntity>
    <Address></Address>
    <Position></Position>
</AddressEntity>
```

 <span data-ttu-id="abdef-105">**аддрессентититипе**</span><span class="sxs-lookup"><span data-stu-id="abdef-105">**AddressEntityType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="abdef-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="abdef-106">Attributes and elements</span></span>

<span data-ttu-id="abdef-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="abdef-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="abdef-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="abdef-108">Attributes</span></span>

<span data-ttu-id="abdef-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="abdef-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="abdef-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="abdef-110">Child elements</span></span>

|<span data-ttu-id="abdef-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="abdef-111">**Element**</span></span>|<span data-ttu-id="abdef-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="abdef-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="abdef-113">Address (строка)</span><span class="sxs-lookup"><span data-stu-id="abdef-113">Address (string)</span></span>](address-string.md) <br/> |<span data-ttu-id="abdef-114">Указывает адрес.</span><span class="sxs-lookup"><span data-stu-id="abdef-114">Specifies an address.</span></span>  <br/> |
|[<span data-ttu-id="abdef-115">Position</span><span class="sxs-lookup"><span data-stu-id="abdef-115">Position</span></span>](position.md) <br/> |<span data-ttu-id="abdef-116">Указывает позицию в сообщении электронной почты.</span><span class="sxs-lookup"><span data-stu-id="abdef-116">Specifies the position in an email message.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="abdef-117">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="abdef-117">Parent elements</span></span>

|<span data-ttu-id="abdef-118">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="abdef-118">**Element**</span></span>|<span data-ttu-id="abdef-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="abdef-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="abdef-120">Адреса (Аррайофаддрессентитиестипе)</span><span class="sxs-lookup"><span data-stu-id="abdef-120">Addresses (ArrayOfAddressEntitiesType)</span></span>](addresses-arrayofaddressentitiestype.md) <br/> |<span data-ttu-id="abdef-121">Указывает массив элементов **аддрессентити** .</span><span class="sxs-lookup"><span data-stu-id="abdef-121">Specifies an array of **AddressEntity** elements.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="abdef-122">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="abdef-122">Text value</span></span>

<span data-ttu-id="abdef-123">Нет.</span><span class="sxs-lookup"><span data-stu-id="abdef-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="abdef-124">Примечания</span><span class="sxs-lookup"><span data-stu-id="abdef-124">Remarks</span></span>

<span data-ttu-id="abdef-125">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="abdef-125">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="abdef-126">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="abdef-126">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="abdef-127">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="abdef-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="abdef-128">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="abdef-128">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="abdef-129">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="abdef-129">Schema Name</span></span>  <br/> |<span data-ttu-id="abdef-130">Схема типа</span><span class="sxs-lookup"><span data-stu-id="abdef-130">Type schema</span></span>  <br/> |
|<span data-ttu-id="abdef-131">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="abdef-131">Validation File</span></span>  <br/> |<span data-ttu-id="abdef-132">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="abdef-132">types.xsd</span></span>  <br/> |
|<span data-ttu-id="abdef-133">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="abdef-133">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="abdef-134">См. также</span><span class="sxs-lookup"><span data-stu-id="abdef-134">See also</span></span>

- [<span data-ttu-id="abdef-135">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="abdef-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

