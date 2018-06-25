---
title: PhoneCallState
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- PhoneCallState
api_type:
- schema
ms.assetid: ac009eb3-6334-49ce-82be-48fe83577f9c
description: Элемент PhoneCallState указывает текущее состояние телефонного звонка.
ms.openlocfilehash: 184a7400810711442e565d1ef37094bd63b00914
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834761"
---
# <a name="phonecallstate"></a><span data-ttu-id="f1e1c-103">PhoneCallState</span><span class="sxs-lookup"><span data-stu-id="f1e1c-103">PhoneCallState</span></span>

<span data-ttu-id="f1e1c-104">Элемент **PhoneCallState** указывает текущее состояние телефонного звонка.</span><span class="sxs-lookup"><span data-stu-id="f1e1c-104">The **PhoneCallState** element specifies the current state for a phone call.</span></span> 
  
```xml
<PhoneCallState>Idle or Connecting or Alerted or Connected or Disconnected or Incoming or Transferring or Forwarding</PhoneCallState>
```

 <span data-ttu-id="f1e1c-105">**PhoneCallStateType**</span><span class="sxs-lookup"><span data-stu-id="f1e1c-105">**PhoneCallStateType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f1e1c-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="f1e1c-106">Attributes and elements</span></span>

<span data-ttu-id="f1e1c-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="f1e1c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f1e1c-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="f1e1c-108">Attributes</span></span>

<span data-ttu-id="f1e1c-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="f1e1c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f1e1c-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="f1e1c-110">Child elements</span></span>

<span data-ttu-id="f1e1c-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="f1e1c-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="f1e1c-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="f1e1c-112">Parent elements</span></span>

|<span data-ttu-id="f1e1c-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="f1e1c-113">**Element**</span></span>|<span data-ttu-id="f1e1c-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="f1e1c-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f1e1c-115">PhoneCallInformation</span><span class="sxs-lookup"><span data-stu-id="f1e1c-115">PhoneCallInformation</span></span>](phonecallinformation.md) <br/> |<span data-ttu-id="f1e1c-116">Задает сведения о состоянии для телефонного звонка.</span><span class="sxs-lookup"><span data-stu-id="f1e1c-116">Specifies the state information for a phone call.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="f1e1c-117">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="f1e1c-117">Text value</span></span>

<span data-ttu-id="f1e1c-118">В следующей таблице приведены возможные значения для элемента **PhoneCallState** .</span><span class="sxs-lookup"><span data-stu-id="f1e1c-118">The following table lists the possible values for the **PhoneCallState** element.</span></span> 
  
<span data-ttu-id="f1e1c-119">**Значения элементов PhoneCallState**</span><span class="sxs-lookup"><span data-stu-id="f1e1c-119">**PhoneCallState element values**</span></span>

|<span data-ttu-id="f1e1c-120">**Значение**</span><span class="sxs-lookup"><span data-stu-id="f1e1c-120">**Value**</span></span>|<span data-ttu-id="f1e1c-121">**Описание**</span><span class="sxs-lookup"><span data-stu-id="f1e1c-121">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="f1e1c-122">Простоя</span><span class="sxs-lookup"><span data-stu-id="f1e1c-122">Idle</span></span>  <br/> |<span data-ttu-id="f1e1c-123">Состояние первого вызова.</span><span class="sxs-lookup"><span data-stu-id="f1e1c-123">Initial call state.</span></span>  <br/> |
|<span data-ttu-id="f1e1c-124">Подключение</span><span class="sxs-lookup"><span data-stu-id="f1e1c-124">Connecting</span></span>  <br/> |<span data-ttu-id="f1e1c-125">Система — это набору номера, этот вызов.</span><span class="sxs-lookup"><span data-stu-id="f1e1c-125">The system is dialing this call.</span></span>  <br/> |
|<span data-ttu-id="f1e1c-126">Оповещения</span><span class="sxs-lookup"><span data-stu-id="f1e1c-126">Alerted</span></span>  <br/> |<span data-ttu-id="f1e1c-127">Вызов выполнен в элемент интерфейса, предупреждающий состояние (телефонных звонков).</span><span class="sxs-lookup"><span data-stu-id="f1e1c-127">The call is in alerting state (phone is ringing).</span></span>  <br/> |
|<span data-ttu-id="f1e1c-128">Подключено</span><span class="sxs-lookup"><span data-stu-id="f1e1c-128">Connected</span></span>  <br/> |<span data-ttu-id="f1e1c-129">Вызов выполнен в состояние подключения.</span><span class="sxs-lookup"><span data-stu-id="f1e1c-129">The call is in the connected state.</span></span>  <br/> |
|<span data-ttu-id="f1e1c-130">Отключено</span><span class="sxs-lookup"><span data-stu-id="f1e1c-130">Disconnected</span></span>  <br/> |<span data-ttu-id="f1e1c-131">Вызов разъединен.</span><span class="sxs-lookup"><span data-stu-id="f1e1c-131">The call is disconnected.</span></span>  <br/> |
|<span data-ttu-id="f1e1c-132">Входящая</span><span class="sxs-lookup"><span data-stu-id="f1e1c-132">Incoming</span></span>  <br/> |<span data-ttu-id="f1e1c-133">Входящий звонок.</span><span class="sxs-lookup"><span data-stu-id="f1e1c-133">The call is inbound.</span></span>  <br/> |
|<span data-ttu-id="f1e1c-134">Передача</span><span class="sxs-lookup"><span data-stu-id="f1e1c-134">Transferring</span></span>  <br/> |<span data-ttu-id="f1e1c-135">Звонок переводится другому получателю.</span><span class="sxs-lookup"><span data-stu-id="f1e1c-135">The call is being transferred to another destination.</span></span>  <br/> |
|<span data-ttu-id="f1e1c-136">Переадресация</span><span class="sxs-lookup"><span data-stu-id="f1e1c-136">Forwarding</span></span>  <br/> |<span data-ttu-id="f1e1c-137">Переадресация звонка другому получателю.</span><span class="sxs-lookup"><span data-stu-id="f1e1c-137">The call is being forwarded to another destination.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="f1e1c-138">Замечания</span><span class="sxs-lookup"><span data-stu-id="f1e1c-138">Remarks</span></span>

<span data-ttu-id="f1e1c-139">Схема, описывающая этот элемент находится в каталоге /ews/ компьютера, на котором выполняется Microsoft Exchange Server 2010 с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="f1e1c-139">The schema that describes this element is located in the /ews/ directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f1e1c-140">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="f1e1c-140">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f1e1c-141">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="f1e1c-141">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f1e1c-142">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="f1e1c-142">Schema Name</span></span>  <br/> |<span data-ttu-id="f1e1c-143">Схема Types</span><span class="sxs-lookup"><span data-stu-id="f1e1c-143">Types schema</span></span>  <br/> |
|<span data-ttu-id="f1e1c-144">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="f1e1c-144">Validation File</span></span>  <br/> |<span data-ttu-id="f1e1c-145">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="f1e1c-145">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="f1e1c-146">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="f1e1c-146">Can be Empty</span></span>  <br/> |<span data-ttu-id="f1e1c-147">False</span><span class="sxs-lookup"><span data-stu-id="f1e1c-147">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f1e1c-148">См. также</span><span class="sxs-lookup"><span data-stu-id="f1e1c-148">See also</span></span>



- [<span data-ttu-id="f1e1c-149">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="f1e1c-149">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

