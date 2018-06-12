---
title: IsPermissionControlled
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsPermissionControlled
api_type:
- schema
ms.assetid: a2fd0340-f31f-4389-a1cd-7e93b40bb3c6
description: Элемент IsPermissionControlled указывает ли входящих сообщений должны быть управляются разрешение (защищенные RMS) в порядке для условие или исключение для применения.
ms.openlocfilehash: fdd9910b8c35d9d57e724d6fec57d203f38f0359
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19834088"
---
# <a name="ispermissioncontrolled"></a><span data-ttu-id="bc679-103">IsPermissionControlled</span><span class="sxs-lookup"><span data-stu-id="bc679-103">IsPermissionControlled</span></span>

<span data-ttu-id="bc679-104">Элемент **IsPermissionControlled** указывает ли входящих сообщений должны быть управляются разрешение (защищенные RMS) в порядке для условие или исключение для применения.</span><span class="sxs-lookup"><span data-stu-id="bc679-104">The **IsPermissionControlled** element indicates whether incoming messages must be permission controlled (RMS protected) in order for the condition or exception to apply.</span></span> 
  
```XML
<IsPermissionControlled>true | false</IsPermissionControlled>
```

 <span data-ttu-id="bc679-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="bc679-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="bc679-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="bc679-106">Attributes and elements</span></span>

<span data-ttu-id="bc679-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="bc679-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="bc679-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="bc679-108">Attributes</span></span>

<span data-ttu-id="bc679-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="bc679-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="bc679-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="bc679-110">Child elements</span></span>

<span data-ttu-id="bc679-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="bc679-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="bc679-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="bc679-112">Parent elements</span></span>

|<span data-ttu-id="bc679-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="bc679-113">**Element**</span></span>|<span data-ttu-id="bc679-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="bc679-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bc679-115">Условия</span><span class="sxs-lookup"><span data-stu-id="bc679-115">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="bc679-116">Представляет условия, которые, если удовлетворены, запускают действия правила для правила.</span><span class="sxs-lookup"><span data-stu-id="bc679-116">Represents the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span>  <br/> |
|[<span data-ttu-id="bc679-117">Исключения</span><span class="sxs-lookup"><span data-stu-id="bc679-117">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="bc679-118">Представляет доступных исключение условий для правила папки «Входящие».</span><span class="sxs-lookup"><span data-stu-id="bc679-118">Represents all the available rule exception conditions for an Inbox rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="bc679-119">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="bc679-119">Text value</span></span>

<span data-ttu-id="bc679-120">Текстовое значение **true,** указывает, что сообщения должны быть защищены в порядке для условие или исключение для применения службы управления правами.</span><span class="sxs-lookup"><span data-stu-id="bc679-120">A text value of **true** indicates that the message must be RMS protected in order for the condition or exception to apply.</span></span> <span data-ttu-id="bc679-121">Значение **false** указывает, что сообщение не должна быть защищены в порядке для условие или исключение для применения службы управления правами.</span><span class="sxs-lookup"><span data-stu-id="bc679-121">A value of **false** indicates that the message must not be RMS protected in order for the condition or exception to apply.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="bc679-122">Замечания</span><span class="sxs-lookup"><span data-stu-id="bc679-122">Remarks</span></span>

<span data-ttu-id="bc679-123">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="bc679-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="bc679-124">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="bc679-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="bc679-125">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="bc679-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="bc679-126">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="bc679-126">Schema Name</span></span>  <br/> |<span data-ttu-id="bc679-127">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="bc679-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="bc679-128">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="bc679-128">Validation File</span></span>  <br/> |<span data-ttu-id="bc679-129">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="bc679-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="bc679-130">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="bc679-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="bc679-131">True</span><span class="sxs-lookup"><span data-stu-id="bc679-131">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="bc679-132">См. также</span><span class="sxs-lookup"><span data-stu-id="bc679-132">See also</span></span>



- [<span data-ttu-id="bc679-133">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="bc679-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

