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
ms.openlocfilehash: 56947ea9ba56c76bb02d6a425ff43b3b846a2f60
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762137"
---
# <a name="disconnectphonecall"></a><span data-ttu-id="e9273-103">DisconnectPhoneCall</span><span class="sxs-lookup"><span data-stu-id="e9273-103">DisconnectPhoneCall</span></span>

<span data-ttu-id="e9273-104">Элемент **DisconnectPhoneCall** представляет запрос на отключение вызова.</span><span class="sxs-lookup"><span data-stu-id="e9273-104">The **DisconnectPhoneCall** element represents a request to disconnect a call.</span></span> 
  
```xml
<DisconnectPhoneCall>
   <PhoneCallId/>
</DisconnectPhoneCall>
```

 <span data-ttu-id="e9273-105">**DisconnectPhoneCallType**</span><span class="sxs-lookup"><span data-stu-id="e9273-105">**DisconnectPhoneCallType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e9273-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="e9273-106">Attributes and elements</span></span>

<span data-ttu-id="e9273-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="e9273-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e9273-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="e9273-108">Attributes</span></span>

<span data-ttu-id="e9273-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="e9273-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e9273-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="e9273-110">Child elements</span></span>

|<span data-ttu-id="e9273-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="e9273-111">**Element**</span></span>|<span data-ttu-id="e9273-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="e9273-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e9273-113">PhoneCallId</span><span class="sxs-lookup"><span data-stu-id="e9273-113">PhoneCallId</span></span>](phonecallid.md) <br/> |<span data-ttu-id="e9273-114">Задает идентификатор звонка для отключения.</span><span class="sxs-lookup"><span data-stu-id="e9273-114">Specifies the identifier of the call to disconnect.</span></span> <span data-ttu-id="e9273-115">Этот элемент обязательный.</span><span class="sxs-lookup"><span data-stu-id="e9273-115">This element is required.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="e9273-116">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="e9273-116">Parent elements</span></span>

<span data-ttu-id="e9273-117">Нет.</span><span class="sxs-lookup"><span data-stu-id="e9273-117">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="e9273-118">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="e9273-118">Text value</span></span>

<span data-ttu-id="e9273-119">Нет.</span><span class="sxs-lookup"><span data-stu-id="e9273-119">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="e9273-120">Замечания</span><span class="sxs-lookup"><span data-stu-id="e9273-120">Remarks</span></span>

<span data-ttu-id="e9273-121">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="e9273-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e9273-122">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="e9273-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e9273-123">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="e9273-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="e9273-124">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="e9273-124">Schema Name</span></span>  <br/> |<span data-ttu-id="e9273-125">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="e9273-125">Messages schema</span></span>  <br/> |
|<span data-ttu-id="e9273-126">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="e9273-126">Validation File</span></span>  <br/> |<span data-ttu-id="e9273-127">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="e9273-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="e9273-128">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="e9273-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="e9273-129">False</span><span class="sxs-lookup"><span data-stu-id="e9273-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e9273-130">См. также</span><span class="sxs-lookup"><span data-stu-id="e9273-130">See also</span></span>

- [<span data-ttu-id="e9273-131">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="e9273-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
