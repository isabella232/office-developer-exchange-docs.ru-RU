---
title: SubscriptionStatus
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SubscriptionStatus
api_type:
- schema
ms.assetid: 2d64ebb7-f26a-4d02-b7ef-d9d7da75f0c3
description: Элемент SubscriptionStatus описывает состояние принудительной подписки.
ms.openlocfilehash: 1f6de15f7a3b07714899aef2ff74a8d556f8ca1d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19840107"
---
# <a name="subscriptionstatus"></a><span data-ttu-id="adebc-103">SubscriptionStatus</span><span class="sxs-lookup"><span data-stu-id="adebc-103">SubscriptionStatus</span></span>

<span data-ttu-id="adebc-104">Элемент **SubscriptionStatus** описывает состояние принудительной подписки.</span><span class="sxs-lookup"><span data-stu-id="adebc-104">The **SubscriptionStatus** element describes the status of a push subscription.</span></span> 
  
```xml
<SubscriptionStatus>OK or Unsubscribe</SubscriptionStatus>
```

 <span data-ttu-id="adebc-105">**SubscriptionStatusType**</span><span class="sxs-lookup"><span data-stu-id="adebc-105">**SubscriptionStatusType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="adebc-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="adebc-106">Attributes and elements</span></span>

<span data-ttu-id="adebc-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="adebc-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="adebc-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="adebc-108">Attributes</span></span>

<span data-ttu-id="adebc-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="adebc-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="adebc-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="adebc-110">Child elements</span></span>

<span data-ttu-id="adebc-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="adebc-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="adebc-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="adebc-112">Parent elements</span></span>

|<span data-ttu-id="adebc-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="adebc-113">**Element**</span></span>|<span data-ttu-id="adebc-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="adebc-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="adebc-115">SendNotificationResult</span><span class="sxs-lookup"><span data-stu-id="adebc-115">SendNotificationResult</span></span>](sendnotificationresult.md) <br/> |<span data-ttu-id="adebc-116">Содержит ответ в клиентском приложении "для push-уведомлений.</span><span class="sxs-lookup"><span data-stu-id="adebc-116">Contains the response of the client application' to a push notification.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="adebc-117">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="adebc-117">Text value</span></span>

<span data-ttu-id="adebc-118">Текстовое значение является обязательным.</span><span class="sxs-lookup"><span data-stu-id="adebc-118">A text value is required.</span></span> <span data-ttu-id="adebc-119">Ниже приведены возможные значения для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="adebc-119">The following are the possible text values for this element:</span></span>
  
- <span data-ttu-id="adebc-120">OK</span><span class="sxs-lookup"><span data-stu-id="adebc-120">OK</span></span>
    
- <span data-ttu-id="adebc-121">Отмена подписки</span><span class="sxs-lookup"><span data-stu-id="adebc-121">Unsubscribe</span></span>
    
## <a name="remarks"></a><span data-ttu-id="adebc-122">Замечания</span><span class="sxs-lookup"><span data-stu-id="adebc-122">Remarks</span></span>

<span data-ttu-id="adebc-123">В этом элементе представлено описание состояния подписки.</span><span class="sxs-lookup"><span data-stu-id="adebc-123">This element describes the status of the subscription.</span></span> <span data-ttu-id="adebc-124">Клиентское приложение подписки push отправляет состояние на компьютер, на котором работает Exchange 2007, который имеет роль сервера клиентского доступа, установленные после каждого push-уведомлений.</span><span class="sxs-lookup"><span data-stu-id="adebc-124">The push subscription client application sends the status back to the computer that is running Exchange 2007 that has the Client Access server role installed after each push notification.</span></span> <span data-ttu-id="adebc-125">Если значение **SubscriptionStatus** равно **отказа от подписки**, сервер клиентского доступа Остановить отправку уведомлений и end подписки.</span><span class="sxs-lookup"><span data-stu-id="adebc-125">If the **SubscriptionStatus** value equals **Unsubscribe**, the Client Access server will stop sending notifications and end the subscription.</span></span> <span data-ttu-id="adebc-126">Если значение **SubscriptionStatus** равно **ОК**, сервер клиентского доступа будет продолжать отправлять уведомления.</span><span class="sxs-lookup"><span data-stu-id="adebc-126">If the **SubscriptionStatus** value equals **OK**, the Client Access server will continue to send notifications.</span></span>
  
<span data-ttu-id="adebc-127">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="adebc-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="adebc-128">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="adebc-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="adebc-129">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="adebc-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="adebc-130">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="adebc-130">Schema Name</span></span>  <br/> |<span data-ttu-id="adebc-131">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="adebc-131">Messages schema</span></span>  <br/> |
|<span data-ttu-id="adebc-132">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="adebc-132">Validation File</span></span>  <br/> |<span data-ttu-id="adebc-133">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="adebc-133">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="adebc-134">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="adebc-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="adebc-135">False</span><span class="sxs-lookup"><span data-stu-id="adebc-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="adebc-136">См. также</span><span class="sxs-lookup"><span data-stu-id="adebc-136">See also</span></span>



- [<span data-ttu-id="adebc-137">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="adebc-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

