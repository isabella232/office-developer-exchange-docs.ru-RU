---
title: контаиншеадерстрингс
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
description: Элемент Контаиншеадерстрингс указывает строки, которые должны отображаться в заголовках входящих сообщений, чтобы применялось условие или исключение.
ms.openlocfilehash: 23e3d0e7cff9c78edbac10a6275514af93cab325
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458994"
---
# <a name="containsheaderstrings"></a><span data-ttu-id="80cbc-103">контаиншеадерстрингс</span><span class="sxs-lookup"><span data-stu-id="80cbc-103">ContainsHeaderStrings</span></span>

<span data-ttu-id="80cbc-104">Элемент **контаиншеадерстрингс** указывает строки, которые должны отображаться в заголовках входящих сообщений, чтобы применялось условие или исключение.</span><span class="sxs-lookup"><span data-stu-id="80cbc-104">The **ContainsHeaderStrings** element indicates the strings that must appear in the headers of incoming messages in order for the condition or exception to apply.</span></span> 
  
```XML
<ContainsHeaderStrings>
    <String/>
</ContainsHeaderStrings>
```

 <span data-ttu-id="80cbc-105">**аррайофстрингстипе**</span><span class="sxs-lookup"><span data-stu-id="80cbc-105">**ArrayOfStringsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="80cbc-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="80cbc-106">Attributes and elements</span></span>

<span data-ttu-id="80cbc-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="80cbc-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="80cbc-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="80cbc-108">Attributes</span></span>

<span data-ttu-id="80cbc-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="80cbc-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="80cbc-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="80cbc-110">Child elements</span></span>

|<span data-ttu-id="80cbc-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="80cbc-111">**Element**</span></span>|<span data-ttu-id="80cbc-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="80cbc-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="80cbc-113">Строка</span><span class="sxs-lookup"><span data-stu-id="80cbc-113">String</span></span>](string.md) <br/> |<span data-ttu-id="80cbc-114">Представляет строку, которая должна присутствовать в заголовках сообщений, чтобы применить условие или исключение.</span><span class="sxs-lookup"><span data-stu-id="80cbc-114">Represents a string that must appear in message headers in order for the condition or exception to apply.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="80cbc-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="80cbc-115">Parent elements</span></span>

|<span data-ttu-id="80cbc-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="80cbc-116">**Element**</span></span>|<span data-ttu-id="80cbc-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="80cbc-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="80cbc-118">Условия</span><span class="sxs-lookup"><span data-stu-id="80cbc-118">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="80cbc-119">Представляет условия, которые, если удовлетворены, запускают действия правила для правила.</span><span class="sxs-lookup"><span data-stu-id="80cbc-119">Represents the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span>  <br/> |
|[<span data-ttu-id="80cbc-120">Исключения</span><span class="sxs-lookup"><span data-stu-id="80cbc-120">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="80cbc-121">Представляет исключения, которые представляют все доступные правила условия исключений для правила папки «Входящие».</span><span class="sxs-lookup"><span data-stu-id="80cbc-121">Represents the exceptions that represent all the available rule exception conditions for an Inbox rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="80cbc-122">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="80cbc-122">Text value</span></span>

<span data-ttu-id="80cbc-123">Нет.</span><span class="sxs-lookup"><span data-stu-id="80cbc-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="80cbc-124">Примечания</span><span class="sxs-lookup"><span data-stu-id="80cbc-124">Remarks</span></span>

<span data-ttu-id="80cbc-125">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="80cbc-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="80cbc-126">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="80cbc-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="80cbc-127">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="80cbc-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="80cbc-128">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="80cbc-128">Schema Name</span></span>  <br/> |<span data-ttu-id="80cbc-129">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="80cbc-129">Messages schema</span></span>  <br/> |
|<span data-ttu-id="80cbc-130">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="80cbc-130">Validation File</span></span>  <br/> |<span data-ttu-id="80cbc-131">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="80cbc-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="80cbc-132">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="80cbc-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="80cbc-133">True</span><span class="sxs-lookup"><span data-stu-id="80cbc-133">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="80cbc-134">См. также</span><span class="sxs-lookup"><span data-stu-id="80cbc-134">See also</span></span>



- [<span data-ttu-id="80cbc-135">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="80cbc-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

