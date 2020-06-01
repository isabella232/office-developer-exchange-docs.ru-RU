---
title: Операции
manager: sethgros
ms.date: 09/17/2015
ms.audience: ITPro
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Operations
api_type:
- schema
ms.assetid: d8cd41b1-28ae-4c95-9ff6-8b25c8e18306
description: Элемент Operations содержит массив операций с правилами, которые можно выполнить для папки "Входящие".
ms.openlocfilehash: 4bbec4ad6424f802bb6781a870d65f23705e88c4
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462488"
---
# <a name="operations"></a><span data-ttu-id="7561d-103">Операции</span><span class="sxs-lookup"><span data-stu-id="7561d-103">Operations</span></span>

<span data-ttu-id="7561d-104">Элемент **Operations** содержит массив операций с правилами, которые можно выполнить для папки "Входящие".</span><span class="sxs-lookup"><span data-stu-id="7561d-104">The **Operations** element contains an array of rule operations that can be performed on an Inbox.</span></span> 
  
[<span data-ttu-id="7561d-105">UpdateInboxRules</span><span class="sxs-lookup"><span data-stu-id="7561d-105">UpdateInboxRules</span></span>](updateinboxrules.md)
  
```XML
<Operations>
    <CreateRuleOperation/>
    <SetRuleOperation/>
    <DeleteRuleOperation/>
</Operations>
```

 <span data-ttu-id="7561d-106">**аррайофрулеоператионстипе**</span><span class="sxs-lookup"><span data-stu-id="7561d-106">**ArrayOfRuleOperationsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7561d-107">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="7561d-107">Attributes and elements</span></span>

<span data-ttu-id="7561d-108">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="7561d-108">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7561d-109">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="7561d-109">Attributes</span></span>

<span data-ttu-id="7561d-110">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="7561d-110">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7561d-111">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="7561d-111">Child elements</span></span>

|<span data-ttu-id="7561d-112">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="7561d-112">**Element**</span></span>|<span data-ttu-id="7561d-113">**Описание**</span><span class="sxs-lookup"><span data-stu-id="7561d-113">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7561d-114">креатерулеоператион</span><span class="sxs-lookup"><span data-stu-id="7561d-114">CreateRuleOperation</span></span>](createruleoperation.md) <br/> |<span data-ttu-id="7561d-115">Представляет операцию для создания нового правила для папки "Входящие".</span><span class="sxs-lookup"><span data-stu-id="7561d-115">Represents an operation to create a new Inbox rule.</span></span>  <br/> |
|[<span data-ttu-id="7561d-116">сетрулеоператион</span><span class="sxs-lookup"><span data-stu-id="7561d-116">SetRuleOperation</span></span>](setruleoperation.md) <br/> |<span data-ttu-id="7561d-117">Представляет операцию обновления правила для папки "Входящие".</span><span class="sxs-lookup"><span data-stu-id="7561d-117">Represents an operation to update an Inbox rule.</span></span>  <br/> |
|[<span data-ttu-id="7561d-118">делетерулеоператион</span><span class="sxs-lookup"><span data-stu-id="7561d-118">DeleteRuleOperation</span></span>](deleteruleoperation.md) <br/> |<span data-ttu-id="7561d-119">Представляет операцию удаления правила для папки "Входящие".</span><span class="sxs-lookup"><span data-stu-id="7561d-119">Represents an operation to delete an Inbox rule.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="7561d-120">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="7561d-120">Parent elements</span></span>

|<span data-ttu-id="7561d-121">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="7561d-121">**Element**</span></span>|<span data-ttu-id="7561d-122">**Описание**</span><span class="sxs-lookup"><span data-stu-id="7561d-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7561d-123">UpdateInboxRules</span><span class="sxs-lookup"><span data-stu-id="7561d-123">UpdateInboxRules</span></span>](updateinboxrules.md) <br/> |<span data-ttu-id="7561d-124">Определяет запрос на обновление правил папки "Входящие" в почтовом ящике в хранилище сервера.</span><span class="sxs-lookup"><span data-stu-id="7561d-124">Defines a request to update the Inbox rules in a mailbox in the server store.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="7561d-125">Примечания</span><span class="sxs-lookup"><span data-stu-id="7561d-125">Remarks</span></span>

<span data-ttu-id="7561d-126">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="7561d-126">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7561d-127">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="7561d-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7561d-128">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="7561d-128">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="7561d-129">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="7561d-129">Schema Name</span></span>  <br/> |<span data-ttu-id="7561d-130">Схема Types</span><span class="sxs-lookup"><span data-stu-id="7561d-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="7561d-131">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="7561d-131">Validation File</span></span>  <br/> |<span data-ttu-id="7561d-132">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="7561d-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="7561d-133">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="7561d-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="7561d-134">False</span><span class="sxs-lookup"><span data-stu-id="7561d-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7561d-135">См. также</span><span class="sxs-lookup"><span data-stu-id="7561d-135">See also</span></span>



[<span data-ttu-id="7561d-136">Операция UpdateInboxRules</span><span class="sxs-lookup"><span data-stu-id="7561d-136">UpdateInboxRules operation</span></span>](updateinboxrules-operation.md)


- [<span data-ttu-id="7561d-137">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="7561d-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

