---
title: IsInError
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsInError
api_type:
- schema
ms.assetid: f56e6c31-a566-4761-8755-d90ffe6fe790
description: Элемент IsInError указывает, является ли правило в случае ошибки.
ms.openlocfilehash: 9f77bbe11106174d0e82c5257e08c3728d67c60c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834033"
---
# <a name="isinerror"></a><span data-ttu-id="9b8e8-103">IsInError</span><span class="sxs-lookup"><span data-stu-id="9b8e8-103">IsInError</span></span>

<span data-ttu-id="9b8e8-104">Элемент **IsInError** указывает, является ли правило в случае ошибки.</span><span class="sxs-lookup"><span data-stu-id="9b8e8-104">The **IsInError** element indicates whether the rule is in an error condition.</span></span> 
  
```XML
<IsInError/>
```

 <span data-ttu-id="9b8e8-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="9b8e8-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9b8e8-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="9b8e8-106">Attributes and elements</span></span>

<span data-ttu-id="9b8e8-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="9b8e8-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9b8e8-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="9b8e8-108">Attributes</span></span>

<span data-ttu-id="9b8e8-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="9b8e8-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9b8e8-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="9b8e8-110">Child elements</span></span>

<span data-ttu-id="9b8e8-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="9b8e8-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="9b8e8-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="9b8e8-112">Parent elements</span></span>

|<span data-ttu-id="9b8e8-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="9b8e8-113">**Element**</span></span>|<span data-ttu-id="9b8e8-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="9b8e8-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9b8e8-115">Правило (RuleType)</span><span class="sxs-lookup"><span data-stu-id="9b8e8-115">Rule (RuleType)</span></span>](rule-ruletype.md) <br/> |<span data-ttu-id="9b8e8-116">Представляет правило в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="9b8e8-116">Represents a rule in the user's mailbox.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="9b8e8-117">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="9b8e8-117">Text value</span></span>

<span data-ttu-id="9b8e8-118">Текстовое значение **true,** указывает, что правило в случае ошибки.</span><span class="sxs-lookup"><span data-stu-id="9b8e8-118">A text value of **true** indicates that the rule is in an error condition.</span></span> <span data-ttu-id="9b8e8-119">Значение **false** указывает, что правило не является в случае ошибки.</span><span class="sxs-lookup"><span data-stu-id="9b8e8-119">A value of **false** indicates that the rule is not in an error condition.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="9b8e8-120">Замечания</span><span class="sxs-lookup"><span data-stu-id="9b8e8-120">Remarks</span></span>

<span data-ttu-id="9b8e8-121">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="9b8e8-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9b8e8-122">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="9b8e8-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9b8e8-123">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="9b8e8-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="9b8e8-124">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="9b8e8-124">Schema Name</span></span>  <br/> |<span data-ttu-id="9b8e8-125">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="9b8e8-125">Messages schema</span></span>  <br/> |
|<span data-ttu-id="9b8e8-126">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="9b8e8-126">Validation File</span></span>  <br/> |<span data-ttu-id="9b8e8-127">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="9b8e8-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="9b8e8-128">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="9b8e8-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="9b8e8-129">True</span><span class="sxs-lookup"><span data-stu-id="9b8e8-129">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9b8e8-130">См. также</span><span class="sxs-lookup"><span data-stu-id="9b8e8-130">See also</span></span>



- [<span data-ttu-id="9b8e8-131">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="9b8e8-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

