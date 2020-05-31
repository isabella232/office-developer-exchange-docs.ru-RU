---
title: фромаддрессес
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FromAddresses
api_type:
- schema
ms.assetid: b219f315-c20a-4633-af3e-94bd3e4526b6
description: Элемент Фромаддрессес указывает адреса электронной почты, из которых должны отправляться входящие сообщения, чтобы применялось условие или исключение.
ms.openlocfilehash: 40ecb1f3e16ad961b8e4c38d5aa9d15f4f74469a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762664"
---
# <a name="fromaddresses"></a><span data-ttu-id="87333-103">фромаддрессес</span><span class="sxs-lookup"><span data-stu-id="87333-103">FromAddresses</span></span>

<span data-ttu-id="87333-104">Элемент **фромаддрессес** указывает адреса электронной почты, из которых должны отправляться входящие сообщения, чтобы применялось условие или исключение.</span><span class="sxs-lookup"><span data-stu-id="87333-104">The **FromAddresses** element indicates the e-mail addresses from which incoming messages must be sent in order for the condition or exception to apply.</span></span> 
  
```XML
<FromAddresses>
   <Address/>
</FromAddresses>
```

 <span data-ttu-id="87333-105">**аррайофемаиладдрессестипе**</span><span class="sxs-lookup"><span data-stu-id="87333-105">**ArrayOfEmailAddressesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="87333-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="87333-106">Attributes and elements</span></span>

<span data-ttu-id="87333-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="87333-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="87333-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="87333-108">Attributes</span></span>

<span data-ttu-id="87333-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="87333-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="87333-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="87333-110">Child elements</span></span>

|<span data-ttu-id="87333-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="87333-111">**Element**</span></span>|<span data-ttu-id="87333-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="87333-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="87333-113">Адрес (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="87333-113">Address (EmailAddressType)</span></span>](address-emailaddresstype.md) <br/> |<span data-ttu-id="87333-114">Представляет адрес электронной почты полностью разрешенной.</span><span class="sxs-lookup"><span data-stu-id="87333-114">Represents a fully resolved e-mail address.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="87333-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="87333-115">Parent elements</span></span>

|<span data-ttu-id="87333-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="87333-116">**Element**</span></span>|<span data-ttu-id="87333-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="87333-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="87333-118">Условия</span><span class="sxs-lookup"><span data-stu-id="87333-118">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="87333-119">Представляет условия, которые, если удовлетворены, запускают действия правила для правила.</span><span class="sxs-lookup"><span data-stu-id="87333-119">Represents the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span>  <br/> |
|[<span data-ttu-id="87333-120">Исключения</span><span class="sxs-lookup"><span data-stu-id="87333-120">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="87333-121">Представляет все доступные условия исключения правила для правила папки "Входящие".</span><span class="sxs-lookup"><span data-stu-id="87333-121">Represents all the available rule exception conditions for an Inbox rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="87333-122">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="87333-122">Text value</span></span>

<span data-ttu-id="87333-123">Нет.</span><span class="sxs-lookup"><span data-stu-id="87333-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="87333-124">Примечания</span><span class="sxs-lookup"><span data-stu-id="87333-124">Remarks</span></span>

<span data-ttu-id="87333-125">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="87333-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="87333-126">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="87333-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="87333-127">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="87333-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="87333-128">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="87333-128">Schema Name</span></span>  <br/> |<span data-ttu-id="87333-129">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="87333-129">Messages schema</span></span>  <br/> |
|<span data-ttu-id="87333-130">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="87333-130">Validation File</span></span>  <br/> |<span data-ttu-id="87333-131">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="87333-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="87333-132">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="87333-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="87333-133">True</span><span class="sxs-lookup"><span data-stu-id="87333-133">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="87333-134">См. также</span><span class="sxs-lookup"><span data-stu-id="87333-134">See also</span></span>



- [<span data-ttu-id="87333-135">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="87333-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

