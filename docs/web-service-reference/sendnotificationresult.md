---
title: сенднотификатионресулт
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SendNotificationResult
api_type:
- schema
ms.assetid: fa9d6202-fa66-4f10-9858-53f4f1ce14bc
description: Элемент Сенднотификатионресулт содержит ответ клиентского приложения на push-уведомление.
ms.openlocfilehash: 9acaa396430cf4e06a9c996834874d19dcab50ac
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835350"
---
# <a name="sendnotificationresult"></a><span data-ttu-id="e4e24-103">сенднотификатионресулт</span><span class="sxs-lookup"><span data-stu-id="e4e24-103">SendNotificationResult</span></span>

<span data-ttu-id="e4e24-104">Элемент **сенднотификатионресулт** содержит ответ клиентского приложения на push-уведомление.</span><span class="sxs-lookup"><span data-stu-id="e4e24-104">The **SendNotificationResult** element contains the response of a client application to a push notification.</span></span> 
  
```xml
<SendNotificationResult>
   <SubscriptionStatus/>
</SendNotificationResult>
```

 <span data-ttu-id="e4e24-105">**сенднотификатионресулттипе**</span><span class="sxs-lookup"><span data-stu-id="e4e24-105">**SendNotificationResultType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e4e24-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="e4e24-106">Attributes and elements</span></span>

<span data-ttu-id="e4e24-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="e4e24-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e4e24-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="e4e24-108">Attributes</span></span>

<span data-ttu-id="e4e24-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="e4e24-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e4e24-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="e4e24-110">Child elements</span></span>

|<span data-ttu-id="e4e24-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="e4e24-111">**Element**</span></span>|<span data-ttu-id="e4e24-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="e4e24-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e4e24-113">SubscriptionStatus</span><span class="sxs-lookup"><span data-stu-id="e4e24-113">SubscriptionStatus</span></span>](subscriptionstatus.md) <br/> |<span data-ttu-id="e4e24-114">Описывает состояние принудительной подписки.</span><span class="sxs-lookup"><span data-stu-id="e4e24-114">Describes the status of a push subscription.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="e4e24-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="e4e24-115">Parent elements</span></span>

<span data-ttu-id="e4e24-116">Нет.</span><span class="sxs-lookup"><span data-stu-id="e4e24-116">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="e4e24-117">Примечания</span><span class="sxs-lookup"><span data-stu-id="e4e24-117">Remarks</span></span>

<span data-ttu-id="e4e24-118">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="e4e24-118">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e4e24-119">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="e4e24-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e4e24-120">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="e4e24-120">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="e4e24-121">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="e4e24-121">Schema Name</span></span>  <br/> |<span data-ttu-id="e4e24-122">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="e4e24-122">Messages schema</span></span>  <br/> |
|<span data-ttu-id="e4e24-123">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="e4e24-123">Validation File</span></span>  <br/> |<span data-ttu-id="e4e24-124">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="e4e24-124">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="e4e24-125">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="e4e24-125">Can be Empty</span></span>  <br/> |<span data-ttu-id="e4e24-126">False</span><span class="sxs-lookup"><span data-stu-id="e4e24-126">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e4e24-127">См. также</span><span class="sxs-lookup"><span data-stu-id="e4e24-127">See also</span></span>



- [<span data-ttu-id="e4e24-128">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="e4e24-128">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

