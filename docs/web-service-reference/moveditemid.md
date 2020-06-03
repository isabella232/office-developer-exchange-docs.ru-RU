---
title: моведитемид
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 7d5425ab-1e75-43d1-b801-802ff5139df6
description: Элемент Моведитемид указывает идентификатор элемента, перемещенного операцией MarkAsJunk.
ms.openlocfilehash: 5cf8800ec672278691348bbcd8c6c8cc7a12905b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44468616"
---
# <a name="moveditemid"></a><span data-ttu-id="93b5f-103">моведитемид</span><span class="sxs-lookup"><span data-stu-id="93b5f-103">MovedItemId</span></span>

<span data-ttu-id="93b5f-104">Элемент **моведитемид** указывает идентификатор элемента, перемещенного операцией **MarkAsJunk** .</span><span class="sxs-lookup"><span data-stu-id="93b5f-104">The **MovedItemId** element specifies the identifier of the item that was moved by the **MarkAsJunk** operation.</span></span> 
  
```XML
<MovedItemId Id="" ChangeKey=""/>
```

 <span data-ttu-id="93b5f-105">**итемидтипе**</span><span class="sxs-lookup"><span data-stu-id="93b5f-105">**ItemIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="93b5f-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="93b5f-106">Attributes and elements</span></span>

<span data-ttu-id="93b5f-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="93b5f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="93b5f-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="93b5f-108">Attributes</span></span>

|<span data-ttu-id="93b5f-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="93b5f-109">**Attribute**</span></span>|<span data-ttu-id="93b5f-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="93b5f-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="93b5f-111">Id</span><span class="sxs-lookup"><span data-stu-id="93b5f-111">Id</span></span>  <br/> |<span data-ttu-id="93b5f-112">Значение атрибута **ID** — это идентификатор элемента, который перемещается с помощью операции **MarkAsJunk** .</span><span class="sxs-lookup"><span data-stu-id="93b5f-112">The value of the **Id** attribute is the item identifier of the item that is moved by the **MarkAsJunk** operation.</span></span> <span data-ttu-id="93b5f-113">После перемещения идентификатор элемента останется прежним.</span><span class="sxs-lookup"><span data-stu-id="93b5f-113">The item identifier will remain the same after the move.</span></span>  <br/> |
|<span data-ttu-id="93b5f-114">чанжекэй</span><span class="sxs-lookup"><span data-stu-id="93b5f-114">ChangeKey</span></span>  <br/> |<span data-ttu-id="93b5f-115">Значение атрибута **чанжекэй** — это ключ изменения перемещенного элемента.</span><span class="sxs-lookup"><span data-stu-id="93b5f-115">The value of the **ChangeKey** attribute is the change key of the moved item.</span></span> <span data-ttu-id="93b5f-116">Изменение ключа изменения после перемещения элемента с помощью операции **MarkAsJunk** .</span><span class="sxs-lookup"><span data-stu-id="93b5f-116">The change key changes after the item is moved by the **MarkAsJunk** operation.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="93b5f-117">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="93b5f-117">Child elements</span></span>

<span data-ttu-id="93b5f-118">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="93b5f-118">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="93b5f-119">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="93b5f-119">Parent elements</span></span>

[<span data-ttu-id="93b5f-120">маркасжункреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="93b5f-120">MarkAsJunkResponseMessage</span></span>](markasjunkresponsemessage.md)
  
## <a name="remarks"></a><span data-ttu-id="93b5f-121">Примечания</span><span class="sxs-lookup"><span data-stu-id="93b5f-121">Remarks</span></span>

<span data-ttu-id="93b5f-122">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="93b5f-122">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="93b5f-123">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="93b5f-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="93b5f-124">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="93b5f-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="93b5f-125">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="93b5f-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="93b5f-126">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="93b5f-126">Schema name</span></span>  <br/> |<span data-ttu-id="93b5f-127">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="93b5f-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="93b5f-128">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="93b5f-128">Validation file</span></span>  <br/> |<span data-ttu-id="93b5f-129">messages. xsd</span><span class="sxs-lookup"><span data-stu-id="93b5f-129">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="93b5f-130">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="93b5f-130">Can be empty</span></span>  <br/> ||
   

