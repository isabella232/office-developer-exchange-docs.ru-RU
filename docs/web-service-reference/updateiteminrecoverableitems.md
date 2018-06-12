---
title: UpdateItemInRecoverableItems
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: c49816b1-dbb5-4716-86c7-30790e86f30e
description: Элемент UpdateItemInRecoverableItems указывает запрос на обновление элемента в элементов для восстановления.
ms.openlocfilehash: 768de4bb8abe4780ab520405bae3149b8f17637c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19840349"
---
# <a name="updateiteminrecoverableitems"></a><span data-ttu-id="0ebc9-103">UpdateItemInRecoverableItems</span><span class="sxs-lookup"><span data-stu-id="0ebc9-103">UpdateItemInRecoverableItems</span></span>

<span data-ttu-id="0ebc9-104">Элемент **UpdateItemInRecoverableItems** указывает запрос на обновление элемента в элементов для восстановления.</span><span class="sxs-lookup"><span data-stu-id="0ebc9-104">The **UpdateItemInRecoverableItems** element specifies a request to update an item in recoverable items.</span></span> 
  
```XML
<UpdateItemInRecoverableItems>
   <ItemId/>
   <Updates/>
   <Attachments/>
   <MakeItemImmutable/>
</UpdateItemInRecoverableItems>
```

 <span data-ttu-id="0ebc9-105">**UpdateItemInRecoverableItemsType**</span><span class="sxs-lookup"><span data-stu-id="0ebc9-105">**UpdateItemInRecoverableItemsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0ebc9-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="0ebc9-106">Attributes and elements</span></span>

<span data-ttu-id="0ebc9-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="0ebc9-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0ebc9-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="0ebc9-108">Attributes</span></span>

<span data-ttu-id="0ebc9-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="0ebc9-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0ebc9-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="0ebc9-110">Child elements</span></span>

<span data-ttu-id="0ebc9-111">[Идентификатор элемента](itemid.md) | [обновления (элемент)](updates-item.md) | [вложения](attachments-ex15websvcsotherref.md) | [MakeItemImmutable](makeitemimmutable.md)</span><span class="sxs-lookup"><span data-stu-id="0ebc9-111">[ItemId](itemid.md) | [Updates (Item)](updates-item.md) | [Attachments](attachments-ex15websvcsotherref.md) | [MakeItemImmutable](makeitemimmutable.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="0ebc9-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="0ebc9-112">Parent elements</span></span>

<span data-ttu-id="0ebc9-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="0ebc9-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="0ebc9-114">Замечания</span><span class="sxs-lookup"><span data-stu-id="0ebc9-114">Remarks</span></span>

<span data-ttu-id="0ebc9-115">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="0ebc9-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="0ebc9-116">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="0ebc9-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0ebc9-117">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="0ebc9-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0ebc9-118">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="0ebc9-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="0ebc9-119">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="0ebc9-119">Schema name</span></span>  <br/> |<span data-ttu-id="0ebc9-120">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="0ebc9-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="0ebc9-121">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="0ebc9-121">Validation file</span></span>  <br/> |<span data-ttu-id="0ebc9-122">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="0ebc9-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="0ebc9-123">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="0ebc9-123">Can be empty</span></span>  <br/> |<span data-ttu-id="0ebc9-124">Нет</span><span class="sxs-lookup"><span data-stu-id="0ebc9-124">false</span></span>  <br/> |
   

