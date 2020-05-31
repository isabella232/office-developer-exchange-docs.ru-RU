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
description: Элемент с подписью указывает, должны ли входящие сообщения быть подписаны для того, чтобы применялось условие или исключение.
ms.openlocfilehash: 33ff204260465490c701c6573ff4140967ac625a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834105"
---
# <a name="issigned"></a><span data-ttu-id="6c36b-103">IsSigned</span><span class="sxs-lookup"><span data-stu-id="6c36b-103">IsSigned</span></span>

<span data-ttu-id="6c36b-104">Элемент с **подписью** указывает, должны ли входящие сообщения быть подписаны для того, чтобы применялось условие или исключение.</span><span class="sxs-lookup"><span data-stu-id="6c36b-104">The **IsSigned** element indicates whether incoming messages must be signed in order for the condition or exception to apply.</span></span> 
  
```XML
<IsSigned>true | false</IsSigned>
```

 <span data-ttu-id="6c36b-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="6c36b-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6c36b-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="6c36b-106">Attributes and elements</span></span>

<span data-ttu-id="6c36b-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="6c36b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6c36b-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="6c36b-108">Attributes</span></span>

<span data-ttu-id="6c36b-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="6c36b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6c36b-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="6c36b-110">Child elements</span></span>

<span data-ttu-id="6c36b-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="6c36b-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="6c36b-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="6c36b-112">Parent elements</span></span>

|<span data-ttu-id="6c36b-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="6c36b-113">**Element**</span></span>|<span data-ttu-id="6c36b-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="6c36b-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6c36b-115">Условия</span><span class="sxs-lookup"><span data-stu-id="6c36b-115">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="6c36b-116">Представляет условия, которые, если удовлетворены, запускают действия правила для правила.</span><span class="sxs-lookup"><span data-stu-id="6c36b-116">Represents the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span>  <br/> |
|[<span data-ttu-id="6c36b-117">Исключения</span><span class="sxs-lookup"><span data-stu-id="6c36b-117">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="6c36b-118">Представляет исключения, которые представляют все доступные правила условия исключений для правила папки «Входящие».</span><span class="sxs-lookup"><span data-stu-id="6c36b-118">Represents the exceptions that represent all the available rule exception conditions for an Inbox rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="6c36b-119">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="6c36b-119">Text value</span></span>

<span data-ttu-id="6c36b-120">Текстовое значение **true** указывает, что сообщение должно быть подписано, чтобы применялось условие или исключение.</span><span class="sxs-lookup"><span data-stu-id="6c36b-120">A text value of **true** indicates that the message must be signed in order for the condition or exception to apply.</span></span> <span data-ttu-id="6c36b-121">Текстовое значение **false** указывает на то, что сообщение не обязательно должно быть подписано на условие или исключение, которое необходимо применить.</span><span class="sxs-lookup"><span data-stu-id="6c36b-121">A text value of **false** indicates that the message does not have to be signed for the condition or exception to apply.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="6c36b-122">Примечания</span><span class="sxs-lookup"><span data-stu-id="6c36b-122">Remarks</span></span>

<span data-ttu-id="6c36b-123">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="6c36b-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6c36b-124">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="6c36b-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6c36b-125">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="6c36b-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="6c36b-126">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="6c36b-126">Schema Name</span></span>  <br/> |<span data-ttu-id="6c36b-127">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="6c36b-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="6c36b-128">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="6c36b-128">Validation File</span></span>  <br/> |<span data-ttu-id="6c36b-129">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="6c36b-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="6c36b-130">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="6c36b-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="6c36b-131">True</span><span class="sxs-lookup"><span data-stu-id="6c36b-131">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6c36b-132">См. также</span><span class="sxs-lookup"><span data-stu-id="6c36b-132">See also</span></span>



- [<span data-ttu-id="6c36b-133">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="6c36b-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

