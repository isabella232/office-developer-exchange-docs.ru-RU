---
title: Участники
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 837bb372-39eb-48ae-9c09-0d2552511f93
description: Элемент участники указывает получателей приглашения на собрание.
ms.openlocfilehash: 22d88bb092b416c553144496e133680b53f5d30e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761519"
---
# <a name="attendees"></a><span data-ttu-id="8180a-103">Участники</span><span class="sxs-lookup"><span data-stu-id="8180a-103">Attendees</span></span>

<span data-ttu-id="8180a-104">Элемент **Участники** указывает получателей приглашения на собрание.</span><span class="sxs-lookup"><span data-stu-id="8180a-104">The **Attendees** element specifies the recipients of an invitation to a meeting.</span></span> 
  
```XML
<Attendees>
    <EmailUser></EmailUser>
</Attendees>
```

 <span data-ttu-id="8180a-105">**аррайофемаилусерстипе**</span><span class="sxs-lookup"><span data-stu-id="8180a-105">**ArrayOfEmailUsersType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8180a-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="8180a-106">Attributes and elements</span></span>

<span data-ttu-id="8180a-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="8180a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8180a-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="8180a-108">Attributes</span></span>

<span data-ttu-id="8180a-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="8180a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8180a-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="8180a-110">Child elements</span></span>

|<span data-ttu-id="8180a-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="8180a-111">**Element**</span></span>|<span data-ttu-id="8180a-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="8180a-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8180a-113">Свойства emailuser</span><span class="sxs-lookup"><span data-stu-id="8180a-113">EmailUser</span></span>](emailuser.md) <br/> |<span data-ttu-id="8180a-114">Указывает получателя электронной почты или контакта Active Directory.</span><span class="sxs-lookup"><span data-stu-id="8180a-114">Specifies an email recipient or Active Directory contact.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="8180a-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="8180a-115">Parent elements</span></span>

|<span data-ttu-id="8180a-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="8180a-116">**Element**</span></span>|<span data-ttu-id="8180a-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="8180a-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8180a-118">MeetingSuggestion</span><span class="sxs-lookup"><span data-stu-id="8180a-118">MeetingSuggestion</span></span>](meetingsuggestion.md) <br/> |<span data-ttu-id="8180a-119">Указывает предложенное собрание.</span><span class="sxs-lookup"><span data-stu-id="8180a-119">Specifies a proposed meeting.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="8180a-120">Примечания</span><span class="sxs-lookup"><span data-stu-id="8180a-120">Remarks</span></span>

<span data-ttu-id="8180a-121">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="8180a-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="8180a-122">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="8180a-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8180a-123">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="8180a-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8180a-124">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="8180a-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="8180a-125">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="8180a-125">Schema Name</span></span>  <br/> |<span data-ttu-id="8180a-126">Схема типа</span><span class="sxs-lookup"><span data-stu-id="8180a-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="8180a-127">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="8180a-127">Validation File</span></span>  <br/> |<span data-ttu-id="8180a-128">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="8180a-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="8180a-129">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="8180a-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="8180a-130">См. также</span><span class="sxs-lookup"><span data-stu-id="8180a-130">See also</span></span>

- [<span data-ttu-id="8180a-131">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="8180a-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

