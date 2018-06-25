---
title: ItemChanges
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ItemChanges
api_type:
- schema
ms.assetid: cd307892-2f69-4494-8325-219bdb5c3ad5
description: Элемент ItemChanges содержит массив элементов ItemChange, чтобы указать элементы и обновления, чтобы применить к элементам.
ms.openlocfilehash: 38fe112441a8773a2d6b494ed57c63341cab2b58
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834141"
---
# <a name="itemchanges"></a><span data-ttu-id="e47a0-103">ItemChanges</span><span class="sxs-lookup"><span data-stu-id="e47a0-103">ItemChanges</span></span>

<span data-ttu-id="e47a0-104">Элемент **ItemChanges** содержит массив элементов [ItemChange](itemchange.md) , чтобы указать элементы и обновления, чтобы применить к элементам.</span><span class="sxs-lookup"><span data-stu-id="e47a0-104">The **ItemChanges** element contains an array of [ItemChange](itemchange.md) elements that identify items and the updates to apply to the items.</span></span> 
  
[<span data-ttu-id="e47a0-105">UpdateItem</span><span class="sxs-lookup"><span data-stu-id="e47a0-105">UpdateItem</span></span>](updateitem.md)
  
[<span data-ttu-id="e47a0-106">ItemChanges</span><span class="sxs-lookup"><span data-stu-id="e47a0-106">ItemChanges</span></span>](itemchanges.md)
  
```xml
<ItemChanges>
   <ItemChange/>
</ItemChanges>
```

 <span data-ttu-id="e47a0-107">**NonEmptyArrayOfItemChangesType**</span><span class="sxs-lookup"><span data-stu-id="e47a0-107">**NonEmptyArrayOfItemChangesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e47a0-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="e47a0-108">Attributes and elements</span></span>

<span data-ttu-id="e47a0-109">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="e47a0-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e47a0-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="e47a0-110">Attributes</span></span>

<span data-ttu-id="e47a0-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="e47a0-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e47a0-112">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="e47a0-112">Child elements</span></span>

|<span data-ttu-id="e47a0-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="e47a0-113">**Element**</span></span>|<span data-ttu-id="e47a0-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="e47a0-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e47a0-115">ItemChange</span><span class="sxs-lookup"><span data-stu-id="e47a0-115">ItemChange</span></span>](itemchange.md) <br/> |<span data-ttu-id="e47a0-116">Содержит идентификатор элемента и обновления для применения к элементу.</span><span class="sxs-lookup"><span data-stu-id="e47a0-116">Contains an item identifier and the updates to apply to the item.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="e47a0-117">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="e47a0-117">Parent elements</span></span>

|<span data-ttu-id="e47a0-118">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="e47a0-118">**Element**</span></span>|<span data-ttu-id="e47a0-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="e47a0-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e47a0-120">UpdateItem</span><span class="sxs-lookup"><span data-stu-id="e47a0-120">UpdateItem</span></span>](updateitem.md) <br/> |<span data-ttu-id="e47a0-121">Определяет запрос для обновления элементов в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="e47a0-121">Defines a request to update items in a mailbox.</span></span>  <br/> <span data-ttu-id="e47a0-122">Ниже приведен выражение XPath для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="e47a0-122">The following is the XPath expression to this element:</span></span>  <br/>  `/UpdateItem` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="e47a0-123">Замечания</span><span class="sxs-lookup"><span data-stu-id="e47a0-123">Remarks</span></span>

<span data-ttu-id="e47a0-124">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="e47a0-124">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e47a0-125">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="e47a0-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e47a0-126">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="e47a0-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="e47a0-127">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="e47a0-127">Schema Name</span></span>  <br/> |<span data-ttu-id="e47a0-128">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="e47a0-128">Messages schema</span></span>  <br/> |
|<span data-ttu-id="e47a0-129">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="e47a0-129">Validation File</span></span>  <br/> |<span data-ttu-id="e47a0-130">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="e47a0-130">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="e47a0-131">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="e47a0-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="e47a0-132">False</span><span class="sxs-lookup"><span data-stu-id="e47a0-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e47a0-133">См. также</span><span class="sxs-lookup"><span data-stu-id="e47a0-133">See also</span></span>



[<span data-ttu-id="e47a0-134">UpdateItem Operation</span><span class="sxs-lookup"><span data-stu-id="e47a0-134">UpdateItem operation</span></span>](updateitem-operation.md)

