---
title: хасирм
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: fedc04e0-cfd2-4652-a2a8-51de859ae847
description: Элемент Хасирм указывает, является ли по крайней мере одно сообщение в беседе и в текущей папке защищенным сообщением управления правами на доступ к данным.
ms.openlocfilehash: c129370d7920da7cf1f9f32eed2f075e6c21cf8b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833803"
---
# <a name="hasirm"></a><span data-ttu-id="2c7ca-103">хасирм</span><span class="sxs-lookup"><span data-stu-id="2c7ca-103">HasIrm</span></span>

<span data-ttu-id="2c7ca-104">Элемент **хасирм** указывает, является ли по крайней мере одно сообщение в беседе и в текущей папке защищенным сообщением управления правами на доступ к данным.</span><span class="sxs-lookup"><span data-stu-id="2c7ca-104">The **HasIrm** element specifies whether at least one message in the conversation and the current folder is an IRM protected message.</span></span> 
  
```XML
<HasIrm> true | false </HasIrm>
```

 <span data-ttu-id="2c7ca-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="2c7ca-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2c7ca-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="2c7ca-106">Attributes and elements</span></span>

<span data-ttu-id="2c7ca-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="2c7ca-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2c7ca-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="2c7ca-108">Attributes</span></span>

<span data-ttu-id="2c7ca-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="2c7ca-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2c7ca-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="2c7ca-110">Child elements</span></span>

<span data-ttu-id="2c7ca-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="2c7ca-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="2c7ca-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="2c7ca-112">Parent elements</span></span>

[<span data-ttu-id="2c7ca-113">Беседы (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="2c7ca-113">Conversation (ConversationType)</span></span>](conversation-conversationtype.md)
  
## <a name="text-value"></a><span data-ttu-id="2c7ca-114">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="2c7ca-114">Text value</span></span>

<span data-ttu-id="2c7ca-115">Текстовое значение элемента **хасирм** имеет значение **true** , если по крайней мере одно сообщение в беседе и текущая папка имеют IRM.</span><span class="sxs-lookup"><span data-stu-id="2c7ca-115">The text value of the **HasIrm** element is **true** if at least one message in the conversation and the current folder has IRM.</span></span> <span data-ttu-id="2c7ca-116">В противном случае — значение **false**.</span><span class="sxs-lookup"><span data-stu-id="2c7ca-116">Otherwise, the value is **false**.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="2c7ca-117">Примечания</span><span class="sxs-lookup"><span data-stu-id="2c7ca-117">Remarks</span></span>

<span data-ttu-id="2c7ca-118">Этот элемент появился в Exchange Server 2013 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="2c7ca-118">This element was introduced in Exchange Server 2013 Service Pack 1 (SP1).</span></span>
  
<span data-ttu-id="2c7ca-119">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="2c7ca-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2c7ca-120">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="2c7ca-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2c7ca-121">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="2c7ca-121">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="2c7ca-122">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="2c7ca-122">Schema Name</span></span>  <br/> |<span data-ttu-id="2c7ca-123">Схема Types</span><span class="sxs-lookup"><span data-stu-id="2c7ca-123">Types schema</span></span>  <br/> |
|<span data-ttu-id="2c7ca-124">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="2c7ca-124">Validation File</span></span>  <br/> |<span data-ttu-id="2c7ca-125">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="2c7ca-125">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="2c7ca-126">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="2c7ca-126">Can be Empty</span></span>  <br/> |<span data-ttu-id="2c7ca-127">True</span><span class="sxs-lookup"><span data-stu-id="2c7ca-127">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="2c7ca-128">См. также</span><span class="sxs-lookup"><span data-stu-id="2c7ca-128">See also</span></span>



[<span data-ttu-id="2c7ca-129">Беседы (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="2c7ca-129">Conversation (ConversationType)</span></span>](conversation-conversationtype.md)


- [<span data-ttu-id="2c7ca-130">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="2c7ca-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

