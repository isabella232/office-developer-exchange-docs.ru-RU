---
title: Значение (Протектионрулевалуетипе)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Value
api_type:
- schema
ms.assetid: b039bd6e-2198-47cf-9c78-a5e8b9d51c98
description: Элемент value определяет одного получателя или отправителя.
ms.openlocfilehash: 6173f94dcfb83eafd62e35f185a5e8c669d50f6c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19840463"
---
# <a name="value-protectionrulevaluetype"></a><span data-ttu-id="c99e3-103">Значение (Протектионрулевалуетипе)</span><span class="sxs-lookup"><span data-stu-id="c99e3-103">Value (ProtectionRuleValueType)</span></span>

<span data-ttu-id="c99e3-104">Элемент **value** определяет одного получателя или отправителя.</span><span class="sxs-lookup"><span data-stu-id="c99e3-104">The **Value** element identifies a single recipient or sender department.</span></span> 
  
```XML
<Value/>
```

<span data-ttu-id="c99e3-105">**протектионрулевалуетипе**</span><span class="sxs-lookup"><span data-stu-id="c99e3-105">**ProtectionRuleValueType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="c99e3-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="c99e3-106">Attributes and elements</span></span>

<span data-ttu-id="c99e3-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="c99e3-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c99e3-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="c99e3-108">Attributes</span></span>

<span data-ttu-id="c99e3-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="c99e3-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c99e3-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="c99e3-110">Child elements</span></span>

<span data-ttu-id="c99e3-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="c99e3-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="c99e3-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="c99e3-112">Parent elements</span></span>

|<span data-ttu-id="c99e3-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="c99e3-113">**Element**</span></span>|<span data-ttu-id="c99e3-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="c99e3-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c99e3-115">Получательявляется</span><span class="sxs-lookup"><span data-stu-id="c99e3-115">RecipientIs</span></span>](recipientis.md) <br/> |<span data-ttu-id="c99e3-116">Указывает, что любой получатель сообщения электронной почты соответствует любому из указанных получателей в дочерних элементах **value** .</span><span class="sxs-lookup"><span data-stu-id="c99e3-116">Specifies that any recipient of the email message matches any of the specified recipients in the child **Value** elements.</span></span>  <br/> |
|[<span data-ttu-id="c99e3-117">сендердепартментс</span><span class="sxs-lookup"><span data-stu-id="c99e3-117">SenderDepartments</span></span>](senderdepartments.md) <br/> |<span data-ttu-id="c99e3-118">Указывает, что отдел отправителя соответствует любой из указанных отделов в дочерних элементах **value** .</span><span class="sxs-lookup"><span data-stu-id="c99e3-118">Specifies that the department of the sender matches any of the specified departments in the child **Value** elements.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="c99e3-119">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="c99e3-119">Text value</span></span>

<span data-ttu-id="c99e3-120">Этот элемент должен содержать непустое строковое значение.</span><span class="sxs-lookup"><span data-stu-id="c99e3-120">This element must contain a nonempty string value.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="c99e3-121">Примечания</span><span class="sxs-lookup"><span data-stu-id="c99e3-121">Remarks</span></span>

<span data-ttu-id="c99e3-122">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="c99e3-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c99e3-123">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="c99e3-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c99e3-124">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="c99e3-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="c99e3-125">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="c99e3-125">Schema Name</span></span>  <br/> |<span data-ttu-id="c99e3-126">Схема Types</span><span class="sxs-lookup"><span data-stu-id="c99e3-126">Types schema</span></span>  <br/> |
|<span data-ttu-id="c99e3-127">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="c99e3-127">Validation File</span></span>  <br/> |<span data-ttu-id="c99e3-128">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="c99e3-128">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="c99e3-129">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="c99e3-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="c99e3-130">False</span><span class="sxs-lookup"><span data-stu-id="c99e3-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c99e3-131">См. также</span><span class="sxs-lookup"><span data-stu-id="c99e3-131">See also</span></span>

- [<span data-ttu-id="c99e3-132">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="c99e3-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

