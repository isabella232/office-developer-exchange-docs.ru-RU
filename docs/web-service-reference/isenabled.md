---
title: IsEnabled
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsEnabled
api_type:
- schema
ms.assetid: c7e3035e-a4ef-4c11-8cb0-214790a554ff
description: Элемент Enable указывает, включено ли правило.
ms.openlocfilehash: d0f0a77ec1ec952ac1cd9d9ad686ccfcb8f70c42
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834000"
---
# <a name="isenabled"></a><span data-ttu-id="667f1-103">IsEnabled</span><span class="sxs-lookup"><span data-stu-id="667f1-103">IsEnabled</span></span>

<span data-ttu-id="667f1-104">Элемент **Enable** указывает, включено ли правило.</span><span class="sxs-lookup"><span data-stu-id="667f1-104">The **IsEnabled** element indicates whether the rule is enabled.</span></span> 
  
```XML
<IsEnabled/>
```

 <span data-ttu-id="667f1-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="667f1-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="667f1-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="667f1-106">Attributes and elements</span></span>

<span data-ttu-id="667f1-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="667f1-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="667f1-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="667f1-108">Attributes</span></span>

<span data-ttu-id="667f1-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="667f1-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="667f1-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="667f1-110">Child elements</span></span>

<span data-ttu-id="667f1-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="667f1-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="667f1-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="667f1-112">Parent elements</span></span>

|<span data-ttu-id="667f1-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="667f1-113">**Element**</span></span>|<span data-ttu-id="667f1-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="667f1-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="667f1-115">Правило (RuleType)</span><span class="sxs-lookup"><span data-stu-id="667f1-115">Rule (RuleType)</span></span>](rule-ruletype.md) <br/> |<span data-ttu-id="667f1-116">Представляет правило в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="667f1-116">Represents a rule in the user's mailbox.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="667f1-117">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="667f1-117">Text value</span></span>

<span data-ttu-id="667f1-118">Текстовое значение **true** указывает, что правило включено и может быть выполнено.</span><span class="sxs-lookup"><span data-stu-id="667f1-118">A text value of **true** indicates that the rule is enabled and can be executed.</span></span> <span data-ttu-id="667f1-119">Значение **false** указывает, что правило не может быть выполнено.</span><span class="sxs-lookup"><span data-stu-id="667f1-119">A value of **false** indicates that the rule cannot be executed.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="667f1-120">Примечания</span><span class="sxs-lookup"><span data-stu-id="667f1-120">Remarks</span></span>

<span data-ttu-id="667f1-121">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="667f1-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="667f1-122">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="667f1-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="667f1-123">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="667f1-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="667f1-124">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="667f1-124">Schema Name</span></span>  <br/> |<span data-ttu-id="667f1-125">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="667f1-125">Messages schema</span></span>  <br/> |
|<span data-ttu-id="667f1-126">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="667f1-126">Validation File</span></span>  <br/> |<span data-ttu-id="667f1-127">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="667f1-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="667f1-128">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="667f1-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="667f1-129">True</span><span class="sxs-lookup"><span data-stu-id="667f1-129">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="667f1-130">См. также</span><span class="sxs-lookup"><span data-stu-id="667f1-130">See also</span></span>



- [<span data-ttu-id="667f1-131">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="667f1-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

