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
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465935"
---
# <a name="ismeetingresponse"></a><span data-ttu-id="898cb-103">исмитингреспонсе</span><span class="sxs-lookup"><span data-stu-id="898cb-103">IsMeetingResponse</span></span>

<span data-ttu-id="898cb-104">Элемент **исмитнгреспонсекуест** указывает, должны ли входящие сообщения быть ответом на приглашение на собрание, чтобы применялось условие или исключение.</span><span class="sxs-lookup"><span data-stu-id="898cb-104">The **IsMeetngResponsequest** element indicates whether incoming messages must be a meeting response in order for the condition or exception to apply.</span></span> 
  
```XML
<IsMeetingResponse/>true | false</IsMeetingResponse>
```

 <span data-ttu-id="898cb-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="898cb-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="898cb-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="898cb-106">Attributes and elements</span></span>

<span data-ttu-id="898cb-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="898cb-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="898cb-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="898cb-108">Attributes</span></span>

<span data-ttu-id="898cb-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="898cb-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="898cb-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="898cb-110">Child elements</span></span>

<span data-ttu-id="898cb-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="898cb-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="898cb-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="898cb-112">Parent elements</span></span>

|<span data-ttu-id="898cb-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="898cb-113">**Element**</span></span>|<span data-ttu-id="898cb-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="898cb-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="898cb-115">Условия</span><span class="sxs-lookup"><span data-stu-id="898cb-115">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="898cb-116">Представляет условия, которые, если удовлетворены, запускают действия правила для правила.</span><span class="sxs-lookup"><span data-stu-id="898cb-116">Represents the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span>  <br/> |
|[<span data-ttu-id="898cb-117">Исключения</span><span class="sxs-lookup"><span data-stu-id="898cb-117">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="898cb-118">Представляет все доступные условия исключения правила для правила папки "Входящие".</span><span class="sxs-lookup"><span data-stu-id="898cb-118">Represents all the available rule exception conditions for an Inbox rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="898cb-119">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="898cb-119">Text value</span></span>

<span data-ttu-id="898cb-120">Текстовое значение **true** указывает, что сообщение должно быть ответом на приглашение на собрание, чтобы применялось условие или исключение.</span><span class="sxs-lookup"><span data-stu-id="898cb-120">A text value of **true** indicates that the message must be a meeting response in order for the condition or exception to apply.</span></span> <span data-ttu-id="898cb-121">Текстовое значение **false** указывает, что сообщение не должно быть ответом на приглашение на собрание, чтобы применялось условие или исключение.</span><span class="sxs-lookup"><span data-stu-id="898cb-121">A text value of **false** indicates that the message must not be a meeting response in order for the condition or exception to apply.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="898cb-122">Примечания</span><span class="sxs-lookup"><span data-stu-id="898cb-122">Remarks</span></span>

<span data-ttu-id="898cb-123">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="898cb-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="898cb-124">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="898cb-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="898cb-125">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="898cb-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="898cb-126">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="898cb-126">Schema Name</span></span>  <br/> |<span data-ttu-id="898cb-127">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="898cb-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="898cb-128">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="898cb-128">Validation File</span></span>  <br/> |<span data-ttu-id="898cb-129">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="898cb-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="898cb-130">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="898cb-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="898cb-131">True</span><span class="sxs-lookup"><span data-stu-id="898cb-131">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="898cb-132">См. также</span><span class="sxs-lookup"><span data-stu-id="898cb-132">See also</span></span>



- [<span data-ttu-id="898cb-133">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="898cb-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

