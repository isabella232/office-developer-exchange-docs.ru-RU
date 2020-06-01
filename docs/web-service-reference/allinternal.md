---
title: аллинтернал
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AllInternal
api_type:
- schema
ms.assetid: b7e5072f-5d9f-4ee0-b58b-4d75d878ea1c
description: Элемент Аллинтернал имеет значение true, если все получатели сообщения электронной почты являются внутренними для организации отправителя.
ms.openlocfilehash: c5ffe15eca5d680994acb62913ebf5effacce214
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44464835"
---
# <a name="allinternal"></a><span data-ttu-id="ee4d1-103">аллинтернал</span><span class="sxs-lookup"><span data-stu-id="ee4d1-103">AllInternal</span></span>

<span data-ttu-id="ee4d1-104">Элемент **аллинтернал** имеет **значение true** , если все получатели сообщения электронной почты являются внутренними для организации отправителя.</span><span class="sxs-lookup"><span data-stu-id="ee4d1-104">The **AllInternal** element evaluates to **true** if all recipients of an e-mail message are internal to the sender's organization.</span></span> 
  
```xml
<AllInternal/>
```

 <span data-ttu-id="ee4d1-105">**протектионрулеаллинтерналтипе**</span><span class="sxs-lookup"><span data-stu-id="ee4d1-105">**ProtectionRuleAllInternalType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ee4d1-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="ee4d1-106">Attributes and elements</span></span>

<span data-ttu-id="ee4d1-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="ee4d1-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ee4d1-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="ee4d1-108">Attributes</span></span>

<span data-ttu-id="ee4d1-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="ee4d1-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ee4d1-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="ee4d1-110">Child elements</span></span>

<span data-ttu-id="ee4d1-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="ee4d1-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="ee4d1-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="ee4d1-112">Parent elements</span></span>

|<span data-ttu-id="ee4d1-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="ee4d1-113">**Element**</span></span>|<span data-ttu-id="ee4d1-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="ee4d1-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ee4d1-115">Условие</span><span class="sxs-lookup"><span data-stu-id="ee4d1-115">Condition</span></span>](condition.md) <br/> |<span data-ttu-id="ee4d1-116">Определяет условие, которое должно быть удовлетворено для части действия правила, которое необходимо выполнить.</span><span class="sxs-lookup"><span data-stu-id="ee4d1-116">Identifies the condition that must be satisfied for the action part of the rule to be executed.</span></span>  <br/> |
|[<span data-ttu-id="ee4d1-117">И (Протектионрулеандтипе)</span><span class="sxs-lookup"><span data-stu-id="ee4d1-117">And (ProtectionRuleAndType)</span></span>](and-protectionruleandtype.md) <br/> |<span data-ttu-id="ee4d1-118">Указывает, что все дочерние элементы должны сопоставляться со значением **true**.</span><span class="sxs-lookup"><span data-stu-id="ee4d1-118">Specifies that all child elements must match to evaluate to **true**.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="ee4d1-119">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="ee4d1-119">Text value</span></span>

<span data-ttu-id="ee4d1-120">Элемент **аллинтернал** должен быть пустым.</span><span class="sxs-lookup"><span data-stu-id="ee4d1-120">The **AllInternal** element must be empty.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="ee4d1-121">Примечания</span><span class="sxs-lookup"><span data-stu-id="ee4d1-121">Remarks</span></span>

<span data-ttu-id="ee4d1-122">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="ee4d1-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ee4d1-123">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="ee4d1-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ee4d1-124">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="ee4d1-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="ee4d1-125">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="ee4d1-125">Schema Name</span></span>  <br/> |<span data-ttu-id="ee4d1-126">Схема Types</span><span class="sxs-lookup"><span data-stu-id="ee4d1-126">Types schema</span></span>  <br/> |
|<span data-ttu-id="ee4d1-127">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="ee4d1-127">Validation File</span></span>  <br/> |<span data-ttu-id="ee4d1-128">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="ee4d1-128">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="ee4d1-129">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="ee4d1-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="ee4d1-130">False</span><span class="sxs-lookup"><span data-stu-id="ee4d1-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ee4d1-131">См. также</span><span class="sxs-lookup"><span data-stu-id="ee4d1-131">See also</span></span>

- [<span data-ttu-id="ee4d1-132">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="ee4d1-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

