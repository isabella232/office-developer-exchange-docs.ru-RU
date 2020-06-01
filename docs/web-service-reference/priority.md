---
title: Priority
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Priority
api_type:
- schema
ms.assetid: e1adb8b9-e3d5-469a-b188-822733d2503e
description: Элемент Priority указывает порядок, в котором должно выполняться правило.
ms.openlocfilehash: a5a894bba583618dd04430fc89f125c8920b0202
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462404"
---
# <a name="priority"></a><span data-ttu-id="50af5-103">Priority</span><span class="sxs-lookup"><span data-stu-id="50af5-103">Priority</span></span>

<span data-ttu-id="50af5-104">Элемент **Priority** указывает порядок, в котором должно выполняться правило.</span><span class="sxs-lookup"><span data-stu-id="50af5-104">The **Priority** element indicates the order in which a rule is to be run.</span></span> 
  
```XML
<Priority/>
```

 <span data-ttu-id="50af5-105">**int**</span><span class="sxs-lookup"><span data-stu-id="50af5-105">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="50af5-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="50af5-106">Attributes and elements</span></span>

<span data-ttu-id="50af5-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="50af5-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="50af5-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="50af5-108">Attributes</span></span>

<span data-ttu-id="50af5-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="50af5-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="50af5-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="50af5-110">Child elements</span></span>

<span data-ttu-id="50af5-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="50af5-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="50af5-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="50af5-112">Parent elements</span></span>

|<span data-ttu-id="50af5-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="50af5-113">**Element**</span></span>|<span data-ttu-id="50af5-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="50af5-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="50af5-115">Правило (RuleType)</span><span class="sxs-lookup"><span data-stu-id="50af5-115">Rule (RuleType)</span></span>](rule-ruletype.md) <br/> |<span data-ttu-id="50af5-116">Представляет правило в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="50af5-116">Represents a rule in the user's mailbox.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="50af5-117">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="50af5-117">Text value</span></span>

<span data-ttu-id="50af5-118">Текстовое значение элемента **Priority** — это целое число, которое указывает порядок выполнения, в котором должно выполняться правило.</span><span class="sxs-lookup"><span data-stu-id="50af5-118">The text value for the **Priority** element is an integer that indicates the execution order in which a rule should be run.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="50af5-119">Примечания</span><span class="sxs-lookup"><span data-stu-id="50af5-119">Remarks</span></span>

<span data-ttu-id="50af5-120">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="50af5-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="50af5-121">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="50af5-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="50af5-122">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="50af5-122">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="50af5-123">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="50af5-123">Schema Name</span></span>  <br/> |<span data-ttu-id="50af5-124">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="50af5-124">Messages schema</span></span>  <br/> |
|<span data-ttu-id="50af5-125">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="50af5-125">Validation File</span></span>  <br/> |<span data-ttu-id="50af5-126">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="50af5-126">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="50af5-127">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="50af5-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="50af5-128">False</span><span class="sxs-lookup"><span data-stu-id="50af5-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="50af5-129">См. также</span><span class="sxs-lookup"><span data-stu-id="50af5-129">See also</span></span>



- [<span data-ttu-id="50af5-130">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="50af5-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

