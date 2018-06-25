---
title: Запись (PhysicalAddress)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Entry
api_type:
- schema
ms.assetid: 9e5b6515-453e-4f4c-b55e-6ffefe23c31b
description: Элемент описывает один физический адрес для элемента контакта.
ms.openlocfilehash: 4551e6117e5f91d901fe160f37e8f67cb1bc5ac7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762369"
---
# <a name="entry-physicaladdress"></a><span data-ttu-id="53a45-103">Запись (PhysicalAddress)</span><span class="sxs-lookup"><span data-stu-id="53a45-103">Entry (PhysicalAddress)</span></span>

<span data-ttu-id="53a45-104">**Элемент** описывает один физический адрес для элемента контакта.</span><span class="sxs-lookup"><span data-stu-id="53a45-104">The **Entry** element describes a single physical address for a contact item.</span></span> 
  
```xml
<Entry Key="">
   <Street/>
   <City/>
   <State/>
   <Country/>
   <PostalCode/>
</Entry>
```

 <span data-ttu-id="53a45-105">**PhysicalAddressDictionaryEntryType**</span><span class="sxs-lookup"><span data-stu-id="53a45-105">**PhysicalAddressDictionaryEntryType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="53a45-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="53a45-106">Attributes and elements</span></span>

<span data-ttu-id="53a45-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="53a45-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="53a45-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="53a45-108">Attributes</span></span>

|<span data-ttu-id="53a45-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="53a45-109">**Attribute**</span></span>|<span data-ttu-id="53a45-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="53a45-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="53a45-111">**Key**</span><span class="sxs-lookup"><span data-stu-id="53a45-111">**Key**</span></span> <br/> | <span data-ttu-id="53a45-112">Определяет физический адрес.</span><span class="sxs-lookup"><span data-stu-id="53a45-112">Identifies a physical address.</span></span><br/><br/> <span data-ttu-id="53a45-113">Ниже приведены возможные значения этого атрибута.</span><span class="sxs-lookup"><span data-stu-id="53a45-113">The following are the possible values for this attribute:</span></span><br/>  <br/><span data-ttu-id="53a45-114">-Бизнес</span><span class="sxs-lookup"><span data-stu-id="53a45-114">-  Business</span></span>  <br/><span data-ttu-id="53a45-115">-Домашняя страница</span><span class="sxs-lookup"><span data-stu-id="53a45-115">-  Home</span></span>  <br/><span data-ttu-id="53a45-116">-Другие</span><span class="sxs-lookup"><span data-stu-id="53a45-116">-  Other</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="53a45-117">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="53a45-117">Child elements</span></span>

|<span data-ttu-id="53a45-118">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="53a45-118">**Element**</span></span>|<span data-ttu-id="53a45-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="53a45-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="53a45-120">Улица</span><span class="sxs-lookup"><span data-stu-id="53a45-120">Street</span></span>](street.md) <br/> |<span data-ttu-id="53a45-121">Представляет почтовый адрес для элемента контакта.</span><span class="sxs-lookup"><span data-stu-id="53a45-121">Represents a street address for a contact item.</span></span>  <br/> |
|[<span data-ttu-id="53a45-122">Город</span><span class="sxs-lookup"><span data-stu-id="53a45-122">City</span></span>](city.md) <br/> |<span data-ttu-id="53a45-123">Представляет название города, связанного с контактом.</span><span class="sxs-lookup"><span data-stu-id="53a45-123">Represents the city name that is associated with a contact.</span></span>  <br/> |
|[<span data-ttu-id="53a45-124">Состояние</span><span class="sxs-lookup"><span data-stu-id="53a45-124">State</span></span>](state-ex15websvcsotherref.md) <br/> |<span data-ttu-id="53a45-125">Представляет состояние расположения для элемента контакта.</span><span class="sxs-lookup"><span data-stu-id="53a45-125">Represents the state of residence for a contact item.</span></span>  <br/> |
|[<span data-ttu-id="53a45-126">CountryOrRegion</span><span class="sxs-lookup"><span data-stu-id="53a45-126">CountryOrRegion</span></span>](countryorregion.md) <br/> |<span data-ttu-id="53a45-127">Представляет страну или регион для заданного физического адреса.</span><span class="sxs-lookup"><span data-stu-id="53a45-127">Represents the country or region for a given physical address.</span></span>  <br/> |
|[<span data-ttu-id="53a45-128">Индекс</span><span class="sxs-lookup"><span data-stu-id="53a45-128">PostalCode</span></span>](postalcode.md) <br/> |<span data-ttu-id="53a45-129">Представляет почтовый индекс для элемента контакта.</span><span class="sxs-lookup"><span data-stu-id="53a45-129">Represents the postal code for a contact item.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="53a45-130">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="53a45-130">Parent elements</span></span>

|<span data-ttu-id="53a45-131">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="53a45-131">**Element**</span></span>|<span data-ttu-id="53a45-132">**Описание**</span><span class="sxs-lookup"><span data-stu-id="53a45-132">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="53a45-133">PhysicalAddresses</span><span class="sxs-lookup"><span data-stu-id="53a45-133">PhysicalAddresses</span></span>](physicaladdresses.md) <br/> |<span data-ttu-id="53a45-134">Содержит коллекцию физических адресов, связанные с контактом.</span><span class="sxs-lookup"><span data-stu-id="53a45-134">Contains a collection of physical addresses that are associated with a contact.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="53a45-135">Замечания</span><span class="sxs-lookup"><span data-stu-id="53a45-135">Remarks</span></span>

<span data-ttu-id="53a45-136">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="53a45-136">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="53a45-137">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="53a45-137">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="53a45-138">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="53a45-138">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="53a45-139">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="53a45-139">Schema Name</span></span>  <br/> |<span data-ttu-id="53a45-140">Схема Types</span><span class="sxs-lookup"><span data-stu-id="53a45-140">Types schema</span></span>  <br/> |
|<span data-ttu-id="53a45-141">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="53a45-141">Validation File</span></span>  <br/> |<span data-ttu-id="53a45-142">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="53a45-142">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="53a45-143">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="53a45-143">Can be Empty</span></span>  <br/> |<span data-ttu-id="53a45-144">False</span><span class="sxs-lookup"><span data-stu-id="53a45-144">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="53a45-145">См. также</span><span class="sxs-lookup"><span data-stu-id="53a45-145">See also</span></span>

- [<span data-ttu-id="53a45-146">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="53a45-146">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="53a45-147">Создание контактов (веб-служб Exchange)</span><span class="sxs-lookup"><span data-stu-id="53a45-147">Creating Contacts (Exchange Web Services)</span></span>](http://msdn.microsoft.com/library/4845917e-70d1-481c-bbd7-011ec6571789%28Office.15%29.aspx)  
- [<span data-ttu-id="53a45-148">Обновление контактов</span><span class="sxs-lookup"><span data-stu-id="53a45-148">Updating Contacts</span></span>](http://msdn.microsoft.com/library/9a865953-b94a-4229-b632-2dee433314be%28Office.15%29.aspx)  
- [<span data-ttu-id="53a45-149">Удаление контактов</span><span class="sxs-lookup"><span data-stu-id="53a45-149">Deleting Contacts</span></span>](http://msdn.microsoft.com/library/fcc3dc84-cd3e-455e-a1a7-ae6921c9b588%28Office.15%29.aspx)

