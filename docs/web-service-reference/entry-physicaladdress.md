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
description: Элемент entry описывает один физический адрес элемента контакта.
ms.openlocfilehash: 5e8343e9abebeeff8c2b81327b2e0f4ddcf45364
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459632"
---
# <a name="entry-physicaladdress"></a><span data-ttu-id="f8fcd-103">Запись (PhysicalAddress)</span><span class="sxs-lookup"><span data-stu-id="f8fcd-103">Entry (PhysicalAddress)</span></span>

<span data-ttu-id="f8fcd-104">Элемент **entry** описывает один физический адрес элемента контакта.</span><span class="sxs-lookup"><span data-stu-id="f8fcd-104">The **Entry** element describes a single physical address for a contact item.</span></span> 
  
```xml
<Entry Key="">
   <Street/>
   <City/>
   <State/>
   <Country/>
   <PostalCode/>
</Entry>
```

 <span data-ttu-id="f8fcd-105">**фисикаладдрессдиктионарентритипе**</span><span class="sxs-lookup"><span data-stu-id="f8fcd-105">**PhysicalAddressDictionaryEntryType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f8fcd-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="f8fcd-106">Attributes and elements</span></span>

<span data-ttu-id="f8fcd-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="f8fcd-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f8fcd-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="f8fcd-108">Attributes</span></span>

|<span data-ttu-id="f8fcd-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="f8fcd-109">**Attribute**</span></span>|<span data-ttu-id="f8fcd-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="f8fcd-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="f8fcd-111">**Key**</span><span class="sxs-lookup"><span data-stu-id="f8fcd-111">**Key**</span></span> <br/> | <span data-ttu-id="f8fcd-112">Определяет физический адрес.</span><span class="sxs-lookup"><span data-stu-id="f8fcd-112">Identifies a physical address.</span></span><br/><br/> <span data-ttu-id="f8fcd-113">Ниже приведены возможные значения для этого атрибута.</span><span class="sxs-lookup"><span data-stu-id="f8fcd-113">The following are the possible values for this attribute:</span></span><br/>  <br/><span data-ttu-id="f8fcd-114">-Предприятие</span><span class="sxs-lookup"><span data-stu-id="f8fcd-114">-  Business</span></span>  <br/><span data-ttu-id="f8fcd-115">— Домашний</span><span class="sxs-lookup"><span data-stu-id="f8fcd-115">-  Home</span></span>  <br/><span data-ttu-id="f8fcd-116">— Другие</span><span class="sxs-lookup"><span data-stu-id="f8fcd-116">-  Other</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="f8fcd-117">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="f8fcd-117">Child elements</span></span>

|<span data-ttu-id="f8fcd-118">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="f8fcd-118">**Element**</span></span>|<span data-ttu-id="f8fcd-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="f8fcd-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f8fcd-120">Назван</span><span class="sxs-lookup"><span data-stu-id="f8fcd-120">Street</span></span>](street.md) <br/> |<span data-ttu-id="f8fcd-121">Представляет почтовый адрес элемента контакта.</span><span class="sxs-lookup"><span data-stu-id="f8fcd-121">Represents a street address for a contact item.</span></span>  <br/> |
|[<span data-ttu-id="f8fcd-122">City</span><span class="sxs-lookup"><span data-stu-id="f8fcd-122">City</span></span>](city.md) <br/> |<span data-ttu-id="f8fcd-123">Представляет название города, связанное с контактом.</span><span class="sxs-lookup"><span data-stu-id="f8fcd-123">Represents the city name that is associated with a contact.</span></span>  <br/> |
|[<span data-ttu-id="f8fcd-124">State</span><span class="sxs-lookup"><span data-stu-id="f8fcd-124">State</span></span>](state-ex15websvcsotherref.md) <br/> |<span data-ttu-id="f8fcd-125">Представляет состояние проживания для элемента контакта.</span><span class="sxs-lookup"><span data-stu-id="f8fcd-125">Represents the state of residence for a contact item.</span></span>  <br/> |
|[<span data-ttu-id="f8fcd-126">CountryOrRegion</span><span class="sxs-lookup"><span data-stu-id="f8fcd-126">CountryOrRegion</span></span>](countryorregion.md) <br/> |<span data-ttu-id="f8fcd-127">Представляет страну или регион для данного физического адреса.</span><span class="sxs-lookup"><span data-stu-id="f8fcd-127">Represents the country or region for a given physical address.</span></span>  <br/> |
|[<span data-ttu-id="f8fcd-128">PostalCode</span><span class="sxs-lookup"><span data-stu-id="f8fcd-128">PostalCode</span></span>](postalcode.md) <br/> |<span data-ttu-id="f8fcd-129">Представляет почтовый индекс элемента контакта.</span><span class="sxs-lookup"><span data-stu-id="f8fcd-129">Represents the postal code for a contact item.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f8fcd-130">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="f8fcd-130">Parent elements</span></span>

|<span data-ttu-id="f8fcd-131">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="f8fcd-131">**Element**</span></span>|<span data-ttu-id="f8fcd-132">**Описание**</span><span class="sxs-lookup"><span data-stu-id="f8fcd-132">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f8fcd-133">фисикаладдрессес</span><span class="sxs-lookup"><span data-stu-id="f8fcd-133">PhysicalAddresses</span></span>](physicaladdresses.md) <br/> |<span data-ttu-id="f8fcd-134">Содержит коллекцию физических адресов, связанных с контактом.</span><span class="sxs-lookup"><span data-stu-id="f8fcd-134">Contains a collection of physical addresses that are associated with a contact.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="f8fcd-135">Примечания</span><span class="sxs-lookup"><span data-stu-id="f8fcd-135">Remarks</span></span>

<span data-ttu-id="f8fcd-136">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="f8fcd-136">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f8fcd-137">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="f8fcd-137">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f8fcd-138">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="f8fcd-138">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f8fcd-139">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="f8fcd-139">Schema Name</span></span>  <br/> |<span data-ttu-id="f8fcd-140">Схема Types</span><span class="sxs-lookup"><span data-stu-id="f8fcd-140">Types schema</span></span>  <br/> |
|<span data-ttu-id="f8fcd-141">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="f8fcd-141">Validation File</span></span>  <br/> |<span data-ttu-id="f8fcd-142">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="f8fcd-142">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="f8fcd-143">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="f8fcd-143">Can be Empty</span></span>  <br/> |<span data-ttu-id="f8fcd-144">False</span><span class="sxs-lookup"><span data-stu-id="f8fcd-144">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f8fcd-145">См. также</span><span class="sxs-lookup"><span data-stu-id="f8fcd-145">See also</span></span>

- [<span data-ttu-id="f8fcd-146">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="f8fcd-146">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="f8fcd-147">Создание контактов (веб-службы Exchange)</span><span class="sxs-lookup"><span data-stu-id="f8fcd-147">Creating Contacts (Exchange Web Services)</span></span>](https://msdn.microsoft.com/library/4845917e-70d1-481c-bbd7-011ec6571789%28Office.15%29.aspx)  
- [<span data-ttu-id="f8fcd-148">Обновление контактов</span><span class="sxs-lookup"><span data-stu-id="f8fcd-148">Updating Contacts</span></span>](https://msdn.microsoft.com/library/9a865953-b94a-4229-b632-2dee433314be%28Office.15%29.aspx)  
- [<span data-ttu-id="f8fcd-149">Удаление контактов</span><span class="sxs-lookup"><span data-stu-id="f8fcd-149">Deleting Contacts</span></span>](https://msdn.microsoft.com/library/fcc3dc84-cd3e-455e-a1a7-ae6921c9b588%28Office.15%29.aspx)

