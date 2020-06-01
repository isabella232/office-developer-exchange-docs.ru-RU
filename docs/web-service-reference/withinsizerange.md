---
title: висинсизеранже
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- WithinSizeRange
api_type:
- schema
ms.assetid: 6f98650e-3399-4f87-9b7f-40bf20cdb821
description: Элемент Висинсизеранже указывает минимальный и максимальный размеры для входящих сообщений, которые должны быть применены к указанному условию или исключению.
ms.openlocfilehash: 31da5815b70e20c47594da89b0b7ccab87eaf8f3
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459744"
---
# <a name="withinsizerange"></a><span data-ttu-id="c306a-103">висинсизеранже</span><span class="sxs-lookup"><span data-stu-id="c306a-103">WithinSizeRange</span></span>

<span data-ttu-id="c306a-104">Элемент **висинсизеранже** указывает минимальный и максимальный размеры для входящих сообщений, которые должны быть применены к указанному условию или исключению.</span><span class="sxs-lookup"><span data-stu-id="c306a-104">The **WithinSizeRange** element specifies the minimum and maximum sizes that incoming messages must be in order for the condition or exception to apply.</span></span> 
  
```XML
<WithinSizeRange>
     <MinimumSize/>
     <MaximumSize/>
</WithinSizeRange>
```

 <span data-ttu-id="c306a-105">**рулепредикатесизеранжетипе**</span><span class="sxs-lookup"><span data-stu-id="c306a-105">**RulePredicateSizeRangeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c306a-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="c306a-106">Attributes and elements</span></span>

<span data-ttu-id="c306a-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="c306a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c306a-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="c306a-108">Attributes</span></span>

<span data-ttu-id="c306a-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="c306a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c306a-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="c306a-110">Child elements</span></span>

|<span data-ttu-id="c306a-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="c306a-111">**Element**</span></span>|<span data-ttu-id="c306a-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="c306a-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c306a-113">минимумсизе</span><span class="sxs-lookup"><span data-stu-id="c306a-113">MinimumSize</span></span>](minimumsize.md) <br/> |<span data-ttu-id="c306a-114">Указывает минимальный размер сообщения, которое должно быть применено к определенному условию или исключению.</span><span class="sxs-lookup"><span data-stu-id="c306a-114">Specifies the minimum size that a message must be in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="c306a-115">максимумсизе</span><span class="sxs-lookup"><span data-stu-id="c306a-115">MaximumSize</span></span>](maximumsize.md) <br/> |<span data-ttu-id="c306a-116">Задает максимальный размер сообщения для применения условия или исключения.</span><span class="sxs-lookup"><span data-stu-id="c306a-116">Specifies the maximum size that a message must be in order for the condition or exception to apply.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="c306a-117">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="c306a-117">Parent elements</span></span>

|<span data-ttu-id="c306a-118">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="c306a-118">**Element**</span></span>|<span data-ttu-id="c306a-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="c306a-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c306a-120">Условия</span><span class="sxs-lookup"><span data-stu-id="c306a-120">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="c306a-121">Представляет условия, которые, если удовлетворены, запускают действия правила для правила.</span><span class="sxs-lookup"><span data-stu-id="c306a-121">Represents the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span>  <br/> |
|[<span data-ttu-id="c306a-122">Исключения</span><span class="sxs-lookup"><span data-stu-id="c306a-122">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="c306a-123">Представляет все доступные условия исключения правила для правила папки "Входящие".</span><span class="sxs-lookup"><span data-stu-id="c306a-123">Represents all the available rule exception conditions for an Inbox rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="c306a-124">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="c306a-124">Text value</span></span>

<span data-ttu-id="c306a-125">Нет.</span><span class="sxs-lookup"><span data-stu-id="c306a-125">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="c306a-126">Примечания</span><span class="sxs-lookup"><span data-stu-id="c306a-126">Remarks</span></span>

<span data-ttu-id="c306a-127">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="c306a-127">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c306a-128">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="c306a-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c306a-129">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="c306a-129">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="c306a-130">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="c306a-130">Schema Name</span></span>  <br/> |<span data-ttu-id="c306a-131">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="c306a-131">Messages schema</span></span>  <br/> |
|<span data-ttu-id="c306a-132">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="c306a-132">Validation File</span></span>  <br/> |<span data-ttu-id="c306a-133">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="c306a-133">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="c306a-134">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="c306a-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="c306a-135">True</span><span class="sxs-lookup"><span data-stu-id="c306a-135">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c306a-136">См. также</span><span class="sxs-lookup"><span data-stu-id="c306a-136">See also</span></span>



- [<span data-ttu-id="c306a-137">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="c306a-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

