---
title: Ветвление
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Transition
api_type:
- schema
ms.assetid: 23ce171a-a9c9-47ed-a366-822777048eea
description: Элемент TRANSITION представляет переход часового пояса.
ms.openlocfilehash: 5dcd2f0dae7c3df2dcf660d6fe1a41b216c67b59
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19840239"
---
# <a name="transition"></a><span data-ttu-id="5e87e-103">Ветвление</span><span class="sxs-lookup"><span data-stu-id="5e87e-103">Transition</span></span>

<span data-ttu-id="5e87e-104">Элемент **TRANSITION** представляет переход часового пояса.</span><span class="sxs-lookup"><span data-stu-id="5e87e-104">The **Transition** element represents a time zone transition.</span></span> 
  
```xml
<Transition>
   <To/>
</Transition>
```

 <span data-ttu-id="5e87e-105">**транситионтипе**</span><span class="sxs-lookup"><span data-stu-id="5e87e-105">**TransitionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5e87e-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="5e87e-106">Attributes and elements</span></span>

<span data-ttu-id="5e87e-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="5e87e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5e87e-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="5e87e-108">Attributes</span></span>

<span data-ttu-id="5e87e-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="5e87e-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5e87e-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="5e87e-110">Child elements</span></span>

|<span data-ttu-id="5e87e-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="5e87e-111">**Element**</span></span>|<span data-ttu-id="5e87e-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="5e87e-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5e87e-113">To</span><span class="sxs-lookup"><span data-stu-id="5e87e-113">To</span></span>](to.md) <br/> |<span data-ttu-id="5e87e-114">Указывает [период](period.md) или [транситионсграуп](transitionsgroup.md) , который является целевым объектом перехода часового пояса.</span><span class="sxs-lookup"><span data-stu-id="5e87e-114">Specifies the [Period](period.md) or [TransitionsGroup](transitionsgroup.md) that is the target of the time zone transition.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="5e87e-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="5e87e-115">Parent elements</span></span>

|<span data-ttu-id="5e87e-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="5e87e-116">**Element**</span></span>|<span data-ttu-id="5e87e-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="5e87e-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5e87e-118">Выполняет</span><span class="sxs-lookup"><span data-stu-id="5e87e-118">Transitions</span></span>](transitions.md) <br/> |<span data-ttu-id="5e87e-119">Представляет коллекцию переходов часового пояса.</span><span class="sxs-lookup"><span data-stu-id="5e87e-119">Represents a collection of time zone transitions.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="5e87e-120">Примечания</span><span class="sxs-lookup"><span data-stu-id="5e87e-120">Remarks</span></span>

<span data-ttu-id="5e87e-121">Схема, описывающая этот элемент, находится в виртуальном каталоге EWS компьютера, на котором работает сервер Microsoft Exchange с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="5e87e-121">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5e87e-122">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="5e87e-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5e87e-123">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="5e87e-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="5e87e-124">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="5e87e-124">Schema Name</span></span>  <br/> |<span data-ttu-id="5e87e-125">Схема Types</span><span class="sxs-lookup"><span data-stu-id="5e87e-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="5e87e-126">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="5e87e-126">Validation File</span></span>  <br/> |<span data-ttu-id="5e87e-127">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="5e87e-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="5e87e-128">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="5e87e-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="5e87e-129">False</span><span class="sxs-lookup"><span data-stu-id="5e87e-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5e87e-130">См. также</span><span class="sxs-lookup"><span data-stu-id="5e87e-130">See also</span></span>



- [<span data-ttu-id="5e87e-131">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="5e87e-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

