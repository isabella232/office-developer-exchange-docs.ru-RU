---
title: контаинссендерстрингс
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ContainsSenderStrings
api_type:
- schema
ms.assetid: 3e16163f-cffe-4c4e-9a2a-00245d25ba96
description: Элемент Контаинссендерстрингс указывает строки, которые должны отображаться в свойстве From входящих сообщений, чтобы применялось условие или исключение.
ms.openlocfilehash: e7b78f1311d288db7969a0024bde84433e18d37f
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458980"
---
# <a name="containssenderstrings"></a><span data-ttu-id="e5a67-103">контаинссендерстрингс</span><span class="sxs-lookup"><span data-stu-id="e5a67-103">ContainsSenderStrings</span></span>

<span data-ttu-id="e5a67-104">Элемент **контаинссендерстрингс** указывает строки, которые должны отображаться в свойстве **from** входящих сообщений, чтобы применялось условие или исключение.</span><span class="sxs-lookup"><span data-stu-id="e5a67-104">The **ContainsSenderStrings** element indicates the strings that must appear in the **From** property of incoming messages in order for the condition or exception to apply.</span></span> 
  
```XML
<ContainsSenderStrings>
    <String/>
</ContainsSenderStrings>
```

 <span data-ttu-id="e5a67-105">**аррайофстрингстипе**</span><span class="sxs-lookup"><span data-stu-id="e5a67-105">**ArrayOfStringsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e5a67-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="e5a67-106">Attributes and elements</span></span>

<span data-ttu-id="e5a67-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="e5a67-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e5a67-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="e5a67-108">Attributes</span></span>

<span data-ttu-id="e5a67-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="e5a67-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e5a67-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="e5a67-110">Child elements</span></span>

|<span data-ttu-id="e5a67-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="e5a67-111">**Element**</span></span>|<span data-ttu-id="e5a67-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="e5a67-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e5a67-113">Строка</span><span class="sxs-lookup"><span data-stu-id="e5a67-113">String</span></span>](string.md) <br/> |<span data-ttu-id="e5a67-114">Представляет строку, которая должна отображаться в свойстве **from** входящих сообщений, чтобы применить условие или исключение.</span><span class="sxs-lookup"><span data-stu-id="e5a67-114">Represents a string that must appear in the **From** property of incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="e5a67-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="e5a67-115">Parent elements</span></span>

|<span data-ttu-id="e5a67-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="e5a67-116">**Element**</span></span>|<span data-ttu-id="e5a67-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="e5a67-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e5a67-118">Условия</span><span class="sxs-lookup"><span data-stu-id="e5a67-118">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="e5a67-119">Представляет условия, которые, если удовлетворены, запускают действия правила для правила.</span><span class="sxs-lookup"><span data-stu-id="e5a67-119">Represents the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span>  <br/> |
|[<span data-ttu-id="e5a67-120">Исключения</span><span class="sxs-lookup"><span data-stu-id="e5a67-120">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="e5a67-121">Представляет исключения, которые представляют все доступные правила условия исключений для правила папки «Входящие».</span><span class="sxs-lookup"><span data-stu-id="e5a67-121">Represents the exceptions that represent all the available rule exception conditions for an Inbox rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="e5a67-122">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="e5a67-122">Text value</span></span>

<span data-ttu-id="e5a67-123">Нет.</span><span class="sxs-lookup"><span data-stu-id="e5a67-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="e5a67-124">Примечания</span><span class="sxs-lookup"><span data-stu-id="e5a67-124">Remarks</span></span>

<span data-ttu-id="e5a67-125">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="e5a67-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e5a67-126">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="e5a67-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e5a67-127">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="e5a67-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="e5a67-128">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="e5a67-128">Schema Name</span></span>  <br/> |<span data-ttu-id="e5a67-129">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="e5a67-129">Messages schema</span></span>  <br/> |
|<span data-ttu-id="e5a67-130">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="e5a67-130">Validation File</span></span>  <br/> |<span data-ttu-id="e5a67-131">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="e5a67-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="e5a67-132">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="e5a67-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="e5a67-133">True</span><span class="sxs-lookup"><span data-stu-id="e5a67-133">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e5a67-134">См. также</span><span class="sxs-lookup"><span data-stu-id="e5a67-134">See also</span></span>



- [<span data-ttu-id="e5a67-135">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="e5a67-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

