---
title: Уполномоченные
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 20ef18c2-daa0-4f65-a515-e84e9993a77f
description: Элемент уполномоченные указывает пользователей, которым назначена задача.
ms.openlocfilehash: 3e98273e859dbe2128b0ad3b4df42c8016fd3bc5
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44464716"
---
# <a name="assignees"></a><span data-ttu-id="d9ec9-103">Уполномоченные</span><span class="sxs-lookup"><span data-stu-id="d9ec9-103">Assignees</span></span>

<span data-ttu-id="d9ec9-104">Элемент **уполномоченные** указывает пользователей, которым назначена задача.</span><span class="sxs-lookup"><span data-stu-id="d9ec9-104">The **Assignees** element specifies the people to whom a task is assigned.</span></span> 
  
```XML
<Assignees>
    <Name></Name>
    <UserID></UserID>
</Assignees>
```

 <span data-ttu-id="d9ec9-105">**емаилусертипе**</span><span class="sxs-lookup"><span data-stu-id="d9ec9-105">**EmailUserType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d9ec9-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="d9ec9-106">Attributes and elements</span></span>

<span data-ttu-id="d9ec9-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="d9ec9-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d9ec9-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="d9ec9-108">Attributes</span></span>

<span data-ttu-id="d9ec9-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="d9ec9-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d9ec9-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="d9ec9-110">Child elements</span></span>

|<span data-ttu-id="d9ec9-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="d9ec9-111">**Element**</span></span>|<span data-ttu-id="d9ec9-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d9ec9-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d9ec9-113">Имя (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="d9ec9-113">Name (EmailAddress)</span></span>](name-emailaddress.md) <br/> |<span data-ttu-id="d9ec9-114">Представляет отображаемое имя пользователя почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="d9ec9-114">Represents the display name of the mailbox user.</span></span>  <br/> |
|[<span data-ttu-id="d9ec9-115">UserId (строка)</span><span class="sxs-lookup"><span data-stu-id="d9ec9-115">UserId (string)</span></span>](userid-string.md) <br/> |<span data-ttu-id="d9ec9-116">Указывает идентификатор пользователя электронной почты.</span><span class="sxs-lookup"><span data-stu-id="d9ec9-116">Specifies the user identifier of an email user.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d9ec9-117">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="d9ec9-117">Parent elements</span></span>

|<span data-ttu-id="d9ec9-118">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="d9ec9-118">**Element**</span></span>|<span data-ttu-id="d9ec9-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d9ec9-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d9ec9-120">TaskSuggestion</span><span class="sxs-lookup"><span data-stu-id="d9ec9-120">TaskSuggestion</span></span>](tasksuggestion.md) <br/> |<span data-ttu-id="d9ec9-121">Указывает предложенную задачу.</span><span class="sxs-lookup"><span data-stu-id="d9ec9-121">Specifies a proposed task.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="d9ec9-122">Примечания</span><span class="sxs-lookup"><span data-stu-id="d9ec9-122">Remarks</span></span>

<span data-ttu-id="d9ec9-123">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="d9ec9-123">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="d9ec9-124">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="d9ec9-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d9ec9-125">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="d9ec9-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d9ec9-126">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="d9ec9-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d9ec9-127">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="d9ec9-127">Schema Name</span></span>  <br/> |<span data-ttu-id="d9ec9-128">Схема типа</span><span class="sxs-lookup"><span data-stu-id="d9ec9-128">Type schema</span></span>  <br/> |
|<span data-ttu-id="d9ec9-129">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="d9ec9-129">Validation File</span></span>  <br/> |<span data-ttu-id="d9ec9-130">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="d9ec9-130">types.xsd</span></span>  <br/> |
|<span data-ttu-id="d9ec9-131">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="d9ec9-131">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="d9ec9-132">См. также</span><span class="sxs-lookup"><span data-stu-id="d9ec9-132">See also</span></span>

- [<span data-ttu-id="d9ec9-133">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="d9ec9-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

