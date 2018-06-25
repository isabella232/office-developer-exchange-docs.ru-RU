---
title: PhoneCallId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- PhoneCallId
api_type:
- schema
ms.assetid: 79e31a4c-fc84-4802-8761-470df8d63694
description: Элемент PhoneCallId указывает идентификатор телефонного звонка. Этот элемент обязательный.
ms.openlocfilehash: 1886d9510fe254c016779166efccc9882fd77d2c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834757"
---
# <a name="phonecallid"></a><span data-ttu-id="b7279-104">PhoneCallId</span><span class="sxs-lookup"><span data-stu-id="b7279-104">PhoneCallId</span></span>

<span data-ttu-id="b7279-105">Элемент **PhoneCallId** указывает идентификатор телефонного звонка.</span><span class="sxs-lookup"><span data-stu-id="b7279-105">The **PhoneCallId** element specifies the identifier of a phone call.</span></span> <span data-ttu-id="b7279-106">Этот элемент обязательный.</span><span class="sxs-lookup"><span data-stu-id="b7279-106">This element is required.</span></span> 
  
```xml
<PhoneCallId Id="" />
```

 <span data-ttu-id="b7279-107">**PhoneCallIdType**</span><span class="sxs-lookup"><span data-stu-id="b7279-107">**PhoneCallIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b7279-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="b7279-108">Attributes and elements</span></span>

<span data-ttu-id="b7279-109">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="b7279-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b7279-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="b7279-110">Attributes</span></span>

|<span data-ttu-id="b7279-111">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="b7279-111">**Attribute**</span></span>|<span data-ttu-id="b7279-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="b7279-112">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="b7279-113">Id</span><span class="sxs-lookup"><span data-stu-id="b7279-113">Id</span></span>  <br/> |<span data-ttu-id="b7279-114">Определяет телефонный звонок для отключения.</span><span class="sxs-lookup"><span data-stu-id="b7279-114">Identifies the phone call to disconnect.</span></span> <span data-ttu-id="b7279-115">Этот атрибут является обязательным.</span><span class="sxs-lookup"><span data-stu-id="b7279-115">This attribute is required.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="b7279-116">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="b7279-116">Child elements</span></span>

<span data-ttu-id="b7279-117">Нет.</span><span class="sxs-lookup"><span data-stu-id="b7279-117">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="b7279-118">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="b7279-118">Parent elements</span></span>

|<span data-ttu-id="b7279-119">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="b7279-119">**Element**</span></span>|<span data-ttu-id="b7279-120">**Описание**</span><span class="sxs-lookup"><span data-stu-id="b7279-120">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b7279-121">DisconnectPhoneCall</span><span class="sxs-lookup"><span data-stu-id="b7279-121">DisconnectPhoneCall</span></span>](disconnectphonecall.md) <br/> |<span data-ttu-id="b7279-122">Представляет запрос на отключение вызова.</span><span class="sxs-lookup"><span data-stu-id="b7279-122">Represents a request to disconnect a call.</span></span>  <br/> |
|[<span data-ttu-id="b7279-123">GetPhoneCallInformation</span><span class="sxs-lookup"><span data-stu-id="b7279-123">GetPhoneCallInformation</span></span>](getphonecallinformation.md) <br/> |<span data-ttu-id="b7279-124">Представляет запрос на получение сведений о телефонный звонок.</span><span class="sxs-lookup"><span data-stu-id="b7279-124">Represents a request to get telephone call information.</span></span>  <br/> |
|[<span data-ttu-id="b7279-125">PlayOnPhoneResponse (веб-служб Exchange)</span><span class="sxs-lookup"><span data-stu-id="b7279-125">PlayOnPhoneResponse (Exchange Web Services)</span></span>](playonphoneresponse-exchange-web-services.md) <br/> |<span data-ttu-id="b7279-126">Определяет ответ на запрос PlayOnPhone.</span><span class="sxs-lookup"><span data-stu-id="b7279-126">Defines a response to a PlayOnPhone request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="b7279-127">Замечания</span><span class="sxs-lookup"><span data-stu-id="b7279-127">Remarks</span></span>

<span data-ttu-id="b7279-128">Схема, описывающая этот элемент находится в виртуальном каталоге EWS компьютера, на котором выполняется Microsoft Exchange Server 2010 с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="b7279-128">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b7279-129">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="b7279-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b7279-130">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="b7279-130">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="b7279-131">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="b7279-131">Schema Name</span></span>  <br/> |<span data-ttu-id="b7279-132">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="b7279-132">Messages schema</span></span>  <br/> |
|<span data-ttu-id="b7279-133">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="b7279-133">Validation File</span></span>  <br/> |<span data-ttu-id="b7279-134">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="b7279-134">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="b7279-135">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="b7279-135">Can be Empty</span></span>  <br/> |<span data-ttu-id="b7279-136">False</span><span class="sxs-lookup"><span data-stu-id="b7279-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b7279-137">См. также</span><span class="sxs-lookup"><span data-stu-id="b7279-137">See also</span></span>



- [<span data-ttu-id="b7279-138">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="b7279-138">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

