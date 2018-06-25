---
title: Нет на месте
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- OutOfOffice
api_type:
- schema
ms.assetid: fe1256ab-5c0f-467d-abb3-b38a2dc312ae
description: Нет на месте элемент представляет ответное сообщение и время для отправки сообщения ответа.
ms.openlocfilehash: 4e1e06ee332c44aeba03e1343c8c3258a2c9631e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834675"
---
# <a name="outofoffice"></a><span data-ttu-id="94681-103">Нет на месте</span><span class="sxs-lookup"><span data-stu-id="94681-103">OutOfOffice</span></span>

<span data-ttu-id="94681-104">**Нет на месте** элемент представляет ответное сообщение и время для отправки сообщения ответа.</span><span class="sxs-lookup"><span data-stu-id="94681-104">The **OutOfOffice** element represents the response message and a duration time for sending the response message.</span></span> 
  
```XML
<OutOfOffice>
   <ReplyBody/>
   <Duration/>
</OutOfOffice>
```

 <span data-ttu-id="94681-105">**OutOfOfficeMailTip**</span><span class="sxs-lookup"><span data-stu-id="94681-105">**OutOfOfficeMailTip**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="94681-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="94681-106">Attributes and elements</span></span>

<span data-ttu-id="94681-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="94681-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="94681-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="94681-108">Attributes</span></span>

<span data-ttu-id="94681-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="94681-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="94681-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="94681-110">Child elements</span></span>

|<span data-ttu-id="94681-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="94681-111">**Element**</span></span>|<span data-ttu-id="94681-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="94681-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="94681-113">ReplyBody</span><span class="sxs-lookup"><span data-stu-id="94681-113">ReplyBody</span></span>](replybody.md) <br/> |<span data-ttu-id="94681-114">Содержит сообщение об отсутствии на работе Office (OOF) и язык, используемый для сообщения.</span><span class="sxs-lookup"><span data-stu-id="94681-114">Contains an Out of Office (OOF) message and the language used for the message.</span></span>  <br/> |
|[<span data-ttu-id="94681-115">Продолжительность (UserOofSettings)</span><span class="sxs-lookup"><span data-stu-id="94681-115">Duration (UserOofSettings)</span></span>](duration-useroofsettings.md) <br/> |<span data-ttu-id="94681-116">Содержит длительность с поддержкой состояние об отсутствии на работе, если элемент [OofState](oofstate.md) задано значение расписанию.</span><span class="sxs-lookup"><span data-stu-id="94681-116">Contains the duration that the OOF status is enabled if the [OofState](oofstate.md) element is set to Scheduled.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="94681-117">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="94681-117">Parent elements</span></span>

|<span data-ttu-id="94681-118">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="94681-118">**Element**</span></span>|<span data-ttu-id="94681-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="94681-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="94681-120">Почтовые подсказки</span><span class="sxs-lookup"><span data-stu-id="94681-120">MailTips</span></span>](mailtips.md) <br/> |<span data-ttu-id="94681-121">Представляет значения для различных типов почтовые подсказки.</span><span class="sxs-lookup"><span data-stu-id="94681-121">Represents values for various types of mail tips.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="94681-122">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="94681-122">Text value</span></span>

<span data-ttu-id="94681-123">Нет.</span><span class="sxs-lookup"><span data-stu-id="94681-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="94681-124">Замечания</span><span class="sxs-lookup"><span data-stu-id="94681-124">Remarks</span></span>

<span data-ttu-id="94681-125">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="94681-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="94681-126">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="94681-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="94681-127">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="94681-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="94681-128">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="94681-128">Schema Name</span></span>  <br/> |<span data-ttu-id="94681-129">Схема Types</span><span class="sxs-lookup"><span data-stu-id="94681-129">Types schema</span></span>  <br/> |
|<span data-ttu-id="94681-130">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="94681-130">Validation File</span></span>  <br/> |<span data-ttu-id="94681-131">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="94681-131">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="94681-132">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="94681-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="94681-133">False</span><span class="sxs-lookup"><span data-stu-id="94681-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="94681-134">См. также</span><span class="sxs-lookup"><span data-stu-id="94681-134">See also</span></span>



- [<span data-ttu-id="94681-135">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="94681-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

