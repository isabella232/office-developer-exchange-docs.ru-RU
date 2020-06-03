---
title: глобалхасирм
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 425272b2-7a4e-4376-aea9-d9b10c1ad6ee
description: Элемент Глобалхасирм указывает, является ли по крайней мере одно сообщение в беседе и во всех папках сообщением, защищенным службой управления правами на доступ к данным.
ms.openlocfilehash: 10b99c9a6421a89a549b69e918087f3e542ffa09
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459471"
---
# <a name="globalhasirm"></a><span data-ttu-id="8b154-103">глобалхасирм</span><span class="sxs-lookup"><span data-stu-id="8b154-103">GlobalHasIrm</span></span>

<span data-ttu-id="8b154-104">Элемент **глобалхасирм** указывает, является ли по крайней мере одно сообщение в беседе и во всех папках сообщением, защищенным службой управления правами на доступ к данным.</span><span class="sxs-lookup"><span data-stu-id="8b154-104">The **GlobalHasIrm** element specifies whether at least one message in the conversation and across all folders is an IRM protected message.</span></span> 
  
```XML
<GlobalHasIrm> true | false </GlobalHasIrm>
```

 <span data-ttu-id="8b154-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="8b154-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8b154-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="8b154-106">Attributes and elements</span></span>

<span data-ttu-id="8b154-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="8b154-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8b154-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="8b154-108">Attributes</span></span>

<span data-ttu-id="8b154-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="8b154-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8b154-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="8b154-110">Child elements</span></span>

<span data-ttu-id="8b154-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="8b154-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="8b154-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="8b154-112">Parent elements</span></span>

[<span data-ttu-id="8b154-113">Беседы (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="8b154-113">Conversation (ConversationType)</span></span>](conversation-conversationtype.md)
  
## <a name="text-value"></a><span data-ttu-id="8b154-114">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="8b154-114">Text value</span></span>

<span data-ttu-id="8b154-115">Текстовое значение элемента **глобалхасирм** имеет значение **true** , если по крайней мере одно сообщение в беседе и во всех папках является сообщением, защищенным службой управления правами на доступ к данным.</span><span class="sxs-lookup"><span data-stu-id="8b154-115">The text value of the **GlobalHasIrm** element is **true** if at least one message in the conversation and across all folders is an IRM protected message.</span></span> <span data-ttu-id="8b154-116">В противном случае — значение **false**.</span><span class="sxs-lookup"><span data-stu-id="8b154-116">Otherwise the value is **false**.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="8b154-117">Примечания</span><span class="sxs-lookup"><span data-stu-id="8b154-117">Remarks</span></span>

<span data-ttu-id="8b154-118">Этот элемент появился в Exchange Server 2013 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="8b154-118">This element was introduced in Exchange Server 2013 Service Pack 1 (SP1).</span></span>
  
<span data-ttu-id="8b154-119">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="8b154-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8b154-120">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="8b154-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8b154-121">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="8b154-121">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="8b154-122">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="8b154-122">Schema Name</span></span>  <br/> |<span data-ttu-id="8b154-123">Схема Types</span><span class="sxs-lookup"><span data-stu-id="8b154-123">Types schema</span></span>  <br/> |
|<span data-ttu-id="8b154-124">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="8b154-124">Validation File</span></span>  <br/> |<span data-ttu-id="8b154-125">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="8b154-125">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="8b154-126">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="8b154-126">Can be Empty</span></span>  <br/> |<span data-ttu-id="8b154-127">True</span><span class="sxs-lookup"><span data-stu-id="8b154-127">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="8b154-128">См. также</span><span class="sxs-lookup"><span data-stu-id="8b154-128">See also</span></span>



[<span data-ttu-id="8b154-129">Беседы (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="8b154-129">Conversation (ConversationType)</span></span>](conversation-conversationtype.md)


- [<span data-ttu-id="8b154-130">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="8b154-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

