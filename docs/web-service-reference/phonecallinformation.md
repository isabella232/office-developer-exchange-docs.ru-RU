---
title: фонекаллинформатион
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
description: Элемент Фонекаллинформатион указывает сведения о состоянии телефонного звонка.
ms.openlocfilehash: 75370bccb841818a8302bdd055ad96fd16b2e8df
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44468847"
---
# <a name="phonecallinformation"></a><span data-ttu-id="78b50-103">фонекаллинформатион</span><span class="sxs-lookup"><span data-stu-id="78b50-103">PhoneCallInformation</span></span>

<span data-ttu-id="78b50-104">Элемент **фонекаллинформатион** указывает сведения о состоянии телефонного звонка.</span><span class="sxs-lookup"><span data-stu-id="78b50-104">The **PhoneCallInformation** element specifies the state information for a phone call.</span></span> 
  
```XML
<PhoneCallInformation>
   <PhoneCallState/>
   <ConnectionFailureCause/>
   <SIPResponseText/>
   <SIPResponseCode/>
</PhoneCallInformation>
```

 <span data-ttu-id="78b50-105">**фонекаллинформатионтипе**</span><span class="sxs-lookup"><span data-stu-id="78b50-105">**PhoneCallInformationType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="78b50-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="78b50-106">Attributes and elements</span></span>

<span data-ttu-id="78b50-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="78b50-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="78b50-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="78b50-108">Attributes</span></span>

<span data-ttu-id="78b50-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="78b50-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="78b50-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="78b50-110">Child elements</span></span>

|<span data-ttu-id="78b50-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="78b50-111">**Element**</span></span>|<span data-ttu-id="78b50-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="78b50-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="78b50-113">фонекаллстате</span><span class="sxs-lookup"><span data-stu-id="78b50-113">PhoneCallState</span></span>](phonecallstate.md) <br/> |<span data-ttu-id="78b50-114">Указывает состояние телефонного звонка.</span><span class="sxs-lookup"><span data-stu-id="78b50-114">Specifies the state for a phone call.</span></span> <span data-ttu-id="78b50-115">Этот элемент обязательный.</span><span class="sxs-lookup"><span data-stu-id="78b50-115">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="78b50-116">коннектионфаилурекаусе</span><span class="sxs-lookup"><span data-stu-id="78b50-116">ConnectionFailureCause</span></span>](connectionfailurecause.md) <br/> |<span data-ttu-id="78b50-117">Указывает причину сбоя подключения.</span><span class="sxs-lookup"><span data-stu-id="78b50-117">Specifies the cause of a connection failure.</span></span> <span data-ttu-id="78b50-118">Этот элемент обязательный.</span><span class="sxs-lookup"><span data-stu-id="78b50-118">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="78b50-119">сипреспонсетекст</span><span class="sxs-lookup"><span data-stu-id="78b50-119">SIPResponseText</span></span>](sipresponsetext.md) <br/> |<span data-ttu-id="78b50-120">Задает текст ответа SIP.</span><span class="sxs-lookup"><span data-stu-id="78b50-120">Specifies the SIP response text.</span></span> <span data-ttu-id="78b50-121">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="78b50-121">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="78b50-122">сипреспонсекоде</span><span class="sxs-lookup"><span data-stu-id="78b50-122">SIPResponseCode</span></span>](sipresponsecode.md) <br/> |<span data-ttu-id="78b50-123">Задает код ответа SIP.</span><span class="sxs-lookup"><span data-stu-id="78b50-123">Specifies the SIP response code.</span></span> <span data-ttu-id="78b50-124">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="78b50-124">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="78b50-125">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="78b50-125">Parent elements</span></span>

|<span data-ttu-id="78b50-126">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="78b50-126">**Element**</span></span>|<span data-ttu-id="78b50-127">**Описание**</span><span class="sxs-lookup"><span data-stu-id="78b50-127">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="78b50-128">жетфонекаллинформатионреспонсе</span><span class="sxs-lookup"><span data-stu-id="78b50-128">GetPhoneCallInformationResponse</span></span>](getphonecallinformationresponse.md) <br/> |<span data-ttu-id="78b50-129">Определяет ответ на запрос [операции GetPhoneCallInformation](getphonecallinformation-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="78b50-129">Defines a response to a [GetPhoneCallInformation operation](getphonecallinformation-operation.md) request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="78b50-130">Примечания</span><span class="sxs-lookup"><span data-stu-id="78b50-130">Remarks</span></span>

<span data-ttu-id="78b50-131">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="78b50-131">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="78b50-132">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="78b50-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="78b50-133">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="78b50-133">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="78b50-134">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="78b50-134">Schema Name</span></span>  <br/> |<span data-ttu-id="78b50-135">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="78b50-135">Messages schema</span></span>  <br/> |
|<span data-ttu-id="78b50-136">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="78b50-136">Validation File</span></span>  <br/> |<span data-ttu-id="78b50-137">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="78b50-137">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="78b50-138">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="78b50-138">Can be Empty</span></span>  <br/> |<span data-ttu-id="78b50-139">False</span><span class="sxs-lookup"><span data-stu-id="78b50-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="78b50-140">См. также</span><span class="sxs-lookup"><span data-stu-id="78b50-140">See also</span></span>



- [<span data-ttu-id="78b50-141">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="78b50-141">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

