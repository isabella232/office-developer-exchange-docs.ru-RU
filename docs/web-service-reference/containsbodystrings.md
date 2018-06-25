---
title: ContainsBodyStrings
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ContainsBodyStrings
api_type:
- schema
ms.assetid: 70639472-64bb-456a-8b40-dce727542443
description: Элемент ContainsBodyStrings указывает строк, которые должны встречаться в теле входящих сообщений в порядке для условие или исключение для применения.
ms.openlocfilehash: 5993bd4061298e82a2393768eccb051326564e98
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761757"
---
# <a name="containsbodystrings"></a><span data-ttu-id="4c188-103">ContainsBodyStrings</span><span class="sxs-lookup"><span data-stu-id="4c188-103">ContainsBodyStrings</span></span>

<span data-ttu-id="4c188-104">Элемент **ContainsBodyStrings** указывает строк, которые должны встречаться в теле входящих сообщений в порядке для условие или исключение для применения.</span><span class="sxs-lookup"><span data-stu-id="4c188-104">The **ContainsBodyStrings** element indicates the strings that must appear in the body of incoming messages in order for the condition or exception to apply.</span></span> 
  
```XML
<ContainsBodyStrings>
    <String/>
</ContainsBodyStrings>
```

 <span data-ttu-id="4c188-105">**ArrayOfStringsType**</span><span class="sxs-lookup"><span data-stu-id="4c188-105">**ArrayOfStringsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4c188-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="4c188-106">Attributes and elements</span></span>

<span data-ttu-id="4c188-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="4c188-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4c188-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="4c188-108">Attributes</span></span>

<span data-ttu-id="4c188-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="4c188-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4c188-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="4c188-110">Child elements</span></span>

|<span data-ttu-id="4c188-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="4c188-111">**Element**</span></span>|<span data-ttu-id="4c188-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="4c188-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4c188-113">Строка</span><span class="sxs-lookup"><span data-stu-id="4c188-113">String</span></span>](string.md) <br/> |<span data-ttu-id="4c188-114">Представляет строку, которые должны встречаться в теле входящих сообщений в порядке для условие или исключение для применения.</span><span class="sxs-lookup"><span data-stu-id="4c188-114">Represents a string that must appear in the body of incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="4c188-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="4c188-115">Parent elements</span></span>

|<span data-ttu-id="4c188-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="4c188-116">**Element**</span></span>|<span data-ttu-id="4c188-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="4c188-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4c188-118">Условия</span><span class="sxs-lookup"><span data-stu-id="4c188-118">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="4c188-119">Представляет условия, которые, если удовлетворены, запускают действия правила для правила.</span><span class="sxs-lookup"><span data-stu-id="4c188-119">Represents the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span>  <br/> |
|[<span data-ttu-id="4c188-120">Исключения</span><span class="sxs-lookup"><span data-stu-id="4c188-120">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="4c188-121">Представляет исключения, которые представляют все доступные правила условия исключений для правила папки «Входящие».</span><span class="sxs-lookup"><span data-stu-id="4c188-121">Represents the exceptions that represent all the available rule exception conditions for an Inbox rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="4c188-122">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="4c188-122">Text value</span></span>

<span data-ttu-id="4c188-123">Нет.</span><span class="sxs-lookup"><span data-stu-id="4c188-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="4c188-124">Замечания</span><span class="sxs-lookup"><span data-stu-id="4c188-124">Remarks</span></span>

<span data-ttu-id="4c188-125">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="4c188-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4c188-126">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="4c188-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4c188-127">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="4c188-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="4c188-128">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="4c188-128">Schema Name</span></span>  <br/> |<span data-ttu-id="4c188-129">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="4c188-129">Messages schema</span></span>  <br/> |
|<span data-ttu-id="4c188-130">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="4c188-130">Validation File</span></span>  <br/> |<span data-ttu-id="4c188-131">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="4c188-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="4c188-132">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="4c188-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="4c188-133">True</span><span class="sxs-lookup"><span data-stu-id="4c188-133">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4c188-134">См. также</span><span class="sxs-lookup"><span data-stu-id="4c188-134">See also</span></span>



- [<span data-ttu-id="4c188-135">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="4c188-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

