---
title: RemoveOutlookRuleBlob
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RemoveOutlookRuleBlob
api_type:
- schema
ms.assetid: 69614475-8bd3-4475-b988-614fe9cad8ef
description: Элемент RemoveOutlookRuleBlob указывает, следует ли удалять больших двоичных объектов Microsoft Outlook правило.
ms.openlocfilehash: 45336e296c39161704ce6e0d51fba1d2c61797b1
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835102"
---
# <a name="removeoutlookruleblob"></a><span data-ttu-id="f6e20-103">RemoveOutlookRuleBlob</span><span class="sxs-lookup"><span data-stu-id="f6e20-103">RemoveOutlookRuleBlob</span></span>

<span data-ttu-id="f6e20-104">Элемент **RemoveOutlookRuleBlob** указывает, следует ли удалять больших двоичных объектов Microsoft Outlook правило.</span><span class="sxs-lookup"><span data-stu-id="f6e20-104">The **RemoveOutlookRuleBlob** element indicates whether to remove the Microsoft Outlook rule blob.</span></span> 
  
[<span data-ttu-id="f6e20-105">UpdateInboxRules</span><span class="sxs-lookup"><span data-stu-id="f6e20-105">UpdateInboxRules</span></span>](updateinboxrules.md)
  
[<span data-ttu-id="f6e20-106">RemoveOutlookRuleBlob</span><span class="sxs-lookup"><span data-stu-id="f6e20-106">RemoveOutlookRuleBlob</span></span>](removeoutlookruleblob.md)
  
```XML
<RemoveOutlookRuleBlob>true | false</RemoveOutlookRuleBlob>
```

 <span data-ttu-id="f6e20-107">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="f6e20-107">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f6e20-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="f6e20-108">Attributes and elements</span></span>

<span data-ttu-id="f6e20-109">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="f6e20-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f6e20-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="f6e20-110">Attributes</span></span>

<span data-ttu-id="f6e20-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="f6e20-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f6e20-112">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="f6e20-112">Child elements</span></span>

<span data-ttu-id="f6e20-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="f6e20-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="f6e20-114">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="f6e20-114">Parent elements</span></span>

|<span data-ttu-id="f6e20-115">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="f6e20-115">**Element**</span></span>|<span data-ttu-id="f6e20-116">**Описание**</span><span class="sxs-lookup"><span data-stu-id="f6e20-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f6e20-117">UpdateInboxRules</span><span class="sxs-lookup"><span data-stu-id="f6e20-117">UpdateInboxRules</span></span>](updateinboxrules.md) <br/> |<span data-ttu-id="f6e20-118">Определяет запрос на обновление правил папки "Входящие" почтового ящика в хранилище сервера.</span><span class="sxs-lookup"><span data-stu-id="f6e20-118">Defines a request to update the Inbox rules in a mailbox in the server store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="f6e20-119">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="f6e20-119">Text value</span></span>

<span data-ttu-id="f6e20-120">Текстовое значение **true,** указывает, что больших двоичных объектов правила Outlook должна быть удалена.</span><span class="sxs-lookup"><span data-stu-id="f6e20-120">A text value of **true** indicates that the Outlook rule blob should be removed.</span></span> <span data-ttu-id="f6e20-121">Текстовое значение **false** указывает, что больших двоичных объектов Outlook правила не будут удалены.</span><span class="sxs-lookup"><span data-stu-id="f6e20-121">A text value of **false** indicates that the Outlook rule blob should not be removed.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="f6e20-122">Замечания</span><span class="sxs-lookup"><span data-stu-id="f6e20-122">Remarks</span></span>

<span data-ttu-id="f6e20-123">Присвойте этому элементу **значение true,** чтобы разрешить обновление правила папки «Входящие».</span><span class="sxs-lookup"><span data-stu-id="f6e20-123">Set this element to **true** to allow for an Inbox rule update.</span></span> 
  
<span data-ttu-id="f6e20-124">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="f6e20-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f6e20-125">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="f6e20-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f6e20-126">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="f6e20-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f6e20-127">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="f6e20-127">Schema Name</span></span>  <br/> |<span data-ttu-id="f6e20-128">Схема Types</span><span class="sxs-lookup"><span data-stu-id="f6e20-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="f6e20-129">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="f6e20-129">Validation File</span></span>  <br/> |<span data-ttu-id="f6e20-130">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="f6e20-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="f6e20-131">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="f6e20-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="f6e20-132">True</span><span class="sxs-lookup"><span data-stu-id="f6e20-132">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f6e20-133">См. также</span><span class="sxs-lookup"><span data-stu-id="f6e20-133">See also</span></span>



[<span data-ttu-id="f6e20-134">Операция UpdateInboxRules</span><span class="sxs-lookup"><span data-stu-id="f6e20-134">UpdateInboxRules operation</span></span>](updateinboxrules-operation.md)


- [<span data-ttu-id="f6e20-135">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="f6e20-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

