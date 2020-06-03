---
title: DisconnectPhoneCall
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DisconnectPhoneCall
api_type:
- schema
ms.assetid: f9252536-9852-4dd9-9ebc-91f5cf281171
description: Элемент DisconnectPhoneCall представляет запрос на отключение вызова.
ms.openlocfilehash: 8d64ecb9dce1d8b7efcebc70686db8fcbf867217
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529709"
---
# <a name="disconnectphonecall"></a><span data-ttu-id="175b6-103">DisconnectPhoneCall</span><span class="sxs-lookup"><span data-stu-id="175b6-103">DisconnectPhoneCall</span></span>

<span data-ttu-id="175b6-104">Элемент **DisconnectPhoneCall** представляет запрос на отключение вызова.</span><span class="sxs-lookup"><span data-stu-id="175b6-104">The **DisconnectPhoneCall** element represents a request to disconnect a call.</span></span> 
  
```xml
<DisconnectPhoneCall>
   <PhoneCallId/>
</DisconnectPhoneCall>
```

 <span data-ttu-id="175b6-105">**дисконнектфонекаллтипе**</span><span class="sxs-lookup"><span data-stu-id="175b6-105">**DisconnectPhoneCallType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="175b6-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="175b6-106">Attributes and elements</span></span>

<span data-ttu-id="175b6-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="175b6-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="175b6-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="175b6-108">Attributes</span></span>

<span data-ttu-id="175b6-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="175b6-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="175b6-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="175b6-110">Child elements</span></span>

|<span data-ttu-id="175b6-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="175b6-111">**Element**</span></span>|<span data-ttu-id="175b6-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="175b6-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="175b6-113">фонекаллид</span><span class="sxs-lookup"><span data-stu-id="175b6-113">PhoneCallId</span></span>](phonecallid.md) <br/> |<span data-ttu-id="175b6-114">Задает идентификатор вызова для отключения.</span><span class="sxs-lookup"><span data-stu-id="175b6-114">Specifies the identifier of the call to disconnect.</span></span> <span data-ttu-id="175b6-115">Этот элемент обязательный.</span><span class="sxs-lookup"><span data-stu-id="175b6-115">This element is required.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="175b6-116">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="175b6-116">Parent elements</span></span>

<span data-ttu-id="175b6-117">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="175b6-117">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="175b6-118">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="175b6-118">Text value</span></span>

<span data-ttu-id="175b6-119">Нет.</span><span class="sxs-lookup"><span data-stu-id="175b6-119">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="175b6-120">Примечания</span><span class="sxs-lookup"><span data-stu-id="175b6-120">Remarks</span></span>

<span data-ttu-id="175b6-121">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="175b6-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="175b6-122">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="175b6-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="175b6-123">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="175b6-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="175b6-124">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="175b6-124">Schema Name</span></span>  <br/> |<span data-ttu-id="175b6-125">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="175b6-125">Messages schema</span></span>  <br/> |
|<span data-ttu-id="175b6-126">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="175b6-126">Validation File</span></span>  <br/> |<span data-ttu-id="175b6-127">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="175b6-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="175b6-128">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="175b6-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="175b6-129">False</span><span class="sxs-lookup"><span data-stu-id="175b6-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="175b6-130">См. также</span><span class="sxs-lookup"><span data-stu-id="175b6-130">See also</span></span>

- [<span data-ttu-id="175b6-131">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="175b6-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

