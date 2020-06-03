---
title: контаинсреЦипиентстрингс
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
description: Элемент КонтаинсреЦипиентстрингс указывает строки, которые должны отображаться в свойствах ToRecipients или CcRecipients входящих сообщений, чтобы применялось условие или исключение.
ms.openlocfilehash: ba717de6b3c53b37d12c4c0be8301083b2080c8b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458987"
---
# <a name="containsrecipientstrings"></a><span data-ttu-id="70fa3-103">контаинсреЦипиентстрингс</span><span class="sxs-lookup"><span data-stu-id="70fa3-103">ContainsRecipientStrings</span></span>

<span data-ttu-id="70fa3-104">Элемент **контаинсреЦипиентстрингс** указывает строки, которые должны отображаться в свойствах **ToRecipients** или **CcRecipients** входящих сообщений, чтобы применялось условие или исключение.</span><span class="sxs-lookup"><span data-stu-id="70fa3-104">The **ContainsRecipientStrings** element indicates the strings that must appear in either the **ToRecipients** or **CcRecipients** properties of incoming messages in order for the condition or exception to apply.</span></span> 
  
```XML
<ContainsRecipientStrings>
    <String/>
</ContainsRecipientStrings>
```

 <span data-ttu-id="70fa3-105">**аррайофстрингстипе**</span><span class="sxs-lookup"><span data-stu-id="70fa3-105">**ArrayOfStringsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="70fa3-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="70fa3-106">Attributes and elements</span></span>

<span data-ttu-id="70fa3-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="70fa3-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="70fa3-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="70fa3-108">Attributes</span></span>

<span data-ttu-id="70fa3-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="70fa3-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="70fa3-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="70fa3-110">Child elements</span></span>

|<span data-ttu-id="70fa3-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="70fa3-111">**Element**</span></span>|<span data-ttu-id="70fa3-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="70fa3-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="70fa3-113">Строка</span><span class="sxs-lookup"><span data-stu-id="70fa3-113">String</span></span>](string.md) <br/> |<span data-ttu-id="70fa3-114">Представляет строку, которая должна отображаться в свойствах **ToRecipients** или **CcRecipients** входящих сообщений, чтобы применялось условие или исключение.</span><span class="sxs-lookup"><span data-stu-id="70fa3-114">Represents a string that must appear in either the **ToRecipients** or **CcRecipients** properties of incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="70fa3-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="70fa3-115">Parent elements</span></span>

|<span data-ttu-id="70fa3-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="70fa3-116">**Element**</span></span>|<span data-ttu-id="70fa3-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="70fa3-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="70fa3-118">Условия</span><span class="sxs-lookup"><span data-stu-id="70fa3-118">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="70fa3-119">Представляет условия, которые, если удовлетворены, запускают действия правила для правила.</span><span class="sxs-lookup"><span data-stu-id="70fa3-119">Represents the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span>  <br/> |
|[<span data-ttu-id="70fa3-120">Исключения</span><span class="sxs-lookup"><span data-stu-id="70fa3-120">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="70fa3-121">Представляет исключения, которые представляют все доступные правила условия исключений для правила папки «Входящие».</span><span class="sxs-lookup"><span data-stu-id="70fa3-121">Represents the exceptions that represent all the available rule exception conditions for an Inbox rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="70fa3-122">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="70fa3-122">Text value</span></span>

<span data-ttu-id="70fa3-123">Нет.</span><span class="sxs-lookup"><span data-stu-id="70fa3-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="70fa3-124">Примечания</span><span class="sxs-lookup"><span data-stu-id="70fa3-124">Remarks</span></span>

<span data-ttu-id="70fa3-125">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="70fa3-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="70fa3-126">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="70fa3-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="70fa3-127">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="70fa3-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="70fa3-128">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="70fa3-128">Schema Name</span></span>  <br/> |<span data-ttu-id="70fa3-129">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="70fa3-129">Messages schema</span></span>  <br/> |
|<span data-ttu-id="70fa3-130">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="70fa3-130">Validation File</span></span>  <br/> |<span data-ttu-id="70fa3-131">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="70fa3-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="70fa3-132">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="70fa3-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="70fa3-133">True</span><span class="sxs-lookup"><span data-stu-id="70fa3-133">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="70fa3-134">См. также</span><span class="sxs-lookup"><span data-stu-id="70fa3-134">See also</span></span>



- [<span data-ttu-id="70fa3-135">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="70fa3-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

