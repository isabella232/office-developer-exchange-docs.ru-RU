---
title: исинеррор
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
description: Элемент Исинеррор указывает, находится ли правило в состоянии ошибки.
ms.openlocfilehash: 9e642c9f89434bdcad97b0c16dc35f99196051d7
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44464219"
---
# <a name="isinerror"></a><span data-ttu-id="20a94-103">исинеррор</span><span class="sxs-lookup"><span data-stu-id="20a94-103">IsInError</span></span>

<span data-ttu-id="20a94-104">Элемент **исинеррор** указывает, находится ли правило в состоянии ошибки.</span><span class="sxs-lookup"><span data-stu-id="20a94-104">The **IsInError** element indicates whether the rule is in an error condition.</span></span> 
  
```XML
<IsInError/>
```

 <span data-ttu-id="20a94-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="20a94-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="20a94-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="20a94-106">Attributes and elements</span></span>

<span data-ttu-id="20a94-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="20a94-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="20a94-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="20a94-108">Attributes</span></span>

<span data-ttu-id="20a94-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="20a94-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="20a94-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="20a94-110">Child elements</span></span>

<span data-ttu-id="20a94-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="20a94-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="20a94-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="20a94-112">Parent elements</span></span>

|<span data-ttu-id="20a94-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="20a94-113">**Element**</span></span>|<span data-ttu-id="20a94-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="20a94-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="20a94-115">Правило (RuleType)</span><span class="sxs-lookup"><span data-stu-id="20a94-115">Rule (RuleType)</span></span>](rule-ruletype.md) <br/> |<span data-ttu-id="20a94-116">Представляет правило в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="20a94-116">Represents a rule in the user's mailbox.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="20a94-117">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="20a94-117">Text value</span></span>

<span data-ttu-id="20a94-118">Текстовое значение **true** указывает, что правило находится в состоянии ошибки.</span><span class="sxs-lookup"><span data-stu-id="20a94-118">A text value of **true** indicates that the rule is in an error condition.</span></span> <span data-ttu-id="20a94-119">Значение **false** указывает, что правило не находится в состоянии ошибки.</span><span class="sxs-lookup"><span data-stu-id="20a94-119">A value of **false** indicates that the rule is not in an error condition.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="20a94-120">Примечания</span><span class="sxs-lookup"><span data-stu-id="20a94-120">Remarks</span></span>

<span data-ttu-id="20a94-121">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="20a94-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="20a94-122">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="20a94-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="20a94-123">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="20a94-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="20a94-124">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="20a94-124">Schema Name</span></span>  <br/> |<span data-ttu-id="20a94-125">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="20a94-125">Messages schema</span></span>  <br/> |
|<span data-ttu-id="20a94-126">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="20a94-126">Validation File</span></span>  <br/> |<span data-ttu-id="20a94-127">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="20a94-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="20a94-128">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="20a94-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="20a94-129">True</span><span class="sxs-lookup"><span data-stu-id="20a94-129">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="20a94-130">См. также</span><span class="sxs-lookup"><span data-stu-id="20a94-130">See also</span></span>



- [<span data-ttu-id="20a94-131">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="20a94-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

