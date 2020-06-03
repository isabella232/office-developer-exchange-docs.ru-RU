---
title: итемклассес
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ItemClasses
api_type:
- schema
ms.assetid: f95430cc-2860-47c1-af2d-8c4156c9b281
description: Элемент Итемклассес представляет классы элементов, которые должны быть помечены для входящих сообщений, чтобы применить условие или исключение.
ms.openlocfilehash: 56b99cad2abef0a9953e1793e5b633acca83a9eb
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460115"
---
# <a name="itemclasses"></a><span data-ttu-id="1e7ca-103">итемклассес</span><span class="sxs-lookup"><span data-stu-id="1e7ca-103">ItemClasses</span></span>

<span data-ttu-id="1e7ca-104">Элемент **итемклассес** представляет классы элементов, которые должны быть помечены для входящих сообщений, чтобы применить условие или исключение.</span><span class="sxs-lookup"><span data-stu-id="1e7ca-104">The **ItemClasses** element represents the item classes that must be stamped on incoming messages in order for the condition or exception to apply.</span></span> 
  
```XML
<ItemClasses>
    <String/>
</ItemClasses>
```

 <span data-ttu-id="1e7ca-105">**аррайофстрингстипе**</span><span class="sxs-lookup"><span data-stu-id="1e7ca-105">**ArrayOfStringsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1e7ca-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="1e7ca-106">Attributes and elements</span></span>

<span data-ttu-id="1e7ca-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="1e7ca-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1e7ca-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="1e7ca-108">Attributes</span></span>

<span data-ttu-id="1e7ca-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="1e7ca-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1e7ca-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="1e7ca-110">Child elements</span></span>

|<span data-ttu-id="1e7ca-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="1e7ca-111">**Element**</span></span>|<span data-ttu-id="1e7ca-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="1e7ca-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1e7ca-113">Строка</span><span class="sxs-lookup"><span data-stu-id="1e7ca-113">String</span></span>](string.md) <br/> |<span data-ttu-id="1e7ca-114">Представляет один класс элемента.</span><span class="sxs-lookup"><span data-stu-id="1e7ca-114">Represents a single item class.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="1e7ca-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="1e7ca-115">Parent elements</span></span>

|<span data-ttu-id="1e7ca-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="1e7ca-116">**Element**</span></span>|<span data-ttu-id="1e7ca-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="1e7ca-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1e7ca-118">Условия</span><span class="sxs-lookup"><span data-stu-id="1e7ca-118">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="1e7ca-119">Представляет условия, которые, если удовлетворены, запускают действия правила для правила.</span><span class="sxs-lookup"><span data-stu-id="1e7ca-119">Represents the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span>  <br/> |
|[<span data-ttu-id="1e7ca-120">Исключения</span><span class="sxs-lookup"><span data-stu-id="1e7ca-120">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="1e7ca-121">Представляет исключения, которые представляют все доступные правила условия исключений для правила папки «Входящие».</span><span class="sxs-lookup"><span data-stu-id="1e7ca-121">Represents the exceptions that represent all the available rule exception conditions for an Inbox rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="1e7ca-122">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="1e7ca-122">Text value</span></span>

<span data-ttu-id="1e7ca-123">Нет.</span><span class="sxs-lookup"><span data-stu-id="1e7ca-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="1e7ca-124">Примечания</span><span class="sxs-lookup"><span data-stu-id="1e7ca-124">Remarks</span></span>

<span data-ttu-id="1e7ca-125">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="1e7ca-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1e7ca-126">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="1e7ca-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1e7ca-127">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="1e7ca-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="1e7ca-128">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="1e7ca-128">Schema name</span></span>  <br/> |<span data-ttu-id="1e7ca-129">Схема Types</span><span class="sxs-lookup"><span data-stu-id="1e7ca-129">Types schema</span></span>  <br/> |
|<span data-ttu-id="1e7ca-130">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="1e7ca-130">Validation file</span></span>  <br/> |<span data-ttu-id="1e7ca-131">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="1e7ca-131">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="1e7ca-132">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="1e7ca-132">Can be empty</span></span>  <br/> |<span data-ttu-id="1e7ca-133">False</span><span class="sxs-lookup"><span data-stu-id="1e7ca-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1e7ca-134">См. также</span><span class="sxs-lookup"><span data-stu-id="1e7ca-134">See also</span></span>



- [<span data-ttu-id="1e7ca-135">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="1e7ca-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

