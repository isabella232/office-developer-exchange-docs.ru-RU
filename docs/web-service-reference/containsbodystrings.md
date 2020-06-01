---
title: контаинсбодистрингс
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
description: Элемент Контаинсбодистрингс указывает строки, которые должны присутствовать в теле входящих сообщений, чтобы применить условие или исключение.
ms.openlocfilehash: 008261ab94b1bed33cc72cacf7abe7aa58927d1a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463806"
---
# <a name="containsbodystrings"></a><span data-ttu-id="1d6ad-103">контаинсбодистрингс</span><span class="sxs-lookup"><span data-stu-id="1d6ad-103">ContainsBodyStrings</span></span>

<span data-ttu-id="1d6ad-104">Элемент **контаинсбодистрингс** указывает строки, которые должны присутствовать в теле входящих сообщений, чтобы применить условие или исключение.</span><span class="sxs-lookup"><span data-stu-id="1d6ad-104">The **ContainsBodyStrings** element indicates the strings that must appear in the body of incoming messages in order for the condition or exception to apply.</span></span> 
  
```XML
<ContainsBodyStrings>
    <String/>
</ContainsBodyStrings>
```

 <span data-ttu-id="1d6ad-105">**аррайофстрингстипе**</span><span class="sxs-lookup"><span data-stu-id="1d6ad-105">**ArrayOfStringsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1d6ad-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="1d6ad-106">Attributes and elements</span></span>

<span data-ttu-id="1d6ad-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="1d6ad-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1d6ad-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="1d6ad-108">Attributes</span></span>

<span data-ttu-id="1d6ad-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="1d6ad-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1d6ad-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="1d6ad-110">Child elements</span></span>

|<span data-ttu-id="1d6ad-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="1d6ad-111">**Element**</span></span>|<span data-ttu-id="1d6ad-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="1d6ad-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1d6ad-113">Строка</span><span class="sxs-lookup"><span data-stu-id="1d6ad-113">String</span></span>](string.md) <br/> |<span data-ttu-id="1d6ad-114">Представляет строку, которая должна находиться в теле входящих сообщений, чтобы применить условие или исключение.</span><span class="sxs-lookup"><span data-stu-id="1d6ad-114">Represents a string that must appear in the body of incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="1d6ad-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="1d6ad-115">Parent elements</span></span>

|<span data-ttu-id="1d6ad-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="1d6ad-116">**Element**</span></span>|<span data-ttu-id="1d6ad-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="1d6ad-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1d6ad-118">Условия</span><span class="sxs-lookup"><span data-stu-id="1d6ad-118">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="1d6ad-119">Представляет условия, которые, если удовлетворены, запускают действия правила для правила.</span><span class="sxs-lookup"><span data-stu-id="1d6ad-119">Represents the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span>  <br/> |
|[<span data-ttu-id="1d6ad-120">Исключения</span><span class="sxs-lookup"><span data-stu-id="1d6ad-120">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="1d6ad-121">Представляет исключения, которые представляют все доступные правила условия исключений для правила папки «Входящие».</span><span class="sxs-lookup"><span data-stu-id="1d6ad-121">Represents the exceptions that represent all the available rule exception conditions for an Inbox rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="1d6ad-122">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="1d6ad-122">Text value</span></span>

<span data-ttu-id="1d6ad-123">Нет.</span><span class="sxs-lookup"><span data-stu-id="1d6ad-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="1d6ad-124">Примечания</span><span class="sxs-lookup"><span data-stu-id="1d6ad-124">Remarks</span></span>

<span data-ttu-id="1d6ad-125">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="1d6ad-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1d6ad-126">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="1d6ad-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1d6ad-127">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="1d6ad-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="1d6ad-128">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="1d6ad-128">Schema Name</span></span>  <br/> |<span data-ttu-id="1d6ad-129">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="1d6ad-129">Messages schema</span></span>  <br/> |
|<span data-ttu-id="1d6ad-130">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="1d6ad-130">Validation File</span></span>  <br/> |<span data-ttu-id="1d6ad-131">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="1d6ad-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="1d6ad-132">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="1d6ad-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="1d6ad-133">True</span><span class="sxs-lookup"><span data-stu-id="1d6ad-133">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1d6ad-134">См. также</span><span class="sxs-lookup"><span data-stu-id="1d6ad-134">See also</span></span>



- [<span data-ttu-id="1d6ad-135">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="1d6ad-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

