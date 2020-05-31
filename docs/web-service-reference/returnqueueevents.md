---
title: ретурнкуеуивентс
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ReturnQueueEvents
api_type:
- schema
ms.assetid: 69d22417-320c-4c6f-9fb4-2020f2480bb2
description: Элемент Ретурнкуеуивентс указывает, что пользователь, выполняющий задачу, находится в привилегированной роли.
ms.openlocfilehash: 02f4ca86ffa14117105ec186ae039065cb626670
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835233"
---
# <a name="returnqueueevents"></a><span data-ttu-id="c7789-103">ретурнкуеуивентс</span><span class="sxs-lookup"><span data-stu-id="c7789-103">ReturnQueueEvents</span></span>

<span data-ttu-id="c7789-104">Элемент **ретурнкуеуивентс** указывает, что пользователь, выполняющий задачу, находится в привилегированной роли.</span><span class="sxs-lookup"><span data-stu-id="c7789-104">The **ReturnQueueEvents** element indicates that the person who is running the task is in a privileged role.</span></span> 
  
```XML
<ReturnQueueEvents>true | false</ReturnQueueEvents>
```

 <span data-ttu-id="c7789-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="c7789-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c7789-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="c7789-106">Attributes and elements</span></span>

<span data-ttu-id="c7789-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="c7789-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c7789-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="c7789-108">Attributes</span></span>

<span data-ttu-id="c7789-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="c7789-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c7789-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="c7789-110">Child elements</span></span>

<span data-ttu-id="c7789-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="c7789-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="c7789-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="c7789-112">Parent elements</span></span>

|<span data-ttu-id="c7789-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="c7789-113">**Element**</span></span>|<span data-ttu-id="c7789-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="c7789-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c7789-115">GetMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="c7789-115">GetMessageTrackingReport</span></span>](getmessagetrackingreport.md) <br/> |<span data-ttu-id="c7789-116">Содержит запрос для [операции GetMessageTrackingReport](getmessagetrackingreport-operation.md) , чтобы получить полный отчет об отслеживании сообщений для указанного идентификатора.</span><span class="sxs-lookup"><span data-stu-id="c7789-116">Contains the request for the [GetMessageTrackingReport operation](getmessagetrackingreport-operation.md) to retrieve the full message tracking report for the specified ID.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="c7789-117">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="c7789-117">Text value</span></span>

<span data-ttu-id="c7789-118">Текстовое значение, представляющее логическое значение является обязательным.</span><span class="sxs-lookup"><span data-stu-id="c7789-118">A text value that represents a Boolean value is required.</span></span> <span data-ttu-id="c7789-119">Значение **true** указывает, что пользователь, выполняющий задачу, находится в привилегированной роли; значение **false** указывает, что пользователь, выполняющий задачу, не является привилегированной ролью.</span><span class="sxs-lookup"><span data-stu-id="c7789-119">A value of **true** indicates that the person who is running the task is in a privileged role; a value of **false** indicates that the person who is running the task is not in a privileged role.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="c7789-120">Примечания</span><span class="sxs-lookup"><span data-stu-id="c7789-120">Remarks</span></span>

<span data-ttu-id="c7789-121">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="c7789-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c7789-122">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="c7789-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c7789-123">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="c7789-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="c7789-124">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="c7789-124">Schema Name</span></span>  <br/> |<span data-ttu-id="c7789-125">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="c7789-125">Messages schema</span></span>  <br/> |
|<span data-ttu-id="c7789-126">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="c7789-126">Validation File</span></span>  <br/> |<span data-ttu-id="c7789-127">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="c7789-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="c7789-128">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="c7789-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="c7789-129">False</span><span class="sxs-lookup"><span data-stu-id="c7789-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c7789-130">См. также</span><span class="sxs-lookup"><span data-stu-id="c7789-130">See also</span></span>



[<span data-ttu-id="c7789-131">Операция GetMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="c7789-131">GetMessageTrackingReport operation</span></span>](getmessagetrackingreport-operation.md)


- [<span data-ttu-id="c7789-132">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="c7789-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

