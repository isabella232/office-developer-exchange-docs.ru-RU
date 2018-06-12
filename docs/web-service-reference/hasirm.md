---
title: HasIrm
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: fedc04e0-cfd2-4652-a2a8-51de859ae847
description: Элемент HasIrm указывает, является ли хотя бы один сообщение в беседе и текущей папки сообщение защищенные IRM.
ms.openlocfilehash: c129370d7920da7cf1f9f32eed2f075e6c21cf8b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833803"
---
# <a name="hasirm"></a><span data-ttu-id="a31bf-103">HasIrm</span><span class="sxs-lookup"><span data-stu-id="a31bf-103">HasIrm</span></span>

<span data-ttu-id="a31bf-104">Элемент **HasIrm** указывает, является ли хотя бы один сообщение в беседе и текущей папки сообщение защищенные IRM.</span><span class="sxs-lookup"><span data-stu-id="a31bf-104">The **HasIrm** element specifies whether at least one message in the conversation and the current folder is an IRM protected message.</span></span> 
  
```XML
<HasIrm> true | false </HasIrm>
```

 <span data-ttu-id="a31bf-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="a31bf-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a31bf-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="a31bf-106">Attributes and elements</span></span>

<span data-ttu-id="a31bf-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="a31bf-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a31bf-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="a31bf-108">Attributes</span></span>

<span data-ttu-id="a31bf-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="a31bf-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a31bf-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="a31bf-110">Child elements</span></span>

<span data-ttu-id="a31bf-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="a31bf-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="a31bf-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="a31bf-112">Parent elements</span></span>

[<span data-ttu-id="a31bf-113">Беседы (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="a31bf-113">Conversation (ConversationType)</span></span>](conversation-conversationtype.md)
  
## <a name="text-value"></a><span data-ttu-id="a31bf-114">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="a31bf-114">Text value</span></span>

<span data-ttu-id="a31bf-115">Текстовое значение элемента **HasIrm** равно **true** , если хотя бы один сообщение в беседе и текущей папки имеет IRM.</span><span class="sxs-lookup"><span data-stu-id="a31bf-115">The text value of the **HasIrm** element is **true** if at least one message in the conversation and the current folder has IRM.</span></span> <span data-ttu-id="a31bf-116">В противном случае — значение **false**.</span><span class="sxs-lookup"><span data-stu-id="a31bf-116">Otherwise, the value is **false**.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="a31bf-117">Замечания</span><span class="sxs-lookup"><span data-stu-id="a31bf-117">Remarks</span></span>

<span data-ttu-id="a31bf-118">Этот элемент появился в Exchange Server 2013 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="a31bf-118">This element was introduced in Exchange Server 2013 Service Pack 1 (SP1).</span></span>
  
<span data-ttu-id="a31bf-119">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="a31bf-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a31bf-120">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="a31bf-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a31bf-121">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="a31bf-121">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="a31bf-122">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="a31bf-122">Schema Name</span></span>  <br/> |<span data-ttu-id="a31bf-123">Схема Types</span><span class="sxs-lookup"><span data-stu-id="a31bf-123">Types schema</span></span>  <br/> |
|<span data-ttu-id="a31bf-124">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="a31bf-124">Validation File</span></span>  <br/> |<span data-ttu-id="a31bf-125">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="a31bf-125">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="a31bf-126">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="a31bf-126">Can be Empty</span></span>  <br/> |<span data-ttu-id="a31bf-127">True</span><span class="sxs-lookup"><span data-stu-id="a31bf-127">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a31bf-128">См. также</span><span class="sxs-lookup"><span data-stu-id="a31bf-128">See also</span></span>



[<span data-ttu-id="a31bf-129">Беседы (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="a31bf-129">Conversation (ConversationType)</span></span>](conversation-conversationtype.md)


- [<span data-ttu-id="a31bf-130">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="a31bf-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

