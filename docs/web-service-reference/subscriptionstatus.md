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
ms.lasthandoff: 06/25/2018
ms.locfileid: "19840107"
---
# <a name="subscriptionstatus"></a><span data-ttu-id="7d9b7-103">SubscriptionStatus</span><span class="sxs-lookup"><span data-stu-id="7d9b7-103">SubscriptionStatus</span></span>

<span data-ttu-id="7d9b7-104">Элемент **SubscriptionStatus** описывает состояние принудительной подписки.</span><span class="sxs-lookup"><span data-stu-id="7d9b7-104">The **SubscriptionStatus** element describes the status of a push subscription.</span></span> 
  
```xml
<SubscriptionStatus>OK or Unsubscribe</SubscriptionStatus>
```

 <span data-ttu-id="7d9b7-105">**субскриптионстатустипе**</span><span class="sxs-lookup"><span data-stu-id="7d9b7-105">**SubscriptionStatusType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7d9b7-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="7d9b7-106">Attributes and elements</span></span>

<span data-ttu-id="7d9b7-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="7d9b7-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7d9b7-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="7d9b7-108">Attributes</span></span>

<span data-ttu-id="7d9b7-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="7d9b7-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7d9b7-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="7d9b7-110">Child elements</span></span>

<span data-ttu-id="7d9b7-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="7d9b7-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="7d9b7-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="7d9b7-112">Parent elements</span></span>

|<span data-ttu-id="7d9b7-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="7d9b7-113">**Element**</span></span>|<span data-ttu-id="7d9b7-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="7d9b7-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7d9b7-115">сенднотификатионресулт</span><span class="sxs-lookup"><span data-stu-id="7d9b7-115">SendNotificationResult</span></span>](sendnotificationresult.md) <br/> |<span data-ttu-id="7d9b7-116">Содержит ответ клиентского приложения на push-уведомления.</span><span class="sxs-lookup"><span data-stu-id="7d9b7-116">Contains the response of the client application' to a push notification.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="7d9b7-117">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="7d9b7-117">Text value</span></span>

<span data-ttu-id="7d9b7-118">Необходимо указать текстовое значение.</span><span class="sxs-lookup"><span data-stu-id="7d9b7-118">A text value is required.</span></span> <span data-ttu-id="7d9b7-119">Ниже приведены возможные текстовые значения для этого элемента:</span><span class="sxs-lookup"><span data-stu-id="7d9b7-119">The following are the possible text values for this element:</span></span>
  
- <span data-ttu-id="7d9b7-120">OK</span><span class="sxs-lookup"><span data-stu-id="7d9b7-120">OK</span></span>
    
- <span data-ttu-id="7d9b7-121">Отмена подписки</span><span class="sxs-lookup"><span data-stu-id="7d9b7-121">Unsubscribe</span></span>
    
## <a name="remarks"></a><span data-ttu-id="7d9b7-122">Примечания</span><span class="sxs-lookup"><span data-stu-id="7d9b7-122">Remarks</span></span>

<span data-ttu-id="7d9b7-123">Этот элемент описывает состояние подписки.</span><span class="sxs-lookup"><span data-stu-id="7d9b7-123">This element describes the status of the subscription.</span></span> <span data-ttu-id="7d9b7-124">Клиентское приложение принудительной подписки отправляет состояние на компьютер, на котором выполняется Exchange 2007, на котором установлена роль сервера клиентского доступа после каждого push-уведомления.</span><span class="sxs-lookup"><span data-stu-id="7d9b7-124">The push subscription client application sends the status back to the computer that is running Exchange 2007 that has the Client Access server role installed after each push notification.</span></span> <span data-ttu-id="7d9b7-125">Если значение **SubscriptionStatus** равно **Unsubscribe**, сервер клиентского доступа прекратит отправку уведомлений и завершит подписку.</span><span class="sxs-lookup"><span data-stu-id="7d9b7-125">If the **SubscriptionStatus** value equals **Unsubscribe**, the Client Access server will stop sending notifications and end the subscription.</span></span> <span data-ttu-id="7d9b7-126">Если значение **SubscriptionStatus** равно **ОК**, сервер клиентского доступа продолжит отправлять уведомления.</span><span class="sxs-lookup"><span data-stu-id="7d9b7-126">If the **SubscriptionStatus** value equals **OK**, the Client Access server will continue to send notifications.</span></span>
  
<span data-ttu-id="7d9b7-127">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="7d9b7-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7d9b7-128">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="7d9b7-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7d9b7-129">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="7d9b7-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="7d9b7-130">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="7d9b7-130">Schema Name</span></span>  <br/> |<span data-ttu-id="7d9b7-131">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="7d9b7-131">Messages schema</span></span>  <br/> |
|<span data-ttu-id="7d9b7-132">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="7d9b7-132">Validation File</span></span>  <br/> |<span data-ttu-id="7d9b7-133">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="7d9b7-133">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="7d9b7-134">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="7d9b7-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="7d9b7-135">False</span><span class="sxs-lookup"><span data-stu-id="7d9b7-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7d9b7-136">См. также</span><span class="sxs-lookup"><span data-stu-id="7d9b7-136">See also</span></span>



- [<span data-ttu-id="7d9b7-137">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="7d9b7-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

