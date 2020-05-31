---
title: Себя (Холдактионтипе)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f50449b9-e73b-43c5-af96-6433bf434dce
description: Элемент тип действия указывает тип действия для удержания.
ms.openlocfilehash: cb1cfa8a1306c4a6cacf5c82824d19cab57e7941
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761326"
---
# <a name="actiontype-holdactiontype"></a><span data-ttu-id="b094e-103">Себя (Холдактионтипе)</span><span class="sxs-lookup"><span data-stu-id="b094e-103">ActionType (HoldActionType)</span></span>

<span data-ttu-id="b094e-104">Элемент **тип** действия указывает тип действия для удержания.</span><span class="sxs-lookup"><span data-stu-id="b094e-104">The **ActionType** element indicates the type of action for the hold.</span></span> 
  
```XML
<ActionType> Create | Update | Remove </ActionType>
```

 <span data-ttu-id="b094e-105">**холдактионтипе**</span><span class="sxs-lookup"><span data-stu-id="b094e-105">**HoldActionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b094e-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="b094e-106">Attributes and elements</span></span>

<span data-ttu-id="b094e-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="b094e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b094e-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="b094e-108">Attributes</span></span>

<span data-ttu-id="b094e-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="b094e-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b094e-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="b094e-110">Child elements</span></span>

<span data-ttu-id="b094e-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="b094e-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="b094e-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="b094e-112">Parent elements</span></span>

[<span data-ttu-id="b094e-113">SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="b094e-113">SetHoldOnMailboxes</span></span>](setholdonmailboxes.md)
  
## <a name="text-value"></a><span data-ttu-id="b094e-114">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="b094e-114">Text value</span></span>

<span data-ttu-id="b094e-115">Текстовое значение **элемента "объект** " — это тип удержания для почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="b094e-115">The text value of the **ActionType** element is the type of hold set on a mailbox.</span></span> <span data-ttu-id="b094e-116">Текстовое значение **CREATE** указывает на то, что будет создано удержание почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="b094e-116">A text value of **Create** indicates that a mailbox hold will be created.</span></span> <span data-ttu-id="b094e-117">Текстовое значение **Update** указывает на то, что будет обновлено удержание почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="b094e-117">A text value of **Update** indicates that a mailbox hold will be updated.</span></span> <span data-ttu-id="b094e-118">Текстовое значение **Remove** указывает на то, что удержание почтового ящика будет удалено.</span><span class="sxs-lookup"><span data-stu-id="b094e-118">A text value of **Remove** indicates that a mailbox hold will be removed.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="b094e-119">Примечания</span><span class="sxs-lookup"><span data-stu-id="b094e-119">Remarks</span></span>

<span data-ttu-id="b094e-120">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="b094e-120">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="b094e-121">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="b094e-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b094e-122">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="b094e-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b094e-123">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="b094e-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="b094e-124">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="b094e-124">Schema name</span></span>  <br/> |<span data-ttu-id="b094e-125">Схема Types</span><span class="sxs-lookup"><span data-stu-id="b094e-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="b094e-126">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="b094e-126">Validation file</span></span>  <br/> |<span data-ttu-id="b094e-127">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="b094e-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="b094e-128">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="b094e-128">Can be empty</span></span>  <br/> |<span data-ttu-id="b094e-129">false</span><span class="sxs-lookup"><span data-stu-id="b094e-129">false</span></span>  <br/> |
   

