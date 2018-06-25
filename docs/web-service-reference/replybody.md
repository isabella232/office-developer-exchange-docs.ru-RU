---
title: ReplyBody
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ReplyBody
api_type:
- schema
ms.assetid: bb184144-3e4b-4419-a883-cc9fab1085e6
description: Элемент ReplyBody содержит сообщение об отсутствии на работе Office (OOF) и язык, используемый для сообщения.
ms.openlocfilehash: 8400dda1ee810781e129fcc44fd3cd5d6c15cbbe
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835116"
---
# <a name="replybody"></a><span data-ttu-id="8eecc-103">ReplyBody</span><span class="sxs-lookup"><span data-stu-id="8eecc-103">ReplyBody</span></span>

<span data-ttu-id="8eecc-104">Элемент **ReplyBody** содержит сообщение об отсутствии на работе Office (OOF) и язык, используемый для сообщения.</span><span class="sxs-lookup"><span data-stu-id="8eecc-104">The **ReplyBody** element contains an Out of Office (OOF) message and the language used for the message.</span></span> 
  
```XML
<ReplyBody xml:lang="">
   <Message/>
</ReplyBody>
```

 <span data-ttu-id="8eecc-105">**ReplyBody**</span><span class="sxs-lookup"><span data-stu-id="8eecc-105">**ReplyBody**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8eecc-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="8eecc-106">Attributes and elements</span></span>

<span data-ttu-id="8eecc-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="8eecc-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8eecc-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="8eecc-108">Attributes</span></span>

|<span data-ttu-id="8eecc-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="8eecc-109">**Attribute**</span></span>|<span data-ttu-id="8eecc-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="8eecc-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="8eecc-111">XML: lang</span><span class="sxs-lookup"><span data-stu-id="8eecc-111">xml:lang</span></span>  <br/> |<span data-ttu-id="8eecc-112">Указывает язык, используемый в **ReplyBody** содержимое.</span><span class="sxs-lookup"><span data-stu-id="8eecc-112">Specifies the language used in the **ReplyBody** contents.</span></span> <span data-ttu-id="8eecc-113">Этот атрибут является необязательным.</span><span class="sxs-lookup"><span data-stu-id="8eecc-113">This attribute is optional.</span></span> <span data-ttu-id="8eecc-114">Возможные значения этого атрибута определены в IETF RFC 3066.</span><span class="sxs-lookup"><span data-stu-id="8eecc-114">The possible values of this attribute are defined by IETF RFC 3066.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="8eecc-115">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="8eecc-115">Child elements</span></span>

|<span data-ttu-id="8eecc-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="8eecc-116">**Element**</span></span>|<span data-ttu-id="8eecc-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="8eecc-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8eecc-118">Сообщение (доступность)</span><span class="sxs-lookup"><span data-stu-id="8eecc-118">Message (Availability)</span></span>](message-availability.md) <br/> |<span data-ttu-id="8eecc-119">Содержит ожидания ответа на работе (OOF).</span><span class="sxs-lookup"><span data-stu-id="8eecc-119">Contains the out of office (OOF) response.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="8eecc-120">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="8eecc-120">Parent elements</span></span>

|<span data-ttu-id="8eecc-121">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="8eecc-121">**Element**</span></span>|<span data-ttu-id="8eecc-122">**Описание**</span><span class="sxs-lookup"><span data-stu-id="8eecc-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8eecc-123">Нет на месте</span><span class="sxs-lookup"><span data-stu-id="8eecc-123">OutOfOffice</span></span>](outofoffice.md) <br/> |<span data-ttu-id="8eecc-124">Определяет ответное сообщение об отсутствии на работе и продолжительность для отправки сообщения ответа для почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="8eecc-124">Defines the OOF response message and a duration time for sending the response message for a mailbox.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="8eecc-125">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="8eecc-125">Text value</span></span>

<span data-ttu-id="8eecc-126">Нет.</span><span class="sxs-lookup"><span data-stu-id="8eecc-126">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="8eecc-127">Замечания</span><span class="sxs-lookup"><span data-stu-id="8eecc-127">Remarks</span></span>

<span data-ttu-id="8eecc-128">Этот элемент обязательный.</span><span class="sxs-lookup"><span data-stu-id="8eecc-128">This element is required.</span></span>
  
<span data-ttu-id="8eecc-129">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="8eecc-129">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8eecc-130">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="8eecc-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8eecc-131">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="8eecc-131">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="8eecc-132">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="8eecc-132">Schema Name</span></span>  <br/> |<span data-ttu-id="8eecc-133">Схема Types</span><span class="sxs-lookup"><span data-stu-id="8eecc-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="8eecc-134">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="8eecc-134">Validation File</span></span>  <br/> |<span data-ttu-id="8eecc-135">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="8eecc-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="8eecc-136">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="8eecc-136">Can be Empty</span></span>  <br/> |<span data-ttu-id="8eecc-137">False</span><span class="sxs-lookup"><span data-stu-id="8eecc-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="8eecc-138">См. также</span><span class="sxs-lookup"><span data-stu-id="8eecc-138">See also</span></span>



- [<span data-ttu-id="8eecc-139">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="8eecc-139">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

