---
title: исмитингреспонсе
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsMeetingResponse
api_type:
- schema
ms.assetid: 85090943-81c6-4fbe-a2db-007dced6a4cf
description: Элемент Исмитнгреспонсекуест указывает, должны ли входящие сообщения быть ответом на приглашение на собрание, чтобы применялось условие или исключение.
ms.openlocfilehash: 40714b7e926768f55207d870b79f21f07163bb37
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465935"
---
# <a name="ismeetingresponse"></a><span data-ttu-id="0c518-103">исмитингреспонсе</span><span class="sxs-lookup"><span data-stu-id="0c518-103">IsMeetingResponse</span></span>

<span data-ttu-id="0c518-104">Элемент **исмитнгреспонсекуест** указывает, должны ли входящие сообщения быть ответом на приглашение на собрание, чтобы применялось условие или исключение.</span><span class="sxs-lookup"><span data-stu-id="0c518-104">The **IsMeetngResponsequest** element indicates whether incoming messages must be a meeting response in order for the condition or exception to apply.</span></span> 
  
```XML
<IsMeetingResponse/>true | false</IsMeetingResponse>
```

 <span data-ttu-id="0c518-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="0c518-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0c518-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="0c518-106">Attributes and elements</span></span>

<span data-ttu-id="0c518-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="0c518-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0c518-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="0c518-108">Attributes</span></span>

<span data-ttu-id="0c518-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="0c518-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0c518-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="0c518-110">Child elements</span></span>

<span data-ttu-id="0c518-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="0c518-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="0c518-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="0c518-112">Parent elements</span></span>

|<span data-ttu-id="0c518-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="0c518-113">**Element**</span></span>|<span data-ttu-id="0c518-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="0c518-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0c518-115">Условия</span><span class="sxs-lookup"><span data-stu-id="0c518-115">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="0c518-116">Представляет условия, которые, если удовлетворены, запускают действия правила для правила.</span><span class="sxs-lookup"><span data-stu-id="0c518-116">Represents the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span>  <br/> |
|[<span data-ttu-id="0c518-117">Исключения</span><span class="sxs-lookup"><span data-stu-id="0c518-117">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="0c518-118">Представляет все доступные условия исключения правила для правила папки "Входящие".</span><span class="sxs-lookup"><span data-stu-id="0c518-118">Represents all the available rule exception conditions for an Inbox rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="0c518-119">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="0c518-119">Text value</span></span>

<span data-ttu-id="0c518-120">Текстовое значение **true** указывает, что сообщение должно быть ответом на приглашение на собрание, чтобы применялось условие или исключение.</span><span class="sxs-lookup"><span data-stu-id="0c518-120">A text value of **true** indicates that the message must be a meeting response in order for the condition or exception to apply.</span></span> <span data-ttu-id="0c518-121">Текстовое значение **false** указывает, что сообщение не должно быть ответом на приглашение на собрание, чтобы применялось условие или исключение.</span><span class="sxs-lookup"><span data-stu-id="0c518-121">A text value of **false** indicates that the message must not be a meeting response in order for the condition or exception to apply.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="0c518-122">Примечания</span><span class="sxs-lookup"><span data-stu-id="0c518-122">Remarks</span></span>

<span data-ttu-id="0c518-123">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="0c518-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0c518-124">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="0c518-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0c518-125">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="0c518-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="0c518-126">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="0c518-126">Schema Name</span></span>  <br/> |<span data-ttu-id="0c518-127">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="0c518-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="0c518-128">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="0c518-128">Validation File</span></span>  <br/> |<span data-ttu-id="0c518-129">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="0c518-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="0c518-130">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="0c518-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="0c518-131">True</span><span class="sxs-lookup"><span data-stu-id="0c518-131">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0c518-132">См. также</span><span class="sxs-lookup"><span data-stu-id="0c518-132">See also</span></span>



- [<span data-ttu-id="0c518-133">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="0c518-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

