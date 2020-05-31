---
title: реплибоди
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
description: Элемент Реплибоди содержит сообщение об отсутствии на работе (отсутствие на работе) и язык, используемый для сообщения.
ms.openlocfilehash: 8400dda1ee810781e129fcc44fd3cd5d6c15cbbe
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835116"
---
# <a name="replybody"></a><span data-ttu-id="3692e-103">реплибоди</span><span class="sxs-lookup"><span data-stu-id="3692e-103">ReplyBody</span></span>

<span data-ttu-id="3692e-104">Элемент **реплибоди** содержит сообщение об отсутствии на работе (отсутствие на работе) и язык, используемый для сообщения.</span><span class="sxs-lookup"><span data-stu-id="3692e-104">The **ReplyBody** element contains an Out of Office (OOF) message and the language used for the message.</span></span> 
  
```XML
<ReplyBody xml:lang="">
   <Message/>
</ReplyBody>
```

 <span data-ttu-id="3692e-105">**реплибоди**</span><span class="sxs-lookup"><span data-stu-id="3692e-105">**ReplyBody**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3692e-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="3692e-106">Attributes and elements</span></span>

<span data-ttu-id="3692e-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="3692e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3692e-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="3692e-108">Attributes</span></span>

|<span data-ttu-id="3692e-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="3692e-109">**Attribute**</span></span>|<span data-ttu-id="3692e-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="3692e-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="3692e-111">XML: lang</span><span class="sxs-lookup"><span data-stu-id="3692e-111">xml:lang</span></span>  <br/> |<span data-ttu-id="3692e-112">Указывает язык, используемый в содержимом **реплибоди** .</span><span class="sxs-lookup"><span data-stu-id="3692e-112">Specifies the language used in the **ReplyBody** contents.</span></span> <span data-ttu-id="3692e-113">Этот атрибут является необязательным.</span><span class="sxs-lookup"><span data-stu-id="3692e-113">This attribute is optional.</span></span> <span data-ttu-id="3692e-114">Возможные значения этого атрибута определены в документе IETF RFC 3066.</span><span class="sxs-lookup"><span data-stu-id="3692e-114">The possible values of this attribute are defined by IETF RFC 3066.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="3692e-115">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="3692e-115">Child elements</span></span>

|<span data-ttu-id="3692e-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="3692e-116">**Element**</span></span>|<span data-ttu-id="3692e-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="3692e-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3692e-118">Сообщение (доступность)</span><span class="sxs-lookup"><span data-stu-id="3692e-118">Message (Availability)</span></span>](message-availability.md) <br/> |<span data-ttu-id="3692e-119">Содержит ответ "нет на месте" (отсутствие на работе).</span><span class="sxs-lookup"><span data-stu-id="3692e-119">Contains the out of office (OOF) response.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="3692e-120">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="3692e-120">Parent elements</span></span>

|<span data-ttu-id="3692e-121">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="3692e-121">**Element**</span></span>|<span data-ttu-id="3692e-122">**Описание**</span><span class="sxs-lookup"><span data-stu-id="3692e-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3692e-123">аутофоффице</span><span class="sxs-lookup"><span data-stu-id="3692e-123">OutOfOffice</span></span>](outofoffice.md) <br/> |<span data-ttu-id="3692e-124">Определяет ответное сообщение об отсутствии на работе и продолжительность отправки ответного сообщения для почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="3692e-124">Defines the OOF response message and a duration time for sending the response message for a mailbox.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="3692e-125">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="3692e-125">Text value</span></span>

<span data-ttu-id="3692e-126">Нет.</span><span class="sxs-lookup"><span data-stu-id="3692e-126">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="3692e-127">Примечания</span><span class="sxs-lookup"><span data-stu-id="3692e-127">Remarks</span></span>

<span data-ttu-id="3692e-128">Этот элемент обязательный.</span><span class="sxs-lookup"><span data-stu-id="3692e-128">This element is required.</span></span>
  
<span data-ttu-id="3692e-129">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="3692e-129">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3692e-130">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="3692e-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3692e-131">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="3692e-131">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="3692e-132">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="3692e-132">Schema Name</span></span>  <br/> |<span data-ttu-id="3692e-133">Схема Types</span><span class="sxs-lookup"><span data-stu-id="3692e-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="3692e-134">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="3692e-134">Validation File</span></span>  <br/> |<span data-ttu-id="3692e-135">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="3692e-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="3692e-136">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="3692e-136">Can be Empty</span></span>  <br/> |<span data-ttu-id="3692e-137">False</span><span class="sxs-lookup"><span data-stu-id="3692e-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3692e-138">См. также</span><span class="sxs-lookup"><span data-stu-id="3692e-138">See also</span></span>



- [<span data-ttu-id="3692e-139">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="3692e-139">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

