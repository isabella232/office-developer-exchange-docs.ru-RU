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
ms.openlocfilehash: 9040859452a48916a969b6d8e4e370b5785c1c1a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834053"
---
# <a name="ismeetingresponse"></a><span data-ttu-id="723a9-103">исмитингреспонсе</span><span class="sxs-lookup"><span data-stu-id="723a9-103">IsMeetingResponse</span></span>

<span data-ttu-id="723a9-104">Элемент **исмитнгреспонсекуест** указывает, должны ли входящие сообщения быть ответом на приглашение на собрание, чтобы применялось условие или исключение.</span><span class="sxs-lookup"><span data-stu-id="723a9-104">The **IsMeetngResponsequest** element indicates whether incoming messages must be a meeting response in order for the condition or exception to apply.</span></span> 
  
```XML
<IsMeetingResponse/>true | false</IsMeetingResponse>
```

 <span data-ttu-id="723a9-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="723a9-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="723a9-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="723a9-106">Attributes and elements</span></span>

<span data-ttu-id="723a9-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="723a9-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="723a9-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="723a9-108">Attributes</span></span>

<span data-ttu-id="723a9-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="723a9-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="723a9-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="723a9-110">Child elements</span></span>

<span data-ttu-id="723a9-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="723a9-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="723a9-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="723a9-112">Parent elements</span></span>

|<span data-ttu-id="723a9-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="723a9-113">**Element**</span></span>|<span data-ttu-id="723a9-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="723a9-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="723a9-115">Условия</span><span class="sxs-lookup"><span data-stu-id="723a9-115">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="723a9-116">Представляет условия, которые, если удовлетворены, запускают действия правила для правила.</span><span class="sxs-lookup"><span data-stu-id="723a9-116">Represents the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span>  <br/> |
|[<span data-ttu-id="723a9-117">Исключения</span><span class="sxs-lookup"><span data-stu-id="723a9-117">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="723a9-118">Представляет все доступные условия исключения правила для правила папки "Входящие".</span><span class="sxs-lookup"><span data-stu-id="723a9-118">Represents all the available rule exception conditions for an Inbox rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="723a9-119">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="723a9-119">Text value</span></span>

<span data-ttu-id="723a9-120">Текстовое значение **true** указывает, что сообщение должно быть ответом на приглашение на собрание, чтобы применялось условие или исключение.</span><span class="sxs-lookup"><span data-stu-id="723a9-120">A text value of **true** indicates that the message must be a meeting response in order for the condition or exception to apply.</span></span> <span data-ttu-id="723a9-121">Текстовое значение **false** указывает, что сообщение не должно быть ответом на приглашение на собрание, чтобы применялось условие или исключение.</span><span class="sxs-lookup"><span data-stu-id="723a9-121">A text value of **false** indicates that the message must not be a meeting response in order for the condition or exception to apply.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="723a9-122">Примечания</span><span class="sxs-lookup"><span data-stu-id="723a9-122">Remarks</span></span>

<span data-ttu-id="723a9-123">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="723a9-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="723a9-124">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="723a9-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="723a9-125">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="723a9-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="723a9-126">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="723a9-126">Schema Name</span></span>  <br/> |<span data-ttu-id="723a9-127">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="723a9-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="723a9-128">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="723a9-128">Validation File</span></span>  <br/> |<span data-ttu-id="723a9-129">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="723a9-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="723a9-130">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="723a9-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="723a9-131">True</span><span class="sxs-lookup"><span data-stu-id="723a9-131">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="723a9-132">См. также</span><span class="sxs-lookup"><span data-stu-id="723a9-132">See also</span></span>



- [<span data-ttu-id="723a9-133">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="723a9-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

