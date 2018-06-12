---
title: FromAddresses
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
description: Элемент FromAddresses указывает адреса электронной почты, из которых необходимо отправить входящих сообщений в порядке для условие или исключение для применения.
ms.openlocfilehash: 40ecb1f3e16ad961b8e4c38d5aa9d15f4f74469a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762664"
---
# <a name="fromaddresses"></a><span data-ttu-id="81c62-103">FromAddresses</span><span class="sxs-lookup"><span data-stu-id="81c62-103">FromAddresses</span></span>

<span data-ttu-id="81c62-104">Элемент **FromAddresses** указывает адреса электронной почты, из которых необходимо отправить входящих сообщений в порядке для условие или исключение для применения.</span><span class="sxs-lookup"><span data-stu-id="81c62-104">The **FromAddresses** element indicates the e-mail addresses from which incoming messages must be sent in order for the condition or exception to apply.</span></span> 
  
```XML
<FromAddresses>
   <Address/>
</FromAddresses>
```

 <span data-ttu-id="81c62-105">**ArrayOfEmailAddressesType**</span><span class="sxs-lookup"><span data-stu-id="81c62-105">**ArrayOfEmailAddressesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="81c62-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="81c62-106">Attributes and elements</span></span>

<span data-ttu-id="81c62-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="81c62-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="81c62-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="81c62-108">Attributes</span></span>

<span data-ttu-id="81c62-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="81c62-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="81c62-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="81c62-110">Child elements</span></span>

|<span data-ttu-id="81c62-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="81c62-111">**Element**</span></span>|<span data-ttu-id="81c62-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="81c62-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="81c62-113">Адрес (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="81c62-113">Address (EmailAddressType)</span></span>](address-emailaddresstype.md) <br/> |<span data-ttu-id="81c62-114">Представляет адрес электронной почты полностью разрешенной.</span><span class="sxs-lookup"><span data-stu-id="81c62-114">Represents a fully resolved e-mail address.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="81c62-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="81c62-115">Parent elements</span></span>

|<span data-ttu-id="81c62-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="81c62-116">**Element**</span></span>|<span data-ttu-id="81c62-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="81c62-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="81c62-118">Условия</span><span class="sxs-lookup"><span data-stu-id="81c62-118">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="81c62-119">Представляет условия, которые, если удовлетворены, запускают действия правила для правила.</span><span class="sxs-lookup"><span data-stu-id="81c62-119">Represents the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span>  <br/> |
|[<span data-ttu-id="81c62-120">Исключения</span><span class="sxs-lookup"><span data-stu-id="81c62-120">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="81c62-121">Представляет доступных исключение условий для правила папки «Входящие».</span><span class="sxs-lookup"><span data-stu-id="81c62-121">Represents all the available rule exception conditions for an Inbox rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="81c62-122">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="81c62-122">Text value</span></span>

<span data-ttu-id="81c62-123">Нет.</span><span class="sxs-lookup"><span data-stu-id="81c62-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="81c62-124">Замечания</span><span class="sxs-lookup"><span data-stu-id="81c62-124">Remarks</span></span>

<span data-ttu-id="81c62-125">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="81c62-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="81c62-126">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="81c62-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="81c62-127">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="81c62-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="81c62-128">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="81c62-128">Schema Name</span></span>  <br/> |<span data-ttu-id="81c62-129">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="81c62-129">Messages schema</span></span>  <br/> |
|<span data-ttu-id="81c62-130">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="81c62-130">Validation File</span></span>  <br/> |<span data-ttu-id="81c62-131">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="81c62-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="81c62-132">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="81c62-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="81c62-133">True</span><span class="sxs-lookup"><span data-stu-id="81c62-133">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="81c62-134">См. также</span><span class="sxs-lookup"><span data-stu-id="81c62-134">See also</span></span>



- [<span data-ttu-id="81c62-135">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="81c62-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

