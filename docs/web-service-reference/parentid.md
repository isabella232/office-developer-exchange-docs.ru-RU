---
title: ParentId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: bb7aaa46-3a04-4197-aebb-8881ff10603f
description: Элемент ParentId указывает идентификатор родительского элемента в предварительном просмотре поиска.
ms.openlocfilehash: e09b5f9e463c7ecdfc595c87a84584f69cab3f2c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529023"
---
# <a name="parentid"></a><span data-ttu-id="2e25d-103">ParentId</span><span class="sxs-lookup"><span data-stu-id="2e25d-103">ParentId</span></span>

<span data-ttu-id="2e25d-104">Элемент **ParentID** указывает идентификатор родительского элемента в предварительном просмотре поиска.</span><span class="sxs-lookup"><span data-stu-id="2e25d-104">The **ParentId** element specifies the identifier of the parent item in a search preview.</span></span> 
  
```XML
<ParentId Id="" ChangeKey=""/>
```

<span data-ttu-id="2e25d-105">**итемидтипе**</span><span class="sxs-lookup"><span data-stu-id="2e25d-105">**ItemIdType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="2e25d-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="2e25d-106">Attributes and elements</span></span>

<span data-ttu-id="2e25d-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="2e25d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2e25d-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="2e25d-108">Attributes</span></span>

|<span data-ttu-id="2e25d-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="2e25d-109">**Attribute**</span></span>|<span data-ttu-id="2e25d-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="2e25d-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="2e25d-111">Id</span><span class="sxs-lookup"><span data-stu-id="2e25d-111">Id</span></span>  <br/> |<span data-ttu-id="2e25d-112">Текстовое значение атрибута **ID** — идентификатор родительского элемента.</span><span class="sxs-lookup"><span data-stu-id="2e25d-112">The text value of the **Id** attribute is the identifier of the parent item.</span></span>  <br/> |
|<span data-ttu-id="2e25d-113">чанжекэй</span><span class="sxs-lookup"><span data-stu-id="2e25d-113">ChangeKey</span></span>  <br/> |<span data-ttu-id="2e25d-114">Текстовое значение атрибута **чанжекэй** — это ключ изменения родительского элемента.</span><span class="sxs-lookup"><span data-stu-id="2e25d-114">The text value of the **ChangeKey** attribute is the change key of the parent item.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="2e25d-115">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="2e25d-115">Child elements</span></span>

<span data-ttu-id="2e25d-116">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="2e25d-116">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="2e25d-117">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="2e25d-117">Parent elements</span></span>

[<span data-ttu-id="2e25d-118">сеарчпревиевитем</span><span class="sxs-lookup"><span data-stu-id="2e25d-118">SearchPreviewItem</span></span>](searchpreviewitem.md)
  
## <a name="remarks"></a><span data-ttu-id="2e25d-119">Примечания</span><span class="sxs-lookup"><span data-stu-id="2e25d-119">Remarks</span></span>

<span data-ttu-id="2e25d-120">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="2e25d-120">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="2e25d-121">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="2e25d-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2e25d-122">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="2e25d-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2e25d-123">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="2e25d-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="2e25d-124">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="2e25d-124">Schema name</span></span>  <br/> |<span data-ttu-id="2e25d-125">Схема Types</span><span class="sxs-lookup"><span data-stu-id="2e25d-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="2e25d-126">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="2e25d-126">Validation file</span></span>  <br/> |<span data-ttu-id="2e25d-127">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="2e25d-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="2e25d-128">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="2e25d-128">Can be empty</span></span>  <br/> |<span data-ttu-id="2e25d-129">true</span><span class="sxs-lookup"><span data-stu-id="2e25d-129">true</span></span>  <br/> |
   

