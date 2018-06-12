---
title: AddressEntity
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: ead22eab-f1e7-48b4-a165-db0e49fe86a8
description: Элемент AddressEntity указывает один адрес сущности.
ms.openlocfilehash: 6a46a64c9824efdd8df6a08fe1a159e7e42b3731
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761366"
---
# <a name="addressentity"></a><span data-ttu-id="43080-103">AddressEntity</span><span class="sxs-lookup"><span data-stu-id="43080-103">AddressEntity</span></span>

<span data-ttu-id="43080-104">Элемент **AddressEntity** указывает один адрес сущности.</span><span class="sxs-lookup"><span data-stu-id="43080-104">The **AddressEntity** element specifies a single address entity.</span></span> 
  
```XML
<AddressEntity>
    <Address></Address>
    <Position></Position>
</AddressEntity>
```

 <span data-ttu-id="43080-105">**AddressEntityType**</span><span class="sxs-lookup"><span data-stu-id="43080-105">**AddressEntityType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="43080-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="43080-106">Attributes and elements</span></span>

<span data-ttu-id="43080-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="43080-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="43080-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="43080-108">Attributes</span></span>

<span data-ttu-id="43080-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="43080-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="43080-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="43080-110">Child elements</span></span>

|<span data-ttu-id="43080-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="43080-111">**Element**</span></span>|<span data-ttu-id="43080-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="43080-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="43080-113">Адрес (строка)</span><span class="sxs-lookup"><span data-stu-id="43080-113">Address (string)</span></span>](address-string.md) <br/> |<span data-ttu-id="43080-114">Указывает адрес.</span><span class="sxs-lookup"><span data-stu-id="43080-114">Specifies an address.</span></span>  <br/> |
|[<span data-ttu-id="43080-115">Position</span><span class="sxs-lookup"><span data-stu-id="43080-115">Position</span></span>](position.md) <br/> |<span data-ttu-id="43080-116">Задает позицию в сообщении электронной почты.</span><span class="sxs-lookup"><span data-stu-id="43080-116">Specifies the position in an email message.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="43080-117">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="43080-117">Parent elements</span></span>

|<span data-ttu-id="43080-118">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="43080-118">**Element**</span></span>|<span data-ttu-id="43080-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="43080-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="43080-120">Адреса (ArrayOfAddressEntitiesType)</span><span class="sxs-lookup"><span data-stu-id="43080-120">Addresses (ArrayOfAddressEntitiesType)</span></span>](addresses-arrayofaddressentitiestype.md) <br/> |<span data-ttu-id="43080-121">Указывает массив элементов **AddressEntity** .</span><span class="sxs-lookup"><span data-stu-id="43080-121">Specifies an array of **AddressEntity** elements.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="43080-122">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="43080-122">Text value</span></span>

<span data-ttu-id="43080-123">Нет.</span><span class="sxs-lookup"><span data-stu-id="43080-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="43080-124">Замечания</span><span class="sxs-lookup"><span data-stu-id="43080-124">Remarks</span></span>

<span data-ttu-id="43080-125">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="43080-125">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="43080-126">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="43080-126">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="43080-127">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="43080-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="43080-128">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="43080-128">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="43080-129">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="43080-129">Schema Name</span></span>  <br/> |<span data-ttu-id="43080-130">Схема типа</span><span class="sxs-lookup"><span data-stu-id="43080-130">Type schema</span></span>  <br/> |
|<span data-ttu-id="43080-131">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="43080-131">Validation File</span></span>  <br/> |<span data-ttu-id="43080-132">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="43080-132">types.xsd</span></span>  <br/> |
|<span data-ttu-id="43080-133">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="43080-133">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="43080-134">См. также</span><span class="sxs-lookup"><span data-stu-id="43080-134">See also</span></span>

- [<span data-ttu-id="43080-135">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="43080-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

