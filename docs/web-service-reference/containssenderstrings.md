---
title: ContainsSenderStrings
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
description: Элемент ContainsSenderStrings указывает строк, которые должны встречаться в свойства From входящих сообщений в порядке для условие или исключение для применения.
ms.openlocfilehash: d174c0d7e2cbfd5b671a825a867d3ee7e24c2f2a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761771"
---
# <a name="containssenderstrings"></a><span data-ttu-id="c9405-103">ContainsSenderStrings</span><span class="sxs-lookup"><span data-stu-id="c9405-103">ContainsSenderStrings</span></span>

<span data-ttu-id="c9405-104">Элемент **ContainsSenderStrings** указывает строк, которые должны встречаться в свойстве **из** входящих сообщений в порядке для условие или исключение для применения.</span><span class="sxs-lookup"><span data-stu-id="c9405-104">The **ContainsSenderStrings** element indicates the strings that must appear in the **From** property of incoming messages in order for the condition or exception to apply.</span></span> 
  
```XML
<ContainsSenderStrings>
    <String/>
</ContainsSenderStrings>
```

 <span data-ttu-id="c9405-105">**ArrayOfStringsType**</span><span class="sxs-lookup"><span data-stu-id="c9405-105">**ArrayOfStringsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c9405-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="c9405-106">Attributes and elements</span></span>

<span data-ttu-id="c9405-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="c9405-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c9405-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="c9405-108">Attributes</span></span>

<span data-ttu-id="c9405-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="c9405-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c9405-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="c9405-110">Child elements</span></span>

|<span data-ttu-id="c9405-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="c9405-111">**Element**</span></span>|<span data-ttu-id="c9405-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="c9405-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c9405-113">Строка</span><span class="sxs-lookup"><span data-stu-id="c9405-113">String</span></span>](string.md) <br/> |<span data-ttu-id="c9405-114">Представляет строку, которые должны встречаться в свойстве **из** входящих сообщений в порядке для условие или исключение для применения.</span><span class="sxs-lookup"><span data-stu-id="c9405-114">Represents a string that must appear in the **From** property of incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="c9405-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="c9405-115">Parent elements</span></span>

|<span data-ttu-id="c9405-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="c9405-116">**Element**</span></span>|<span data-ttu-id="c9405-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="c9405-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c9405-118">Условия</span><span class="sxs-lookup"><span data-stu-id="c9405-118">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="c9405-119">Представляет условия, которые, если удовлетворены, запускают действия правила для правила.</span><span class="sxs-lookup"><span data-stu-id="c9405-119">Represents the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span>  <br/> |
|[<span data-ttu-id="c9405-120">Исключения</span><span class="sxs-lookup"><span data-stu-id="c9405-120">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="c9405-121">Представляет исключения, которые представляют все доступные правила условия исключений для правила папки «Входящие».</span><span class="sxs-lookup"><span data-stu-id="c9405-121">Represents the exceptions that represent all the available rule exception conditions for an Inbox rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="c9405-122">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="c9405-122">Text value</span></span>

<span data-ttu-id="c9405-123">Нет.</span><span class="sxs-lookup"><span data-stu-id="c9405-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="c9405-124">Замечания</span><span class="sxs-lookup"><span data-stu-id="c9405-124">Remarks</span></span>

<span data-ttu-id="c9405-125">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="c9405-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c9405-126">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="c9405-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c9405-127">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="c9405-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="c9405-128">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="c9405-128">Schema Name</span></span>  <br/> |<span data-ttu-id="c9405-129">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="c9405-129">Messages schema</span></span>  <br/> |
|<span data-ttu-id="c9405-130">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="c9405-130">Validation File</span></span>  <br/> |<span data-ttu-id="c9405-131">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="c9405-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="c9405-132">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="c9405-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="c9405-133">True</span><span class="sxs-lookup"><span data-stu-id="c9405-133">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c9405-134">См. также</span><span class="sxs-lookup"><span data-stu-id="c9405-134">See also</span></span>



- [<span data-ttu-id="c9405-135">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="c9405-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

