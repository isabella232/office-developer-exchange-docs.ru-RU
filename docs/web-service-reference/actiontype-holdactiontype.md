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
ms.openlocfilehash: 8f2796df818dac2bd285b055aa44fbcecd0de5e6
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457860"
---
# <a name="actiontype-holdactiontype"></a><span data-ttu-id="84bc3-103">Себя (Холдактионтипе)</span><span class="sxs-lookup"><span data-stu-id="84bc3-103">ActionType (HoldActionType)</span></span>

<span data-ttu-id="84bc3-104">Элемент **тип** действия указывает тип действия для удержания.</span><span class="sxs-lookup"><span data-stu-id="84bc3-104">The **ActionType** element indicates the type of action for the hold.</span></span> 
  
```XML
<ActionType> Create | Update | Remove </ActionType>
```

 <span data-ttu-id="84bc3-105">**холдактионтипе**</span><span class="sxs-lookup"><span data-stu-id="84bc3-105">**HoldActionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="84bc3-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="84bc3-106">Attributes and elements</span></span>

<span data-ttu-id="84bc3-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="84bc3-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="84bc3-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="84bc3-108">Attributes</span></span>

<span data-ttu-id="84bc3-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="84bc3-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="84bc3-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="84bc3-110">Child elements</span></span>

<span data-ttu-id="84bc3-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="84bc3-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="84bc3-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="84bc3-112">Parent elements</span></span>

[<span data-ttu-id="84bc3-113">SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="84bc3-113">SetHoldOnMailboxes</span></span>](setholdonmailboxes.md)
  
## <a name="text-value"></a><span data-ttu-id="84bc3-114">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="84bc3-114">Text value</span></span>

<span data-ttu-id="84bc3-115">Текстовое значение **элемента "объект** " — это тип удержания для почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="84bc3-115">The text value of the **ActionType** element is the type of hold set on a mailbox.</span></span> <span data-ttu-id="84bc3-116">Текстовое значение **CREATE** указывает на то, что будет создано удержание почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="84bc3-116">A text value of **Create** indicates that a mailbox hold will be created.</span></span> <span data-ttu-id="84bc3-117">Текстовое значение **Update** указывает на то, что будет обновлено удержание почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="84bc3-117">A text value of **Update** indicates that a mailbox hold will be updated.</span></span> <span data-ttu-id="84bc3-118">Текстовое значение **Remove** указывает на то, что удержание почтового ящика будет удалено.</span><span class="sxs-lookup"><span data-stu-id="84bc3-118">A text value of **Remove** indicates that a mailbox hold will be removed.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="84bc3-119">Примечания</span><span class="sxs-lookup"><span data-stu-id="84bc3-119">Remarks</span></span>

<span data-ttu-id="84bc3-120">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="84bc3-120">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="84bc3-121">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="84bc3-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="84bc3-122">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="84bc3-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="84bc3-123">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="84bc3-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="84bc3-124">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="84bc3-124">Schema name</span></span>  <br/> |<span data-ttu-id="84bc3-125">Схема Types</span><span class="sxs-lookup"><span data-stu-id="84bc3-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="84bc3-126">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="84bc3-126">Validation file</span></span>  <br/> |<span data-ttu-id="84bc3-127">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="84bc3-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="84bc3-128">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="84bc3-128">Can be empty</span></span>  <br/> |<span data-ttu-id="84bc3-129">false</span><span class="sxs-lookup"><span data-stu-id="84bc3-129">false</span></span>  <br/> |
   

