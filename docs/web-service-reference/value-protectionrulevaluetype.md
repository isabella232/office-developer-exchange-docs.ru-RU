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
ms.openlocfilehash: 908ea451800abc343fb6e4d4a4ed98d57223bd23
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465242"
---
# <a name="value-protectionrulevaluetype"></a><span data-ttu-id="e7278-103">Значение (Протектионрулевалуетипе)</span><span class="sxs-lookup"><span data-stu-id="e7278-103">Value (ProtectionRuleValueType)</span></span>

<span data-ttu-id="e7278-104">Элемент **value** определяет одного получателя или отправителя.</span><span class="sxs-lookup"><span data-stu-id="e7278-104">The **Value** element identifies a single recipient or sender department.</span></span> 
  
```XML
<Value/>
```

<span data-ttu-id="e7278-105">**протектионрулевалуетипе**</span><span class="sxs-lookup"><span data-stu-id="e7278-105">**ProtectionRuleValueType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="e7278-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="e7278-106">Attributes and elements</span></span>

<span data-ttu-id="e7278-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="e7278-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e7278-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="e7278-108">Attributes</span></span>

<span data-ttu-id="e7278-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="e7278-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e7278-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="e7278-110">Child elements</span></span>

<span data-ttu-id="e7278-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="e7278-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="e7278-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="e7278-112">Parent elements</span></span>

|<span data-ttu-id="e7278-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="e7278-113">**Element**</span></span>|<span data-ttu-id="e7278-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="e7278-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e7278-115">Получательявляется</span><span class="sxs-lookup"><span data-stu-id="e7278-115">RecipientIs</span></span>](recipientis.md) <br/> |<span data-ttu-id="e7278-116">Указывает, что любой получатель сообщения электронной почты соответствует любому из указанных получателей в дочерних элементах **value** .</span><span class="sxs-lookup"><span data-stu-id="e7278-116">Specifies that any recipient of the email message matches any of the specified recipients in the child **Value** elements.</span></span>  <br/> |
|[<span data-ttu-id="e7278-117">сендердепартментс</span><span class="sxs-lookup"><span data-stu-id="e7278-117">SenderDepartments</span></span>](senderdepartments.md) <br/> |<span data-ttu-id="e7278-118">Указывает, что отдел отправителя соответствует любой из указанных отделов в дочерних элементах **value** .</span><span class="sxs-lookup"><span data-stu-id="e7278-118">Specifies that the department of the sender matches any of the specified departments in the child **Value** elements.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="e7278-119">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="e7278-119">Text value</span></span>

<span data-ttu-id="e7278-120">Этот элемент должен содержать непустое строковое значение.</span><span class="sxs-lookup"><span data-stu-id="e7278-120">This element must contain a nonempty string value.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="e7278-121">Примечания</span><span class="sxs-lookup"><span data-stu-id="e7278-121">Remarks</span></span>

<span data-ttu-id="e7278-122">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="e7278-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e7278-123">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="e7278-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e7278-124">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="e7278-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e7278-125">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="e7278-125">Schema Name</span></span>  <br/> |<span data-ttu-id="e7278-126">Схема Types</span><span class="sxs-lookup"><span data-stu-id="e7278-126">Types schema</span></span>  <br/> |
|<span data-ttu-id="e7278-127">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="e7278-127">Validation File</span></span>  <br/> |<span data-ttu-id="e7278-128">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="e7278-128">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="e7278-129">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="e7278-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="e7278-130">False</span><span class="sxs-lookup"><span data-stu-id="e7278-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e7278-131">См. также</span><span class="sxs-lookup"><span data-stu-id="e7278-131">See also</span></span>

- [<span data-ttu-id="e7278-132">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="e7278-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

