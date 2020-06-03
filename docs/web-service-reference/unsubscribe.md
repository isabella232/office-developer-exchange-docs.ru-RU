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
description: Элемент unsubscribe содержит свойства, которые используются для отмены подписки на подписку.
ms.openlocfilehash: d3d9c3bf9ad97cc0fdabf574c6505c797583838a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467216"
---
# <a name="unsubscribe"></a><span data-ttu-id="60cc5-103">Отмена подписки</span><span class="sxs-lookup"><span data-stu-id="60cc5-103">Unsubscribe</span></span>

<span data-ttu-id="60cc5-104">Элемент **Unsubscribe** содержит свойства, которые используются для отмены подписки на подписку.</span><span class="sxs-lookup"><span data-stu-id="60cc5-104">The **Unsubscribe** element contains the properties used to unsubscribe from a subscription.</span></span> 
  
[<span data-ttu-id="60cc5-105">Отмена подписки</span><span class="sxs-lookup"><span data-stu-id="60cc5-105">Unsubscribe</span></span>](unsubscribe.md)
  
```xml
<Unsubscribe>
   <SubscriptionId/>
</Unsubscribe>
```

 <span data-ttu-id="60cc5-106">**унсубскрибетипе**</span><span class="sxs-lookup"><span data-stu-id="60cc5-106">**UnsubscribeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="60cc5-107">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="60cc5-107">Attributes and elements</span></span>

<span data-ttu-id="60cc5-108">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="60cc5-108">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="60cc5-109">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="60cc5-109">Attributes</span></span>

<span data-ttu-id="60cc5-110">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="60cc5-110">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="60cc5-111">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="60cc5-111">Child elements</span></span>

|<span data-ttu-id="60cc5-112">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="60cc5-112">**Element**</span></span>|<span data-ttu-id="60cc5-113">**Описание**</span><span class="sxs-lookup"><span data-stu-id="60cc5-113">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="60cc5-114">SubscriptionId (Events)</span><span class="sxs-lookup"><span data-stu-id="60cc5-114">SubscriptionId (GetEvents)</span></span>](subscriptionid-getevents.md) <br/> |<span data-ttu-id="60cc5-115">Представляет идентификатор подписки.</span><span class="sxs-lookup"><span data-stu-id="60cc5-115">Represents the identifier for a subscription.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="60cc5-116">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="60cc5-116">Parent elements</span></span>

<span data-ttu-id="60cc5-117">Нет.</span><span class="sxs-lookup"><span data-stu-id="60cc5-117">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="60cc5-118">Примечания</span><span class="sxs-lookup"><span data-stu-id="60cc5-118">Remarks</span></span>

<span data-ttu-id="60cc5-119">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="60cc5-119">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="60cc5-120">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="60cc5-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="60cc5-121">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="60cc5-121">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="60cc5-122">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="60cc5-122">Schema name</span></span>  <br/> |<span data-ttu-id="60cc5-123">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="60cc5-123">Messages schema</span></span>  <br/> |
|<span data-ttu-id="60cc5-124">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="60cc5-124">Validation file</span></span>  <br/> |<span data-ttu-id="60cc5-125">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="60cc5-125">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="60cc5-126">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="60cc5-126">Can be empty</span></span>  <br/> |<span data-ttu-id="60cc5-127">False</span><span class="sxs-lookup"><span data-stu-id="60cc5-127">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="60cc5-128">См. также</span><span class="sxs-lookup"><span data-stu-id="60cc5-128">See also</span></span>



[<span data-ttu-id="60cc5-129">Операции подписки</span><span class="sxs-lookup"><span data-stu-id="60cc5-129">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="60cc5-130">Операция GetEvents</span><span class="sxs-lookup"><span data-stu-id="60cc5-130">GetEvents operation</span></span>](getevents-operation.md)
  
[<span data-ttu-id="60cc5-131">Операция по отмене подписки</span><span class="sxs-lookup"><span data-stu-id="60cc5-131">Unsubscribe operation</span></span>](unsubscribe-operation.md)

