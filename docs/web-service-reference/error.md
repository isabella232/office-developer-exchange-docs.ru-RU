---
title: Ошибка
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Error
api_type:
- schema
ms.assetid: b1f54673-578a-496b-99f5-0fde2c669278
description: Элемент error представляет одну ошибку проверки для определенного значения свойства правила, значения свойства предиката или значения свойства Action.
ms.openlocfilehash: adb2de56b7610aa92b5bf5b8d43ac22f35021b64
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762379"
---
# <a name="error"></a><span data-ttu-id="ec01a-103">Ошибка</span><span class="sxs-lookup"><span data-stu-id="ec01a-103">Error</span></span>

<span data-ttu-id="ec01a-104">Элемент **Error** представляет одну ошибку проверки для определенного значения свойства правила, значения свойства предиката или значения свойства Action.</span><span class="sxs-lookup"><span data-stu-id="ec01a-104">The **Error** element represents a single validation error on a particular rule property value, predicate property value, or action property value.</span></span> 
  
```XML
<Error>
   <FieldUri/>
   <ErrorCode/>
   <ErrorMessage/>
   <FieldValue/>
</Error>
```

 <span data-ttu-id="ec01a-105">**рулевалидатионеррортипе**</span><span class="sxs-lookup"><span data-stu-id="ec01a-105">**RuleValidationErrorType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ec01a-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="ec01a-106">Attributes and elements</span></span>

<span data-ttu-id="ec01a-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="ec01a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ec01a-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="ec01a-108">Attributes</span></span>

<span data-ttu-id="ec01a-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="ec01a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ec01a-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="ec01a-110">Child elements</span></span>

|<span data-ttu-id="ec01a-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="ec01a-111">**Element**</span></span>|<span data-ttu-id="ec01a-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="ec01a-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ec01a-113">Фиелдури (правило)</span><span class="sxs-lookup"><span data-stu-id="ec01a-113">FieldUri (Rule)</span></span>](fielduri-rule.md) <br/> |<span data-ttu-id="ec01a-114">Задает универсальный код ресурса (URI) для поля правила, вызвавшего ошибку проверки.</span><span class="sxs-lookup"><span data-stu-id="ec01a-114">Specifies the URI to the rule field that caused the validation error.</span></span>  <br/> |
|[<span data-ttu-id="ec01a-115">ErrorCode</span><span class="sxs-lookup"><span data-stu-id="ec01a-115">ErrorCode</span></span>](errorcode.md) <br/> |<span data-ttu-id="ec01a-116">Представляет код ошибки проверки правила, указывающий, что не прошло проверку для каждого предиката правила или действия.</span><span class="sxs-lookup"><span data-stu-id="ec01a-116">Represents a rule validation error code that describes what failed validation for each rule predicate or action.</span></span>  <br/> |
|[<span data-ttu-id="ec01a-117">ErrorMessage</span><span class="sxs-lookup"><span data-stu-id="ec01a-117">ErrorMessage</span></span>](errormessage.md) <br/> |<span data-ttu-id="ec01a-118">Представляет причину ошибки проверки.</span><span class="sxs-lookup"><span data-stu-id="ec01a-118">Represents the reason for the validation error.</span></span>  <br/> |
|[<span data-ttu-id="ec01a-119">FieldValue</span><span class="sxs-lookup"><span data-stu-id="ec01a-119">FieldValue</span></span>](fieldvalue.md) <br/> |<span data-ttu-id="ec01a-120">Представляет значение поля, вызвавшего ошибку проверки.</span><span class="sxs-lookup"><span data-stu-id="ec01a-120">Represents the value of the field that caused the validation error.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="ec01a-121">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="ec01a-121">Parent elements</span></span>

|<span data-ttu-id="ec01a-122">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="ec01a-122">**Element**</span></span>|<span data-ttu-id="ec01a-123">**Описание**</span><span class="sxs-lookup"><span data-stu-id="ec01a-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ec01a-124">валидатионеррорс</span><span class="sxs-lookup"><span data-stu-id="ec01a-124">ValidationErrors</span></span>](validationerrors.md) <br/> |<span data-ttu-id="ec01a-125">Представляет массив ошибок проверки правил для каждого поля правила, в котором возникла ошибка.</span><span class="sxs-lookup"><span data-stu-id="ec01a-125">Represents an array of rule validation errors on each rule field that has an error.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="ec01a-126">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="ec01a-126">Text value</span></span>

<span data-ttu-id="ec01a-127">Нет.</span><span class="sxs-lookup"><span data-stu-id="ec01a-127">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="ec01a-128">Примечания</span><span class="sxs-lookup"><span data-stu-id="ec01a-128">Remarks</span></span>

<span data-ttu-id="ec01a-129">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="ec01a-129">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ec01a-130">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="ec01a-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ec01a-131">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="ec01a-131">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="ec01a-132">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="ec01a-132">Schema Name</span></span>  <br/> |<span data-ttu-id="ec01a-133">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="ec01a-133">Messages schema</span></span>  <br/> |
|<span data-ttu-id="ec01a-134">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="ec01a-134">Validation File</span></span>  <br/> |<span data-ttu-id="ec01a-135">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="ec01a-135">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="ec01a-136">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="ec01a-136">Can be Empty</span></span>  <br/> |<span data-ttu-id="ec01a-137">True</span><span class="sxs-lookup"><span data-stu-id="ec01a-137">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ec01a-138">См. также</span><span class="sxs-lookup"><span data-stu-id="ec01a-138">See also</span></span>



- [<span data-ttu-id="ec01a-139">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="ec01a-139">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

