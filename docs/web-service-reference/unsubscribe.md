---
title: Отмена подписки
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Unsubscribe
api_type:
- schema
ms.assetid: 5584db5f-553a-47ce-85fb-f9902c9990ab
description: Элемент отказа от подписки содержит свойства, используемые для отмены подписки.
ms.openlocfilehash: bab797ff74a921e3e93c993229bc6d6d289e0c5c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19840307"
---
# <a name="unsubscribe"></a><span data-ttu-id="06d72-103">Отмена подписки</span><span class="sxs-lookup"><span data-stu-id="06d72-103">Unsubscribe</span></span>

<span data-ttu-id="06d72-104">Элемент **отказа от подписки** содержит свойства, используемые для отмены подписки.</span><span class="sxs-lookup"><span data-stu-id="06d72-104">The **Unsubscribe** element contains the properties used to unsubscribe from a subscription.</span></span> 
  
[<span data-ttu-id="06d72-105">Отписаться</span><span class="sxs-lookup"><span data-stu-id="06d72-105">Unsubscribe</span></span>](unsubscribe.md)
  
```xml
<Unsubscribe>
   <SubscriptionId/>
</Unsubscribe>
```

 <span data-ttu-id="06d72-106">**UnsubscribeType**</span><span class="sxs-lookup"><span data-stu-id="06d72-106">**UnsubscribeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="06d72-107">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="06d72-107">Attributes and elements</span></span>

<span data-ttu-id="06d72-108">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="06d72-108">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="06d72-109">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="06d72-109">Attributes</span></span>

<span data-ttu-id="06d72-110">Нет.</span><span class="sxs-lookup"><span data-stu-id="06d72-110">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="06d72-111">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="06d72-111">Child elements</span></span>

|<span data-ttu-id="06d72-112">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="06d72-112">**Element**</span></span>|<span data-ttu-id="06d72-113">**Описание**</span><span class="sxs-lookup"><span data-stu-id="06d72-113">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="06d72-114">SubscriptionId (GetEvents)</span><span class="sxs-lookup"><span data-stu-id="06d72-114">SubscriptionId (GetEvents)</span></span>](subscriptionid-getevents.md) <br/> |<span data-ttu-id="06d72-115">Представляет идентификатор для подписки.</span><span class="sxs-lookup"><span data-stu-id="06d72-115">Represents the identifier for a subscription.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="06d72-116">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="06d72-116">Parent elements</span></span>

<span data-ttu-id="06d72-117">Нет.</span><span class="sxs-lookup"><span data-stu-id="06d72-117">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="06d72-118">Замечания</span><span class="sxs-lookup"><span data-stu-id="06d72-118">Remarks</span></span>

<span data-ttu-id="06d72-119">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="06d72-119">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="06d72-120">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="06d72-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="06d72-121">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="06d72-121">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="06d72-122">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="06d72-122">Schema name</span></span>  <br/> |<span data-ttu-id="06d72-123">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="06d72-123">Messages schema</span></span>  <br/> |
|<span data-ttu-id="06d72-124">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="06d72-124">Validation file</span></span>  <br/> |<span data-ttu-id="06d72-125">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="06d72-125">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="06d72-126">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="06d72-126">Can be empty</span></span>  <br/> |<span data-ttu-id="06d72-127">False</span><span class="sxs-lookup"><span data-stu-id="06d72-127">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="06d72-128">См. также</span><span class="sxs-lookup"><span data-stu-id="06d72-128">See also</span></span>



[<span data-ttu-id="06d72-129">Операции подписки</span><span class="sxs-lookup"><span data-stu-id="06d72-129">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="06d72-130">Операция GetEvents</span><span class="sxs-lookup"><span data-stu-id="06d72-130">GetEvents operation</span></span>](getevents-operation.md)
  
[<span data-ttu-id="06d72-131">Отписаться операции</span><span class="sxs-lookup"><span data-stu-id="06d72-131">Unsubscribe operation</span></span>](unsubscribe-operation.md)

