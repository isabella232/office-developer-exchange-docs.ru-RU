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
ms.openlocfilehash: 3e4b9dba5e8be6e45a0c16508531fbc6cf91c170
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459702"
---
# <a name="phonecallid"></a><span data-ttu-id="67edf-104">фонекаллид</span><span class="sxs-lookup"><span data-stu-id="67edf-104">PhoneCallId</span></span>

<span data-ttu-id="67edf-105">Элемент **фонекаллид** указывает идентификатор телефонного звонка.</span><span class="sxs-lookup"><span data-stu-id="67edf-105">The **PhoneCallId** element specifies the identifier of a phone call.</span></span> <span data-ttu-id="67edf-106">Этот элемент обязательный.</span><span class="sxs-lookup"><span data-stu-id="67edf-106">This element is required.</span></span> 
  
```xml
<PhoneCallId Id="" />
```

 <span data-ttu-id="67edf-107">**фонекаллидтипе**</span><span class="sxs-lookup"><span data-stu-id="67edf-107">**PhoneCallIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="67edf-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="67edf-108">Attributes and elements</span></span>

<span data-ttu-id="67edf-109">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="67edf-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="67edf-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="67edf-110">Attributes</span></span>

|<span data-ttu-id="67edf-111">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="67edf-111">**Attribute**</span></span>|<span data-ttu-id="67edf-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="67edf-112">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="67edf-113">Id</span><span class="sxs-lookup"><span data-stu-id="67edf-113">Id</span></span>  <br/> |<span data-ttu-id="67edf-114">Определяет телефонный звонок для отключения.</span><span class="sxs-lookup"><span data-stu-id="67edf-114">Identifies the phone call to disconnect.</span></span> <span data-ttu-id="67edf-115">Этот атрибут является обязательным.</span><span class="sxs-lookup"><span data-stu-id="67edf-115">This attribute is required.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="67edf-116">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="67edf-116">Child elements</span></span>

<span data-ttu-id="67edf-117">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="67edf-117">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="67edf-118">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="67edf-118">Parent elements</span></span>

|<span data-ttu-id="67edf-119">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="67edf-119">**Element**</span></span>|<span data-ttu-id="67edf-120">**Описание**</span><span class="sxs-lookup"><span data-stu-id="67edf-120">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="67edf-121">DisconnectPhoneCall</span><span class="sxs-lookup"><span data-stu-id="67edf-121">DisconnectPhoneCall</span></span>](disconnectphonecall.md) <br/> |<span data-ttu-id="67edf-122">Представляет запрос на отключение вызова.</span><span class="sxs-lookup"><span data-stu-id="67edf-122">Represents a request to disconnect a call.</span></span>  <br/> |
|[<span data-ttu-id="67edf-123">GetPhoneCallInformation</span><span class="sxs-lookup"><span data-stu-id="67edf-123">GetPhoneCallInformation</span></span>](getphonecallinformation.md) <br/> |<span data-ttu-id="67edf-124">Представляет запрос на получение сведений о телефонном звонке.</span><span class="sxs-lookup"><span data-stu-id="67edf-124">Represents a request to get telephone call information.</span></span>  <br/> |
|[<span data-ttu-id="67edf-125">PlayOnPhoneResponse (веб-службы Exchange)</span><span class="sxs-lookup"><span data-stu-id="67edf-125">PlayOnPhoneResponse (Exchange Web Services)</span></span>](playonphoneresponse-exchange-web-services.md) <br/> |<span data-ttu-id="67edf-126">Определяет ответ на запрос PlayOnPhone.</span><span class="sxs-lookup"><span data-stu-id="67edf-126">Defines a response to a PlayOnPhone request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="67edf-127">Примечания</span><span class="sxs-lookup"><span data-stu-id="67edf-127">Remarks</span></span>

<span data-ttu-id="67edf-128">Схема, описывающая этот элемент, находится в виртуальном каталоге EWS компьютера под управлением Microsoft Exchange Server 2010, на котором установлена роль сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="67edf-128">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="67edf-129">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="67edf-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="67edf-130">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="67edf-130">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="67edf-131">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="67edf-131">Schema Name</span></span>  <br/> |<span data-ttu-id="67edf-132">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="67edf-132">Messages schema</span></span>  <br/> |
|<span data-ttu-id="67edf-133">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="67edf-133">Validation File</span></span>  <br/> |<span data-ttu-id="67edf-134">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="67edf-134">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="67edf-135">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="67edf-135">Can be Empty</span></span>  <br/> |<span data-ttu-id="67edf-136">False</span><span class="sxs-lookup"><span data-stu-id="67edf-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="67edf-137">См. также</span><span class="sxs-lookup"><span data-stu-id="67edf-137">See also</span></span>



- [<span data-ttu-id="67edf-138">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="67edf-138">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

