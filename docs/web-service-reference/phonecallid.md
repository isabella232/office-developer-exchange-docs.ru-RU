---
title: фонекаллид
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
description: Элемент Фонекаллид указывает идентификатор телефонного звонка. Этот элемент обязательный.
ms.openlocfilehash: 1886d9510fe254c016779166efccc9882fd77d2c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834757"
---
# <a name="phonecallid"></a><span data-ttu-id="f4fd7-104">фонекаллид</span><span class="sxs-lookup"><span data-stu-id="f4fd7-104">PhoneCallId</span></span>

<span data-ttu-id="f4fd7-105">Элемент **фонекаллид** указывает идентификатор телефонного звонка.</span><span class="sxs-lookup"><span data-stu-id="f4fd7-105">The **PhoneCallId** element specifies the identifier of a phone call.</span></span> <span data-ttu-id="f4fd7-106">Этот элемент обязательный.</span><span class="sxs-lookup"><span data-stu-id="f4fd7-106">This element is required.</span></span> 
  
```xml
<PhoneCallId Id="" />
```

 <span data-ttu-id="f4fd7-107">**фонекаллидтипе**</span><span class="sxs-lookup"><span data-stu-id="f4fd7-107">**PhoneCallIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f4fd7-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="f4fd7-108">Attributes and elements</span></span>

<span data-ttu-id="f4fd7-109">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="f4fd7-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f4fd7-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="f4fd7-110">Attributes</span></span>

|<span data-ttu-id="f4fd7-111">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="f4fd7-111">**Attribute**</span></span>|<span data-ttu-id="f4fd7-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="f4fd7-112">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="f4fd7-113">Id</span><span class="sxs-lookup"><span data-stu-id="f4fd7-113">Id</span></span>  <br/> |<span data-ttu-id="f4fd7-114">Определяет телефонный звонок для отключения.</span><span class="sxs-lookup"><span data-stu-id="f4fd7-114">Identifies the phone call to disconnect.</span></span> <span data-ttu-id="f4fd7-115">Этот атрибут является обязательным.</span><span class="sxs-lookup"><span data-stu-id="f4fd7-115">This attribute is required.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="f4fd7-116">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="f4fd7-116">Child elements</span></span>

<span data-ttu-id="f4fd7-117">Нет.</span><span class="sxs-lookup"><span data-stu-id="f4fd7-117">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="f4fd7-118">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="f4fd7-118">Parent elements</span></span>

|<span data-ttu-id="f4fd7-119">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="f4fd7-119">**Element**</span></span>|<span data-ttu-id="f4fd7-120">**Описание**</span><span class="sxs-lookup"><span data-stu-id="f4fd7-120">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f4fd7-121">DisconnectPhoneCall</span><span class="sxs-lookup"><span data-stu-id="f4fd7-121">DisconnectPhoneCall</span></span>](disconnectphonecall.md) <br/> |<span data-ttu-id="f4fd7-122">Представляет запрос на отключение вызова.</span><span class="sxs-lookup"><span data-stu-id="f4fd7-122">Represents a request to disconnect a call.</span></span>  <br/> |
|[<span data-ttu-id="f4fd7-123">GetPhoneCallInformation</span><span class="sxs-lookup"><span data-stu-id="f4fd7-123">GetPhoneCallInformation</span></span>](getphonecallinformation.md) <br/> |<span data-ttu-id="f4fd7-124">Представляет запрос на получение сведений о телефонном звонке.</span><span class="sxs-lookup"><span data-stu-id="f4fd7-124">Represents a request to get telephone call information.</span></span>  <br/> |
|[<span data-ttu-id="f4fd7-125">PlayOnPhoneResponse (веб-службы Exchange)</span><span class="sxs-lookup"><span data-stu-id="f4fd7-125">PlayOnPhoneResponse (Exchange Web Services)</span></span>](playonphoneresponse-exchange-web-services.md) <br/> |<span data-ttu-id="f4fd7-126">Определяет ответ на запрос PlayOnPhone.</span><span class="sxs-lookup"><span data-stu-id="f4fd7-126">Defines a response to a PlayOnPhone request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="f4fd7-127">Примечания</span><span class="sxs-lookup"><span data-stu-id="f4fd7-127">Remarks</span></span>

<span data-ttu-id="f4fd7-128">Схема, описывающая этот элемент, находится в виртуальном каталоге EWS компьютера под управлением Microsoft Exchange Server 2010, на котором установлена роль сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="f4fd7-128">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f4fd7-129">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="f4fd7-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f4fd7-130">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="f4fd7-130">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="f4fd7-131">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="f4fd7-131">Schema Name</span></span>  <br/> |<span data-ttu-id="f4fd7-132">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="f4fd7-132">Messages schema</span></span>  <br/> |
|<span data-ttu-id="f4fd7-133">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="f4fd7-133">Validation File</span></span>  <br/> |<span data-ttu-id="f4fd7-134">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="f4fd7-134">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="f4fd7-135">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="f4fd7-135">Can be Empty</span></span>  <br/> |<span data-ttu-id="f4fd7-136">False</span><span class="sxs-lookup"><span data-stu-id="f4fd7-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f4fd7-137">См. также</span><span class="sxs-lookup"><span data-stu-id="f4fd7-137">See also</span></span>



- [<span data-ttu-id="f4fd7-138">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="f4fd7-138">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

