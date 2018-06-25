---
title: PhysicalAddresses
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- PhysicalAddresses
api_type:
- schema
ms.assetid: 5276c5f2-9e08-43af-a0b2-da4ff1dcae2d
description: Элемент PhysicalAddresses содержит коллекцию физических адресов, связанные с контактом.
ms.openlocfilehash: d4d5232312c735e389e9f5b0dbcb74f8614b6906
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834814"
---
# <a name="physicaladdresses"></a><span data-ttu-id="2d6d6-103">PhysicalAddresses</span><span class="sxs-lookup"><span data-stu-id="2d6d6-103">PhysicalAddresses</span></span>

<span data-ttu-id="2d6d6-104">Элемент **PhysicalAddresses** содержит коллекцию физических адресов, связанные с контактом.</span><span class="sxs-lookup"><span data-stu-id="2d6d6-104">The **PhysicalAddresses** element contains a collection of physical addresses that are associated with a contact.</span></span> 
  
```xml
<PhysicalAddresses>
   <Entry/>
</PhysicalAddresses>
```

 <span data-ttu-id="2d6d6-105">**PhysicalAddressDictionaryType**</span><span class="sxs-lookup"><span data-stu-id="2d6d6-105">**PhysicalAddressDictionaryType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2d6d6-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="2d6d6-106">Attributes and elements</span></span>

<span data-ttu-id="2d6d6-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="2d6d6-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2d6d6-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="2d6d6-108">Attributes</span></span>

<span data-ttu-id="2d6d6-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="2d6d6-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2d6d6-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="2d6d6-110">Child elements</span></span>

|<span data-ttu-id="2d6d6-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="2d6d6-111">**Element**</span></span>|<span data-ttu-id="2d6d6-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="2d6d6-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2d6d6-113">Запись (PhysicalAddress)</span><span class="sxs-lookup"><span data-stu-id="2d6d6-113">Entry (PhysicalAddress)</span></span>](entry-physicaladdress.md) <br/> |<span data-ttu-id="2d6d6-114">Описывает один физический адрес для элемента контакта.</span><span class="sxs-lookup"><span data-stu-id="2d6d6-114">Describes a single physical address for a contact item.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="2d6d6-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="2d6d6-115">Parent elements</span></span>

|<span data-ttu-id="2d6d6-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="2d6d6-116">**Element**</span></span>|<span data-ttu-id="2d6d6-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="2d6d6-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2d6d6-118">Контакт</span><span class="sxs-lookup"><span data-stu-id="2d6d6-118">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="2d6d6-119">Представляет элемент контакта Exchange.</span><span class="sxs-lookup"><span data-stu-id="2d6d6-119">Represents an Exchange contact item.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="2d6d6-120">Замечания</span><span class="sxs-lookup"><span data-stu-id="2d6d6-120">Remarks</span></span>

<span data-ttu-id="2d6d6-121">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="2d6d6-121">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2d6d6-122">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="2d6d6-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2d6d6-123">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="2d6d6-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="2d6d6-124">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="2d6d6-124">Schema name</span></span>  <br/> |<span data-ttu-id="2d6d6-125">Схема Types</span><span class="sxs-lookup"><span data-stu-id="2d6d6-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="2d6d6-126">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="2d6d6-126">Validation file</span></span>  <br/> |<span data-ttu-id="2d6d6-127">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="2d6d6-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="2d6d6-128">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="2d6d6-128">Can be empty</span></span>  <br/> |<span data-ttu-id="2d6d6-129">False</span><span class="sxs-lookup"><span data-stu-id="2d6d6-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="2d6d6-130">См. также</span><span class="sxs-lookup"><span data-stu-id="2d6d6-130">See also</span></span>



- [<span data-ttu-id="2d6d6-131">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="2d6d6-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="2d6d6-132">Создание контактов (веб-служб Exchange)</span><span class="sxs-lookup"><span data-stu-id="2d6d6-132">Creating Contacts (Exchange Web Services)</span></span>](http://msdn.microsoft.com/library/4845917e-70d1-481c-bbd7-011ec6571789%28Office.15%29.aspx)
  
[<span data-ttu-id="2d6d6-133">Обновление контактов</span><span class="sxs-lookup"><span data-stu-id="2d6d6-133">Updating Contacts</span></span>](http://msdn.microsoft.com/library/9a865953-b94a-4229-b632-2dee433314be%28Office.15%29.aspx)
  
[<span data-ttu-id="2d6d6-134">Удаление контактов</span><span class="sxs-lookup"><span data-stu-id="2d6d6-134">Deleting Contacts</span></span>](http://msdn.microsoft.com/library/fcc3dc84-cd3e-455e-a1a7-ae6921c9b588%28Office.15%29.aspx)

