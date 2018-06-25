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
ms.lasthandoff: 06/25/2018
ms.locfileid: "19840307"
---
# <a name="unsubscribe"></a><span data-ttu-id="8ec32-103">Отмена подписки</span><span class="sxs-lookup"><span data-stu-id="8ec32-103">Unsubscribe</span></span>

<span data-ttu-id="8ec32-104">Элемент **отказа от подписки** содержит свойства, используемые для отмены подписки.</span><span class="sxs-lookup"><span data-stu-id="8ec32-104">The **Unsubscribe** element contains the properties used to unsubscribe from a subscription.</span></span> 
  
[<span data-ttu-id="8ec32-105">Отписаться</span><span class="sxs-lookup"><span data-stu-id="8ec32-105">Unsubscribe</span></span>](unsubscribe.md)
  
```xml
<Unsubscribe>
   <SubscriptionId/>
</Unsubscribe>
```

 <span data-ttu-id="8ec32-106">**UnsubscribeType**</span><span class="sxs-lookup"><span data-stu-id="8ec32-106">**UnsubscribeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8ec32-107">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="8ec32-107">Attributes and elements</span></span>

<span data-ttu-id="8ec32-108">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="8ec32-108">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8ec32-109">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="8ec32-109">Attributes</span></span>

<span data-ttu-id="8ec32-110">Нет.</span><span class="sxs-lookup"><span data-stu-id="8ec32-110">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8ec32-111">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="8ec32-111">Child elements</span></span>

|<span data-ttu-id="8ec32-112">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="8ec32-112">**Element**</span></span>|<span data-ttu-id="8ec32-113">**Описание**</span><span class="sxs-lookup"><span data-stu-id="8ec32-113">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8ec32-114">SubscriptionId (GetEvents)</span><span class="sxs-lookup"><span data-stu-id="8ec32-114">SubscriptionId (GetEvents)</span></span>](subscriptionid-getevents.md) <br/> |<span data-ttu-id="8ec32-115">Представляет идентификатор для подписки.</span><span class="sxs-lookup"><span data-stu-id="8ec32-115">Represents the identifier for a subscription.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="8ec32-116">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="8ec32-116">Parent elements</span></span>

<span data-ttu-id="8ec32-117">Нет.</span><span class="sxs-lookup"><span data-stu-id="8ec32-117">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="8ec32-118">Замечания</span><span class="sxs-lookup"><span data-stu-id="8ec32-118">Remarks</span></span>

<span data-ttu-id="8ec32-119">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="8ec32-119">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8ec32-120">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="8ec32-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8ec32-121">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="8ec32-121">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="8ec32-122">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="8ec32-122">Schema name</span></span>  <br/> |<span data-ttu-id="8ec32-123">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="8ec32-123">Messages schema</span></span>  <br/> |
|<span data-ttu-id="8ec32-124">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="8ec32-124">Validation file</span></span>  <br/> |<span data-ttu-id="8ec32-125">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="8ec32-125">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="8ec32-126">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="8ec32-126">Can be empty</span></span>  <br/> |<span data-ttu-id="8ec32-127">False</span><span class="sxs-lookup"><span data-stu-id="8ec32-127">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="8ec32-128">См. также</span><span class="sxs-lookup"><span data-stu-id="8ec32-128">See also</span></span>



[<span data-ttu-id="8ec32-129">Операции подписки</span><span class="sxs-lookup"><span data-stu-id="8ec32-129">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="8ec32-130">Операция GetEvents</span><span class="sxs-lookup"><span data-stu-id="8ec32-130">GetEvents operation</span></span>](getevents-operation.md)
  
[<span data-ttu-id="8ec32-131">Отписаться операции</span><span class="sxs-lookup"><span data-stu-id="8ec32-131">Unsubscribe operation</span></span>](unsubscribe-operation.md)

