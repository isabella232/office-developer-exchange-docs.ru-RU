---
title: итемчанжес
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
description: Элемент Итемчанжес содержит массив элементов Итемчанже, определяющих элементы и обновления, которые необходимо применить к элементам.
ms.openlocfilehash: ea6fb2023b88360f9558057e80c7fe0d855173b5
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459912"
---
# <a name="itemchanges"></a><span data-ttu-id="43047-103">итемчанжес</span><span class="sxs-lookup"><span data-stu-id="43047-103">ItemChanges</span></span>

<span data-ttu-id="43047-104">Элемент **итемчанжес** содержит массив элементов [итемчанже](itemchange.md) , определяющих элементы и обновления, которые необходимо применить к элементам.</span><span class="sxs-lookup"><span data-stu-id="43047-104">The **ItemChanges** element contains an array of [ItemChange](itemchange.md) elements that identify items and the updates to apply to the items.</span></span> 
  
[<span data-ttu-id="43047-105">UpdateItem</span><span class="sxs-lookup"><span data-stu-id="43047-105">UpdateItem</span></span>](updateitem.md)
  
[<span data-ttu-id="43047-106">итемчанжес</span><span class="sxs-lookup"><span data-stu-id="43047-106">ItemChanges</span></span>](itemchanges.md)
  
```xml
<ItemChanges>
   <ItemChange/>
</ItemChanges>
```

 <span data-ttu-id="43047-107">**нонемптяррайофитемчанжестипе**</span><span class="sxs-lookup"><span data-stu-id="43047-107">**NonEmptyArrayOfItemChangesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="43047-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="43047-108">Attributes and elements</span></span>

<span data-ttu-id="43047-109">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="43047-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="43047-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="43047-110">Attributes</span></span>

<span data-ttu-id="43047-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="43047-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="43047-112">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="43047-112">Child elements</span></span>

|<span data-ttu-id="43047-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="43047-113">**Element**</span></span>|<span data-ttu-id="43047-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="43047-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="43047-115">ItemChange</span><span class="sxs-lookup"><span data-stu-id="43047-115">ItemChange</span></span>](itemchange.md) <br/> |<span data-ttu-id="43047-116">Содержит идентификатор элемента и обновления, применяемые к элементу.</span><span class="sxs-lookup"><span data-stu-id="43047-116">Contains an item identifier and the updates to apply to the item.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="43047-117">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="43047-117">Parent elements</span></span>

|<span data-ttu-id="43047-118">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="43047-118">**Element**</span></span>|<span data-ttu-id="43047-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="43047-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="43047-120">UpdateItem</span><span class="sxs-lookup"><span data-stu-id="43047-120">UpdateItem</span></span>](updateitem.md) <br/> |<span data-ttu-id="43047-121">Определяет запрос на обновление элементов в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="43047-121">Defines a request to update items in a mailbox.</span></span>  <br/> <span data-ttu-id="43047-122">Ниже приведено выражение XPath для этого элемента:</span><span class="sxs-lookup"><span data-stu-id="43047-122">The following is the XPath expression to this element:</span></span>  <br/>  `/UpdateItem` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="43047-123">Примечания</span><span class="sxs-lookup"><span data-stu-id="43047-123">Remarks</span></span>

<span data-ttu-id="43047-124">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="43047-124">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="43047-125">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="43047-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="43047-126">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="43047-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="43047-127">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="43047-127">Schema Name</span></span>  <br/> |<span data-ttu-id="43047-128">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="43047-128">Messages schema</span></span>  <br/> |
|<span data-ttu-id="43047-129">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="43047-129">Validation File</span></span>  <br/> |<span data-ttu-id="43047-130">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="43047-130">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="43047-131">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="43047-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="43047-132">False</span><span class="sxs-lookup"><span data-stu-id="43047-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="43047-133">См. также</span><span class="sxs-lookup"><span data-stu-id="43047-133">See also</span></span>



[<span data-ttu-id="43047-134">Операция UpdateItem</span><span class="sxs-lookup"><span data-stu-id="43047-134">UpdateItem operation</span></span>](updateitem-operation.md)

