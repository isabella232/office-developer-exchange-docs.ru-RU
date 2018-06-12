---
title: UpdatedItemIds
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 9199aeb2-abdf-40c5-8743-40b61853c951
description: Элемент UpdatedItemIds указывает идентификаторы элементов напоминания.
ms.openlocfilehash: b95ebb20823706e68b1fd66dc64f756808bb7375
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19840323"
---
# <a name="updateditemids"></a><span data-ttu-id="edd55-103">UpdatedItemIds</span><span class="sxs-lookup"><span data-stu-id="edd55-103">UpdatedItemIds</span></span>

<span data-ttu-id="edd55-104">Элемент **UpdatedItemIds** указывает идентификаторы элементов напоминания.</span><span class="sxs-lookup"><span data-stu-id="edd55-104">The **UpdatedItemIds** element specifies the identifiers of updated reminder items.</span></span> 
  
```XML
<UpdatedItemIds>
   <ItemId></ItemId>
</UpdatedItemIds>

```

 <span data-ttu-id="edd55-105">**NonEmptyArrayOfItemIdsType**</span><span class="sxs-lookup"><span data-stu-id="edd55-105">**NonEmptyArrayOfItemIdsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="edd55-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="edd55-106">Attributes and elements</span></span>

<span data-ttu-id="edd55-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="edd55-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="edd55-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="edd55-108">Attributes</span></span>

<span data-ttu-id="edd55-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="edd55-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="edd55-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="edd55-110">Child elements</span></span>

[<span data-ttu-id="edd55-111">Идентификатор элемента</span><span class="sxs-lookup"><span data-stu-id="edd55-111">ItemId</span></span>](itemid.md)
  
### <a name="parent-elements"></a><span data-ttu-id="edd55-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="edd55-112">Parent elements</span></span>

[<span data-ttu-id="edd55-113">PerformReminderActionResponse</span><span class="sxs-lookup"><span data-stu-id="edd55-113">PerformReminderActionResponse</span></span>](performreminderactionresponse.md)
  
## <a name="remarks"></a><span data-ttu-id="edd55-114">Замечания</span><span class="sxs-lookup"><span data-stu-id="edd55-114">Remarks</span></span>

<span data-ttu-id="edd55-115">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="edd55-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="edd55-116">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="edd55-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
<span data-ttu-id="edd55-117">Если операция [PerformReminderAction](performreminderaction-operation.md) не завершается успешно, а не был изменен на сервере, элемент **UpdatedItemIds** возвращается как пустое значение.</span><span class="sxs-lookup"><span data-stu-id="edd55-117">If the [PerformReminderAction](performreminderaction-operation.md) operation did not complete successfully, or no changes were made on the server, the **UpdatedItemIds** element is returned as an empty value.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="edd55-118">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="edd55-118">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="edd55-119">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="edd55-119">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="edd55-120">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="edd55-120">Schema Name</span></span>  <br/> |<span data-ttu-id="edd55-121">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="edd55-121">Messages schema</span></span>  <br/> |
|<span data-ttu-id="edd55-122">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="edd55-122">Validation File</span></span>  <br/> |<span data-ttu-id="edd55-123">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="edd55-123">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="edd55-124">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="edd55-124">Can be Empty</span></span>  <br/> |<span data-ttu-id="edd55-125">True</span><span class="sxs-lookup"><span data-stu-id="edd55-125">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="edd55-126">См. также</span><span class="sxs-lookup"><span data-stu-id="edd55-126">See also</span></span>



[<span data-ttu-id="edd55-127">PerformReminderActionResponse</span><span class="sxs-lookup"><span data-stu-id="edd55-127">PerformReminderActionResponse</span></span>](performreminderactionresponse.md)


- [<span data-ttu-id="edd55-128">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="edd55-128">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

