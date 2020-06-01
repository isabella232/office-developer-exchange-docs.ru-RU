---
title: мессажеклассификатионс
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MessageClassifications
api_type:
- schema
ms.assetid: 041b3d48-8f43-47f3-869f-72b66bef372a
description: Элемент Мессажеклассификатионс представляет классификации сообщений, которые должны быть помечены для входящих сообщений, чтобы применить условие или исключение.
ms.openlocfilehash: 63481aa8903c4e9637870130eb9154118471c3b0
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/01/2020
ms.locfileid: "44467972"
---
# <a name="messageclassifications"></a><span data-ttu-id="c968e-103">мессажеклассификатионс</span><span class="sxs-lookup"><span data-stu-id="c968e-103">MessageClassifications</span></span>

<span data-ttu-id="c968e-104">Элемент **мессажеклассификатионс** представляет классификации сообщений, которые должны быть помечены для входящих сообщений, чтобы применить условие или исключение.</span><span class="sxs-lookup"><span data-stu-id="c968e-104">The **MessageClassifications** element represents the message classifications that must be stamped on incoming messages in order for the condition or exception to apply.</span></span> 
  
```XML
<MessageClassifications>
    <String/>
</MessageClassifications>
```

 <span data-ttu-id="c968e-105">**аррайофстрингстипе**</span><span class="sxs-lookup"><span data-stu-id="c968e-105">**ArrayOfStringsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c968e-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="c968e-106">Attributes and elements</span></span>

<span data-ttu-id="c968e-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="c968e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c968e-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="c968e-108">Attributes</span></span>

<span data-ttu-id="c968e-109">Нет</span><span class="sxs-lookup"><span data-stu-id="c968e-109">None</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c968e-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="c968e-110">Child elements</span></span>

|<span data-ttu-id="c968e-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="c968e-111">**Element**</span></span>|<span data-ttu-id="c968e-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="c968e-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c968e-113">Строка</span><span class="sxs-lookup"><span data-stu-id="c968e-113">String</span></span>](string.md) <br/> |<span data-ttu-id="c968e-114">Представляет классификацию сообщений.</span><span class="sxs-lookup"><span data-stu-id="c968e-114">Represents a message classification.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="c968e-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="c968e-115">Parent elements</span></span>

|<span data-ttu-id="c968e-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="c968e-116">**Element**</span></span>|<span data-ttu-id="c968e-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="c968e-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c968e-118">Условия</span><span class="sxs-lookup"><span data-stu-id="c968e-118">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="c968e-119">Представляет условия, которые, если удовлетворены, запускают действия правила для правила.</span><span class="sxs-lookup"><span data-stu-id="c968e-119">Represents the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span>  <br/> |
|[<span data-ttu-id="c968e-120">Исключения</span><span class="sxs-lookup"><span data-stu-id="c968e-120">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="c968e-121">Представляет исключения, которые представляют все доступные правила условия исключений для правила папки «Входящие».</span><span class="sxs-lookup"><span data-stu-id="c968e-121">Represents the exceptions that represent all the available rule exception conditions for an Inbox rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="c968e-122">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="c968e-122">Text value</span></span>

<span data-ttu-id="c968e-123">Нет.</span><span class="sxs-lookup"><span data-stu-id="c968e-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="c968e-124">Примечания</span><span class="sxs-lookup"><span data-stu-id="c968e-124">Remarks</span></span>

<span data-ttu-id="c968e-125">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="c968e-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c968e-126">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="c968e-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c968e-127">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="c968e-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="c968e-128">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="c968e-128">Schema Name</span></span>  <br/> |<span data-ttu-id="c968e-129">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="c968e-129">Messages schema</span></span>  <br/> |
|<span data-ttu-id="c968e-130">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="c968e-130">Validation File</span></span>  <br/> |<span data-ttu-id="c968e-131">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="c968e-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="c968e-132">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="c968e-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="c968e-133">True</span><span class="sxs-lookup"><span data-stu-id="c968e-133">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c968e-134">См. также</span><span class="sxs-lookup"><span data-stu-id="c968e-134">See also</span></span>



- [<span data-ttu-id="c968e-135">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="c968e-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

