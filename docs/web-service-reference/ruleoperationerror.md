---
title: рулеоператионеррор
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RuleOperationError
api_type:
- schema
ms.assetid: b447e610-d37c-40d3-9158-aa108a9f248e
description: Элемент Рулеоператионеррор представляет ошибку операции с правилом.
ms.openlocfilehash: b5e0105a1fdb1564b3115a4c3a8411019f725483
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/01/2020
ms.locfileid: "44464961"
---
# <a name="ruleoperationerror"></a><span data-ttu-id="c23cf-103">рулеоператионеррор</span><span class="sxs-lookup"><span data-stu-id="c23cf-103">RuleOperationError</span></span>

<span data-ttu-id="c23cf-104">Элемент **рулеоператионеррор** представляет ошибку операции с правилом.</span><span class="sxs-lookup"><span data-stu-id="c23cf-104">The **RuleOperationError** element represents a rule operation error.</span></span> 
  
```XML
<RuleOperationError>
    <OperationIndex/>
    <ValidationErrors/>
</RuleOperationError>
```

 <span data-ttu-id="c23cf-105">**рулеоператионеррортипе**</span><span class="sxs-lookup"><span data-stu-id="c23cf-105">**RuleOperationErrorType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c23cf-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="c23cf-106">Attributes and elements</span></span>

<span data-ttu-id="c23cf-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="c23cf-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c23cf-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="c23cf-108">Attributes</span></span>

<span data-ttu-id="c23cf-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="c23cf-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c23cf-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="c23cf-110">Child elements</span></span>

|<span data-ttu-id="c23cf-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="c23cf-111">**Element**</span></span>|<span data-ttu-id="c23cf-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="c23cf-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c23cf-113">оператиониндекс</span><span class="sxs-lookup"><span data-stu-id="c23cf-113">OperationIndex</span></span>](operationindex.md) <br/> |<span data-ttu-id="c23cf-114">Указывает индекс операции в запросе, вызвавшей ошибку операции с правилом.</span><span class="sxs-lookup"><span data-stu-id="c23cf-114">Indicates the index of the operation in the request that caused the rule operation error.</span></span>  <br/> |
|[<span data-ttu-id="c23cf-115">валидатионеррорс</span><span class="sxs-lookup"><span data-stu-id="c23cf-115">ValidationErrors</span></span>](validationerrors.md) <br/> |<span data-ttu-id="c23cf-116">Представляет массив ошибок проверки правил для каждого поля правила, в котором возникла ошибка.</span><span class="sxs-lookup"><span data-stu-id="c23cf-116">Represents an array of rule validation errors on each rule field that has an error.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="c23cf-117">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="c23cf-117">Parent elements</span></span>

|<span data-ttu-id="c23cf-118">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="c23cf-118">**Element**</span></span>|<span data-ttu-id="c23cf-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="c23cf-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c23cf-120">рулеоператионеррорс</span><span class="sxs-lookup"><span data-stu-id="c23cf-120">RuleOperationErrors</span></span>](ruleoperationerrors.md) <br/> |<span data-ttu-id="c23cf-121">Представляет массив ошибок проверки правил для каждого поля правила, в котором возникла ошибка.</span><span class="sxs-lookup"><span data-stu-id="c23cf-121">Represents an array of rule validation errors on each rule field that has an error.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="c23cf-122">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="c23cf-122">Text value</span></span>

<span data-ttu-id="c23cf-123">Нет.</span><span class="sxs-lookup"><span data-stu-id="c23cf-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="c23cf-124">Примечания</span><span class="sxs-lookup"><span data-stu-id="c23cf-124">Remarks</span></span>

<span data-ttu-id="c23cf-125">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="c23cf-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c23cf-126">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="c23cf-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c23cf-127">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="c23cf-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="c23cf-128">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="c23cf-128">Schema Name</span></span>  <br/> |<span data-ttu-id="c23cf-129">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="c23cf-129">Messages schema</span></span>  <br/> |
|<span data-ttu-id="c23cf-130">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="c23cf-130">Validation File</span></span>  <br/> |<span data-ttu-id="c23cf-131">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="c23cf-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="c23cf-132">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="c23cf-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="c23cf-133">True</span><span class="sxs-lookup"><span data-stu-id="c23cf-133">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c23cf-134">См. также</span><span class="sxs-lookup"><span data-stu-id="c23cf-134">See also</span></span>



- [<span data-ttu-id="c23cf-135">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="c23cf-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

