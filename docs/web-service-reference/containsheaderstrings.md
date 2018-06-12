---
title: ContainsHeaderStrings
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
description: Элемент ContainsHeaderStrings указывает строк, которые должны встречаться в заголовках входящих сообщений в порядке для условие или исключение для применения.
ms.openlocfilehash: 360870d63853a0e79f801cc2f17473b1a1b28c25
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761763"
---
# <a name="containsheaderstrings"></a><span data-ttu-id="dd57e-103">ContainsHeaderStrings</span><span class="sxs-lookup"><span data-stu-id="dd57e-103">ContainsHeaderStrings</span></span>

<span data-ttu-id="dd57e-104">Элемент **ContainsHeaderStrings** указывает строк, которые должны встречаться в заголовках входящих сообщений в порядке для условие или исключение для применения.</span><span class="sxs-lookup"><span data-stu-id="dd57e-104">The **ContainsHeaderStrings** element indicates the strings that must appear in the headers of incoming messages in order for the condition or exception to apply.</span></span> 
  
```XML
<ContainsHeaderStrings>
    <String/>
</ContainsHeaderStrings>
```

 <span data-ttu-id="dd57e-105">**ArrayOfStringsType**</span><span class="sxs-lookup"><span data-stu-id="dd57e-105">**ArrayOfStringsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="dd57e-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="dd57e-106">Attributes and elements</span></span>

<span data-ttu-id="dd57e-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="dd57e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="dd57e-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="dd57e-108">Attributes</span></span>

<span data-ttu-id="dd57e-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="dd57e-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="dd57e-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="dd57e-110">Child elements</span></span>

|<span data-ttu-id="dd57e-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="dd57e-111">**Element**</span></span>|<span data-ttu-id="dd57e-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="dd57e-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="dd57e-113">Строка</span><span class="sxs-lookup"><span data-stu-id="dd57e-113">String</span></span>](string.md) <br/> |<span data-ttu-id="dd57e-114">Представляет строку, которые должны встречаться в заголовки сообщений, чтобы условие или исключение можно применить.</span><span class="sxs-lookup"><span data-stu-id="dd57e-114">Represents a string that must appear in message headers in order for the condition or exception to apply.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="dd57e-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="dd57e-115">Parent elements</span></span>

|<span data-ttu-id="dd57e-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="dd57e-116">**Element**</span></span>|<span data-ttu-id="dd57e-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="dd57e-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="dd57e-118">Условия</span><span class="sxs-lookup"><span data-stu-id="dd57e-118">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="dd57e-119">Представляет условия, которые, если удовлетворены, запускают действия правила для правила.</span><span class="sxs-lookup"><span data-stu-id="dd57e-119">Represents the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span>  <br/> |
|[<span data-ttu-id="dd57e-120">Исключения</span><span class="sxs-lookup"><span data-stu-id="dd57e-120">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="dd57e-121">Представляет исключения, которые представляют все доступные правила условия исключений для правила папки «Входящие».</span><span class="sxs-lookup"><span data-stu-id="dd57e-121">Represents the exceptions that represent all the available rule exception conditions for an Inbox rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="dd57e-122">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="dd57e-122">Text value</span></span>

<span data-ttu-id="dd57e-123">Нет.</span><span class="sxs-lookup"><span data-stu-id="dd57e-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="dd57e-124">Замечания</span><span class="sxs-lookup"><span data-stu-id="dd57e-124">Remarks</span></span>

<span data-ttu-id="dd57e-125">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="dd57e-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="dd57e-126">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="dd57e-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="dd57e-127">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="dd57e-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="dd57e-128">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="dd57e-128">Schema Name</span></span>  <br/> |<span data-ttu-id="dd57e-129">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="dd57e-129">Messages schema</span></span>  <br/> |
|<span data-ttu-id="dd57e-130">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="dd57e-130">Validation File</span></span>  <br/> |<span data-ttu-id="dd57e-131">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="dd57e-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="dd57e-132">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="dd57e-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="dd57e-133">True</span><span class="sxs-lookup"><span data-stu-id="dd57e-133">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="dd57e-134">См. также</span><span class="sxs-lookup"><span data-stu-id="dd57e-134">See also</span></span>



- [<span data-ttu-id="dd57e-135">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="dd57e-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

