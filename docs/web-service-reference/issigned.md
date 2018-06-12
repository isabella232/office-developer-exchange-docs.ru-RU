---
title: IsSigned
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsSigned
api_type:
- schema
ms.assetid: a4f90fe5-2834-4621-9aa3-b561f74d4674
description: Элемент IsSigned указывает ли входящих сообщений должны войти в порядке для условие или исключение для применения.
ms.openlocfilehash: 33ff204260465490c701c6573ff4140967ac625a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19834105"
---
# <a name="issigned"></a><span data-ttu-id="853bd-103">IsSigned</span><span class="sxs-lookup"><span data-stu-id="853bd-103">IsSigned</span></span>

<span data-ttu-id="853bd-104">Элемент **IsSigned** указывает ли входящих сообщений должны войти в порядке для условие или исключение для применения.</span><span class="sxs-lookup"><span data-stu-id="853bd-104">The **IsSigned** element indicates whether incoming messages must be signed in order for the condition or exception to apply.</span></span> 
  
```XML
<IsSigned>true | false</IsSigned>
```

 <span data-ttu-id="853bd-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="853bd-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="853bd-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="853bd-106">Attributes and elements</span></span>

<span data-ttu-id="853bd-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="853bd-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="853bd-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="853bd-108">Attributes</span></span>

<span data-ttu-id="853bd-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="853bd-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="853bd-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="853bd-110">Child elements</span></span>

<span data-ttu-id="853bd-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="853bd-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="853bd-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="853bd-112">Parent elements</span></span>

|<span data-ttu-id="853bd-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="853bd-113">**Element**</span></span>|<span data-ttu-id="853bd-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="853bd-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="853bd-115">Условия</span><span class="sxs-lookup"><span data-stu-id="853bd-115">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="853bd-116">Представляет условия, которые, если удовлетворены, запускают действия правила для правила.</span><span class="sxs-lookup"><span data-stu-id="853bd-116">Represents the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span>  <br/> |
|[<span data-ttu-id="853bd-117">Исключения</span><span class="sxs-lookup"><span data-stu-id="853bd-117">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="853bd-118">Представляет исключения, которые представляют все доступные правила условия исключений для правила папки «Входящие».</span><span class="sxs-lookup"><span data-stu-id="853bd-118">Represents the exceptions that represent all the available rule exception conditions for an Inbox rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="853bd-119">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="853bd-119">Text value</span></span>

<span data-ttu-id="853bd-120">Текстовое значение **true,** указывает, что сообщения должны войти в порядке для условие или исключение для применения.</span><span class="sxs-lookup"><span data-stu-id="853bd-120">A text value of **true** indicates that the message must be signed in order for the condition or exception to apply.</span></span> <span data-ttu-id="853bd-121">Текстовое значение **false** указывает, что сообщение не имеет подписи для условие или исключение для применения.</span><span class="sxs-lookup"><span data-stu-id="853bd-121">A text value of **false** indicates that the message does not have to be signed for the condition or exception to apply.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="853bd-122">Замечания</span><span class="sxs-lookup"><span data-stu-id="853bd-122">Remarks</span></span>

<span data-ttu-id="853bd-123">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="853bd-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="853bd-124">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="853bd-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="853bd-125">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="853bd-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="853bd-126">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="853bd-126">Schema Name</span></span>  <br/> |<span data-ttu-id="853bd-127">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="853bd-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="853bd-128">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="853bd-128">Validation File</span></span>  <br/> |<span data-ttu-id="853bd-129">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="853bd-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="853bd-130">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="853bd-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="853bd-131">True</span><span class="sxs-lookup"><span data-stu-id="853bd-131">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="853bd-132">См. также</span><span class="sxs-lookup"><span data-stu-id="853bd-132">See also</span></span>



- [<span data-ttu-id="853bd-133">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="853bd-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

