---
title: контаинссубжекторбодистрингс
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
description: Элемент Контаинссубжекторбодистрингс указывает строки, которые должны присутствовать в тексте или теме входящих сообщений, чтобы применить условие или исключение.
ms.openlocfilehash: 6f9c7862912632e7e86a0b704e760c7fd0f5f14c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44466824"
---
# <a name="containssubjectorbodystrings"></a><span data-ttu-id="362fb-103">контаинссубжекторбодистрингс</span><span class="sxs-lookup"><span data-stu-id="362fb-103">ContainsSubjectOrBodyStrings</span></span>

<span data-ttu-id="362fb-104">Элемент **контаинссубжекторбодистрингс** указывает строки, которые должны присутствовать в тексте или теме входящих сообщений, чтобы применить условие или исключение.</span><span class="sxs-lookup"><span data-stu-id="362fb-104">The **ContainsSubjectOrBodyStrings** element indicates the strings that must appear in either the body or the subject of incoming messages in order for the condition or exception to apply.</span></span> 
  
```XML
<ContainsSubjectOrBodyStrings>
    <String/>
</ContainsSubjectOrBodyStrings>
```

 <span data-ttu-id="362fb-105">**аррайофстрингстипе**</span><span class="sxs-lookup"><span data-stu-id="362fb-105">**ArrayOfStringsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="362fb-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="362fb-106">Attributes and elements</span></span>

<span data-ttu-id="362fb-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="362fb-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="362fb-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="362fb-108">Attributes</span></span>

<span data-ttu-id="362fb-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="362fb-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="362fb-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="362fb-110">Child elements</span></span>

|<span data-ttu-id="362fb-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="362fb-111">**Element**</span></span>|<span data-ttu-id="362fb-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="362fb-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="362fb-113">Строка</span><span class="sxs-lookup"><span data-stu-id="362fb-113">String</span></span>](string.md) <br/> |<span data-ttu-id="362fb-114">Представляет строку, которая должна присутствовать в тексте или теме входящих сообщений, чтобы применить условие или исключение.</span><span class="sxs-lookup"><span data-stu-id="362fb-114">Represents a string that must appear in either the body or the subject of incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="362fb-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="362fb-115">Parent elements</span></span>

|<span data-ttu-id="362fb-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="362fb-116">**Element**</span></span>|<span data-ttu-id="362fb-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="362fb-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="362fb-118">Условия</span><span class="sxs-lookup"><span data-stu-id="362fb-118">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="362fb-119">Представляет условия, которые, если удовлетворены, запускают действия правила для правила.</span><span class="sxs-lookup"><span data-stu-id="362fb-119">Represents the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span>  <br/> |
|[<span data-ttu-id="362fb-120">Исключения</span><span class="sxs-lookup"><span data-stu-id="362fb-120">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="362fb-121">Представляет исключения, которые представляют все доступные правила условия исключений для правила папки «Входящие».</span><span class="sxs-lookup"><span data-stu-id="362fb-121">Represents the exceptions that represent all the available rule exception conditions for an Inbox rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="362fb-122">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="362fb-122">Text value</span></span>

<span data-ttu-id="362fb-123">Нет.</span><span class="sxs-lookup"><span data-stu-id="362fb-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="362fb-124">Примечания</span><span class="sxs-lookup"><span data-stu-id="362fb-124">Remarks</span></span>

<span data-ttu-id="362fb-125">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="362fb-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="362fb-126">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="362fb-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="362fb-127">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="362fb-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="362fb-128">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="362fb-128">Schema Name</span></span>  <br/> |<span data-ttu-id="362fb-129">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="362fb-129">Messages schema</span></span>  <br/> |
|<span data-ttu-id="362fb-130">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="362fb-130">Validation File</span></span>  <br/> |<span data-ttu-id="362fb-131">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="362fb-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="362fb-132">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="362fb-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="362fb-133">True</span><span class="sxs-lookup"><span data-stu-id="362fb-133">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="362fb-134">См. также</span><span class="sxs-lookup"><span data-stu-id="362fb-134">See also</span></span>



- [<span data-ttu-id="362fb-135">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="362fb-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

