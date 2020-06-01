---
title: Member
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
description: Элемент Member представляет члена списка рассылки.
ms.openlocfilehash: e84223b7c41846ca2f174293bff46a8825777a0e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457307"
---
# <a name="member"></a><span data-ttu-id="e55b2-103">Member</span><span class="sxs-lookup"><span data-stu-id="e55b2-103">Member</span></span>

<span data-ttu-id="e55b2-104">Элемент **member** представляет члена списка рассылки.</span><span class="sxs-lookup"><span data-stu-id="e55b2-104">The **Member** element represents a member of a distribution list.</span></span> 
  
```xml
<Member Key="">
   <Mailbox/>
   <Status/>
</Member>
```

<span data-ttu-id="e55b2-105">**мембертипе**</span><span class="sxs-lookup"><span data-stu-id="e55b2-105">**MemberType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="e55b2-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="e55b2-106">Attributes and elements</span></span>

<span data-ttu-id="e55b2-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="e55b2-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e55b2-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="e55b2-108">Attributes</span></span>

|<span data-ttu-id="e55b2-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="e55b2-109">**Attribute**</span></span>|<span data-ttu-id="e55b2-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="e55b2-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="e55b2-111">Key</span><span class="sxs-lookup"><span data-stu-id="e55b2-111">Key</span></span>  <br/> |<span data-ttu-id="e55b2-112">Предоставляет уникальный идентификатор для члена списка рассылки.</span><span class="sxs-lookup"><span data-stu-id="e55b2-112">Provides a unique identifier for the distribution list member.</span></span> <span data-ttu-id="e55b2-113">Этот атрибут является необязательным.</span><span class="sxs-lookup"><span data-stu-id="e55b2-113">This attribute is optional.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="e55b2-114">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="e55b2-114">Child elements</span></span>

|<span data-ttu-id="e55b2-115">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="e55b2-115">**Element**</span></span>|<span data-ttu-id="e55b2-116">**Описание**</span><span class="sxs-lookup"><span data-stu-id="e55b2-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e55b2-117">Mailbox</span><span class="sxs-lookup"><span data-stu-id="e55b2-117">Mailbox</span></span>](mailbox.md) <br/> |<span data-ttu-id="e55b2-118">Представляет адрес электронной почты участника списка рассылки.</span><span class="sxs-lookup"><span data-stu-id="e55b2-118">Represents the e-mail address of the distribution list member.</span></span> <span data-ttu-id="e55b2-119">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="e55b2-119">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="e55b2-120">Состояние (Мемберстатустипе)</span><span class="sxs-lookup"><span data-stu-id="e55b2-120">Status (MemberStatusType)</span></span>](status-memberstatustype.md) <br/> |<span data-ttu-id="e55b2-121">Предоставляет сведения о состоянии члена списка рассылки.</span><span class="sxs-lookup"><span data-stu-id="e55b2-121">Provides information about the status of a distribution list member.</span></span> <span data-ttu-id="e55b2-122">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="e55b2-122">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="e55b2-123">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="e55b2-123">Parent elements</span></span>

|<span data-ttu-id="e55b2-124">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="e55b2-124">**Element**</span></span>|<span data-ttu-id="e55b2-125">**Описание**</span><span class="sxs-lookup"><span data-stu-id="e55b2-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e55b2-126">Members (Мемберлисттипе)</span><span class="sxs-lookup"><span data-stu-id="e55b2-126">Members (MemberListType)</span></span>](members-memberlisttype.md) <br/> |<span data-ttu-id="e55b2-127">Содержит список участников списка рассылки.</span><span class="sxs-lookup"><span data-stu-id="e55b2-127">Contains a list of distribution list members.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="e55b2-128">Примечания</span><span class="sxs-lookup"><span data-stu-id="e55b2-128">Remarks</span></span>

<span data-ttu-id="e55b2-129">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="e55b2-129">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e55b2-130">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="e55b2-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e55b2-131">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="e55b2-131">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e55b2-132">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="e55b2-132">Schema Name</span></span>  <br/> |<span data-ttu-id="e55b2-133">Схема Types</span><span class="sxs-lookup"><span data-stu-id="e55b2-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="e55b2-134">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="e55b2-134">Validation File</span></span>  <br/> |<span data-ttu-id="e55b2-135">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="e55b2-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="e55b2-136">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="e55b2-136">Can be Empty</span></span>  <br/> |<span data-ttu-id="e55b2-137">False</span><span class="sxs-lookup"><span data-stu-id="e55b2-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e55b2-138">См. также</span><span class="sxs-lookup"><span data-stu-id="e55b2-138">See also</span></span>

- [<span data-ttu-id="e55b2-139">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="e55b2-139">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

