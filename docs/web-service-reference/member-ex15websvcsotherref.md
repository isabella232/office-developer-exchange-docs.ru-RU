---
title: Элемент
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Member
api_type:
- schema
ms.assetid: af9c5ff8-02a4-41fc-876d-14ac05f1ee77
description: Элемент Member представляет элемент в список рассылки.
ms.openlocfilehash: c38e2ed24e78b5199d4d65cce27a00a8e6704037
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19834434"
---
# <a name="member"></a><span data-ttu-id="02ebe-103">Элемент</span><span class="sxs-lookup"><span data-stu-id="02ebe-103">Member</span></span>

<span data-ttu-id="02ebe-104">Элемент **Member** представляет элемент в список рассылки.</span><span class="sxs-lookup"><span data-stu-id="02ebe-104">The **Member** element represents a member of a distribution list.</span></span> 
  
```xml
<Member Key="">
   <Mailbox/>
   <Status/>
</Member>
```

<span data-ttu-id="02ebe-105">**MemberType**</span><span class="sxs-lookup"><span data-stu-id="02ebe-105">**MemberType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="02ebe-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="02ebe-106">Attributes and elements</span></span>

<span data-ttu-id="02ebe-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="02ebe-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="02ebe-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="02ebe-108">Attributes</span></span>

|<span data-ttu-id="02ebe-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="02ebe-109">**Attribute**</span></span>|<span data-ttu-id="02ebe-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="02ebe-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="02ebe-111">Ключ</span><span class="sxs-lookup"><span data-stu-id="02ebe-111">Key</span></span>  <br/> |<span data-ttu-id="02ebe-112">Содержит уникальный идентификатор для списка рассылки.</span><span class="sxs-lookup"><span data-stu-id="02ebe-112">Provides a unique identifier for the distribution list member.</span></span> <span data-ttu-id="02ebe-113">Этот атрибут является необязательным.</span><span class="sxs-lookup"><span data-stu-id="02ebe-113">This attribute is optional.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="02ebe-114">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="02ebe-114">Child elements</span></span>

|<span data-ttu-id="02ebe-115">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="02ebe-115">**Element**</span></span>|<span data-ttu-id="02ebe-116">**Описание**</span><span class="sxs-lookup"><span data-stu-id="02ebe-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="02ebe-117">Mailbox</span><span class="sxs-lookup"><span data-stu-id="02ebe-117">Mailbox</span></span>](mailbox.md) <br/> |<span data-ttu-id="02ebe-118">Представляет адрес электронной почты из списка рассылки.</span><span class="sxs-lookup"><span data-stu-id="02ebe-118">Represents the e-mail address of the distribution list member.</span></span> <span data-ttu-id="02ebe-119">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="02ebe-119">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="02ebe-120">Состояние (MemberStatusType)</span><span class="sxs-lookup"><span data-stu-id="02ebe-120">Status (MemberStatusType)</span></span>](status-memberstatustype.md) <br/> |<span data-ttu-id="02ebe-121">Сведения о состоянии списка рассылки.</span><span class="sxs-lookup"><span data-stu-id="02ebe-121">Provides information about the status of a distribution list member.</span></span> <span data-ttu-id="02ebe-122">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="02ebe-122">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="02ebe-123">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="02ebe-123">Parent elements</span></span>

|<span data-ttu-id="02ebe-124">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="02ebe-124">**Element**</span></span>|<span data-ttu-id="02ebe-125">**Описание**</span><span class="sxs-lookup"><span data-stu-id="02ebe-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="02ebe-126">Члены (MemberListType)</span><span class="sxs-lookup"><span data-stu-id="02ebe-126">Members (MemberListType)</span></span>](members-memberlisttype.md) <br/> |<span data-ttu-id="02ebe-127">Содержит список членов списка рассылки.</span><span class="sxs-lookup"><span data-stu-id="02ebe-127">Contains a list of distribution list members.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="02ebe-128">Замечания</span><span class="sxs-lookup"><span data-stu-id="02ebe-128">Remarks</span></span>

<span data-ttu-id="02ebe-129">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="02ebe-129">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="02ebe-130">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="02ebe-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="02ebe-131">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="02ebe-131">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="02ebe-132">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="02ebe-132">Schema Name</span></span>  <br/> |<span data-ttu-id="02ebe-133">Схема Types</span><span class="sxs-lookup"><span data-stu-id="02ebe-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="02ebe-134">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="02ebe-134">Validation File</span></span>  <br/> |<span data-ttu-id="02ebe-135">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="02ebe-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="02ebe-136">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="02ebe-136">Can be Empty</span></span>  <br/> |<span data-ttu-id="02ebe-137">False</span><span class="sxs-lookup"><span data-stu-id="02ebe-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="02ebe-138">См. также</span><span class="sxs-lookup"><span data-stu-id="02ebe-138">See also</span></span>

- [<span data-ttu-id="02ebe-139">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="02ebe-139">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

