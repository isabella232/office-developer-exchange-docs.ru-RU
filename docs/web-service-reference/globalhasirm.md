---
title: GlobalHasIrm
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 425272b2-7a4e-4376-aea9-d9b10c1ad6ee
description: Элемент GlobalHasIrm указывает, является ли по крайней мере один сообщений в окне беседы и во всех папках сообщение защищенные IRM.
ms.openlocfilehash: ad3eafcb38829e7ea57cbc7535b0f5411ad595d2
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833717"
---
# <a name="globalhasirm"></a><span data-ttu-id="3b8dd-103">GlobalHasIrm</span><span class="sxs-lookup"><span data-stu-id="3b8dd-103">GlobalHasIrm</span></span>

<span data-ttu-id="3b8dd-104">Элемент **GlobalHasIrm** указывает, является ли по крайней мере один сообщений в окне беседы и во всех папках сообщение защищенные IRM.</span><span class="sxs-lookup"><span data-stu-id="3b8dd-104">The **GlobalHasIrm** element specifies whether at least one message in the conversation and across all folders is an IRM protected message.</span></span> 
  
```XML
<GlobalHasIrm> true | false </GlobalHasIrm>
```

 <span data-ttu-id="3b8dd-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="3b8dd-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3b8dd-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="3b8dd-106">Attributes and elements</span></span>

<span data-ttu-id="3b8dd-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="3b8dd-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3b8dd-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="3b8dd-108">Attributes</span></span>

<span data-ttu-id="3b8dd-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="3b8dd-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3b8dd-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="3b8dd-110">Child elements</span></span>

<span data-ttu-id="3b8dd-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="3b8dd-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="3b8dd-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="3b8dd-112">Parent elements</span></span>

[<span data-ttu-id="3b8dd-113">Беседы (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="3b8dd-113">Conversation (ConversationType)</span></span>](conversation-conversationtype.md)
  
## <a name="text-value"></a><span data-ttu-id="3b8dd-114">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="3b8dd-114">Text value</span></span>

<span data-ttu-id="3b8dd-115">Текстовое значение элемента **GlobalHasIrm** равно **true** , если хотя бы один сообщение в окне беседы и во всех папках является сообщением защищенные IRM.</span><span class="sxs-lookup"><span data-stu-id="3b8dd-115">The text value of the **GlobalHasIrm** element is **true** if at least one message in the conversation and across all folders is an IRM protected message.</span></span> <span data-ttu-id="3b8dd-116">В противном случае — значение **false**.</span><span class="sxs-lookup"><span data-stu-id="3b8dd-116">Otherwise the value is **false**.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="3b8dd-117">Замечания</span><span class="sxs-lookup"><span data-stu-id="3b8dd-117">Remarks</span></span>

<span data-ttu-id="3b8dd-118">Этот элемент появился в Exchange Server 2013 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="3b8dd-118">This element was introduced in Exchange Server 2013 Service Pack 1 (SP1).</span></span>
  
<span data-ttu-id="3b8dd-119">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="3b8dd-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3b8dd-120">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="3b8dd-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3b8dd-121">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="3b8dd-121">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="3b8dd-122">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="3b8dd-122">Schema Name</span></span>  <br/> |<span data-ttu-id="3b8dd-123">Схема Types</span><span class="sxs-lookup"><span data-stu-id="3b8dd-123">Types schema</span></span>  <br/> |
|<span data-ttu-id="3b8dd-124">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="3b8dd-124">Validation File</span></span>  <br/> |<span data-ttu-id="3b8dd-125">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="3b8dd-125">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="3b8dd-126">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="3b8dd-126">Can be Empty</span></span>  <br/> |<span data-ttu-id="3b8dd-127">True</span><span class="sxs-lookup"><span data-stu-id="3b8dd-127">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3b8dd-128">См. также</span><span class="sxs-lookup"><span data-stu-id="3b8dd-128">See also</span></span>



[<span data-ttu-id="3b8dd-129">Беседы (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="3b8dd-129">Conversation (ConversationType)</span></span>](conversation-conversationtype.md)


- [<span data-ttu-id="3b8dd-130">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="3b8dd-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

