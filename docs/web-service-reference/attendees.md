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
ms.openlocfilehash: 3a63bdf7e49309697ac503be5f4c95eb805b9635
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460332"
---
# <a name="attendees"></a><span data-ttu-id="0496d-103">Участники</span><span class="sxs-lookup"><span data-stu-id="0496d-103">Attendees</span></span>

<span data-ttu-id="0496d-104">Элемент **Участники** указывает получателей приглашения на собрание.</span><span class="sxs-lookup"><span data-stu-id="0496d-104">The **Attendees** element specifies the recipients of an invitation to a meeting.</span></span> 
  
```XML
<Attendees>
    <EmailUser></EmailUser>
</Attendees>
```

 <span data-ttu-id="0496d-105">**аррайофемаилусерстипе**</span><span class="sxs-lookup"><span data-stu-id="0496d-105">**ArrayOfEmailUsersType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0496d-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="0496d-106">Attributes and elements</span></span>

<span data-ttu-id="0496d-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="0496d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0496d-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="0496d-108">Attributes</span></span>

<span data-ttu-id="0496d-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="0496d-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0496d-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="0496d-110">Child elements</span></span>

|<span data-ttu-id="0496d-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="0496d-111">**Element**</span></span>|<span data-ttu-id="0496d-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="0496d-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0496d-113">Свойства emailuser</span><span class="sxs-lookup"><span data-stu-id="0496d-113">EmailUser</span></span>](emailuser.md) <br/> |<span data-ttu-id="0496d-114">Указывает получателя электронной почты или контакта Active Directory.</span><span class="sxs-lookup"><span data-stu-id="0496d-114">Specifies an email recipient or Active Directory contact.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="0496d-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="0496d-115">Parent elements</span></span>

|<span data-ttu-id="0496d-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="0496d-116">**Element**</span></span>|<span data-ttu-id="0496d-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="0496d-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0496d-118">MeetingSuggestion</span><span class="sxs-lookup"><span data-stu-id="0496d-118">MeetingSuggestion</span></span>](meetingsuggestion.md) <br/> |<span data-ttu-id="0496d-119">Указывает предложенное собрание.</span><span class="sxs-lookup"><span data-stu-id="0496d-119">Specifies a proposed meeting.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="0496d-120">Примечания</span><span class="sxs-lookup"><span data-stu-id="0496d-120">Remarks</span></span>

<span data-ttu-id="0496d-121">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="0496d-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="0496d-122">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="0496d-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0496d-123">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="0496d-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0496d-124">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="0496d-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="0496d-125">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="0496d-125">Schema Name</span></span>  <br/> |<span data-ttu-id="0496d-126">Схема типа</span><span class="sxs-lookup"><span data-stu-id="0496d-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="0496d-127">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="0496d-127">Validation File</span></span>  <br/> |<span data-ttu-id="0496d-128">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="0496d-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="0496d-129">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="0496d-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="0496d-130">См. также</span><span class="sxs-lookup"><span data-stu-id="0496d-130">See also</span></span>

- [<span data-ttu-id="0496d-131">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="0496d-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

