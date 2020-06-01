---
title: Уведомления
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Notifications
api_type:
- schema
ms.assetid: 153cc420-d2fe-42f1-afb2-9a31ee09a750
description: Элемент Notifications содержит массив сведений о подписке и событиях, произошедших с момента последнего уведомления.
ms.openlocfilehash: 88fc56ba6e672e3dea7a1d31f7cc1fda018b9a15
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462621"
---
# <a name="notifications"></a><span data-ttu-id="2c3c1-103">Уведомления</span><span class="sxs-lookup"><span data-stu-id="2c3c1-103">Notifications</span></span>

<span data-ttu-id="2c3c1-104">Элемент **Notifications** содержит массив сведений о подписке и событиях, произошедших с момента последнего уведомления.</span><span class="sxs-lookup"><span data-stu-id="2c3c1-104">The **Notifications** element contains an array of information about the subscription and the events that have occurred since the last notification.</span></span> 
  
```xml
<Notifications>
   <Notification/>
</Notifications>
```

 <span data-ttu-id="2c3c1-105">**нонемптяррайофнотификатионстипе**</span><span class="sxs-lookup"><span data-stu-id="2c3c1-105">**NonEmptyArrayOfNotificationsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2c3c1-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="2c3c1-106">Attributes and elements</span></span>

<span data-ttu-id="2c3c1-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="2c3c1-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2c3c1-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="2c3c1-108">Attributes</span></span>

<span data-ttu-id="2c3c1-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="2c3c1-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2c3c1-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="2c3c1-110">Child elements</span></span>

|<span data-ttu-id="2c3c1-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="2c3c1-111">**Element**</span></span>|<span data-ttu-id="2c3c1-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="2c3c1-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2c3c1-113">Уведомление</span><span class="sxs-lookup"><span data-stu-id="2c3c1-113">Notification</span></span>](notification-ex15websvcsotherref.md) <br/> |<span data-ttu-id="2c3c1-114">Содержит сведения о подписке и событиях, произошедших с момента последнего уведомления.</span><span class="sxs-lookup"><span data-stu-id="2c3c1-114">Contains information about the subscription and the events that have occurred since the last notification.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="2c3c1-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="2c3c1-115">Parent elements</span></span>

|<span data-ttu-id="2c3c1-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="2c3c1-116">**Element**</span></span>|<span data-ttu-id="2c3c1-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="2c3c1-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2c3c1-118">жетстреаминжевентсреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="2c3c1-118">GetStreamingEventsResponseMessage</span></span>](getstreamingeventsresponsemessage.md) <br/> |<span data-ttu-id="2c3c1-119">Содержит состояние и результат одного запроса [операции GetStreamingEvents](getstreamingevents-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="2c3c1-119">Contains the status and result of a single [GetStreamingEvents operation](getstreamingevents-operation.md) request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="2c3c1-120">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="2c3c1-120">Text value</span></span>

<span data-ttu-id="2c3c1-121">Нет.</span><span class="sxs-lookup"><span data-stu-id="2c3c1-121">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="2c3c1-122">Примечания</span><span class="sxs-lookup"><span data-stu-id="2c3c1-122">Remarks</span></span>

<span data-ttu-id="2c3c1-123">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.Этот элемент появился в Exchange Server 2010 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="2c3c1-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2c3c1-124">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="2c3c1-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2c3c1-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="2c3c1-125">Namespace</span></span>  <br/> |<span data-ttu-id="2c3c1-126">https://schemas.microsoft.com/exchange/services/2006/messages и https://schemas.microsoft.com/exchange/services/2006/types</span><span class="sxs-lookup"><span data-stu-id="2c3c1-126">https://schemas.microsoft.com/exchange/services/2006/messages and https://schemas.microsoft.com/exchange/services/2006/types</span></span>  <br/> |
|<span data-ttu-id="2c3c1-127">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="2c3c1-127">Schema Name</span></span>  <br/> |<span data-ttu-id="2c3c1-128">Схема сообщений; Схема Types</span><span class="sxs-lookup"><span data-stu-id="2c3c1-128">Messages schema; Types schema</span></span>  <br/> |
|<span data-ttu-id="2c3c1-129">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="2c3c1-129">Validation File</span></span>  <br/> |<span data-ttu-id="2c3c1-130">Messages. xsd; Types. xsd</span><span class="sxs-lookup"><span data-stu-id="2c3c1-130">Messages.xsd; Types.xsd</span></span>  <br/> |
|<span data-ttu-id="2c3c1-131">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="2c3c1-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="2c3c1-132">False</span><span class="sxs-lookup"><span data-stu-id="2c3c1-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="2c3c1-133">См. также</span><span class="sxs-lookup"><span data-stu-id="2c3c1-133">See also</span></span>



[<span data-ttu-id="2c3c1-134">Операция GetFolder</span><span class="sxs-lookup"><span data-stu-id="2c3c1-134">GetFolder operation</span></span>](getfolder-operation.md)
  
[<span data-ttu-id="2c3c1-135">Операция DeleteFolder</span><span class="sxs-lookup"><span data-stu-id="2c3c1-135">DeleteFolder operation</span></span>](deletefolder-operation.md)
  
[<span data-ttu-id="2c3c1-136">Операция MoveFolder</span><span class="sxs-lookup"><span data-stu-id="2c3c1-136">MoveFolder operation</span></span>](movefolder-operation.md)
  
[<span data-ttu-id="2c3c1-137">Операция CopyFolder</span><span class="sxs-lookup"><span data-stu-id="2c3c1-137">CopyFolder operation</span></span>](copyfolder-operation.md)
  
[<span data-ttu-id="2c3c1-138">Операции подписки</span><span class="sxs-lookup"><span data-stu-id="2c3c1-138">Subscribe operation</span></span>](subscribe-operation.md)

