---
title: IndexedFieldURI
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IndexedFieldURI
api_type:
- schema
ms.assetid: 5c9cd0b5-7eca-480a-8730-fe98b1779afa
description: Элемент IndexedFieldURI определяет отдельных элементов словаря.
ms.openlocfilehash: 6a75e8855ecabf15ca31bb1e05d569c258a43b0b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833909"
---
# <a name="indexedfielduri"></a><span data-ttu-id="7e64d-103">IndexedFieldURI</span><span class="sxs-lookup"><span data-stu-id="7e64d-103">IndexedFieldURI</span></span>

<span data-ttu-id="7e64d-104">Элемент **IndexedFieldURI** определяет отдельных элементов словаря.</span><span class="sxs-lookup"><span data-stu-id="7e64d-104">The **IndexedFieldURI** element identifies individual members of a dictionary.</span></span> 
  
```xml
<IndexedFieldURI FieldURI="" FieldIndex="" />
```

 <span data-ttu-id="7e64d-105">**PathToIndexedFieldType**</span><span class="sxs-lookup"><span data-stu-id="7e64d-105">**PathToIndexedFieldType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7e64d-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="7e64d-106">Attributes and elements</span></span>

<span data-ttu-id="7e64d-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="7e64d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7e64d-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="7e64d-108">Attributes</span></span>

|<span data-ttu-id="7e64d-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="7e64d-109">**Attribute**</span></span>|<span data-ttu-id="7e64d-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="7e64d-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="7e64d-111">**FieldURI**</span><span class="sxs-lookup"><span data-stu-id="7e64d-111">**FieldURI**</span></span> <br/> |<span data-ttu-id="7e64d-112">Задает словарь, содержащий возвращаемый элемент.</span><span class="sxs-lookup"><span data-stu-id="7e64d-112">Identifies the dictionary that contains the member to return.</span></span> <span data-ttu-id="7e64d-113">Этот атрибут является обязательным.</span><span class="sxs-lookup"><span data-stu-id="7e64d-113">This attribute is required.</span></span>  <br/> |
|<span data-ttu-id="7e64d-114">**FieldIndex**</span><span class="sxs-lookup"><span data-stu-id="7e64d-114">**FieldIndex**</span></span> <br/> |<span data-ttu-id="7e64d-115">Определяет возвращаемый элемент словаря.</span><span class="sxs-lookup"><span data-stu-id="7e64d-115">Identifies the member of the dictionary to return.</span></span> <span data-ttu-id="7e64d-116">Этот атрибут является обязательным.</span><span class="sxs-lookup"><span data-stu-id="7e64d-116">This attribute is required.</span></span>  <br/> |
   
#### <a name="fielduri-attribute"></a><span data-ttu-id="7e64d-117">Атрибут FieldURI</span><span class="sxs-lookup"><span data-stu-id="7e64d-117">FieldURI Attribute</span></span>

|<span data-ttu-id="7e64d-118">**Значение**</span><span class="sxs-lookup"><span data-stu-id="7e64d-118">**Value**</span></span>|<span data-ttu-id="7e64d-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="7e64d-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="7e64d-120">элемент: InternetMessageHeader</span><span class="sxs-lookup"><span data-stu-id="7e64d-120">item:InternetMessageHeader</span></span>  <br/> |<span data-ttu-id="7e64d-121">Представляет заголовок сообщения элемента.</span><span class="sxs-lookup"><span data-stu-id="7e64d-121">Represents the message header of an item.</span></span>  <br/> |
|<span data-ttu-id="7e64d-122">Контакты: ImAddress</span><span class="sxs-lookup"><span data-stu-id="7e64d-122">contacts:ImAddress</span></span>  <br/> |<span data-ttu-id="7e64d-123">Представляет обмена мгновенными сообщениями адрес контакта.</span><span class="sxs-lookup"><span data-stu-id="7e64d-123">Represents the instant messaging address of a contact.</span></span>  <br/> |
|<span data-ttu-id="7e64d-124">Контакты: PhysicalAddress:Street</span><span class="sxs-lookup"><span data-stu-id="7e64d-124">contacts:PhysicalAddress:Street</span></span>  <br/> |<span data-ttu-id="7e64d-125">Представляет почтовый адрес контакта.</span><span class="sxs-lookup"><span data-stu-id="7e64d-125">Represents the street address of a contact.</span></span>  <br/> |
|<span data-ttu-id="7e64d-126">Контакты: PhysicalAddress:City</span><span class="sxs-lookup"><span data-stu-id="7e64d-126">contacts:PhysicalAddress:City</span></span>  <br/> |<span data-ttu-id="7e64d-127">Представляет город контакта.</span><span class="sxs-lookup"><span data-stu-id="7e64d-127">Represents the city of a contact.</span></span>  <br/> |
|<span data-ttu-id="7e64d-128">Контакты: PhysicalAddress:State</span><span class="sxs-lookup"><span data-stu-id="7e64d-128">contacts:PhysicalAddress:State</span></span>  <br/> |<span data-ttu-id="7e64d-129">Представляет состояние контакта.</span><span class="sxs-lookup"><span data-stu-id="7e64d-129">Represents the state of a contact.</span></span>  <br/> |
|<span data-ttu-id="7e64d-130">Контакты: PhysicalAddress:Country</span><span class="sxs-lookup"><span data-stu-id="7e64d-130">contacts:PhysicalAddress:Country</span></span>  <br/> |<span data-ttu-id="7e64d-131">Представляет страны или региона контакта.</span><span class="sxs-lookup"><span data-stu-id="7e64d-131">Represents the country/region of a contact.</span></span>  <br/> |
|<span data-ttu-id="7e64d-132">Контакты: PhysicalAddress:PostalCode</span><span class="sxs-lookup"><span data-stu-id="7e64d-132">contacts:PhysicalAddress:PostalCode</span></span>  <br/> |<span data-ttu-id="7e64d-133">Представляет почтовый индекс контакта.</span><span class="sxs-lookup"><span data-stu-id="7e64d-133">Represents the postal code of a contact.</span></span>  <br/> |
|<span data-ttu-id="7e64d-134">Контакты: PhoneNumber</span><span class="sxs-lookup"><span data-stu-id="7e64d-134">contacts:PhoneNumber</span></span>  <br/> |<span data-ttu-id="7e64d-135">Представляет номер телефона контакта.</span><span class="sxs-lookup"><span data-stu-id="7e64d-135">Represents the phone number of a contact.</span></span>  <br/> |
|<span data-ttu-id="7e64d-136">Контакты: EmailAddress</span><span class="sxs-lookup"><span data-stu-id="7e64d-136">contacts:EmailAddress</span></span>  <br/> |<span data-ttu-id="7e64d-137">Представляет адрес электронной почты контакта.</span><span class="sxs-lookup"><span data-stu-id="7e64d-137">Represents the e-mail address of a contact.</span></span>  <br/> |
|<span data-ttu-id="7e64d-138">distributionlist:Members:member</span><span class="sxs-lookup"><span data-stu-id="7e64d-138">distributionlist:Members:Member</span></span>  <br/> |<span data-ttu-id="7e64d-139">Представляет элемент в список рассылки.</span><span class="sxs-lookup"><span data-stu-id="7e64d-139">Represents a member of a distribution list.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="7e64d-140">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="7e64d-140">Child elements</span></span>

<span data-ttu-id="7e64d-141">Нет.</span><span class="sxs-lookup"><span data-stu-id="7e64d-141">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="7e64d-142">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="7e64d-142">Parent elements</span></span>

|<span data-ttu-id="7e64d-143">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="7e64d-143">**Element**</span></span>|<span data-ttu-id="7e64d-144">**Описание**</span><span class="sxs-lookup"><span data-stu-id="7e64d-144">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7e64d-145">AdditionalProperties</span><span class="sxs-lookup"><span data-stu-id="7e64d-145">AdditionalProperties</span></span>](additionalproperties.md) <br/> |<span data-ttu-id="7e64d-146">Определяет дополнительные свойства для получения, установки или создать.</span><span class="sxs-lookup"><span data-stu-id="7e64d-146">Identifies additional properties to get, set, or create.</span></span>  <br/> |
|[<span data-ttu-id="7e64d-147">AggregateOn</span><span class="sxs-lookup"><span data-stu-id="7e64d-147">AggregateOn</span></span>](aggregateon.md) <br/> |<span data-ttu-id="7e64d-148">Представляет свойство, которое используется для определения порядка сгруппированные элементы для группированных FindItem набора результатов.</span><span class="sxs-lookup"><span data-stu-id="7e64d-148">Represents the property that is used to determine the order of grouped items for a grouped FindItem result set.</span></span>  <br/> |
|[<span data-ttu-id="7e64d-149">GroupBy</span><span class="sxs-lookup"><span data-stu-id="7e64d-149">GroupBy</span></span>](groupby.md) <br/> |<span data-ttu-id="7e64d-150">Задает произвольную группировки для запросов FindItem.</span><span class="sxs-lookup"><span data-stu-id="7e64d-150">Specifies an arbitrary grouping for FindItem queries.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="7e64d-151">Замечания</span><span class="sxs-lookup"><span data-stu-id="7e64d-151">Remarks</span></span>

<span data-ttu-id="7e64d-152">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="7e64d-152">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7e64d-153">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="7e64d-153">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7e64d-154">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="7e64d-154">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="7e64d-155">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="7e64d-155">Schema Name</span></span>  <br/> |<span data-ttu-id="7e64d-156">Схема Types</span><span class="sxs-lookup"><span data-stu-id="7e64d-156">Types schema</span></span>  <br/> |
|<span data-ttu-id="7e64d-157">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="7e64d-157">Validation File</span></span>  <br/> |<span data-ttu-id="7e64d-158">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="7e64d-158">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="7e64d-159">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="7e64d-159">Can be Empty</span></span>  <br/> |<span data-ttu-id="7e64d-160">False</span><span class="sxs-lookup"><span data-stu-id="7e64d-160">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7e64d-161">См. также</span><span class="sxs-lookup"><span data-stu-id="7e64d-161">See also</span></span>



- [<span data-ttu-id="7e64d-162">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="7e64d-162">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

