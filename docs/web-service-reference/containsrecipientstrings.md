---
title: ContainsRecipientStrings
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ContainsRecipientStrings
api_type:
- schema
ms.assetid: a7fd13ac-0f13-4610-ac9b-98e27ac3940b
description: Элемент ContainsRecipientStrings указывает строк, которые должны встречаться в ToRecipients или CcRecipients свойства входящих сообщений в порядке для условие или исключение для применения.
ms.openlocfilehash: 861aba22c9474caf02f9c50d8a7b65b9cc8a2eda
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761759"
---
# <a name="containsrecipientstrings"></a><span data-ttu-id="e1deb-103">ContainsRecipientStrings</span><span class="sxs-lookup"><span data-stu-id="e1deb-103">ContainsRecipientStrings</span></span>

<span data-ttu-id="e1deb-104">Элемент **ContainsRecipientStrings** указывает строк, которые должны встречаться в параметр **ToRecipients** или **CcRecipients** свойства входящих сообщений в порядке для условие или исключение для применения.</span><span class="sxs-lookup"><span data-stu-id="e1deb-104">The **ContainsRecipientStrings** element indicates the strings that must appear in either the **ToRecipients** or **CcRecipients** properties of incoming messages in order for the condition or exception to apply.</span></span> 
  
```XML
<ContainsRecipientStrings>
    <String/>
</ContainsRecipientStrings>
```

 <span data-ttu-id="e1deb-105">**ArrayOfStringsType**</span><span class="sxs-lookup"><span data-stu-id="e1deb-105">**ArrayOfStringsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e1deb-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="e1deb-106">Attributes and elements</span></span>

<span data-ttu-id="e1deb-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="e1deb-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e1deb-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="e1deb-108">Attributes</span></span>

<span data-ttu-id="e1deb-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="e1deb-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e1deb-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="e1deb-110">Child elements</span></span>

|<span data-ttu-id="e1deb-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="e1deb-111">**Element**</span></span>|<span data-ttu-id="e1deb-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="e1deb-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e1deb-113">Строка</span><span class="sxs-lookup"><span data-stu-id="e1deb-113">String</span></span>](string.md) <br/> |<span data-ttu-id="e1deb-114">Представляет строку, которые должны встречаться в параметр **ToRecipients** или **CcRecipients** свойства входящих сообщений в порядке для условие или исключение для применения.</span><span class="sxs-lookup"><span data-stu-id="e1deb-114">Represents a string that must appear in either the **ToRecipients** or **CcRecipients** properties of incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="e1deb-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="e1deb-115">Parent elements</span></span>

|<span data-ttu-id="e1deb-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="e1deb-116">**Element**</span></span>|<span data-ttu-id="e1deb-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="e1deb-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e1deb-118">Условия</span><span class="sxs-lookup"><span data-stu-id="e1deb-118">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="e1deb-119">Представляет условия, которые, если удовлетворены, запускают действия правила для правила.</span><span class="sxs-lookup"><span data-stu-id="e1deb-119">Represents the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span>  <br/> |
|[<span data-ttu-id="e1deb-120">Исключения</span><span class="sxs-lookup"><span data-stu-id="e1deb-120">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="e1deb-121">Представляет исключения, которые представляют все доступные правила условия исключений для правила папки «Входящие».</span><span class="sxs-lookup"><span data-stu-id="e1deb-121">Represents the exceptions that represent all the available rule exception conditions for an Inbox rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="e1deb-122">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="e1deb-122">Text value</span></span>

<span data-ttu-id="e1deb-123">Нет.</span><span class="sxs-lookup"><span data-stu-id="e1deb-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="e1deb-124">Замечания</span><span class="sxs-lookup"><span data-stu-id="e1deb-124">Remarks</span></span>

<span data-ttu-id="e1deb-125">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="e1deb-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e1deb-126">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="e1deb-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e1deb-127">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="e1deb-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="e1deb-128">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="e1deb-128">Schema Name</span></span>  <br/> |<span data-ttu-id="e1deb-129">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="e1deb-129">Messages schema</span></span>  <br/> |
|<span data-ttu-id="e1deb-130">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="e1deb-130">Validation File</span></span>  <br/> |<span data-ttu-id="e1deb-131">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="e1deb-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="e1deb-132">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="e1deb-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="e1deb-133">True</span><span class="sxs-lookup"><span data-stu-id="e1deb-133">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e1deb-134">См. также</span><span class="sxs-lookup"><span data-stu-id="e1deb-134">See also</span></span>



- [<span data-ttu-id="e1deb-135">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="e1deb-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

