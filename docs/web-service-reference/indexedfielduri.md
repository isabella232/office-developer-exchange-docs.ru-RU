---
title: индекседфиелдури
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
description: Элемент Индекседфиелдури определяет отдельные элементы словаря.
ms.openlocfilehash: 6a75e8855ecabf15ca31bb1e05d569c258a43b0b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833909"
---
# <a name="indexedfielduri"></a><span data-ttu-id="d5553-103">индекседфиелдури</span><span class="sxs-lookup"><span data-stu-id="d5553-103">IndexedFieldURI</span></span>

<span data-ttu-id="d5553-104">Элемент **индекседфиелдури** определяет отдельные элементы словаря.</span><span class="sxs-lookup"><span data-stu-id="d5553-104">The **IndexedFieldURI** element identifies individual members of a dictionary.</span></span> 
  
```xml
<IndexedFieldURI FieldURI="" FieldIndex="" />
```

 <span data-ttu-id="d5553-105">**пастоиндекседфиелдтипе**</span><span class="sxs-lookup"><span data-stu-id="d5553-105">**PathToIndexedFieldType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d5553-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="d5553-106">Attributes and elements</span></span>

<span data-ttu-id="d5553-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="d5553-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d5553-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="d5553-108">Attributes</span></span>

|<span data-ttu-id="d5553-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="d5553-109">**Attribute**</span></span>|<span data-ttu-id="d5553-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d5553-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="d5553-111">**фиелдури**</span><span class="sxs-lookup"><span data-stu-id="d5553-111">**FieldURI**</span></span> <br/> |<span data-ttu-id="d5553-112">Определяет словарь, содержащий возвращаемый член.</span><span class="sxs-lookup"><span data-stu-id="d5553-112">Identifies the dictionary that contains the member to return.</span></span> <span data-ttu-id="d5553-113">Этот атрибут является обязательным.</span><span class="sxs-lookup"><span data-stu-id="d5553-113">This attribute is required.</span></span>  <br/> |
|<span data-ttu-id="d5553-114">**фиелдиндекс**</span><span class="sxs-lookup"><span data-stu-id="d5553-114">**FieldIndex**</span></span> <br/> |<span data-ttu-id="d5553-115">Определяет возвращаемый элемент словаря.</span><span class="sxs-lookup"><span data-stu-id="d5553-115">Identifies the member of the dictionary to return.</span></span> <span data-ttu-id="d5553-116">Этот атрибут является обязательным.</span><span class="sxs-lookup"><span data-stu-id="d5553-116">This attribute is required.</span></span>  <br/> |
   
#### <a name="fielduri-attribute"></a><span data-ttu-id="d5553-117">Атрибут Фиелдури</span><span class="sxs-lookup"><span data-stu-id="d5553-117">FieldURI Attribute</span></span>

|<span data-ttu-id="d5553-118">**Значение**</span><span class="sxs-lookup"><span data-stu-id="d5553-118">**Value**</span></span>|<span data-ttu-id="d5553-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d5553-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="d5553-120">элемент: InternetMessageHeader</span><span class="sxs-lookup"><span data-stu-id="d5553-120">item:InternetMessageHeader</span></span>  <br/> |<span data-ttu-id="d5553-121">Представляет заголовок сообщения для элемента.</span><span class="sxs-lookup"><span data-stu-id="d5553-121">Represents the message header of an item.</span></span>  <br/> |
|<span data-ttu-id="d5553-122">Контакты: адрес</span><span class="sxs-lookup"><span data-stu-id="d5553-122">contacts:ImAddress</span></span>  <br/> |<span data-ttu-id="d5553-123">Представляет адрес обмена мгновенными сообщениями контакта.</span><span class="sxs-lookup"><span data-stu-id="d5553-123">Represents the instant messaging address of a contact.</span></span>  <br/> |
|<span data-ttu-id="d5553-124">Контакты: PhysicalAddress: улица</span><span class="sxs-lookup"><span data-stu-id="d5553-124">contacts:PhysicalAddress:Street</span></span>  <br/> |<span data-ttu-id="d5553-125">Представляет почтовый адрес контакта.</span><span class="sxs-lookup"><span data-stu-id="d5553-125">Represents the street address of a contact.</span></span>  <br/> |
|<span data-ttu-id="d5553-126">Контакты: PhysicalAddress: City</span><span class="sxs-lookup"><span data-stu-id="d5553-126">contacts:PhysicalAddress:City</span></span>  <br/> |<span data-ttu-id="d5553-127">Представляет город контакта.</span><span class="sxs-lookup"><span data-stu-id="d5553-127">Represents the city of a contact.</span></span>  <br/> |
|<span data-ttu-id="d5553-128">Контакты: PhysicalAddress: State</span><span class="sxs-lookup"><span data-stu-id="d5553-128">contacts:PhysicalAddress:State</span></span>  <br/> |<span data-ttu-id="d5553-129">Представляет состояние контакта.</span><span class="sxs-lookup"><span data-stu-id="d5553-129">Represents the state of a contact.</span></span>  <br/> |
|<span data-ttu-id="d5553-130">Контакты: PhysicalAddress: Country</span><span class="sxs-lookup"><span data-stu-id="d5553-130">contacts:PhysicalAddress:Country</span></span>  <br/> |<span data-ttu-id="d5553-131">Представляет страну или регион контакта.</span><span class="sxs-lookup"><span data-stu-id="d5553-131">Represents the country/region of a contact.</span></span>  <br/> |
|<span data-ttu-id="d5553-132">Contacts: PhysicalAddress: PostalCode</span><span class="sxs-lookup"><span data-stu-id="d5553-132">contacts:PhysicalAddress:PostalCode</span></span>  <br/> |<span data-ttu-id="d5553-133">Представляет почтовый индекс контакта.</span><span class="sxs-lookup"><span data-stu-id="d5553-133">Represents the postal code of a contact.</span></span>  <br/> |
|<span data-ttu-id="d5553-134">Контакты: PhoneNumber</span><span class="sxs-lookup"><span data-stu-id="d5553-134">contacts:PhoneNumber</span></span>  <br/> |<span data-ttu-id="d5553-135">Представляет номер телефона контакта.</span><span class="sxs-lookup"><span data-stu-id="d5553-135">Represents the phone number of a contact.</span></span>  <br/> |
|<span data-ttu-id="d5553-136">Contacts: EmailAddress</span><span class="sxs-lookup"><span data-stu-id="d5553-136">contacts:EmailAddress</span></span>  <br/> |<span data-ttu-id="d5553-137">Представляет адрес электронной почты контакта.</span><span class="sxs-lookup"><span data-stu-id="d5553-137">Represents the e-mail address of a contact.</span></span>  <br/> |
|<span data-ttu-id="d5553-138">дистрибутионлист: Members: Member</span><span class="sxs-lookup"><span data-stu-id="d5553-138">distributionlist:Members:Member</span></span>  <br/> |<span data-ttu-id="d5553-139">Представляет члена списка рассылки.</span><span class="sxs-lookup"><span data-stu-id="d5553-139">Represents a member of a distribution list.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="d5553-140">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="d5553-140">Child elements</span></span>

<span data-ttu-id="d5553-141">Нет.</span><span class="sxs-lookup"><span data-stu-id="d5553-141">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="d5553-142">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="d5553-142">Parent elements</span></span>

|<span data-ttu-id="d5553-143">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="d5553-143">**Element**</span></span>|<span data-ttu-id="d5553-144">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d5553-144">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d5553-145">аддитионалпропертиес</span><span class="sxs-lookup"><span data-stu-id="d5553-145">AdditionalProperties</span></span>](additionalproperties.md) <br/> |<span data-ttu-id="d5553-146">Определяет дополнительные свойства, которые необходимо получить, задать или создать.</span><span class="sxs-lookup"><span data-stu-id="d5553-146">Identifies additional properties to get, set, or create.</span></span>  <br/> |
|[<span data-ttu-id="d5553-147">аггрегатеон</span><span class="sxs-lookup"><span data-stu-id="d5553-147">AggregateOn</span></span>](aggregateon.md) <br/> |<span data-ttu-id="d5553-148">Представляет свойство, используемое для определения порядка сгруппированных элементов для группового результирующего набора FindItem.</span><span class="sxs-lookup"><span data-stu-id="d5553-148">Represents the property that is used to determine the order of grouped items for a grouped FindItem result set.</span></span>  <br/> |
|[<span data-ttu-id="d5553-149">GroupBy</span><span class="sxs-lookup"><span data-stu-id="d5553-149">GroupBy</span></span>](groupby.md) <br/> |<span data-ttu-id="d5553-150">Указывает произвольное группирование для запросов FindItem.</span><span class="sxs-lookup"><span data-stu-id="d5553-150">Specifies an arbitrary grouping for FindItem queries.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="d5553-151">Примечания</span><span class="sxs-lookup"><span data-stu-id="d5553-151">Remarks</span></span>

<span data-ttu-id="d5553-152">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="d5553-152">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d5553-153">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="d5553-153">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d5553-154">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="d5553-154">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d5553-155">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="d5553-155">Schema Name</span></span>  <br/> |<span data-ttu-id="d5553-156">Схема Types</span><span class="sxs-lookup"><span data-stu-id="d5553-156">Types schema</span></span>  <br/> |
|<span data-ttu-id="d5553-157">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="d5553-157">Validation File</span></span>  <br/> |<span data-ttu-id="d5553-158">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="d5553-158">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d5553-159">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="d5553-159">Can be Empty</span></span>  <br/> |<span data-ttu-id="d5553-160">False</span><span class="sxs-lookup"><span data-stu-id="d5553-160">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d5553-161">См. также</span><span class="sxs-lookup"><span data-stu-id="d5553-161">See also</span></span>



- [<span data-ttu-id="d5553-162">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="d5553-162">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

