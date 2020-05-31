---
title: контаиншеадерстрингс
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ContainsHeaderStrings
api_type:
- schema
ms.assetid: 5f68427b-990a-4a27-bfb3-fce3115b02d7
description: Элемент Контаиншеадерстрингс указывает строки, которые должны отображаться в заголовках входящих сообщений, чтобы применялось условие или исключение.
ms.openlocfilehash: 360870d63853a0e79f801cc2f17473b1a1b28c25
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761763"
---
# <a name="containsheaderstrings"></a><span data-ttu-id="23ff4-103">контаиншеадерстрингс</span><span class="sxs-lookup"><span data-stu-id="23ff4-103">ContainsHeaderStrings</span></span>

<span data-ttu-id="23ff4-104">Элемент **контаиншеадерстрингс** указывает строки, которые должны отображаться в заголовках входящих сообщений, чтобы применялось условие или исключение.</span><span class="sxs-lookup"><span data-stu-id="23ff4-104">The **ContainsHeaderStrings** element indicates the strings that must appear in the headers of incoming messages in order for the condition or exception to apply.</span></span> 
  
```XML
<ContainsHeaderStrings>
    <String/>
</ContainsHeaderStrings>
```

 <span data-ttu-id="23ff4-105">**аррайофстрингстипе**</span><span class="sxs-lookup"><span data-stu-id="23ff4-105">**ArrayOfStringsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="23ff4-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="23ff4-106">Attributes and elements</span></span>

<span data-ttu-id="23ff4-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="23ff4-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="23ff4-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="23ff4-108">Attributes</span></span>

<span data-ttu-id="23ff4-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="23ff4-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="23ff4-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="23ff4-110">Child elements</span></span>

|<span data-ttu-id="23ff4-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="23ff4-111">**Element**</span></span>|<span data-ttu-id="23ff4-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="23ff4-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="23ff4-113">Строка</span><span class="sxs-lookup"><span data-stu-id="23ff4-113">String</span></span>](string.md) <br/> |<span data-ttu-id="23ff4-114">Представляет строку, которая должна присутствовать в заголовках сообщений, чтобы применить условие или исключение.</span><span class="sxs-lookup"><span data-stu-id="23ff4-114">Represents a string that must appear in message headers in order for the condition or exception to apply.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="23ff4-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="23ff4-115">Parent elements</span></span>

|<span data-ttu-id="23ff4-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="23ff4-116">**Element**</span></span>|<span data-ttu-id="23ff4-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="23ff4-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="23ff4-118">Условия</span><span class="sxs-lookup"><span data-stu-id="23ff4-118">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="23ff4-119">Представляет условия, которые, если удовлетворены, запускают действия правила для правила.</span><span class="sxs-lookup"><span data-stu-id="23ff4-119">Represents the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span>  <br/> |
|[<span data-ttu-id="23ff4-120">Исключения</span><span class="sxs-lookup"><span data-stu-id="23ff4-120">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="23ff4-121">Представляет исключения, которые представляют все доступные правила условия исключений для правила папки «Входящие».</span><span class="sxs-lookup"><span data-stu-id="23ff4-121">Represents the exceptions that represent all the available rule exception conditions for an Inbox rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="23ff4-122">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="23ff4-122">Text value</span></span>

<span data-ttu-id="23ff4-123">Нет.</span><span class="sxs-lookup"><span data-stu-id="23ff4-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="23ff4-124">Примечания</span><span class="sxs-lookup"><span data-stu-id="23ff4-124">Remarks</span></span>

<span data-ttu-id="23ff4-125">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="23ff4-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="23ff4-126">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="23ff4-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="23ff4-127">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="23ff4-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="23ff4-128">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="23ff4-128">Schema Name</span></span>  <br/> |<span data-ttu-id="23ff4-129">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="23ff4-129">Messages schema</span></span>  <br/> |
|<span data-ttu-id="23ff4-130">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="23ff4-130">Validation File</span></span>  <br/> |<span data-ttu-id="23ff4-131">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="23ff4-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="23ff4-132">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="23ff4-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="23ff4-133">True</span><span class="sxs-lookup"><span data-stu-id="23ff4-133">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="23ff4-134">См. также</span><span class="sxs-lookup"><span data-stu-id="23ff4-134">See also</span></span>



- [<span data-ttu-id="23ff4-135">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="23ff4-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

