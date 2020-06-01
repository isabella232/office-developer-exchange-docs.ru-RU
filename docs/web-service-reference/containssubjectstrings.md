---
title: контаинссубжектстрингс
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
description: Элемент Контаинссубжектстрингс указывает строки, которые должны присутствовать в теме входящих сообщений, чтобы применить условие или исключение.
ms.openlocfilehash: 8b078f61d08864970a123f81688981ffba2864ff
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458959"
---
# <a name="containssubjectstrings"></a><span data-ttu-id="41d15-103">контаинссубжектстрингс</span><span class="sxs-lookup"><span data-stu-id="41d15-103">ContainsSubjectStrings</span></span>

<span data-ttu-id="41d15-104">Элемент **контаинссубжектстрингс** указывает строки, которые должны присутствовать в теме входящих сообщений, чтобы применить условие или исключение.</span><span class="sxs-lookup"><span data-stu-id="41d15-104">The **ContainsSubjectStrings** element indicates the strings that must appear in the subject of incoming messages in order for the condition or exception to apply.</span></span> 
  
```XML
<ContainsSubjectStrings>
    <String/>
</ContainsSubjectStrings>
```

 <span data-ttu-id="41d15-105">**аррайофстрингстипе**</span><span class="sxs-lookup"><span data-stu-id="41d15-105">**ArrayOfStringsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="41d15-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="41d15-106">Attributes and elements</span></span>

<span data-ttu-id="41d15-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="41d15-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="41d15-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="41d15-108">Attributes</span></span>

<span data-ttu-id="41d15-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="41d15-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="41d15-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="41d15-110">Child elements</span></span>

|<span data-ttu-id="41d15-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="41d15-111">**Element**</span></span>|<span data-ttu-id="41d15-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="41d15-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="41d15-113">Строка</span><span class="sxs-lookup"><span data-stu-id="41d15-113">String</span></span>](string.md) <br/> |<span data-ttu-id="41d15-114">Представляет строку, которая должна отображаться в теме входящих сообщений, чтобы применить условие или исключение.</span><span class="sxs-lookup"><span data-stu-id="41d15-114">Represents a string that must appear in the subject of incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="41d15-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="41d15-115">Parent elements</span></span>

|<span data-ttu-id="41d15-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="41d15-116">**Element**</span></span>|<span data-ttu-id="41d15-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="41d15-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="41d15-118">Условия</span><span class="sxs-lookup"><span data-stu-id="41d15-118">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="41d15-119">Представляет условия, которые, если удовлетворены, запускают действия правила для правила.</span><span class="sxs-lookup"><span data-stu-id="41d15-119">Represents the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span>  <br/> |
|[<span data-ttu-id="41d15-120">Исключения</span><span class="sxs-lookup"><span data-stu-id="41d15-120">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="41d15-121">Представляет исключения, которые представляют все доступные правила условия исключений для правила папки «Входящие».</span><span class="sxs-lookup"><span data-stu-id="41d15-121">Represents the exceptions that represent all the available rule exception conditions for an Inbox rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="41d15-122">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="41d15-122">Text value</span></span>

<span data-ttu-id="41d15-123">Нет.</span><span class="sxs-lookup"><span data-stu-id="41d15-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="41d15-124">Примечания</span><span class="sxs-lookup"><span data-stu-id="41d15-124">Remarks</span></span>

<span data-ttu-id="41d15-125">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="41d15-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="41d15-126">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="41d15-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="41d15-127">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="41d15-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="41d15-128">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="41d15-128">Schema Name</span></span>  <br/> |<span data-ttu-id="41d15-129">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="41d15-129">Messages schema</span></span>  <br/> |
|<span data-ttu-id="41d15-130">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="41d15-130">Validation File</span></span>  <br/> |<span data-ttu-id="41d15-131">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="41d15-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="41d15-132">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="41d15-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="41d15-133">True</span><span class="sxs-lookup"><span data-stu-id="41d15-133">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="41d15-134">См. также</span><span class="sxs-lookup"><span data-stu-id="41d15-134">See also</span></span>



- [<span data-ttu-id="41d15-135">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="41d15-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

