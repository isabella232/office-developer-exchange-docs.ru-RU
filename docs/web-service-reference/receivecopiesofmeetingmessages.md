---
title: рецеивекопиесофмитингмессажес
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ReceiveCopiesOfMeetingMessages
api_type:
- schema
ms.assetid: 65217ca8-6aea-47eb-a989-e6cce25f5f09
description: Элемент Рецеивекопиесофмитингмессажес указывает, получает ли делегат копии сообщений, связанных с собранием, которые адресованы участнику. Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).
ms.openlocfilehash: e39a5d3255268b418fa956959da5ae0ea062d831
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834967"
---
# <a name="receivecopiesofmeetingmessages"></a><span data-ttu-id="84668-104">рецеивекопиесофмитингмессажес</span><span class="sxs-lookup"><span data-stu-id="84668-104">ReceiveCopiesOfMeetingMessages</span></span>

<span data-ttu-id="84668-105">Элемент **рецеивекопиесофмитингмессажес** указывает, получает ли делегат копии сообщений, связанных с собранием, которые адресованы участнику.</span><span class="sxs-lookup"><span data-stu-id="84668-105">The **ReceiveCopiesOfMeetingMessages** element indicates whether a delegate receives copies of meeting-related messages that are addressed to the principal.</span></span> <span data-ttu-id="84668-106">Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="84668-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<ReceiveCopiesOfMeetingMessages>true or false</ReceiveCopiesOfMeetingMessages>
```

 <span data-ttu-id="84668-107">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="84668-107">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="84668-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="84668-108">Attributes and elements</span></span>

<span data-ttu-id="84668-109">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="84668-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="84668-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="84668-110">Attributes</span></span>

<span data-ttu-id="84668-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="84668-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="84668-112">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="84668-112">Child elements</span></span>

<span data-ttu-id="84668-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="84668-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="84668-114">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="84668-114">Parent elements</span></span>

|<span data-ttu-id="84668-115">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="84668-115">**Element**</span></span>|<span data-ttu-id="84668-116">**Описание**</span><span class="sxs-lookup"><span data-stu-id="84668-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="84668-117">делегатеусер</span><span class="sxs-lookup"><span data-stu-id="84668-117">DelegateUser</span></span>](delegateuser.md) <br/> |<span data-ttu-id="84668-118">Определяет одного делегата для добавления или обновления в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="84668-118">Identifies a single delegate to add or update in a mailbox.</span></span> <span data-ttu-id="84668-119">Этот элемент появился в Exchange 2007 с пакетом обновления 1.</span><span class="sxs-lookup"><span data-stu-id="84668-119">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="84668-120">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="84668-120">Text value</span></span>

<span data-ttu-id="84668-121">Текстовое значение **true** указывает на то, что делегат получает копию сообщений о собраниях.</span><span class="sxs-lookup"><span data-stu-id="84668-121">A text value of **true** indicates that a delegate receives a copy of meeting messages.</span></span> <span data-ttu-id="84668-122">Текстовое значение **false** указывает, что делегат не получает копии сообщений о собраниях.</span><span class="sxs-lookup"><span data-stu-id="84668-122">A text value of **false** indicates that a delegate does not receive a copy of meeting messages.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="84668-123">Примечания</span><span class="sxs-lookup"><span data-stu-id="84668-123">Remarks</span></span>

<span data-ttu-id="84668-124">Если для **рецеивекопиесофмитингмессажес** задано **значение false**, делегат по-прежнему может отправлять сообщения от имени субъекта, но не будет получать сообщения, связанные с собраниями.</span><span class="sxs-lookup"><span data-stu-id="84668-124">When **ReceiveCopiesOfMeetingMessages** is set to **false**, the delegate can still send message on behalf of the principal, but will not receive any meeting-related messages.</span></span>
  
<span data-ttu-id="84668-125">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="84668-125">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="84668-126">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="84668-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="84668-127">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="84668-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="84668-128">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="84668-128">Schema Name</span></span>  <br/> |<span data-ttu-id="84668-129">Схема Types</span><span class="sxs-lookup"><span data-stu-id="84668-129">Types schema</span></span>  <br/> |
|<span data-ttu-id="84668-130">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="84668-130">Validation File</span></span>  <br/> |<span data-ttu-id="84668-131">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="84668-131">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="84668-132">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="84668-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="84668-133">False</span><span class="sxs-lookup"><span data-stu-id="84668-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="84668-134">См. также</span><span class="sxs-lookup"><span data-stu-id="84668-134">See also</span></span>



[<span data-ttu-id="84668-135">Операция AddDelegate</span><span class="sxs-lookup"><span data-stu-id="84668-135">AddDelegate operation</span></span>](adddelegate-operation.md)
  
[<span data-ttu-id="84668-136">Операция UpdateDelegate</span><span class="sxs-lookup"><span data-stu-id="84668-136">UpdateDelegate operation</span></span>](updatedelegate-operation.md)


- [<span data-ttu-id="84668-137">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="84668-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="84668-138">Добавление делегатов</span><span class="sxs-lookup"><span data-stu-id="84668-138">Adding Delegates</span></span>](http://msdn.microsoft.com/library/3a744150-66a3-4a13-9433-793603ba5038%28Office.15%29.aspx)

