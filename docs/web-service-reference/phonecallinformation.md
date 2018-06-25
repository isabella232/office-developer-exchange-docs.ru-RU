---
title: PhoneCallInformation
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- PhoneCallInformation
api_type:
- schema
ms.assetid: a0363c42-6d35-4074-bc17-946eb12736ff
description: Элемент PhoneCallInformation определяет сведения о состоянии для телефонного звонка.
ms.openlocfilehash: e64e7b38b3801c60df8a966e95d980746533d3a4
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834758"
---
# <a name="phonecallinformation"></a><span data-ttu-id="54de6-103">PhoneCallInformation</span><span class="sxs-lookup"><span data-stu-id="54de6-103">PhoneCallInformation</span></span>

<span data-ttu-id="54de6-104">Элемент **PhoneCallInformation** определяет сведения о состоянии для телефонного звонка.</span><span class="sxs-lookup"><span data-stu-id="54de6-104">The **PhoneCallInformation** element specifies the state information for a phone call.</span></span> 
  
```XML
<PhoneCallInformation>
   <PhoneCallState/>
   <ConnectionFailureCause/>
   <SIPResponseText/>
   <SIPResponseCode/>
</PhoneCallInformation>
```

 <span data-ttu-id="54de6-105">**PhoneCallInformationType**</span><span class="sxs-lookup"><span data-stu-id="54de6-105">**PhoneCallInformationType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="54de6-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="54de6-106">Attributes and elements</span></span>

<span data-ttu-id="54de6-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="54de6-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="54de6-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="54de6-108">Attributes</span></span>

<span data-ttu-id="54de6-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="54de6-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="54de6-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="54de6-110">Child elements</span></span>

|<span data-ttu-id="54de6-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="54de6-111">**Element**</span></span>|<span data-ttu-id="54de6-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="54de6-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="54de6-113">PhoneCallState</span><span class="sxs-lookup"><span data-stu-id="54de6-113">PhoneCallState</span></span>](phonecallstate.md) <br/> |<span data-ttu-id="54de6-114">Указывает состояние для телефонного звонка.</span><span class="sxs-lookup"><span data-stu-id="54de6-114">Specifies the state for a phone call.</span></span> <span data-ttu-id="54de6-115">Этот элемент обязательный.</span><span class="sxs-lookup"><span data-stu-id="54de6-115">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="54de6-116">ConnectionFailureCause</span><span class="sxs-lookup"><span data-stu-id="54de6-116">ConnectionFailureCause</span></span>](connectionfailurecause.md) <br/> |<span data-ttu-id="54de6-117">Указывает причину сбоя подключения.</span><span class="sxs-lookup"><span data-stu-id="54de6-117">Specifies the cause of a connection failure.</span></span> <span data-ttu-id="54de6-118">Этот элемент обязательный.</span><span class="sxs-lookup"><span data-stu-id="54de6-118">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="54de6-119">SIPResponseText</span><span class="sxs-lookup"><span data-stu-id="54de6-119">SIPResponseText</span></span>](sipresponsetext.md) <br/> |<span data-ttu-id="54de6-120">Задает текст ответа SIP.</span><span class="sxs-lookup"><span data-stu-id="54de6-120">Specifies the SIP response text.</span></span> <span data-ttu-id="54de6-121">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="54de6-121">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="54de6-122">SIPResponseCode</span><span class="sxs-lookup"><span data-stu-id="54de6-122">SIPResponseCode</span></span>](sipresponsecode.md) <br/> |<span data-ttu-id="54de6-123">Задает код ответа SIP.</span><span class="sxs-lookup"><span data-stu-id="54de6-123">Specifies the SIP response code.</span></span> <span data-ttu-id="54de6-124">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="54de6-124">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="54de6-125">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="54de6-125">Parent elements</span></span>

|<span data-ttu-id="54de6-126">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="54de6-126">**Element**</span></span>|<span data-ttu-id="54de6-127">**Описание**</span><span class="sxs-lookup"><span data-stu-id="54de6-127">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="54de6-128">GetPhoneCallInformationResponse</span><span class="sxs-lookup"><span data-stu-id="54de6-128">GetPhoneCallInformationResponse</span></span>](getphonecallinformationresponse.md) <br/> |<span data-ttu-id="54de6-129">Определяет ответ на запрос [GetPhoneCallInformation операции](getphonecallinformation-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="54de6-129">Defines a response to a [GetPhoneCallInformation operation](getphonecallinformation-operation.md) request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="54de6-130">Замечания</span><span class="sxs-lookup"><span data-stu-id="54de6-130">Remarks</span></span>

<span data-ttu-id="54de6-131">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="54de6-131">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="54de6-132">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="54de6-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="54de6-133">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="54de6-133">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="54de6-134">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="54de6-134">Schema Name</span></span>  <br/> |<span data-ttu-id="54de6-135">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="54de6-135">Messages schema</span></span>  <br/> |
|<span data-ttu-id="54de6-136">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="54de6-136">Validation File</span></span>  <br/> |<span data-ttu-id="54de6-137">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="54de6-137">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="54de6-138">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="54de6-138">Can be Empty</span></span>  <br/> |<span data-ttu-id="54de6-139">False</span><span class="sxs-lookup"><span data-stu-id="54de6-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="54de6-140">См. также</span><span class="sxs-lookup"><span data-stu-id="54de6-140">See also</span></span>



- [<span data-ttu-id="54de6-141">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="54de6-141">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

