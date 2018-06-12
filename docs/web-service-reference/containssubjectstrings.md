---
title: ContainsSubjectStrings
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ContainsSubjectStrings
api_type:
- schema
ms.assetid: c6ec1d8d-8dd8-4c9a-a3e1-50e24958eb0d
description: Элемент ContainsSubjectStrings указывает строк, которые должны встречаться в теме входящих сообщений в порядке для условие или исключение для применения.
ms.openlocfilehash: a266855effaeb34aa232305db970f97c309a2e4c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761786"
---
# <a name="containssubjectstrings"></a><span data-ttu-id="60fba-103">ContainsSubjectStrings</span><span class="sxs-lookup"><span data-stu-id="60fba-103">ContainsSubjectStrings</span></span>

<span data-ttu-id="60fba-104">Элемент **ContainsSubjectStrings** указывает строк, которые должны встречаться в теме входящих сообщений в порядке для условие или исключение для применения.</span><span class="sxs-lookup"><span data-stu-id="60fba-104">The **ContainsSubjectStrings** element indicates the strings that must appear in the subject of incoming messages in order for the condition or exception to apply.</span></span> 
  
```XML
<ContainsSubjectStrings>
    <String/>
</ContainsSubjectStrings>
```

 <span data-ttu-id="60fba-105">**ArrayOfStringsType**</span><span class="sxs-lookup"><span data-stu-id="60fba-105">**ArrayOfStringsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="60fba-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="60fba-106">Attributes and elements</span></span>

<span data-ttu-id="60fba-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="60fba-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="60fba-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="60fba-108">Attributes</span></span>

<span data-ttu-id="60fba-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="60fba-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="60fba-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="60fba-110">Child elements</span></span>

|<span data-ttu-id="60fba-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="60fba-111">**Element**</span></span>|<span data-ttu-id="60fba-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="60fba-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="60fba-113">Строка</span><span class="sxs-lookup"><span data-stu-id="60fba-113">String</span></span>](string.md) <br/> |<span data-ttu-id="60fba-114">Представляет строку, которые должны встречаться в теме входящих сообщений в порядке для условие или исключение для применения.</span><span class="sxs-lookup"><span data-stu-id="60fba-114">Represents a string that must appear in the subject of incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="60fba-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="60fba-115">Parent elements</span></span>

|<span data-ttu-id="60fba-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="60fba-116">**Element**</span></span>|<span data-ttu-id="60fba-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="60fba-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="60fba-118">Условия</span><span class="sxs-lookup"><span data-stu-id="60fba-118">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="60fba-119">Представляет условия, которые, если удовлетворены, запускают действия правила для правила.</span><span class="sxs-lookup"><span data-stu-id="60fba-119">Represents the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span>  <br/> |
|[<span data-ttu-id="60fba-120">Исключения</span><span class="sxs-lookup"><span data-stu-id="60fba-120">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="60fba-121">Представляет исключения, которые представляют все доступные правила условия исключений для правила папки «Входящие».</span><span class="sxs-lookup"><span data-stu-id="60fba-121">Represents the exceptions that represent all the available rule exception conditions for an Inbox rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="60fba-122">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="60fba-122">Text value</span></span>

<span data-ttu-id="60fba-123">Нет.</span><span class="sxs-lookup"><span data-stu-id="60fba-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="60fba-124">Замечания</span><span class="sxs-lookup"><span data-stu-id="60fba-124">Remarks</span></span>

<span data-ttu-id="60fba-125">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="60fba-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="60fba-126">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="60fba-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="60fba-127">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="60fba-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="60fba-128">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="60fba-128">Schema Name</span></span>  <br/> |<span data-ttu-id="60fba-129">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="60fba-129">Messages schema</span></span>  <br/> |
|<span data-ttu-id="60fba-130">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="60fba-130">Validation File</span></span>  <br/> |<span data-ttu-id="60fba-131">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="60fba-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="60fba-132">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="60fba-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="60fba-133">True</span><span class="sxs-lookup"><span data-stu-id="60fba-133">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="60fba-134">См. также</span><span class="sxs-lookup"><span data-stu-id="60fba-134">See also</span></span>



- [<span data-ttu-id="60fba-135">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="60fba-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

