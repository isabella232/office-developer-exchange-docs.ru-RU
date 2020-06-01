---
title: исмембершипграуп
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 0dc3e285-8f49-48ad-b844-37041c0d782b
description: Элемент Исмембершипграуп указывает логическое значение, которое указывает, является ли объект группой рассылки или почтовым ящиком.
ms.openlocfilehash: ed79961c6d13ab226c0b489103ef3d2c4a08668d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459288"
---
# <a name="ismembershipgroup"></a><span data-ttu-id="91ec7-103">исмембершипграуп</span><span class="sxs-lookup"><span data-stu-id="91ec7-103">IsMembershipGroup</span></span>

<span data-ttu-id="91ec7-104">Элемент **исмембершипграуп** указывает логическое значение, которое указывает, является ли объект группой рассылки или почтовым ящиком.</span><span class="sxs-lookup"><span data-stu-id="91ec7-104">The **IsMembershipGroup** element specifies a Boolean value that indicates whether the entity is a distribution group or a mailbox.</span></span> 
  
```XML
<IsMembershipGroup>true | false</IsMembershipGroup>
```

 <span data-ttu-id="91ec7-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="91ec7-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="91ec7-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="91ec7-106">Attributes and elements</span></span>

<span data-ttu-id="91ec7-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="91ec7-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="91ec7-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="91ec7-108">Attributes</span></span>

<span data-ttu-id="91ec7-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="91ec7-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="91ec7-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="91ec7-110">Child elements</span></span>

<span data-ttu-id="91ec7-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="91ec7-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="91ec7-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="91ec7-112">Parent elements</span></span>

|<span data-ttu-id="91ec7-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="91ec7-113">**Element**</span></span>|<span data-ttu-id="91ec7-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="91ec7-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="91ec7-115">сеарчаблемаилбокс</span><span class="sxs-lookup"><span data-stu-id="91ec7-115">SearchableMailbox</span></span>](searchablemailbox.md) <br/> |<span data-ttu-id="91ec7-116">Указывает почтовый ящик, возвращенный из запроса **GetSearchableMailboxes** .</span><span class="sxs-lookup"><span data-stu-id="91ec7-116">Specifies a mailbox returned from a **GetSearchableMailboxes** request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="91ec7-117">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="91ec7-117">Text value</span></span>

<span data-ttu-id="91ec7-118">Текстовое значение **true** для элемента **исмембершипграуп** указывает на то, что сущность является группой рассылки или почтовым ящиком.</span><span class="sxs-lookup"><span data-stu-id="91ec7-118">A text value of **true** for the **IsMembershipGroup** element indicates that the entity is a distribution group or a mailbox.</span></span> <span data-ttu-id="91ec7-119">Значение false указывает, что объект не является группой рассылки или почтовым ящиком.</span><span class="sxs-lookup"><span data-stu-id="91ec7-119">A value of false indicates that the entity is not a distribution group or a mailbox.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="91ec7-120">Примечания</span><span class="sxs-lookup"><span data-stu-id="91ec7-120">Remarks</span></span>

<span data-ttu-id="91ec7-121">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="91ec7-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="91ec7-122">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="91ec7-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="91ec7-123">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="91ec7-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="91ec7-124">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="91ec7-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="91ec7-125">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="91ec7-125">Schema Name</span></span>  <br/> |<span data-ttu-id="91ec7-126">Схема типа</span><span class="sxs-lookup"><span data-stu-id="91ec7-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="91ec7-127">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="91ec7-127">Validation File</span></span>  <br/> |<span data-ttu-id="91ec7-128">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="91ec7-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="91ec7-129">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="91ec7-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="91ec7-130">См. также</span><span class="sxs-lookup"><span data-stu-id="91ec7-130">See also</span></span>



- [<span data-ttu-id="91ec7-131">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="91ec7-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

