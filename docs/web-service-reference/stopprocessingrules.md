---
title: StopProcessingRules
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- StopProcessingRules
api_type:
- schema
ms.assetid: 5b89a2cb-ab26-444d-b3dd-2b3858872d63
description: Элемент StopProcessingRules указывает, будет ли последующих правил для оценки.
ms.openlocfilehash: 9f068fd6290a39bbab6e3c1e29066c4fefefc64b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44467902"
---
# <a name="stopprocessingrules"></a><span data-ttu-id="22030-103">StopProcessingRules</span><span class="sxs-lookup"><span data-stu-id="22030-103">StopProcessingRules</span></span>

<span data-ttu-id="22030-104">Информация, содержащаяся в этом документе, может относиться к функциям и продуктам предварительной версии и может претерпеть значительные изменения до окончательного коммерческого выпуска. Настоящий документ предоставляется "как есть" и служит только для информационных целей. Корпорация Майкрософт не предоставляет никаких гарантий, явных или подразумеваемых, в связи с этим документом Элемент **StopProcessingRules** указывает, будет ли последующих правил для оценки.</span><span class="sxs-lookup"><span data-stu-id="22030-104">The **StopProcessingRules** element indicates whether subsequent rules are to be evaluated.</span></span> 
  
```XML
<StopProcessingRules>true | false</StopProcessingRules>
```

 <span data-ttu-id="22030-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="22030-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="22030-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="22030-106">Attributes and elements</span></span>

<span data-ttu-id="22030-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="22030-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="22030-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="22030-108">Attributes</span></span>

<span data-ttu-id="22030-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="22030-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="22030-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="22030-110">Child elements</span></span>

<span data-ttu-id="22030-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="22030-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="22030-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="22030-112">Parent elements</span></span>

|<span data-ttu-id="22030-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="22030-113">**Element**</span></span>|<span data-ttu-id="22030-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="22030-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="22030-115">Действия</span><span class="sxs-lookup"><span data-stu-id="22030-115">Actions</span></span>](actions.md) <br/> |<span data-ttu-id="22030-116">Представляет набор действий, которые доступны для выполнения на сообщение при условия будут выполнены.</span><span class="sxs-lookup"><span data-stu-id="22030-116">Represents the set of actions that are available to be taken on a message when the conditions are fulfilled.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="22030-117">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="22030-117">Text value</span></span>

<span data-ttu-id="22030-p101">Текстовое значение **true** указывает, что последующие правила не будут обрабатываться. Значение **false** указывает, что последующие правила должны продолжать оценку.</span><span class="sxs-lookup"><span data-stu-id="22030-p101">A text value of **true** indicates that subsequent rules should not be processed. A value of **false** indicates that subsequent rules should continue to be evaluated.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="22030-120">Примечания</span><span class="sxs-lookup"><span data-stu-id="22030-120">Remarks</span></span>

<span data-ttu-id="22030-121">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="22030-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="22030-122">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="22030-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="22030-123">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="22030-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="22030-124">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="22030-124">Schema Name</span></span>  <br/> |<span data-ttu-id="22030-125">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="22030-125">Messages schema</span></span>  <br/> |
|<span data-ttu-id="22030-126">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="22030-126">Validation File</span></span>  <br/> |<span data-ttu-id="22030-127">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="22030-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="22030-128">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="22030-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="22030-129">True</span><span class="sxs-lookup"><span data-stu-id="22030-129">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="22030-130">См. также</span><span class="sxs-lookup"><span data-stu-id="22030-130">See also</span></span>



- [<span data-ttu-id="22030-131">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="22030-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

