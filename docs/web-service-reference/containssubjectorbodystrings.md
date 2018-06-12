---
title: ContainsSubjectOrBodyStrings
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ContainsSubjectOrBodyStrings
api_type:
- schema
ms.assetid: 22aebf31-d9f4-4e03-bbff-c675409518d1
description: Элемент ContainsSubjectOrBodyStrings указывает строк, которые должны встречаться в тексте или теме входящих сообщений в порядке для условие или исключение для применения.
ms.openlocfilehash: f577e7d26bb7d82ea1017f720e1d3a30892e2ef1
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761775"
---
# <a name="containssubjectorbodystrings"></a><span data-ttu-id="0a5f1-103">ContainsSubjectOrBodyStrings</span><span class="sxs-lookup"><span data-stu-id="0a5f1-103">ContainsSubjectOrBodyStrings</span></span>

<span data-ttu-id="0a5f1-104">Элемент **ContainsSubjectOrBodyStrings** указывает строк, которые должны встречаться в тексте или теме входящих сообщений в порядке для условие или исключение для применения.</span><span class="sxs-lookup"><span data-stu-id="0a5f1-104">The **ContainsSubjectOrBodyStrings** element indicates the strings that must appear in either the body or the subject of incoming messages in order for the condition or exception to apply.</span></span> 
  
```XML
<ContainsSubjectOrBodyStrings>
    <String/>
</ContainsSubjectOrBodyStrings>
```

 <span data-ttu-id="0a5f1-105">**ArrayOfStringsType**</span><span class="sxs-lookup"><span data-stu-id="0a5f1-105">**ArrayOfStringsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0a5f1-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="0a5f1-106">Attributes and elements</span></span>

<span data-ttu-id="0a5f1-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="0a5f1-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0a5f1-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="0a5f1-108">Attributes</span></span>

<span data-ttu-id="0a5f1-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="0a5f1-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0a5f1-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="0a5f1-110">Child elements</span></span>

|<span data-ttu-id="0a5f1-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="0a5f1-111">**Element**</span></span>|<span data-ttu-id="0a5f1-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="0a5f1-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0a5f1-113">Строка</span><span class="sxs-lookup"><span data-stu-id="0a5f1-113">String</span></span>](string.md) <br/> |<span data-ttu-id="0a5f1-114">Представляет строку, которые должны встречаться в тексте или теме входящих сообщений в порядке для условие или исключение для применения.</span><span class="sxs-lookup"><span data-stu-id="0a5f1-114">Represents a string that must appear in either the body or the subject of incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="0a5f1-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="0a5f1-115">Parent elements</span></span>

|<span data-ttu-id="0a5f1-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="0a5f1-116">**Element**</span></span>|<span data-ttu-id="0a5f1-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="0a5f1-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0a5f1-118">Условия</span><span class="sxs-lookup"><span data-stu-id="0a5f1-118">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="0a5f1-119">Представляет условия, которые, если удовлетворены, запускают действия правила для правила.</span><span class="sxs-lookup"><span data-stu-id="0a5f1-119">Represents the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span>  <br/> |
|[<span data-ttu-id="0a5f1-120">Исключения</span><span class="sxs-lookup"><span data-stu-id="0a5f1-120">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="0a5f1-121">Представляет исключения, которые представляют все доступные правила условия исключений для правила папки «Входящие».</span><span class="sxs-lookup"><span data-stu-id="0a5f1-121">Represents the exceptions that represent all the available rule exception conditions for an Inbox rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="0a5f1-122">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="0a5f1-122">Text value</span></span>

<span data-ttu-id="0a5f1-123">Нет.</span><span class="sxs-lookup"><span data-stu-id="0a5f1-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="0a5f1-124">Замечания</span><span class="sxs-lookup"><span data-stu-id="0a5f1-124">Remarks</span></span>

<span data-ttu-id="0a5f1-125">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="0a5f1-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0a5f1-126">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="0a5f1-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0a5f1-127">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="0a5f1-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="0a5f1-128">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="0a5f1-128">Schema Name</span></span>  <br/> |<span data-ttu-id="0a5f1-129">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="0a5f1-129">Messages schema</span></span>  <br/> |
|<span data-ttu-id="0a5f1-130">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="0a5f1-130">Validation File</span></span>  <br/> |<span data-ttu-id="0a5f1-131">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="0a5f1-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="0a5f1-132">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="0a5f1-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="0a5f1-133">True</span><span class="sxs-lookup"><span data-stu-id="0a5f1-133">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0a5f1-134">См. также</span><span class="sxs-lookup"><span data-stu-id="0a5f1-134">See also</span></span>



- [<span data-ttu-id="0a5f1-135">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="0a5f1-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
