---
title: исндр
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsNDR
api_type:
- schema
ms.assetid: 194f5836-7793-463a-a090-4386d1c2487a
description: Элемент Исндр указывает, должны ли входящие сообщения относиться к отчетам о недоставке (NDR), чтобы применялось условие или исключение.
ms.openlocfilehash: 651590d055a0532c904dbf6c481dca2f899d673f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834056"
---
# <a name="isndr"></a><span data-ttu-id="db0db-103">исндр</span><span class="sxs-lookup"><span data-stu-id="db0db-103">IsNDR</span></span>

<span data-ttu-id="db0db-104">Элемент **исндр** указывает, должны ли входящие сообщения относиться к отчетам о недоставке (NDR), чтобы применялось условие или исключение.</span><span class="sxs-lookup"><span data-stu-id="db0db-104">The **IsNDR** element indicates whether incoming messages must be non-delivery reports (NDRs) in order for the condition or exception to apply.</span></span> 
  
```XML
<IsNDR>true | false</IsNDR>
```

 <span data-ttu-id="db0db-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="db0db-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="db0db-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="db0db-106">Attributes and elements</span></span>

<span data-ttu-id="db0db-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="db0db-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="db0db-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="db0db-108">Attributes</span></span>

<span data-ttu-id="db0db-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="db0db-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="db0db-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="db0db-110">Child elements</span></span>

<span data-ttu-id="db0db-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="db0db-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="db0db-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="db0db-112">Parent elements</span></span>

|<span data-ttu-id="db0db-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="db0db-113">**Element**</span></span>|<span data-ttu-id="db0db-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="db0db-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="db0db-115">Условия</span><span class="sxs-lookup"><span data-stu-id="db0db-115">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="db0db-116">Представляет условия, которые, если удовлетворены, запускают действия правила для правила.</span><span class="sxs-lookup"><span data-stu-id="db0db-116">Represents the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span>  <br/> |
|[<span data-ttu-id="db0db-117">Исключения</span><span class="sxs-lookup"><span data-stu-id="db0db-117">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="db0db-118">Представляет все доступные условия исключения правила для правила папки "Входящие".</span><span class="sxs-lookup"><span data-stu-id="db0db-118">Represents all the available rule exception conditions for an Inbox rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="db0db-119">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="db0db-119">Text value</span></span>

<span data-ttu-id="db0db-120">Текстовое значение **true** указывает, что сообщение должно быть отчетом о недоставке, чтобы применялось условие или исключение.</span><span class="sxs-lookup"><span data-stu-id="db0db-120">A text value of **true** indicates that the message must be an NDR in order for the condition or exception to apply.</span></span> <span data-ttu-id="db0db-121">Значение **false** указывает на то, что сообщение не должно быть отчетом о недоставке, чтобы применить условие или исключение.</span><span class="sxs-lookup"><span data-stu-id="db0db-121">A value of **false** indicates that the message must not be an NDR in order for the condition or exception to apply.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="db0db-122">Примечания</span><span class="sxs-lookup"><span data-stu-id="db0db-122">Remarks</span></span>

<span data-ttu-id="db0db-123">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="db0db-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="db0db-124">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="db0db-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="db0db-125">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="db0db-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="db0db-126">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="db0db-126">Schema Name</span></span>  <br/> |<span data-ttu-id="db0db-127">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="db0db-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="db0db-128">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="db0db-128">Validation File</span></span>  <br/> |<span data-ttu-id="db0db-129">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="db0db-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="db0db-130">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="db0db-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="db0db-131">True</span><span class="sxs-lookup"><span data-stu-id="db0db-131">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="db0db-132">См. также</span><span class="sxs-lookup"><span data-stu-id="db0db-132">See also</span></span>



- [<span data-ttu-id="db0db-133">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="db0db-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

