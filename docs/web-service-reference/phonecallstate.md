---
title: фонекаллстате
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
description: Элемент Фонекаллстате указывает текущее состояние телефонного звонка.
ms.openlocfilehash: d2088b9b2811befe80684188d49c8034c577cc55
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44468532"
---
# <a name="phonecallstate"></a><span data-ttu-id="f4be0-103">фонекаллстате</span><span class="sxs-lookup"><span data-stu-id="f4be0-103">PhoneCallState</span></span>

<span data-ttu-id="f4be0-104">Элемент **фонекаллстате** указывает текущее состояние телефонного звонка.</span><span class="sxs-lookup"><span data-stu-id="f4be0-104">The **PhoneCallState** element specifies the current state for a phone call.</span></span> 
  
```xml
<PhoneCallState>Idle or Connecting or Alerted or Connected or Disconnected or Incoming or Transferring or Forwarding</PhoneCallState>
```

 <span data-ttu-id="f4be0-105">**фонекаллстатетипе**</span><span class="sxs-lookup"><span data-stu-id="f4be0-105">**PhoneCallStateType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f4be0-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="f4be0-106">Attributes and elements</span></span>

<span data-ttu-id="f4be0-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="f4be0-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f4be0-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="f4be0-108">Attributes</span></span>

<span data-ttu-id="f4be0-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="f4be0-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f4be0-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="f4be0-110">Child elements</span></span>

<span data-ttu-id="f4be0-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="f4be0-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="f4be0-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="f4be0-112">Parent elements</span></span>

|<span data-ttu-id="f4be0-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="f4be0-113">**Element**</span></span>|<span data-ttu-id="f4be0-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="f4be0-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f4be0-115">фонекаллинформатион</span><span class="sxs-lookup"><span data-stu-id="f4be0-115">PhoneCallInformation</span></span>](phonecallinformation.md) <br/> |<span data-ttu-id="f4be0-116">Задает сведения о состоянии для телефонного звонка.</span><span class="sxs-lookup"><span data-stu-id="f4be0-116">Specifies the state information for a phone call.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="f4be0-117">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="f4be0-117">Text value</span></span>

<span data-ttu-id="f4be0-118">В следующей таблице приведены возможные значения для элемента **фонекаллстате** .</span><span class="sxs-lookup"><span data-stu-id="f4be0-118">The following table lists the possible values for the **PhoneCallState** element.</span></span> 
  
<span data-ttu-id="f4be0-119">**Значения элементов Фонекаллстате**</span><span class="sxs-lookup"><span data-stu-id="f4be0-119">**PhoneCallState element values**</span></span>

|<span data-ttu-id="f4be0-120">**Значение**</span><span class="sxs-lookup"><span data-stu-id="f4be0-120">**Value**</span></span>|<span data-ttu-id="f4be0-121">**Описание**</span><span class="sxs-lookup"><span data-stu-id="f4be0-121">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="f4be0-122">Простоя</span><span class="sxs-lookup"><span data-stu-id="f4be0-122">Idle</span></span>  <br/> |<span data-ttu-id="f4be0-123">Начальное состояние вызова.</span><span class="sxs-lookup"><span data-stu-id="f4be0-123">Initial call state.</span></span>  <br/> |
|<span data-ttu-id="f4be0-124">Connecting</span><span class="sxs-lookup"><span data-stu-id="f4be0-124">Connecting</span></span>  <br/> |<span data-ttu-id="f4be0-125">Система набирает этот вызов.</span><span class="sxs-lookup"><span data-stu-id="f4be0-125">The system is dialing this call.</span></span>  <br/> |
|<span data-ttu-id="f4be0-126">Предупрежден</span><span class="sxs-lookup"><span data-stu-id="f4be0-126">Alerted</span></span>  <br/> |<span data-ttu-id="f4be0-127">Вызов находится в состоянии оповещения (телефонный звонок).</span><span class="sxs-lookup"><span data-stu-id="f4be0-127">The call is in alerting state (phone is ringing).</span></span>  <br/> |
|<span data-ttu-id="f4be0-128">Подключено</span><span class="sxs-lookup"><span data-stu-id="f4be0-128">Connected</span></span>  <br/> |<span data-ttu-id="f4be0-129">Вызов находится в подключенном состоянии.</span><span class="sxs-lookup"><span data-stu-id="f4be0-129">The call is in the connected state.</span></span>  <br/> |
|<span data-ttu-id="f4be0-130">Отключено</span><span class="sxs-lookup"><span data-stu-id="f4be0-130">Disconnected</span></span>  <br/> |<span data-ttu-id="f4be0-131">Вызов отключается.</span><span class="sxs-lookup"><span data-stu-id="f4be0-131">The call is disconnected.</span></span>  <br/> |
|<span data-ttu-id="f4be0-132">Входящее</span><span class="sxs-lookup"><span data-stu-id="f4be0-132">Incoming</span></span>  <br/> |<span data-ttu-id="f4be0-133">Вызов является входящим.</span><span class="sxs-lookup"><span data-stu-id="f4be0-133">The call is inbound.</span></span>  <br/> |
|<span data-ttu-id="f4be0-134">Мещают</span><span class="sxs-lookup"><span data-stu-id="f4be0-134">Transferring</span></span>  <br/> |<span data-ttu-id="f4be0-135">Вызов передается в другой целевой объект.</span><span class="sxs-lookup"><span data-stu-id="f4be0-135">The call is being transferred to another destination.</span></span>  <br/> |
|<span data-ttu-id="f4be0-136">Сообщений</span><span class="sxs-lookup"><span data-stu-id="f4be0-136">Forwarding</span></span>  <br/> |<span data-ttu-id="f4be0-137">Вызов перенаправляется в другую точку назначения.</span><span class="sxs-lookup"><span data-stu-id="f4be0-137">The call is being forwarded to another destination.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="f4be0-138">Примечания</span><span class="sxs-lookup"><span data-stu-id="f4be0-138">Remarks</span></span>

<span data-ttu-id="f4be0-139">Схема, описывающая этот элемент, находится в каталоге/ЕВС/компьютера под управлением Microsoft Exchange Server 2010, на котором установлена роль сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="f4be0-139">The schema that describes this element is located in the /ews/ directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f4be0-140">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="f4be0-140">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f4be0-141">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="f4be0-141">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f4be0-142">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="f4be0-142">Schema Name</span></span>  <br/> |<span data-ttu-id="f4be0-143">Схема Types</span><span class="sxs-lookup"><span data-stu-id="f4be0-143">Types schema</span></span>  <br/> |
|<span data-ttu-id="f4be0-144">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="f4be0-144">Validation File</span></span>  <br/> |<span data-ttu-id="f4be0-145">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="f4be0-145">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="f4be0-146">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="f4be0-146">Can be Empty</span></span>  <br/> |<span data-ttu-id="f4be0-147">False</span><span class="sxs-lookup"><span data-stu-id="f4be0-147">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f4be0-148">См. также</span><span class="sxs-lookup"><span data-stu-id="f4be0-148">See also</span></span>



- [<span data-ttu-id="f4be0-149">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="f4be0-149">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

