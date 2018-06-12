---
title: Участники
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 837bb372-39eb-48ae-9c09-0d2552511f93
description: Элемент участников указывает получателей приглашения на собрание.
ms.openlocfilehash: 22d88bb092b416c553144496e133680b53f5d30e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761519"
---
# <a name="attendees"></a><span data-ttu-id="08bc2-103">Участники</span><span class="sxs-lookup"><span data-stu-id="08bc2-103">Attendees</span></span>

<span data-ttu-id="08bc2-104">Элемент **участников** указывает получателей приглашения на собрание.</span><span class="sxs-lookup"><span data-stu-id="08bc2-104">The **Attendees** element specifies the recipients of an invitation to a meeting.</span></span> 
  
```XML
<Attendees>
    <EmailUser></EmailUser>
</Attendees>
```

 <span data-ttu-id="08bc2-105">**ArrayOfEmailUsersType**</span><span class="sxs-lookup"><span data-stu-id="08bc2-105">**ArrayOfEmailUsersType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="08bc2-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="08bc2-106">Attributes and elements</span></span>

<span data-ttu-id="08bc2-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="08bc2-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="08bc2-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="08bc2-108">Attributes</span></span>

<span data-ttu-id="08bc2-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="08bc2-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="08bc2-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="08bc2-110">Child elements</span></span>

|<span data-ttu-id="08bc2-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="08bc2-111">**Element**</span></span>|<span data-ttu-id="08bc2-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="08bc2-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="08bc2-113">EmailUser</span><span class="sxs-lookup"><span data-stu-id="08bc2-113">EmailUser</span></span>](emailuser.md) <br/> |<span data-ttu-id="08bc2-114">Задает получатель электронной почты или контакта Active Directory.</span><span class="sxs-lookup"><span data-stu-id="08bc2-114">Specifies an email recipient or Active Directory contact.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="08bc2-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="08bc2-115">Parent elements</span></span>

|<span data-ttu-id="08bc2-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="08bc2-116">**Element**</span></span>|<span data-ttu-id="08bc2-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="08bc2-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="08bc2-118">MeetingSuggestion</span><span class="sxs-lookup"><span data-stu-id="08bc2-118">MeetingSuggestion</span></span>](meetingsuggestion.md) <br/> |<span data-ttu-id="08bc2-119">Задает предложенного собрания.</span><span class="sxs-lookup"><span data-stu-id="08bc2-119">Specifies a proposed meeting.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="08bc2-120">Замечания</span><span class="sxs-lookup"><span data-stu-id="08bc2-120">Remarks</span></span>

<span data-ttu-id="08bc2-121">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="08bc2-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="08bc2-122">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="08bc2-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="08bc2-123">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="08bc2-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="08bc2-124">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="08bc2-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="08bc2-125">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="08bc2-125">Schema Name</span></span>  <br/> |<span data-ttu-id="08bc2-126">Схема типа</span><span class="sxs-lookup"><span data-stu-id="08bc2-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="08bc2-127">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="08bc2-127">Validation File</span></span>  <br/> |<span data-ttu-id="08bc2-128">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="08bc2-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="08bc2-129">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="08bc2-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="08bc2-130">См. также</span><span class="sxs-lookup"><span data-stu-id="08bc2-130">See also</span></span>

- [<span data-ttu-id="08bc2-131">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="08bc2-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

