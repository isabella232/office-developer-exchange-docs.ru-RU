---
title: ассигнкатегориес
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AssignCategories
api_type:
- schema
ms.assetid: f5c73fed-7b00-446d-8296-71a0c86e7fc6
description: Элемент Ассигнкатегориес представляет категории, помеченные в сообщениях электронной почты.
ms.openlocfilehash: e2dad0e2ef46421ae92a0d2826d161e5e2af3b93
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44464744"
---
# <a name="assigncategories"></a><span data-ttu-id="ae4b6-103">ассигнкатегориес</span><span class="sxs-lookup"><span data-stu-id="ae4b6-103">AssignCategories</span></span>

<span data-ttu-id="ae4b6-104">Элемент **ассигнкатегориес** представляет категории, помеченные в сообщениях электронной почты.</span><span class="sxs-lookup"><span data-stu-id="ae4b6-104">The **AssignCategories** element represents the categories that are stamped on e-mail messages.</span></span> 
  
- [<span data-ttu-id="ae4b6-105">Правило (RuleType)</span><span class="sxs-lookup"><span data-stu-id="ae4b6-105">Rule (RuleType)</span></span>](rule-ruletype.md)
  
- [<span data-ttu-id="ae4b6-106">Actions</span><span class="sxs-lookup"><span data-stu-id="ae4b6-106">Actions</span></span>](actions.md)
  
```XML
<AssignCategories>
   <String/>
</AssignCategories>
```

 <span data-ttu-id="ae4b6-107">**аррайофстрингстипе**</span><span class="sxs-lookup"><span data-stu-id="ae4b6-107">**ArrayOfStringsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ae4b6-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="ae4b6-108">Attributes and elements</span></span>

<span data-ttu-id="ae4b6-109">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="ae4b6-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ae4b6-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="ae4b6-110">Attributes</span></span>

<span data-ttu-id="ae4b6-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="ae4b6-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ae4b6-112">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="ae4b6-112">Child elements</span></span>

|<span data-ttu-id="ae4b6-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="ae4b6-113">**Element**</span></span>|<span data-ttu-id="ae4b6-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="ae4b6-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ae4b6-115">Строка</span><span class="sxs-lookup"><span data-stu-id="ae4b6-115">String</span></span>](string.md) <br/> |<span data-ttu-id="ae4b6-116">Содержит строку, определяющую одну категорию.</span><span class="sxs-lookup"><span data-stu-id="ae4b6-116">Contains a string that identifies a single category.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="ae4b6-117">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="ae4b6-117">Parent elements</span></span>

|<span data-ttu-id="ae4b6-118">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="ae4b6-118">**Element**</span></span>|<span data-ttu-id="ae4b6-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="ae4b6-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ae4b6-120">Действия</span><span class="sxs-lookup"><span data-stu-id="ae4b6-120">Actions</span></span>](actions.md) <br/> |<span data-ttu-id="ae4b6-121">Представляет набор действий, которые доступны для выполнения на сообщение при условия будут выполнены.</span><span class="sxs-lookup"><span data-stu-id="ae4b6-121">Represents the set of actions that are available to be taken on a message when the conditions are fulfilled.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="ae4b6-122">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="ae4b6-122">Text value</span></span>

<span data-ttu-id="ae4b6-123">Нет.</span><span class="sxs-lookup"><span data-stu-id="ae4b6-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="ae4b6-124">Примечания</span><span class="sxs-lookup"><span data-stu-id="ae4b6-124">Remarks</span></span>

<span data-ttu-id="ae4b6-125">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="ae4b6-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ae4b6-126">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="ae4b6-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ae4b6-127">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="ae4b6-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="ae4b6-128">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="ae4b6-128">Schema Name</span></span>  <br/> |<span data-ttu-id="ae4b6-129">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="ae4b6-129">Messages schema</span></span>  <br/> |
|<span data-ttu-id="ae4b6-130">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="ae4b6-130">Validation File</span></span>  <br/> |<span data-ttu-id="ae4b6-131">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="ae4b6-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="ae4b6-132">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="ae4b6-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="ae4b6-133">True</span><span class="sxs-lookup"><span data-stu-id="ae4b6-133">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ae4b6-134">См. также</span><span class="sxs-lookup"><span data-stu-id="ae4b6-134">See also</span></span>

- [<span data-ttu-id="ae4b6-135">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="ae4b6-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

